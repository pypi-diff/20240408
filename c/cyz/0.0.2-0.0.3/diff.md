# Comparing `tmp/cyz-0.0.2.tar.gz` & `tmp/cyz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyz-0.0.2.tar", last modified: Mon Apr  8 07:03:16 2024, max compression
+gzip compressed data, was "cyz-0.0.3.tar", last modified: Mon Apr  8 07:22:38 2024, max compression
```

## Comparing `cyz-0.0.2.tar` & `cyz-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 07:03:16.182860 cyz-0.0.2/
--rw-rw-rw-   0        0        0      413 2024-04-08 07:03:16.182860 cyz-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-04-08 05:53:36.000000 cyz-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 07:03:16.166960 cyz-0.0.2/cyz/
--rw-rw-rw-   0        0        0       19 2024-04-08 07:01:44.000000 cyz-0.0.2/cyz/__init__.py
--rw-rw-rw-   0        0        0     2010 2024-04-08 07:02:44.000000 cyz-0.0.2/cyz/mail.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:03:16.182860 cyz-0.0.2/cyz.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-08 07:03:16.000000 cyz-0.0.2/cyz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 07:03:16.182860 cyz-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-04-08 07:02:11.000000 cyz-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:22:38.743395 cyz-0.0.3/
+-rw-rw-rw-   0        0        0      386 2024-04-08 07:22:38.736397 cyz-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2024-04-08 07:21:22.000000 cyz-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 07:22:38.727382 cyz-0.0.3/cyz/
+-rw-rw-rw-   0        0        0       19 2024-04-08 07:21:05.000000 cyz-0.0.3/cyz/__init__.py
+-rw-rw-rw-   0        0        0     3548 2024-04-08 07:20:39.000000 cyz-0.0.3/cyz/mail.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:22:38.735387 cyz-0.0.3/cyz.egg-info/
+-rw-rw-rw-   0        0        0      386 2024-04-08 07:22:38.000000 cyz-0.0.3/cyz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2024-04-08 07:22:38.000000 cyz-0.0.3/cyz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 07:22:38.000000 cyz-0.0.3/cyz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-08 07:22:38.000000 cyz-0.0.3/cyz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 07:22:38.743395 cyz-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-04-08 07:22:18.000000 cyz-0.0.3/setup.py
```

### Comparing `cyz-0.0.2/setup.py` & `cyz-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyz',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
-    version='0.0.2',  # 必填，项目的版本，建议遵循语义化版本规范
+    version='0.0.3',  # 必填，项目的版本，建议遵循语义化版本规范
     author='cyz020403',  # 项目的作者
     description='my utils',  # 项目的一个简短描述
     long_description=long_description,  # 项目的详细说明，通常读取 README.md 文件的内容
     long_description_content_type='text/markdown',  # 描述的格式，可选的值： text/plain, text/x-rst, and text/markdown
     author_email='cyz020403@gmail.com',  # 作者的有效邮箱地址
     url='https://github.com/cyz020403',  # 项目的源码地址
     license='MIT',
```

