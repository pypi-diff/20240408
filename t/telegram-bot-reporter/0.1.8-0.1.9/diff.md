# Comparing `tmp/telegram_bot_reporter-0.1.8.tar.gz` & `tmp/telegram_bot_reporter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_bot_reporter-0.1.8.tar", max compression
+gzip compressed data, was "telegram_bot_reporter-0.1.9.tar", max compression
```

## Comparing `telegram_bot_reporter-0.1.8.tar` & `telegram_bot_reporter-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1461 2024-04-06 08:32:39.233383 telegram_bot_reporter-0.1.8/README.md
--rw-r--r--   0        0        0     2293 2024-04-06 08:32:39.169384 telegram_bot_reporter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      111 2024-03-30 10:03:53.561341 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 06:03:42.268386 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/__init__.py
--rw-r--r--   0        0        0     2684 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/async_bot.py
--rw-r--r--   0        0        0      921 2024-04-01 17:44:27.743363 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/base_bot.py
--rw-r--r--   0        0        0     2531 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/sync_bot.py
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 telegram_bot_reporter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1461 2024-04-06 08:32:39.233383 telegram_bot_reporter-0.1.9/README.md
+-rw-r--r--   0        0        0     2311 2024-04-08 09:18:32.615778 telegram_bot_reporter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-03-30 10:03:53.561341 telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 06:03:42.268386 telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/core/__init__.py
+-rw-r--r--   0        0        0     3723 2024-04-08 09:14:47.865633 telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/core/async_bot.py
+-rw-r--r--   0        0        0     1147 2024-04-08 09:20:30.134811 telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/core/base_bot.py
+-rw-r--r--   0        0        0     3432 2024-04-08 09:19:43.095198 telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/core/sync_bot.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 telegram_bot_reporter-0.1.9/PKG-INFO
```

### Comparing `telegram_bot_reporter-0.1.8/README.md` & `telegram_bot_reporter-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.8/pyproject.toml` & `telegram_bot_reporter-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "telegram-bot-reporter"
-version = "0.1.8"
+version = "0.1.9"
 description = "Library for sending messages and files using a Telegram bot."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Deskent/bot_reporter"
 homepage = "https://pypi.org/project/telegram-bot-reporter/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 niquests = "^3.5.5"
+httpx = "^0.27.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "^7.0.0"
 ruff = "^0.3.4"
 pytest = "^8.1.1"
```

### Comparing `telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/async_bot.py` & `telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/core/sync_bot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,131 @@
 from pathlib import Path
+from typing import Callable
 
+import httpx
 import niquests
 
 from telegram_bot_reporter.core.base_bot import BaseBot
 
 
-class AsyncBot(BaseBot):
-    async def send_message(
+class Bot(BaseBot):
+    def send_message(
         self,
         message: str,
         split_message: bool = False,
-    ) -> niquests.Response:
+    ):
         """
         Send message to the Telegram chat.
 
         :param message: Text to send.
         :param split_message: If true, message will be sent by chunks.
             Defaults to False.
-        :return: niquests.Response
-
+        :return: Response
         """
 
         if split_message:
-            return await self._send_chunks(message)
-        return await self._send_message(message)
+            return self._send_chunks(message)
+        return self._send_message(message)
 
-    async def send_document(
+    def send_document(
         self,
         file_path: Path | str,
         caption: str = "",
-    ) -> niquests.Response:
+    ):
         """Send file as Telegram document.
 
         :param file_path: Path to the file.
         :param caption: Caption of the file. Defaults to empty string.
-        :return: niquests.Response
+        :return: Response
         """
 
         with open(file_path, "rb") as f:
             data: dict = {
                 "chat_id": self._chat_id,
                 "caption": caption,
                 "parse_mode": self._parse_mode,
             }
-            return await self._send_api_request(
+            return self._send_api_request(
                 "sendDocument",
                 headers={},
                 data=data,
                 files={"document": f},
             )
 
-    async def _send_chunks(self, message: str) -> niquests.Response:
+    def _send_chunks(self, message: str):
         for chunk in range(0, len(message), self._CHUNK):
-            await self._send_message(message[chunk : chunk + self._CHUNK])
+            self._send_message(message[chunk : chunk + self._CHUNK])
         else:
             response = niquests.Response()
             response.status_code = 200
 
             return response
 
-    async def _send_message(self, message: str) -> niquests.Response:
+    def _send_message(self, message: str):
         if len(message) > self._CHUNK:
             raise ValueError(
                 f"Message too long. Max length is {self._CHUNK} symbols."
             )
 
         data: dict = {
             "chat_id": self._chat_id,
             "text": f"{self._prefix}: {message}",
             "parse_mode": self._parse_mode,
         }
-        return await self._send_api_request(
+        return self._send_api_request(
             "sendMessage",
             json=data,
             headers=self._headers,
         )
 
-    async def _send_api_request(
+    def _send_api_request(
+        self,
+        api_method: str,
+        headers: dict,
+        *_,
+        **kwargs,
+    ):
+        transports: dict = {
+            'niquests': self._send_using_niquests,
+            'httpx': self._send_using_httpx,
+        }
+        func: Callable = transports.get(self._transport)
+        if not func:
+            raise ValueError(f'Invalid transport type: {self._transport}')
+        return func(
+            api_method=api_method,
+            headers=headers,
+            **kwargs,
+        )
+
+    def _send_using_niquests(
         self,
         api_method: str,
         headers: dict,
         *_,
         **kwargs,
     ) -> niquests.Response:
-        async with niquests.AsyncSession() as session:
-            response: niquests.Response = await session.post(
+        response: niquests.Response = niquests.post(
+            url=f"{self._url}/{api_method}",
+            headers=headers,
+            timeout=self._timeout,
+            **kwargs,
+        )
+
+        return response
+
+    def _send_using_httpx(
+        self,
+        api_method: str,
+        headers: dict,
+        *_,
+        **kwargs,
+    ) -> httpx.Response:
+        with httpx.Client() as session:
+            response: httpx.Response = session.post(
                 url=f"{self._url}/{api_method}",
                 headers=headers,
                 timeout=self._timeout,
                 **kwargs,
             )
 
             return response
```

### Comparing `telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/base_bot.py` & `telegram_bot_reporter-0.1.9/src/telegram_bot_reporter/core/base_bot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+from typing import Literal
+
+
 class BaseBot:
     """Telegram Bot API interface
     to send messages to certain chats/users.
 
     :argument bot_token: Telegram bot token.
     :argument chat_id: Telegram chat id.
     :argument timeout: Time to wait Telegram Api response, seconds.
         Defaults is 10.
     :argument parse_mode: Message parse mode. Defaults is 'HTML'.
     :argument prefix: Message prefix. Defaults is empty string.
+    :argument transport: HTTP library transport name.
+        Supported values: ['niquests', 'httpx']
 
     """
 
     _CHUNK: int = 4000
 
     def __init__(
         self,
         bot_token: str,
         chat_id: str | int,
         timeout: int = 10,
         parse_mode: str = "HTML",
         prefix: str = "",
+        transport: Literal['niquests', 'httpx'] = 'httpx',
     ):
         self._token = bot_token
         self._chat_id: str = str(chat_id)
         self._timeout = timeout
         self._parse_mode = parse_mode
         self._prefix = prefix
         self._headers: dict = {"Content-Type": "application/json"}
         self._url = f"https://api.telegram.org/bot{self._token}"
+        self._transport = transport
```

### Comparing `telegram_bot_reporter-0.1.8/PKG-INFO` & `telegram_bot_reporter-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: telegram-bot-reporter
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for sending messages and files using a Telegram bot.
 Home-page: https://pypi.org/project/telegram-bot-reporter/
 License: MIT
 Author: deskent
 Author-email: battenetciz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: niquests (>=3.5.5,<4.0.0)
 Project-URL: Repository, https://github.com/Deskent/bot_reporter
 Description-Content-Type: text/markdown
 
 ### Stack:
 
 - [x] <a href="https://www.python.org/"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-plain.svg" alt="python" width="15" height="15"/>
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: telegram-bot-reporter Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: telegram-bot-reporter Version: 0.1.9 Summary:
 Library for sending messages and files using a Telegram bot. Home-page: https:/
 /pypi.org/project/telegram-bot-reporter/ License: MIT Author: deskent Author-
 email: battenetciz@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: niquests (>=3.5.5,<4.0.0) Project-URL: Repository, https://
-github.com/Deskent/bot_reporter Description-Content-Type: text/markdown ###
-Stack: - [x] _[_p_y_t_h_o_n_]_P_y_t_h_o_n_ _3_._1_0_+_ 
+Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: niquests
+(>=3.5.5,<4.0.0) Project-URL: Repository, https://github.com/Deskent/
+bot_reporter Description-Content-Type: text/markdown ### Stack: - [x]
+_[_p_y_t_h_o_n_]_P_y_t_h_o_n_ _3_._1_0_+_ 
 - [x] _[_n_i_q_u_e_s_t_s_]_N_i_q_u_e_s_t_s_ _3_._5_._5_+_ 
 _#_#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _p_i_p_ _i_n_s_t_a_l_l_ _t_e_l_e_g_r_a_m_-_b_o_t_-_r_e_p_o_r_t_e_r_ _#_#_#_ _U_s_a_g_e_ _S_y_n_c_ _f_r_o_m
 _t_e_l_e_g_r_a_m___b_o_t___r_e_p_o_r_t_e_r_ _i_m_p_o_r_t_ _B_o_t_ _b_o_t_ _=_ _B_o_t_(_b_o_t___t_o_k_e_n_=_T_E_L_E_B_O_T___T_O_K_E_N_,
 _c_h_a_t___i_d_=_C_H_A_T___I_D_)_ _#_ _S_e_n_d_ _m_e_s_s_a_g_e_ _b_o_t_._s_e_n_d___m_e_s_s_a_g_e_(_'_H_e_l_l_o_,_ _w_o_r_l_d_'_)_ _#_ _S_e_n_d_ _f_i_l_e
 _t_e_m_p___f_i_l_e_ _=_ _P_a_t_h_(_'_t_e_s_t_._t_x_t_'_)_ _w_i_t_h_ _o_p_e_n_(_t_e_m_p___f_i_l_e_,_ _m_o_d_e_=_'_w_'_,_ _e_n_c_o_d_i_n_g_=_'_u_t_f_-_8_'_)
 _a_s_ _f_:_ _f_._w_r_i_t_e_(_'_T_e_s_t_ _m_e_s_s_a_g_e_'_)_ _b_o_t_._s_e_n_d___d_o_c_u_m_e_n_t_(_t_e_m_p___f_i_l_e_)_ _#_ _S_e_n_d_ _l_o_n_g_ _m_e_s_s_a_g_e_ 
 _(_m_o_r_e_ _t_h_a_n_ _4_0_0_0_ _s_y_m_b_o_l_s_)_ _b_o_t_._s_e_n_d___m_e_s_s_a_g_e_(_'_V_e_r_y_ _l_o_n_g_ _m_e_s_s_a_g_e_ _o_v_e_r_ _4_0_0_0
```

