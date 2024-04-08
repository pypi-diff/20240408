# Comparing `tmp/cyz-0.0.1.tar.gz` & `tmp/cyz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyz-0.0.1.tar", last modified: Mon Apr  8 05:54:22 2024, max compression
+gzip compressed data, was "cyz-0.0.2.tar", last modified: Mon Apr  8 07:03:16 2024, max compression
```

## Comparing `cyz-0.0.1.tar` & `cyz-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 05:54:22.327148 cyz-0.0.1/
--rw-rw-rw-   0        0        0      413 2024-04-08 05:54:22.327148 cyz-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-04-08 05:53:36.000000 cyz-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 05:54:22.310454 cyz-0.0.1/cyz/
--rw-rw-rw-   0        0        0     2260 2024-04-08 05:33:00.000000 cyz-0.0.1/cyz/email.py
-drwxrwxrwx   0        0        0        0 2024-04-08 05:54:22.327148 cyz-0.0.1/cyz.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-08 05:54:22.000000 cyz-0.0.1/cyz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      139 2024-04-08 05:54:22.000000 cyz-0.0.1/cyz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 05:54:22.000000 cyz-0.0.1/cyz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-08 05:54:22.000000 cyz-0.0.1/cyz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 05:54:22.327148 cyz-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-04-08 05:51:24.000000 cyz-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:03:16.182860 cyz-0.0.2/
+-rw-rw-rw-   0        0        0      413 2024-04-08 07:03:16.182860 cyz-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-04-08 05:53:36.000000 cyz-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 07:03:16.166960 cyz-0.0.2/cyz/
+-rw-rw-rw-   0        0        0       19 2024-04-08 07:01:44.000000 cyz-0.0.2/cyz/__init__.py
+-rw-rw-rw-   0        0        0     2010 2024-04-08 07:02:44.000000 cyz-0.0.2/cyz/mail.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:03:16.182860 cyz-0.0.2/cyz.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 07:03:16.182860 cyz-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-04-08 07:02:11.000000 cyz-0.0.2/setup.py
```

### Comparing `cyz-0.0.1/cyz/email.py` & `cyz-0.0.2/cyz/mail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import smtplib
 from email.mime.text import MIMEText
 from email.header import Header
 import base64
 
-def send(sender, passward, receiver, subject, content, from_nike_name='default', to_nike_name='default'):
+def send_email(sender, passward, receiver, subject, content, from_nike_name='default', to_nike_name='default'):
     mail_host = "smtp.qq.com"
 
     message = MIMEText(content, 'plain', 'utf-8')
 
     if from_nike_name == 'default':
         from_nike_name = sender.split('@')[0]
     from_nike_name = base64.b64encode(from_nike_name.encode('utf-8')).decode()
@@ -33,30 +33,23 @@
         print('发送失败！！')
 
 
 if __name__ == '__main__':
     print('this is a use demo')
     subject = '嘎嘎中文gaga'
     content = 'gagaga gagagaga中文中文\n' + 'gaga! gaga!'
-    send('xxxxxxx@qq.com', 'xxxxxxxxxx', 'xxxxxxx@qq.com', subject, content)
+    send_email('3544103431@qq.com', 'jbysxnfuvogjdcaj', 'cyz020403@qq.com', subject, content)
 
 '''
 qq邮箱官网教程
 
 POP3/SMTP 设置方法
 用户名/帐户： 你的QQ邮箱完整的地址
 
 密码： 生成的授权码
 
 电子邮件地址： 你的QQ邮箱的完整邮件地址
 
 接收邮件服务器： pop.qq.com，使用SSL，端口号995
 
 发送邮件服务器： smtp.qq.com，使用SSL，端口号465或587
-
-
-self.sender = '3544103431@qq.com'  # 填写邮箱地址
-self.passward = "jbysxnfuvogjdcaj"  # 填写在qq邮箱设置中获取的授权码
-
-self.receiver = 'cyz020403@qq.com'  # 填写收件人的邮箱，QQ邮箱或者其他邮箱，可多个，中间用,隔开
-
 '''
```

### Comparing `cyz-0.0.1/setup.py` & `cyz-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyz',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
-    version='0.0.1',  # 必填，项目的版本，建议遵循语义化版本规范
+    version='0.0.2',  # 必填，项目的版本，建议遵循语义化版本规范
     author='cyz020403',  # 项目的作者
     description='my utils',  # 项目的一个简短描述
     long_description=long_description,  # 项目的详细说明，通常读取 README.md 文件的内容
     long_description_content_type='text/markdown',  # 描述的格式，可选的值： text/plain, text/x-rst, and text/markdown
     author_email='cyz020403@gmail.com',  # 作者的有效邮箱地址
     url='https://github.com/cyz020403',  # 项目的源码地址
     license='MIT',
```

