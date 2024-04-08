# Comparing `tmp/xanalyzer-1.0.0.tar.gz` & `tmp/xanalyzer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\files\projects\xanalyzer\dist\.tmp-0dvyugp5\xanalyzer-1.0.0.tar", last modified: Sun Oct 15 05:01:29 2023, max compression
+gzip compressed data, was "xanalyzer-1.1.0.tar", last modified: Mon Apr  8 00:46:08 2024, max compression
```

## Comparing `xanalyzer-1.0.0.tar` & `xanalyzer-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/
--rw-rw-rw-   0        0        0     3617 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2023-10-11 15:20:51.000000 xanalyzer-1.0.0/README.md
--rw-rw-rw-   0        0        0      209 2023-06-17 09:05:09.000000 xanalyzer-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-06-17 10:14:32.000000 xanalyzer-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2022-03-09 15:03:39.000000 xanalyzer-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0      473 2023-01-08 01:18:58.000000 xanalyzer-1.0.0/tests/test_elf_size.py
--rw-rw-rw-   0        0        0      586 2023-09-09 13:45:17.000000 xanalyzer-1.0.0/tests/test_exe_import_api.py
--rw-rw-rw-   0        0        0     3539 2023-02-18 14:03:31.000000 xanalyzer-1.0.0/tests/test_filetype.py
--rw-rw-rw-   0        0        0     1751 2023-06-16 23:29:58.000000 xanalyzer-1.0.0/tests/test_packer.py
--rw-rw-rw-   0        0        0      594 2022-12-26 13:45:38.000000 xanalyzer-1.0.0/tests/test_pe_cert_name.py
--rw-rw-rw-   0        0        0     1101 2023-10-11 14:35:45.000000 xanalyzer-1.0.0/tests/test_pe_compile_time.py
--rw-rw-rw-   0        0        0      412 2023-06-10 14:41:58.000000 xanalyzer-1.0.0/tests/test_pe_dll_name.py
--rw-rw-rw-   0        0        0      505 2022-12-26 13:45:55.000000 xanalyzer-1.0.0/tests/test_pe_pdb.py
--rw-rw-rw-   0        0        0      797 2022-12-26 13:46:10.000000 xanalyzer-1.0.0/tests/test_pe_resource.py
--rw-rw-rw-   0        0        0      468 2022-12-26 13:46:18.000000 xanalyzer-1.0.0/tests/test_pe_size.py
--rw-rw-rw-   0        0        0      682 2022-12-26 13:46:27.000000 xanalyzer-1.0.0/tests/test_pe_versioninfo.py
--rw-rw-rw-   0        0        0     1215 2023-08-21 15:00:04.000000 xanalyzer-1.0.0/tests/test_str.py
--rw-rw-rw-   0        0        0      852 2022-12-26 13:46:32.000000 xanalyzer-1.0.0/tests/test_windows_style_file_size.py
--rw-rw-rw-   0        0        0      330 2023-08-25 15:18:05.000000 xanalyzer-1.0.0/tests/test_yara_chinese_path.py
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer/
--rw-rw-rw-   0        0        0        5 2023-10-15 04:56:33.000000 xanalyzer-1.0.0/xanalyzer/VERSION
--rw-rw-rw-   0        0        0        0 2019-12-08 16:15:13.000000 xanalyzer-1.0.0/xanalyzer/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-06-16 23:35:52.000000 xanalyzer-1.0.0/xanalyzer/config.py
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer/data/
--rw-rw-rw-   0        0        0   499634 2023-07-09 09:19:54.000000 xanalyzer-1.0.0/xanalyzer/data/UserDB.TXT
--rw-rw-rw-   0        0        0      994 2022-11-19 06:18:52.000000 xanalyzer-1.0.0/xanalyzer/data/tools_info.json
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer/data/yara_rules/
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer/data/yara_rules/packers/
--rw-rw-rw-   0        0        0      425 2023-06-16 23:32:45.000000 xanalyzer-1.0.0/xanalyzer/data/yara_rules/packers/UPX_PE.yar
--rw-rw-rw-   0        0        0    14678 2023-10-12 14:38:32.000000 xanalyzer-1.0.0/xanalyzer/file.py
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer/file_process/
--rw-rw-rw-   0        0        0        0 2019-12-08 15:36:09.000000 xanalyzer-1.0.0/xanalyzer/file_process/__init__.py
--rw-rw-rw-   0        0        0     2207 2023-06-16 23:50:03.000000 xanalyzer-1.0.0/xanalyzer/file_process/elf.py
--rw-rw-rw-   0        0        0    17852 2023-10-12 15:35:34.000000 xanalyzer-1.0.0/xanalyzer/file_process/pe.py
--rw-rw-rw-   0        0        0     2669 2023-08-20 23:45:49.000000 xanalyzer-1.0.0/xanalyzer/main.py
--rw-rw-rw-   0        0        0     7727 2023-06-16 23:50:52.000000 xanalyzer-1.0.0/xanalyzer/url.py
--rw-rw-rw-   0        0        0      729 2023-06-16 23:51:03.000000 xanalyzer-1.0.0/xanalyzer/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/
--rw-rw-rw-   0        0        0     3617 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      215 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-10-15 05:01:29.000000 xanalyzer-1.0.0/xanalyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.429550 xanalyzer-1.1.0/
+-rw-rw-rw-   0        0        0     4051 2024-04-08 00:46:08.428553 xanalyzer-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3560 2024-04-07 15:26:39.000000 xanalyzer-1.1.0/README.md
+-rw-rw-rw-   0        0        0      209 2023-06-17 09:05:09.000000 xanalyzer-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 00:46:08.430548 xanalyzer-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-04-07 14:57:32.000000 xanalyzer-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.385672 xanalyzer-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-03-09 15:03:39.000000 xanalyzer-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-01-08 01:18:58.000000 xanalyzer-1.1.0/tests/test_elf_size.py
+-rw-rw-rw-   0        0        0      586 2023-09-09 13:45:17.000000 xanalyzer-1.1.0/tests/test_exe_import_api.py
+-rw-rw-rw-   0        0        0     3606 2024-04-07 11:50:17.000000 xanalyzer-1.1.0/tests/test_filetype.py
+-rw-rw-rw-   0        0        0     1751 2023-06-16 23:29:58.000000 xanalyzer-1.1.0/tests/test_packer.py
+-rw-rw-rw-   0        0        0      594 2022-12-26 13:45:38.000000 xanalyzer-1.1.0/tests/test_pe_cert_name.py
+-rw-rw-rw-   0        0        0     1101 2023-10-11 14:35:45.000000 xanalyzer-1.1.0/tests/test_pe_compile_time.py
+-rw-rw-rw-   0        0        0      412 2023-06-10 14:41:58.000000 xanalyzer-1.1.0/tests/test_pe_dll_name.py
+-rw-rw-rw-   0        0        0      505 2022-12-26 13:45:55.000000 xanalyzer-1.1.0/tests/test_pe_pdb.py
+-rw-rw-rw-   0        0        0      797 2022-12-26 13:46:10.000000 xanalyzer-1.1.0/tests/test_pe_resource.py
+-rw-rw-rw-   0        0        0      468 2022-12-26 13:46:18.000000 xanalyzer-1.1.0/tests/test_pe_size.py
+-rw-rw-rw-   0        0        0      682 2022-12-26 13:46:27.000000 xanalyzer-1.1.0/tests/test_pe_versioninfo.py
+-rw-rw-rw-   0        0        0     1192 2024-04-07 14:43:45.000000 xanalyzer-1.1.0/tests/test_recommended_tool.py
+-rw-rw-rw-   0        0        0     1774 2024-04-07 03:09:41.000000 xanalyzer-1.1.0/tests/test_str.py
+-rw-rw-rw-   0        0        0      852 2022-12-26 13:46:32.000000 xanalyzer-1.1.0/tests/test_windows_style_file_size.py
+-rw-rw-rw-   0        0        0      330 2023-08-25 15:18:05.000000 xanalyzer-1.1.0/tests/test_yara_chinese_path.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.397636 xanalyzer-1.1.0/xanalyzer/
+-rw-rw-rw-   0        0        0        5 2024-04-07 15:04:43.000000 xanalyzer-1.1.0/xanalyzer/VERSION
+-rw-rw-rw-   0        0        0        0 2019-12-08 16:15:13.000000 xanalyzer-1.1.0/xanalyzer/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-06-16 23:35:52.000000 xanalyzer-1.1.0/xanalyzer/config.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.415588 xanalyzer-1.1.0/xanalyzer/data/
+-rw-rw-rw-   0        0        0   499634 2023-07-09 09:19:54.000000 xanalyzer-1.1.0/xanalyzer/data/UserDB.TXT
+-rw-rw-rw-   0        0        0     1162 2024-04-07 14:46:02.000000 xanalyzer-1.1.0/xanalyzer/data/tools_info.json
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.353753 xanalyzer-1.1.0/xanalyzer/data/yara_rules/
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.417582 xanalyzer-1.1.0/xanalyzer/data/yara_rules/packers/
+-rw-rw-rw-   0        0        0      425 2023-06-16 23:32:45.000000 xanalyzer-1.1.0/xanalyzer/data/yara_rules/packers/UPX_PE.yar
+-rw-rw-rw-   0        0        0    18177 2024-04-08 00:38:57.000000 xanalyzer-1.1.0/xanalyzer/file.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.424564 xanalyzer-1.1.0/xanalyzer/file_process/
+-rw-rw-rw-   0        0        0        0 2019-12-08 15:36:09.000000 xanalyzer-1.1.0/xanalyzer/file_process/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-06-16 23:50:03.000000 xanalyzer-1.1.0/xanalyzer/file_process/elf.py
+-rw-rw-rw-   0        0        0    17961 2024-04-07 14:55:58.000000 xanalyzer-1.1.0/xanalyzer/file_process/pe.py
+-rw-rw-rw-   0        0        0     2709 2024-04-07 15:22:00.000000 xanalyzer-1.1.0/xanalyzer/main.py
+-rw-rw-rw-   0        0        0     7727 2023-06-16 23:50:52.000000 xanalyzer-1.1.0/xanalyzer/url.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 23:51:03.000000 xanalyzer-1.1.0/xanalyzer/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:46:08.426559 xanalyzer-1.1.0/xanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     4051 2024-04-08 00:46:08.000000 xanalyzer-1.1.0/xanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-04-08 00:46:08.000000 xanalyzer-1.1.0/xanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 00:46:08.000000 xanalyzer-1.1.0/xanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-08 00:46:08.000000 xanalyzer-1.1.0/xanalyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      215 2024-04-08 00:46:08.000000 xanalyzer-1.1.0/xanalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 00:46:08.000000 xanalyzer-1.1.0/xanalyzer.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xanalyzer-1.0.0/PKG-INFO` & `xanalyzer-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: xanalyzer
-Version: 1.0.0
-Summary: Analyzer for files and urls
-Author: qux-bbb
-Description-Content-Type: text/markdown
-
 # xanalyzer
 
 [English](README-en.md)  
 
 简单分析文件和url，python3下运行。  
 
 1. 文件
@@ -54,15 +47,15 @@
 ```
 
 ## 使用帮助
 ```r
 usage: xanalyzer [-h] (-f FILE [FILE ...] | -u URL | --version) [-s] [--deep]
                  [--minstrlen MINSTRLEN]
 
-Process some files and urls.
+Process some files and urls. 'xa' can be used instead of 'xanalyzer'
 
 optional arguments:
   -h, --help            show this help message and exit
   -f FILE [FILE ...], --file FILE [FILE ...]
                         analyze one or more files, can be a folder path
   -u URL, --url URL     analyze the url
   --version             print version info
@@ -73,24 +66,26 @@
                         4, not less than 2
 ```
 
 ## 使用示例
 ```r
 xanalyzer -f hello.exe
 xanalyzer -u "https://www.baidu.com/s?wd=hello"
+xa -f hello.exe
 ```
 
 ## 开发
 ```r
 git clone https://github.com/qux-bbb/xanalyzer
 cd xanalyzer
-virtualenv venv
+python -m venv venv
 # windws使用虚拟环境: .\venv\Scripts\activate
 # linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.txt
+pip install -r requirements.my.txt
 python setup.py develop
 # 退出虚拟环境: deactivate
 ```
 这样之后就可以用pycharm或vscode开发调试了  
 
 ## 打包发布
 该步骤仅本人使用
```

### Comparing `xanalyzer-1.0.0/README.md` & `xanalyzer-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: xanalyzer
+Version: 1.1.0
+Summary: Analyzer for files and urls
+Author: qux-bbb
+Description-Content-Type: text/markdown
+Requires-Dist: python-magic-bin==0.4.14; platform_system == "Windows"
+Requires-Dist: python-magic==0.4.27; platform_system == "Linux"
+Requires-Dist: signify==0.5.2
+Requires-Dist: pefile==2021.9.3
+Requires-Dist: requests==2.31.0
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: pyelftools==0.28
+Requires-Dist: yara-python==4.3.1
+
 # xanalyzer
 
 [English](README-en.md)  
 
 简单分析文件和url，python3下运行。  
 
 1. 文件
@@ -47,15 +62,15 @@
 ```
 
 ## 使用帮助
 ```r
 usage: xanalyzer [-h] (-f FILE [FILE ...] | -u URL | --version) [-s] [--deep]
                  [--minstrlen MINSTRLEN]
 
-Process some files and urls.
+Process some files and urls. 'xa' can be used instead of 'xanalyzer'
 
 optional arguments:
   -h, --help            show this help message and exit
   -f FILE [FILE ...], --file FILE [FILE ...]
                         analyze one or more files, can be a folder path
   -u URL, --url URL     analyze the url
   --version             print version info
@@ -66,24 +81,26 @@
                         4, not less than 2
 ```
 
 ## 使用示例
 ```r
 xanalyzer -f hello.exe
 xanalyzer -u "https://www.baidu.com/s?wd=hello"
+xa -f hello.exe
 ```
 
 ## 开发
 ```r
 git clone https://github.com/qux-bbb/xanalyzer
 cd xanalyzer
-virtualenv venv
+python -m venv venv
 # windws使用虚拟环境: .\venv\Scripts\activate
 # linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.txt
+pip install -r requirements.my.txt
 python setup.py develop
 # 退出虚拟环境: deactivate
 ```
 这样之后就可以用pycharm或vscode开发调试了  
 
 ## 打包发布
 该步骤仅本人使用
```

### Comparing `xanalyzer-1.0.0/setup.py` & `xanalyzer-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,11 +16,12 @@
     author="qux-bbb",
     description="Analyzer for files and urls",
     long_description=open("README.md", "r", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "xanalyzer = xanalyzer.main:main",
+            "xa = xanalyzer.main:main",
         ],
     },
     install_requires=open("requirements.txt", "r").read().split("\n"),
 )
```

### Comparing `xanalyzer-1.0.0/tests/test_exe_import_api.py` & `xanalyzer-1.1.0/tests/test_exe_import_api.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/tests/test_filetype.py` & `xanalyzer-1.1.0/tests/test_filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         # Windows可执行文件
         "Hello64.exe_",
         "Hello64.dll_",
         "Hello64.sys_",
         "Hello32.exe_",
         "Hello32.dll_",
         "Hello32.sys_",
+        # 一些Windows程序安装包
+        "SetupTest.msi_",
         # 安卓
         "app-debug.apk_",
         # pdf
         "hello.pdf_",
         # 图片
         "hello.png_",
         "hello.jpg_",
```

### Comparing `xanalyzer-1.0.0/tests/test_packer.py` & `xanalyzer-1.1.0/tests/test_packer.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/tests/test_pe_cert_name.py` & `xanalyzer-1.1.0/tests/test_pe_cert_name.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/tests/test_pe_compile_time.py` & `xanalyzer-1.1.0/tests/test_pe_compile_time.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/tests/test_pe_resource.py` & `xanalyzer-1.1.0/tests/test_pe_resource.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/tests/test_pe_versioninfo.py` & `xanalyzer-1.1.0/tests/test_pe_versioninfo.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/tests/test_str.py` & `xanalyzer-1.1.0/tests/test_str.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,24 @@
     assert file_analyzer.get_wide_strs() == [
         b"4\x004\x004\x004\x00",
         b"5\x005\x005\x005\x005\x00",
     ]
 
     file_analyzer = FileAnalyzer(file_path=pe_path, minstrlen=5)
     assert file_analyzer.get_wide_strs() == [b"5\x005\x005\x005\x005\x00"]
+
+
+def test_special_str():
+    pe_path = cur_dir_path / "test_data" / "special_str.txt"
+
+    file_analyzer = FileAnalyzer(file_path=pe_path)
+    assert file_analyzer.get_special_strs() == [b"aGVsbG8=", b"68656c6c6f"]
+
+
+def test_special_wide_str():
+    pe_path = cur_dir_path / "test_data" / "special_wide_str.txt"
+
+    file_analyzer = FileAnalyzer(file_path=pe_path)
+    assert file_analyzer.get_special_wide_strs() == [
+        b"a\x00G\x00V\x00s\x00b\x00G\x008\x00=\x00",
+        b"6\x008\x006\x005\x006\x00c\x006\x00c\x006\x00f\x00",
+    ]
```

### Comparing `xanalyzer-1.0.0/tests/test_windows_style_file_size.py` & `xanalyzer-1.1.0/tests/test_windows_style_file_size.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/xanalyzer/config.py` & `xanalyzer-1.1.0/xanalyzer/config.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/xanalyzer/data/UserDB.TXT` & `xanalyzer-1.1.0/xanalyzer/data/UserDB.TXT`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/xanalyzer/data/tools_info.json` & `xanalyzer-1.1.0/xanalyzer/data/tools_info.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8636363636363636%*

 * *Differences: {"'7z-build-nsis'": "'https://github.com/myfreeer/7z-build-nsis'",*

 * * "'Innounp'": "'https://innounp.sourceforge.net'",*

 * * "'lessmsi'": "'http://lessmsi.activescott.com'"}*

```diff
@@ -1,21 +1,24 @@
 {
+    "7z-build-nsis": "https://github.com/myfreeer/7z-build-nsis",
     "BruteShark": "https://github.com/jilvan1234/BruteShark",
     "Cutter": "https://cutter.re",
     "DIE": "https://github.com/horsicq/Detect-It-Easy",
     "Ghidra": "https://ghidra-sre.org",
     "IDA": "https://hex-rays.com",
+    "Innounp": "https://innounp.sourceforge.net",
     "JADX": "https://github.com/skylot/jadx",
     "Microsoft Office Excel": "https://www.office.com",
     "Microsoft Office PowerPoint": "https://www.office.com",
     "Microsoft Office Word": "https://www.office.com",
     "PyInstaller Extractor": "https://github.com/extremecoders-re/pyinstxtractor",
     "Resource Hacker": "http://www.angusj.com/resourcehacker",
     "UPX": "https://upx.github.io",
     "WPS Office": "https://www.wps.cn",
     "Wireshark": "https://www.wireshark.org",
     "XELFViewer": "https://github.com/horsicq/XELFViewer",
     "XPEViewer": "https://github.com/horsicq/XPEViewer",
     "dnSpy": "https://github.com/dnSpyEx/dnSpy",
+    "lessmsi": "http://lessmsi.activescott.com",
     "oletools": "https://github.com/decalage2/oletools",
     "x64dbg": "https://x64dbg.com"
 }
```

### Comparing `xanalyzer-1.0.0/xanalyzer/file.py` & `xanalyzer-1.1.0/xanalyzer/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,27 +30,26 @@
 
         minstrlen_bytes = str(minstrlen).encode()
         self.str_re = re.compile(rb"[\x20-\x7e]{"+minstrlen_bytes+rb",}")
         self.wide_str_re = re.compile(rb"(?:[\x20-\x7e]\x00){"+minstrlen_bytes+rb",}")
 
         self.packer_list = []
         self.pe_resource_type_list = []
+        self.pe_versioninfo = []
 
         self.init_packer_yara_rules()
 
     @classmethod
     def init_packer_yara_rules(cls):
         if cls.packer_yara_rules:
             return
         yara_filenames = os.listdir(Config.packer_yara_rules_path)
         yara_dict = {}
         for yara_filename in yara_filenames:
-            yara_path = os.path.join(
-                Config.packer_yara_rules_path, yara_filename
-            )
+            yara_path = os.path.join(Config.packer_yara_rules_path, yara_filename)
             yara_dict[yara_filename] = yara_path
         cls.packer_yara_rules = yara.compile(filepaths=yara_dict)
 
     def packer_yara_match(self):
         the_file = open(self.file_path, "rb")
         the_content = the_file.read()
         the_file.close()
@@ -76,15 +75,17 @@
                     the_file_type = "Microsoft Word 2007+"
                 elif "xl/workbook.xml" in zip_namelist:
                     the_file_type = "Microsoft Excel 2007+"
                 elif "ppt/presentation.xml" in zip_namelist:
                     the_file_type = "Microsoft PowerPoint 2007+"
 
         if the_file_type.startswith("Composite Document File V2 Document"):
-            if "WordDocument".encode("utf_16_le") in the_content:
+            if "MSI Installer" in the_file_type:
+                the_ext = [".msi"]
+            elif "WordDocument".encode("utf_16_le") in the_content:
                 if "Name of Creating Application: WPS" in the_file_type:
                     the_ext = [".doc", ".wps"]
                 else:
                     the_ext = [".doc"]
             elif "Workbook".encode("utf_16_le") in the_content:
                 if "Name of Creating Application: WPS" in the_file_type:
                     the_ext = [".xls", ".et"]
@@ -216,21 +217,67 @@
     def get_wide_strs(self):
         the_file = open(self.file_path, "rb")
         file_content = the_file.read()
         the_file.close()
         all_strs = re.findall(self.wide_str_re, file_content)
         return all_strs
 
+    def get_special_strs(self):
+        the_file = open(self.file_path, "rb")
+        file_content = the_file.read()
+        the_file.close()
+        tmp_base64_strs = re.findall(rb"[A-Za-z0-9+/]{6,}={1,2}", file_content)
+        possible_base64_strs = []
+        for tmp_base64_str in tmp_base64_strs:
+            # 过滤hex字符串
+            if re.match(rb"(?:[A-Fa-f0-9]{2}){4,}", tmp_base64_str):
+                continue
+            possible_base64_strs.append(tmp_base64_str)
+        hex_strs = re.findall(rb"(?:[A-Fa-f0-9]{2}){4,}", file_content)
+        special_strs = possible_base64_strs + hex_strs
+        return special_strs
+
+    def get_special_wide_strs(self):
+        the_file = open(self.file_path, "rb")
+        file_content = the_file.read()
+        the_file.close()
+        tmp_base64_strs = re.findall(
+            rb"(?:[A-Za-z0-9+/]\x00){6,}(?:=\x00){1,2}",
+            file_content,
+        )
+        possible_base64_strs = []
+        for tmp_base64_str in tmp_base64_strs:
+            # 过滤hex字符串
+            if re.match(rb"(?:(?:[A-Fa-f0-9]\x00){2}){4,}", tmp_base64_str):
+                continue
+            possible_base64_strs.append(tmp_base64_str)
+        hex_strs = re.findall(rb"(?:(?:[A-Fa-f0-9]\x00){2}){4,}", file_content)
+        special_wide_strs = possible_base64_strs + hex_strs
+        return special_wide_strs
+
     def get_tool_recommendations(self):
         recommended_tool_names = []
 
         if self.file_type.startswith(("PE", "MS-DOS executable")):
             recommended_tool_names.append("XPEViewer")
+
+            for item in self.pe_versioninfo:
+                if (
+                    item["name"] == "Comments"
+                    and item["value"] == "This installation was built with Inno Setup."
+                ):
+                    recommended_tool_names.append("Innounp")
+                    break
+
             if "Mono/.Net assembly" in self.file_type:
                 recommended_tool_names.append("dnSpy")
+
+            if "Nullsoft Installer" in self.file_type:
+                recommended_tool_names.append("7z-build-nsis")
+
             for extension in [
                 ".ico",
                 ".png",
                 ".jpg",
                 ".bmp",
                 ".gif",
                 ".exe",
@@ -271,14 +318,16 @@
             if packer.startswith("UPX "):
                 recommended_tool_names.append("UPX")
             if packer.startswith("PyInstaller,"):
                 recommended_tool_names.append("PyInstaller Extractor")
 
         if ".xls" in self.possible_extension_names:
             recommended_tool_names.append("oletools")
+        elif ".msi" in self.possible_extension_names:
+            recommended_tool_names.append("lessmsi")
 
         with open(Config.tools_info_path, "r") as f:
             tools_info = json.load(f)
         recommended_tool_info_list = []
         for recommended_tool_name in recommended_tool_names:
             recommended_tool_info_list.append(
                 f"{recommended_tool_name}: {tools_info.get(recommended_tool_name)}"
@@ -308,24 +357,56 @@
                     Config.conf["analyze_data_path"], wide_str_file_name
                 )
                 with open(wide_str_data_path, "wb") as f:
                     for a_str in all_wide_strs:
                         f.write(a_str + b"\n\x00")
                 log.info(f"{wide_str_file_name} saved")
 
-                wide_to_normal_str_file_name = Path(self.file_path).name + "_wide_to_normal_strings.txt"
+                wide_to_normal_str_file_name = (
+                    Path(self.file_path).name + "_wide_to_normal_strings.txt"
+                )
                 wide_to_normal_str_data_path = os.path.join(
                     Config.conf["analyze_data_path"], wide_to_normal_str_file_name
                 )
                 with open(wide_to_normal_str_data_path, "wb") as f:
                     for a_str in all_wide_strs:
                         normal_str = a_str.replace(b"\x00", b"")
                         f.write(normal_str + b"\n")
                 log.info(f"{wide_to_normal_str_file_name} saved")
 
+        special_strs = self.get_special_strs()
+        if special_strs:
+            log.info(f"special strs num: {len(special_strs)}")
+            if Config.conf["save_flag"]:
+                special_str_file_name = (
+                    Path(self.file_path).name + "_special_strings.txt"
+                )
+                str_data_path = os.path.join(
+                    Config.conf["analyze_data_path"], special_str_file_name
+                )
+                with open(str_data_path, "wb") as f:
+                    for a_str in special_strs:
+                        f.write(a_str + b"\n")
+                log.info(f"{special_str_file_name} saved")
+
+        special_wide_strs = self.get_special_wide_strs()
+        if special_wide_strs:
+            log.info(f"special wide str num: {len(special_wide_strs)}")
+            if Config.conf["save_flag"]:
+                special_wide_str_file_name = (
+                    Path(self.file_path).name + "_special_wide_strings.txt"
+                )
+                special_wide_str_data_path = os.path.join(
+                    Config.conf["analyze_data_path"], special_wide_str_file_name
+                )
+                with open(special_wide_str_data_path, "wb") as f:
+                    for a_str in special_wide_strs:
+                        f.write(a_str + b"\n\x00")
+                log.info(f"{special_wide_str_file_name} saved")
+
     def tool_recommendations_scan(self):
         recommended_tool_info_list = self.get_tool_recommendations()
         if recommended_tool_info_list:
             log.info("recommended tool info:")
             for recommended_tool_info in recommended_tool_info_list:
                 log.info(f"    {recommended_tool_info}")
```

### Comparing `xanalyzer-1.0.0/xanalyzer/file_process/elf.py` & `xanalyzer-1.1.0/xanalyzer/file_process/elf.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/xanalyzer/file_process/pe.py` & `xanalyzer-1.1.0/xanalyzer/file_process/pe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 
 import pefile
 import peutils
 from signify.authenticode.signed_pe import SignedPEFile
 
 from xanalyzer.config import Config
@@ -103,15 +103,17 @@
                 except Exception as e:
                     log.error(e, exc_info=True)
                     continue
 
         return versioninfo
 
     def get_compile_time(self):
-        compile_time = datetime.utcfromtimestamp(self.pe_file.FILE_HEADER.TimeDateStamp)
+        compile_time = datetime.fromtimestamp(
+            self.pe_file.FILE_HEADER.TimeDateStamp, tz=timezone.utc
+        )
         time_str = compile_time.strftime("%Y-%m-%d %H:%M:%S UTC")
         return time_str
 
     def get_pdb_path(self):
         for debug_entry in getattr(self.pe_file, "DIRECTORY_ENTRY_DEBUG", []):
             if hasattr(debug_entry.entry, "PdbFileName"):
                 return debug_entry.entry.PdbFileName.strip(b"\x00").decode("utf8")
@@ -321,14 +323,15 @@
 
     def versioninfo_scan(self):
         """
         查看pe版本信息
         """
         versioninfo = self.get_versioninfo()
         if versioninfo:
+            self.file_analyzer.pe_versioninfo = versioninfo
             log.info("versioninfo:")
             for item in versioninfo:
                 log.info('    "{}": "{}"'.format(item["name"], item["value"]))
 
     def section_name_scan(self):
         """
         输出节区名
```

### Comparing `xanalyzer-1.0.0/xanalyzer/main.py` & `xanalyzer-1.1.0/xanalyzer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     if not a_path:  # 空文件夹，提示一下
         log.warning(f"folder is empty: {the_path}")
 
 
 def main():
     parser = argparse.ArgumentParser(
-        prog="xanalyzer", description="Process some files and urls."
+        prog="xanalyzer", description="Process some files and urls. 'xa' can be used instead of 'xanalyzer'"
     )
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument(
         "-f",
         "--file",
         nargs="+",
         help="analyze one or more files, can be a folder path",
```

### Comparing `xanalyzer-1.0.0/xanalyzer/url.py` & `xanalyzer-1.1.0/xanalyzer/url.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/xanalyzer/utils.py` & `xanalyzer-1.1.0/xanalyzer/utils.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-1.0.0/xanalyzer.egg-info/PKG-INFO` & `xanalyzer-1.1.0/xanalyzer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Metadata-Version: 2.1
 Name: xanalyzer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Analyzer for files and urls
 Author: qux-bbb
 Description-Content-Type: text/markdown
+Requires-Dist: python-magic-bin==0.4.14; platform_system == "Windows"
+Requires-Dist: python-magic==0.4.27; platform_system == "Linux"
+Requires-Dist: signify==0.5.2
+Requires-Dist: pefile==2021.9.3
+Requires-Dist: requests==2.31.0
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: pyelftools==0.28
+Requires-Dist: yara-python==4.3.1
 
 # xanalyzer
 
 [English](README-en.md)  
 
 简单分析文件和url，python3下运行。  
 
@@ -54,15 +62,15 @@
 ```
 
 ## 使用帮助
 ```r
 usage: xanalyzer [-h] (-f FILE [FILE ...] | -u URL | --version) [-s] [--deep]
                  [--minstrlen MINSTRLEN]
 
-Process some files and urls.
+Process some files and urls. 'xa' can be used instead of 'xanalyzer'
 
 optional arguments:
   -h, --help            show this help message and exit
   -f FILE [FILE ...], --file FILE [FILE ...]
                         analyze one or more files, can be a folder path
   -u URL, --url URL     analyze the url
   --version             print version info
@@ -73,24 +81,26 @@
                         4, not less than 2
 ```
 
 ## 使用示例
 ```r
 xanalyzer -f hello.exe
 xanalyzer -u "https://www.baidu.com/s?wd=hello"
+xa -f hello.exe
 ```
 
 ## 开发
 ```r
 git clone https://github.com/qux-bbb/xanalyzer
 cd xanalyzer
-virtualenv venv
+python -m venv venv
 # windws使用虚拟环境: .\venv\Scripts\activate
 # linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.txt
+pip install -r requirements.my.txt
 python setup.py develop
 # 退出虚拟环境: deactivate
 ```
 这样之后就可以用pycharm或vscode开发调试了  
 
 ## 打包发布
 该步骤仅本人使用
```

### Comparing `xanalyzer-1.0.0/xanalyzer.egg-info/SOURCES.txt` & `xanalyzer-1.1.0/xanalyzer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 tests/test_pe_cert_name.py
 tests/test_pe_compile_time.py
 tests/test_pe_dll_name.py
 tests/test_pe_pdb.py
 tests/test_pe_resource.py
 tests/test_pe_size.py
 tests/test_pe_versioninfo.py
+tests/test_recommended_tool.py
 tests/test_str.py
 tests/test_windows_style_file_size.py
 tests/test_yara_chinese_path.py
 xanalyzer/VERSION
 xanalyzer/__init__.py
 xanalyzer/config.py
 xanalyzer/file.py
```

