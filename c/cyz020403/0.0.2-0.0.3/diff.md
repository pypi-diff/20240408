# Comparing `tmp/cyz020403-0.0.2.tar.gz` & `tmp/cyz020403-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyz020403-0.0.2.tar", last modified: Mon Apr  8 02:41:17 2024, max compression
+gzip compressed data, was "cyz020403-0.0.3.tar", last modified: Mon Apr  8 02:57:08 2024, max compression
```

## Comparing `cyz020403-0.0.2.tar` & `cyz020403-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:41:17.037690 cyz020403-0.0.2/
--rw-rw-rw-   0        0        0      235 2024-04-08 02:41:17.037690 cyz020403-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        8 2024-04-08 02:38:31.000000 cyz020403-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 02:41:17.037690 cyz020403-0.0.2/cyz020403.egg-info/
--rw-rw-rw-   0        0        0      235 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:41:16.000000 cyz020403-0.0.2/cyz020403.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 02:41:17.037690 cyz020403-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1128 2024-04-08 02:41:06.000000 cyz020403-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:57:08.085200 cyz020403-0.0.3/
+-rw-rw-rw-   0        0        0      296 2024-04-08 02:57:08.083299 cyz020403-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-04-08 02:53:05.000000 cyz020403-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:57:08.082305 cyz020403-0.0.3/cyz020403.egg-info/
+-rw-rw-rw-   0        0        0      296 2024-04-08 02:57:08.000000 cyz020403-0.0.3/cyz020403.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-08 02:57:08.000000 cyz020403-0.0.3/cyz020403.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:57:08.000000 cyz020403-0.0.3/cyz020403.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:57:08.000000 cyz020403-0.0.3/cyz020403.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:57:08.085200 cyz020403-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-08 02:54:45.000000 cyz020403-0.0.3/setup.py
```

### Comparing `cyz020403-0.0.2/setup.py` & `cyz020403-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyz020403',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
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

