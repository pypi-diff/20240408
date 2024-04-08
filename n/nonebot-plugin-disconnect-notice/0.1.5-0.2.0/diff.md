# Comparing `tmp/nonebot_plugin_disconnect_notice-0.1.5.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.1.5.tar` & `nonebot_plugin_disconnect_notice-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-07-29 03:19:35.073256 nonebot_plugin_disconnect_notice-0.1.5/LICENSE
--rw-r--r--   0        0        0     5109 2023-07-29 03:19:35.073256 nonebot_plugin_disconnect_notice-0.1.5/README.md
--rw-r--r--   0        0        0     2497 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      688 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      784 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2102 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      445 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-08 08:32:31.468409 nonebot_plugin_disconnect_notice-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5782 2024-04-08 08:32:31.468409 nonebot_plugin_disconnect_notice-0.2.0/README.md
+-rw-r--r--   0        0        0     3606 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      797 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      784 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2102 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      483 2024-04-08 08:32:31.472409 nonebot_plugin_disconnect_notice-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/LICENSE` & `nonebot_plugin_disconnect_notice-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/README.md` & `nonebot_plugin_disconnect_notice-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -94,34 +94,37 @@
 | 网易163邮箱  |  smtp.163.com   |    465    |
 | 移动139邮箱  |  smtp.139.com   |    465    |
 
 
 </details>
 
 
-| 配置项 | 必填 | 值类型 | 默认值 | 说明 |
-|:------:|:----:|:---:|:---:|:--:|
-| disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
-| disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码或授权码,如 114514 |
-| disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
-| disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
-| disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
-| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
+|               配置项                | 必填 | 值类型  |  默认值  |                        说明                         |
+|:--------------------------------:|:--:|:----:|:-----:|:-------------------------------------------------:|
+|   disconnect_notice_smtp_user    | 是  | str  |  ""   |              邮箱账号,如 114514@yeah.net               |
+| disconnect_notice_smtp_password  | 是  | str  |  ""   |                 邮箱密码或授权码,如 114514                 |
+|  disconnect_notice_smtp_server   | 是  | str  |  ""   |              邮箱服务器地址,如 smtp.yeah.net              |
+|   disconnect_notice_smtp_port    | 是  | int  |  465  |                 邮箱端口号，ssl模式时为465                  |
+|  disconnect_notice_notice_email  | 是  | str  |  ""   |                  收件人邮箱，填写自己邮箱即可                   |
+|    disconnect_notice_dev_mode    | 否  | bool | False | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
+| disconnect_notice_max_grace_time | 否  | int  |  10   |      断连后最大宽限时长，单位:秒，如果在此期间bot完成了重连，则不触发邮件通知       |
+
 
 <details>
 <summary>示例配置</summary>
   
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
 disconnect_notice_smtp_password = "114514" #邮箱密码
 disconnect_notice_smtp_server = "smtp.yeah.net" #邮箱服务器地址
 disconnect_notice_smtp_port = 465 #邮箱端口号
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
 disconnect_notice_dev_mode = False #开发者模式，该模式下bot断连不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知
+disconnect_notice_max_grace_time = 10 #断连后最大宽限时长，单位:秒，如果在此期间bot完成了重连，则不触发邮件通知
 ```
 
 </details>
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ |  范围  |           说明            |
```

#### html2text {}

```diff
@@ -25,34 +25,39 @@
 (images/img_4.png) 6.å¤å¶å¾å°çè¿ä¸ªææç  ![img_5.png](images/
 img_5.png)
 7.å¾å°çè¿ä¸ª`ææç `å°±ç¸å½äºé®ç®±å¯ç ï¼é®ç®±è´¦å·å°±æ¯qqé®ç®±ï¼å¶ä»çä¸äºå¸¸è§é®ç®±çsmtp_serveråsmtp_portéç½®åæ°åèä¸è¡¨
 | é®ç®±å | smtp_server | smtp_port | |:--------:|:---------------:|:--------
 -:| | qqé®ç®± | smtp.qq.com | 465 | | ç½æyeahé®ç®± | smtp.yeah.net | 465 |
 | é¿éäºé®ç®± | smtp.aliyun.com | 465 | | ç½æ163é®ç®± | smtp.163.com |
 465 | | ç§»å¨139é®ç®± | smtp.139.com | 465 | | éç½®é¡¹ | å¿å¡« | å¼ç±»å
-| é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:---:|:--:| |
+| é»è®¤å¼ | è¯´æ | |:--------------------------------:|:--:|:----:|:-----:
+|:-------------------------------------------------:| |
 disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦ 114514@yeah.net
 | | disconnect_notice_smtp_password | æ¯ | str | "" |
 é®ç®±å¯ç æææç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ |
 str | "" | é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | |
 disconnect_notice_smtp_port | æ¯ | int | 465 |
 é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | | disconnect_notice_notice_email | æ¯ |
 str | "" | æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | |
 disconnect_notice_dev_mode | å¦ | bool | False |
 å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
-| ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
-disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
-disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
-disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
-disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
+| | disconnect_notice_max_grace_time | å¦ | int | 10 |
+æ­è¿åæå¤§å®½éæ¶é¿ï¼åä½:
+ç§ï¼å¦æå¨æ­¤æé´botå®æäºéè¿ï¼åä¸è§¦åé®ä»¶éç¥ |
+ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½® disconnect_notice_smtp_user
+= "114514@yeah.net" #é®ç®±è´¦å· disconnect_notice_smtp_password = "114514"
+#é®ç®±å¯ç  disconnect_notice_smtp_server = "smtp.yeah.net"
+#é®ç®±æå¡å¨å°å disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®±
 disconnect_notice_dev_mode = False
 #å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­è¿ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
-``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ
-| |:-----:|:----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯
-| ä¸»äºº | å¦ | ææä¼è¯ |
+disconnect_notice_max_grace_time = 10 #æ­è¿åæå¤§å®½éæ¶é¿ï¼åä½:
+ç§ï¼å¦æå¨æ­¤æé´botå®æäºéè¿ï¼åä¸è§¦åé®ä»¶éç¥ ``` ##
+ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
+--:|:----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯ |
+ä¸»äºº | å¦ | ææä¼è¯ |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
 ææå¾ é®ä»¶éç¥ ![mail.png](images/mail.png) ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ ## â³ Star è¶å¿ [!
 [Stargazers over time](https://starchart.cc/Cypas/
 nonebot_plugin_disconnect_notice.svg)](https://starchart.cc/Cypas/
 nonebot_plugin_disconnect_notice)
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/__init__.py` & `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,38 @@
+from datetime import datetime as dt, timedelta
+
 from nonebot.internal.matcher import Matcher
 from nonebot.plugin import PluginMetadata
-from nonebot import Bot
+from nonebot import Bot, require, get_bots
+from nonebot import logger
 
 # onebot11 协议
 from nonebot.adapters.onebot.v11 import Bot as V11Bot
 from nonebot import on_command
 from nonebot.permission import SUPERUSER
 
-from .config import driver, plugin_config, global_config
+from .config import driver, plugin_config, global_config, Config
 from .dataClass import BotParams
 from .utils import send_notice, mail_config, send_mail
 
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
+
 __plugin_meta__ = PluginMetadata(
     name="bot断连通知",
     description="bot断连时的通知插件，当前支持邮件通知",
     usage="""
     超级用户指令:
         断连通知测试:主动触发掉线通知测试
     """,
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
     homepage="https://github.com/Cypas/nonebot_plugin_disconnect_notice",
     # 发布必填。
+    config=Config,
     supported_adapters=None,
 )
 
 notice_test = on_command("断连通知测试", permission=SUPERUSER)
 
 
 @notice_test.handle()
@@ -43,19 +50,42 @@
 
 
 @driver.on_bot_disconnect
 async def disconnect(bot: Bot):
     """bot断连触发器"""
     # 开发者模式下不生效
     if not plugin_config.disconnect_notice_dev_mode:
+        platform = bot.adapter.get_name()
+        bot_id = bot.self_id
+        job_id = f"disconnect_notice_{platform}_{bot_id}"
+        if scheduler.get_job(job_id):
+            scheduler.remove_job(job_id)
+        # 计算运行时间
+        run_time = dt.now() + timedelta(seconds=plugin_config.disconnect_notice_max_grace_time)
+
+        scheduler.add_job(
+            id=job_id, func=cron_send_notice, args=[platform, bot_id],
+            misfire_grace_time=60, coalesce=True, max_instances=1, trigger='date', run_date=run_time
+        )
+
+
+async def cron_send_notice(platform, bot_id):
+    """定时任务：发送通知"""
+    # 重新检查bot是否接入
+    bots = get_bots()
+    bot = bots.get(bot_id)
+    if not bot:
         bot_params = BotParams(
-            adapter_name=bot.adapter.get_name(),
-            bot_id=bot.self_id
+            adapter_name=platform,
+            bot_id=bot_id
         )
+        logger.warning(f"平台:{platform} bot_id:{bot_id} 已掉线，即将进行通知")
         await send_notice(bot_params)
+    else:
+        logger.info(f"平台:{platform} bot_id:{bot_id} 已重连，无需进行通知")
 
 
 @driver.on_bot_connect
 async def connect(bot: Bot):
     """bot接入时检测配置完整性"""
     if isinstance(bot, V11Bot):
         if not mail_config.check_params():
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import List, Optional
 
-from nonebot import get_driver
+from nonebot import get_driver, get_plugin_config
 from pydantic import BaseModel
 
 
 # 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
 class Config(BaseModel):
-    disconnect_notice_smtp_user = ""
-    disconnect_notice_smtp_password = ""
-    disconnect_notice_smtp_server = ""
-    disconnect_notice_smtp_port = 465
-    disconnect_notice_notice_email = ""
-    disconnect_notice_dev_mode = False
+    disconnect_notice_smtp_user: str | int = ""
+    disconnect_notice_smtp_password: str = ""
+    disconnect_notice_smtp_server: str | int = ""
+    disconnect_notice_smtp_port: int = 465
+    disconnect_notice_notice_email: str | int = ""
+    disconnect_notice_dev_mode: bool = False
+    disconnect_notice_max_grace_time: int = 10
 
 
 driver = get_driver()
 # 本地测试时由于不启动 driver，需要将下面两行注释并取消再下一行的注释
 global_config = driver.config
-plugin_config = Config.parse_obj(global_config)
+plugin_config = get_plugin_config(Config)
 
 # plugin_config = Config()
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/dataClass.py` & `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/dataClass.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.2.0/nonebot_plugin_disconnect_notice/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.5/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.1.5
+Version: 0.2.0
 Summary: bot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiosmtplib (>=2.0.2,<3.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.4.1,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0)
+Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -111,34 +113,37 @@
 | 网易163邮箱  |  smtp.163.com   |    465    |
 | 移动139邮箱  |  smtp.139.com   |    465    |
 
 
 </details>
 
 
-| 配置项 | 必填 | 值类型 | 默认值 | 说明 |
-|:------:|:----:|:---:|:---:|:--:|
-| disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
-| disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码或授权码,如 114514 |
-| disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
-| disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
-| disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
-| disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
+|               配置项                | 必填 | 值类型  |  默认值  |                        说明                         |
+|:--------------------------------:|:--:|:----:|:-----:|:-------------------------------------------------:|
+|   disconnect_notice_smtp_user    | 是  | str  |  ""   |              邮箱账号,如 114514@yeah.net               |
+| disconnect_notice_smtp_password  | 是  | str  |  ""   |                 邮箱密码或授权码,如 114514                 |
+|  disconnect_notice_smtp_server   | 是  | str  |  ""   |              邮箱服务器地址,如 smtp.yeah.net              |
+|   disconnect_notice_smtp_port    | 是  | int  |  465  |                 邮箱端口号，ssl模式时为465                  |
+|  disconnect_notice_notice_email  | 是  | str  |  ""   |                  收件人邮箱，填写自己邮箱即可                   |
+|    disconnect_notice_dev_mode    | 否  | bool | False | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
+| disconnect_notice_max_grace_time | 否  | int  |  10   |      断连后最大宽限时长，单位:秒，如果在此期间bot完成了重连，则不触发邮件通知       |
+
 
 <details>
 <summary>示例配置</summary>
   
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
 disconnect_notice_smtp_password = "114514" #邮箱密码
 disconnect_notice_smtp_server = "smtp.yeah.net" #邮箱服务器地址
 disconnect_notice_smtp_port = 465 #邮箱端口号
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
 disconnect_notice_dev_mode = False #开发者模式，该模式下bot断连不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知
+disconnect_notice_max_grace_time = 10 #断连后最大宽限时长，单位:秒，如果在此期间bot完成了重连，则不触发邮件通知
 ```
 
 </details>
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ |  范围  |           说明            |
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.5
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.2.0
 Summary: botæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiosmtplib (>=2.0.2,<3.0.0) Requires-Dist: nonebot-adapter-
-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-
-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: aiosmtplib
+(>=2.0.2,<3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.1,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0) Requires-Dist:
+nonebot2 (>=2.2.0,<3.0.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
    # nonebot-plugin-disconnect-notice _â¨ botæ­è¿æ¶çéç¥æä»¶ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» -
 å¯ä»¥å¨botæ­å¼ä¸nonebotçè¿æ¥æ¶åä¸»äººåéä¾å¦é®ä»¶çéç¥ï¼ç¨æ¥éç¥ä¸»äººbotå¯è½è¢«é£æ§æçº¿
 - ç®åæ¯æå¨é¨ééå¨åè®®ï¼éç¥æ¹å¼æ¯æé®ä»¶éç¥ -
@@ -34,34 +35,39 @@
 (images/img_4.png) 6.å¤å¶å¾å°çè¿ä¸ªææç  ![img_5.png](images/
 img_5.png)
 7.å¾å°çè¿ä¸ª`ææç `å°±ç¸å½äºé®ç®±å¯ç ï¼é®ç®±è´¦å·å°±æ¯qqé®ç®±ï¼å¶ä»çä¸äºå¸¸è§é®ç®±çsmtp_serveråsmtp_portéç½®åæ°åèä¸è¡¨
 | é®ç®±å | smtp_server | smtp_port | |:--------:|:---------------:|:--------
 -:| | qqé®ç®± | smtp.qq.com | 465 | | ç½æyeahé®ç®± | smtp.yeah.net | 465 |
 | é¿éäºé®ç®± | smtp.aliyun.com | 465 | | ç½æ163é®ç®± | smtp.163.com |
 465 | | ç§»å¨139é®ç®± | smtp.139.com | 465 | | éç½®é¡¹ | å¿å¡« | å¼ç±»å
-| é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:---:|:--:| |
+| é»è®¤å¼ | è¯´æ | |:--------------------------------:|:--:|:----:|:-----:
+|:-------------------------------------------------:| |
 disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦ 114514@yeah.net
 | | disconnect_notice_smtp_password | æ¯ | str | "" |
 é®ç®±å¯ç æææç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ |
 str | "" | é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | |
 disconnect_notice_smtp_port | æ¯ | int | 465 |
 é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | | disconnect_notice_notice_email | æ¯ |
 str | "" | æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | |
 disconnect_notice_dev_mode | å¦ | bool | False |
 å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
-| ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
-disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
-disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
-disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
-disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
+| | disconnect_notice_max_grace_time | å¦ | int | 10 |
+æ­è¿åæå¤§å®½éæ¶é¿ï¼åä½:
+ç§ï¼å¦æå¨æ­¤æé´botå®æäºéè¿ï¼åä¸è§¦åé®ä»¶éç¥ |
+ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½® disconnect_notice_smtp_user
+= "114514@yeah.net" #é®ç®±è´¦å· disconnect_notice_smtp_password = "114514"
+#é®ç®±å¯ç  disconnect_notice_smtp_server = "smtp.yeah.net"
+#é®ç®±æå¡å¨å°å disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
 disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®±
 disconnect_notice_dev_mode = False
 #å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­è¿ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
-``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ
-| |:-----:|:----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯
-| ä¸»äºº | å¦ | ææä¼è¯ |
+disconnect_notice_max_grace_time = 10 #æ­è¿åæå¤§å®½éæ¶é¿ï¼åä½:
+ç§ï¼å¦æå¨æ­¤æé´botå®æäºéè¿ï¼åä¸è§¦åé®ä»¶éç¥ ``` ##
+ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
+--:|:----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯ |
+ä¸»äºº | å¦ | ææä¼è¯ |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
 ææå¾ é®ä»¶éç¥ ![mail.png](images/mail.png) ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ ## â³ Star è¶å¿ [!
 [Stargazers over time](https://starchart.cc/Cypas/
 nonebot_plugin_disconnect_notice.svg)](https://starchart.cc/Cypas/
 nonebot_plugin_disconnect_notice)
```

