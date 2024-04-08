# Comparing `tmp/Liacord-0.1.6.tar.gz` & `tmp/Liacord-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liacord-0.1.6.tar", last modified: Mon Apr  8 09:11:28 2024, max compression
+gzip compressed data, was "Liacord-0.1.7.tar", last modified: Mon Apr  8 09:22:59 2024, max compression
```

## Comparing `Liacord-0.1.6.tar` & `Liacord-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 09:11:27.992426 Liacord-0.1.6/
-drwxrwxrwx   0        0        0        0 2024-04-08 09:11:27.980904 Liacord-0.1.6/Liacord/
--rw-rw-rw-   0        0        0       88 2024-04-07 22:17:01.000000 Liacord-0.1.6/Liacord/__init__.py
--rw-rw-rw-   0        0        0     6666 2024-04-07 22:23:59.000000 Liacord-0.1.6/Liacord/client.py
--rw-rw-rw-   0        0        0     1494 2024-04-07 22:24:16.000000 Liacord-0.1.6/Liacord/context.py
--rw-rw-rw-   0        0        0     1854 2024-04-07 22:24:16.000000 Liacord-0.1.6/Liacord/intents.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:11:27.991427 Liacord-0.1.6/Liacord.egg-info/
--rw-rw-rw-   0        0        0     2600 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2600 2024-04-08 09:11:27.993428 Liacord-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2203 2024-04-08 09:11:03.000000 Liacord-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 09:11:27.993428 Liacord-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-08 09:07:05.000000 Liacord-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:22:59.276649 Liacord-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-04-08 09:22:59.258071 Liacord-0.1.7/Liacord/
+-rw-rw-rw-   0        0        0       88 2024-04-07 22:17:01.000000 Liacord-0.1.7/Liacord/__init__.py
+-rw-rw-rw-   0        0        0     6666 2024-04-07 22:23:59.000000 Liacord-0.1.7/Liacord/client.py
+-rw-rw-rw-   0        0        0     1494 2024-04-07 22:24:16.000000 Liacord-0.1.7/Liacord/context.py
+-rw-rw-rw-   0        0        0     1854 2024-04-07 22:24:16.000000 Liacord-0.1.7/Liacord/intents.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:22:59.275138 Liacord-0.1.7/Liacord.egg-info/
+-rw-rw-rw-   0        0        0     2506 2024-04-08 09:22:59.000000 Liacord-0.1.7/Liacord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-04-08 09:22:59.000000 Liacord-0.1.7/Liacord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:22:59.000000 Liacord-0.1.7/Liacord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 09:22:59.000000 Liacord-0.1.7/Liacord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-04-08 09:22:59.000000 Liacord-0.1.7/Liacord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 09:22:59.000000 Liacord-0.1.7/Liacord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2506 2024-04-08 09:22:59.276649 Liacord-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2109 2024-04-08 09:22:09.000000 Liacord-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:22:59.278655 Liacord-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-08 09:22:47.000000 Liacord-0.1.7/setup.py
```

### Comparing `Liacord-0.1.6/Liacord/client.py` & `Liacord-0.1.7/Liacord/client.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.6/Liacord/context.py` & `Liacord-0.1.7/Liacord/context.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.6/Liacord/intents.py` & `Liacord-0.1.7/Liacord/intents.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.6/Liacord.egg-info/PKG-INFO` & `Liacord-0.1.7/Liacord.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liacord
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/masezev/Liacord.py
 Author: Masezev
 Author-email: csgomanagement1@gmail.com
 License: MIT
 Project-URL: Discord, https://discord.gg/H7FQFGEPz5
 Keywords: A Python wrapper for the Discord API
@@ -29,16 +29,14 @@
 - Optimised in both speed and memory.
 
 Installing
 ----------
 
 **Python 3.8 or higher is required**
 
-To install the library without full voice support, you can just run the following command:
-
     # Linux/macOS
     python3 -m pip install -U Liacord
 
     # Windows
     py -3 -m pip install -U Liacord
 
 Bot Example
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: Liacord Version: 0.1.6 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: Liacord Version: 0.1.7 Summary: A Python wrapper
 for the Discord API Home-page: https://github.com/masezev/Liacord.py Author:
 Masezev Author-email: csgomanagement1@gmail.com License: MIT Project-URL:
 Discord, https://discord.gg/H7FQFGEPz5 Keywords: A Python wrapper for the
 Discord API Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 Liacord ==========
   _[_D_i_s_c_o_r_d_ _s_e_r_v_e_r_ _i_n_v_i_t_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_ _i_n_f_o_]_[_P_y_P_I_ _s_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                                _[_C_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]
 Key Features ------------- - Modern Pythonic API using ``async`` and ``await``.
 - Proper rate limit handling. - Optimised in both speed and memory. Installing
----------- **Python 3.8 or higher is required** To install the library without
-full voice support, you can just run the following command: # Linux/macOS
-python3 -m pip install -U Liacord # Windows py -3 -m pip install -U Liacord Bot
-Example ~~~~~~~~~~~~~ import asyncio from Liacord import Client, Intents
-intents = Intents().all() client = Client("your_token_here", prefix="#",
-intents=intents) @client.command(name="name") async def hello(ctx): await
-ctx.send(f"{ctx.author.name}") @client.command(name="ping") async def ping
-(ctx): await ctx.send(f"pong {round(client.latency)}ms.") @client.command
-(name='server_id', brief='get the server id') async def server_id_command(ctx):
-server_id = ctx.guild.id await ctx.send(f"server id: {server_id}") loop =
+---------- **Python 3.8 or higher is required** # Linux/macOS python3 -m pip
+install -U Liacord # Windows py -3 -m pip install -U Liacord Bot Example
+~~~~~~~~~~~~~ import asyncio from Liacord import Client, Intents intents =
+Intents().all() client = Client("your_token_here", prefix="#", intents=intents)
+@client.command(name="name") async def hello(ctx): await ctx.send(f"
+{ctx.author.name}") @client.command(name="ping") async def ping(ctx): await
+ctx.send(f"pong {round(client.latency)}ms.") @client.command(name='server_id',
+brief='get the server id') async def server_id_command(ctx): server_id =
+ctx.guild.id await ctx.send(f"server id: {server_id}") loop =
 asyncio.get_event_loop() loop.run_until_complete(client.run()) ~~~~~~~~~~~~~
 You can find more examples in the examples directory [There](https://
 github.com/MaseZev/Liacord.py/tree/main/examples). Links
                    _D_i_s_c_o_r_d_ _S_e_r_v_e_r Ð²Ðâ¢ _D_i_s_c_o_r_d_ _D_e_v_e_l_o_p_e_r_s
```

### Comparing `Liacord-0.1.6/PKG-INFO` & `Liacord-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liacord
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/masezev/Liacord.py
 Author: Masezev
 Author-email: csgomanagement1@gmail.com
 License: MIT
 Project-URL: Discord, https://discord.gg/H7FQFGEPz5
 Keywords: A Python wrapper for the Discord API
@@ -29,16 +29,14 @@
 - Optimised in both speed and memory.
 
 Installing
 ----------
 
 **Python 3.8 or higher is required**
 
-To install the library without full voice support, you can just run the following command:
-
     # Linux/macOS
     python3 -m pip install -U Liacord
 
     # Windows
     py -3 -m pip install -U Liacord
 
 Bot Example
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: Liacord Version: 0.1.6 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: Liacord Version: 0.1.7 Summary: A Python wrapper
 for the Discord API Home-page: https://github.com/masezev/Liacord.py Author:
 Masezev Author-email: csgomanagement1@gmail.com License: MIT Project-URL:
 Discord, https://discord.gg/H7FQFGEPz5 Keywords: A Python wrapper for the
 Discord API Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 Liacord ==========
   _[_D_i_s_c_o_r_d_ _s_e_r_v_e_r_ _i_n_v_i_t_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_ _i_n_f_o_]_[_P_y_P_I_ _s_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                                _[_C_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]
 Key Features ------------- - Modern Pythonic API using ``async`` and ``await``.
 - Proper rate limit handling. - Optimised in both speed and memory. Installing
----------- **Python 3.8 or higher is required** To install the library without
-full voice support, you can just run the following command: # Linux/macOS
-python3 -m pip install -U Liacord # Windows py -3 -m pip install -U Liacord Bot
-Example ~~~~~~~~~~~~~ import asyncio from Liacord import Client, Intents
-intents = Intents().all() client = Client("your_token_here", prefix="#",
-intents=intents) @client.command(name="name") async def hello(ctx): await
-ctx.send(f"{ctx.author.name}") @client.command(name="ping") async def ping
-(ctx): await ctx.send(f"pong {round(client.latency)}ms.") @client.command
-(name='server_id', brief='get the server id') async def server_id_command(ctx):
-server_id = ctx.guild.id await ctx.send(f"server id: {server_id}") loop =
+---------- **Python 3.8 or higher is required** # Linux/macOS python3 -m pip
+install -U Liacord # Windows py -3 -m pip install -U Liacord Bot Example
+~~~~~~~~~~~~~ import asyncio from Liacord import Client, Intents intents =
+Intents().all() client = Client("your_token_here", prefix="#", intents=intents)
+@client.command(name="name") async def hello(ctx): await ctx.send(f"
+{ctx.author.name}") @client.command(name="ping") async def ping(ctx): await
+ctx.send(f"pong {round(client.latency)}ms.") @client.command(name='server_id',
+brief='get the server id') async def server_id_command(ctx): server_id =
+ctx.guild.id await ctx.send(f"server id: {server_id}") loop =
 asyncio.get_event_loop() loop.run_until_complete(client.run()) ~~~~~~~~~~~~~
 You can find more examples in the examples directory [There](https://
 github.com/MaseZev/Liacord.py/tree/main/examples). Links
                    _D_i_s_c_o_r_d_ _S_e_r_v_e_r Ð²Ðâ¢ _D_i_s_c_o_r_d_ _D_e_v_e_l_o_p_e_r_s
```

### Comparing `Liacord-0.1.6/README.md` & `Liacord-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 - Optimised in both speed and memory.
 
 Installing
 ----------
 
 **Python 3.8 or higher is required**
 
-To install the library without full voice support, you can just run the following command:
-
     # Linux/macOS
     python3 -m pip install -U Liacord
 
     # Windows
     py -3 -m pip install -U Liacord
 
 Bot Example
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
 Liacord ==========
   _[_D_i_s_c_o_r_d_ _s_e_r_v_e_r_ _i_n_v_i_t_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_ _i_n_f_o_]_[_P_y_P_I_ _s_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                                _[_C_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]
 Key Features ------------- - Modern Pythonic API using ``async`` and ``await``.
 - Proper rate limit handling. - Optimised in both speed and memory. Installing
----------- **Python 3.8 or higher is required** To install the library without
-full voice support, you can just run the following command: # Linux/macOS
-python3 -m pip install -U Liacord # Windows py -3 -m pip install -U Liacord Bot
-Example ~~~~~~~~~~~~~ import asyncio from Liacord import Client, Intents
-intents = Intents().all() client = Client("your_token_here", prefix="#",
-intents=intents) @client.command(name="name") async def hello(ctx): await
-ctx.send(f"{ctx.author.name}") @client.command(name="ping") async def ping
-(ctx): await ctx.send(f"pong {round(client.latency)}ms.") @client.command
-(name='server_id', brief='get the server id') async def server_id_command(ctx):
-server_id = ctx.guild.id await ctx.send(f"server id: {server_id}") loop =
+---------- **Python 3.8 or higher is required** # Linux/macOS python3 -m pip
+install -U Liacord # Windows py -3 -m pip install -U Liacord Bot Example
+~~~~~~~~~~~~~ import asyncio from Liacord import Client, Intents intents =
+Intents().all() client = Client("your_token_here", prefix="#", intents=intents)
+@client.command(name="name") async def hello(ctx): await ctx.send(f"
+{ctx.author.name}") @client.command(name="ping") async def ping(ctx): await
+ctx.send(f"pong {round(client.latency)}ms.") @client.command(name='server_id',
+brief='get the server id') async def server_id_command(ctx): server_id =
+ctx.guild.id await ctx.send(f"server id: {server_id}") loop =
 asyncio.get_event_loop() loop.run_until_complete(client.run()) ~~~~~~~~~~~~~
 You can find more examples in the examples directory [There](https://
 github.com/MaseZev/Liacord.py/tree/main/examples). Links
                      _D_i_s_c_o_r_d_ _S_e_r_v_e_r â _D_i_s_c_o_r_d_ _D_e_v_e_l_o_p_e_r_s
```

### Comparing `Liacord-0.1.6/setup.py` & `Liacord-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup(name='Liacord',
       author="Masezev",
       url="https://github.com/masezev/Liacord.py",
       project_urls={
           'Discord': 'https://discord.gg/H7FQFGEPz5',
       },
       repository='https://github.com/masezev/Liacord.py',
-      version='0.1.6',
+      version='0.1.7',
       description='A Python wrapper for the Discord API',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       python_requires='>=3.8.0',
       keywords='A Python wrapper for the Discord API',
       install_requires=[
             'aiohttp'
```

