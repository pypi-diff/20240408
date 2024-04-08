# Comparing `tmp/TerraLib-1.0.3.tar.gz` & `tmp/TerraLib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\Python\TerraLib\dist\tmp2lxl80m9\TerraLib-1.0.3.tar", last modified: Mon Jul 25 01:36:10 2022, max compression
+gzip compressed data, was "TerraLib-1.0.4.tar", last modified: Mon Apr  8 02:03:54 2024, max compression
```

## Comparing `TerraLib-1.0.3.tar` & `TerraLib-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-07-25 01:36:10.000000 TerraLib-1.0.3/
--rw-rw-rw-   0        0        0     1057 2022-07-25 01:36:10.000000 TerraLib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      268 2022-05-13 01:24:46.000000 TerraLib-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2022-07-25 01:36:10.000000 TerraLib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1424 2022-07-22 09:32:30.000000 TerraLib-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib/
--rw-rw-rw-   0        0        0    18380 2022-07-22 09:13:25.000000 TerraLib-1.0.3/TerraLib/TerraExcel.py
--rw-rw-rw-   0        0        0        0 2022-05-12 10:00:18.000000 TerraLib-1.0.3/TerraLib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib.egg-info/
--rw-rw-rw-   0        0        0        1 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1057 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       28 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0      221 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2022-07-25 01:36:10.000000 TerraLib-1.0.3/TerraLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 02:03:54.643240 TerraLib-1.0.4/
+-rw-rw-rw-   0        0        0     1139 2024-04-08 02:03:54.640240 TerraLib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2022-05-13 01:24:46.000000 TerraLib-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:03:54.608238 TerraLib-1.0.4/TerraLib/
+-rw-rw-rw-   0        0        0    18376 2024-04-08 01:17:00.000000 TerraLib-1.0.4/TerraLib/TerraExcel.py
+-rw-rw-rw-   0        0        0        0 2022-05-12 10:00:18.000000 TerraLib-1.0.4/TerraLib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:03:54.639243 TerraLib-1.0.4/TerraLib.egg-info/
+-rw-rw-rw-   0        0        0     1139 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:03:54.643240 TerraLib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1509 2024-04-08 02:03:48.000000 TerraLib-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TerraLib-1.0.3/PKG-INFO` & `TerraLib-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: TerraLib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common libs for use, include operation on excel, print and so on.
-Home-page: UNKNOWN
+Home-page: 
 Author: TerraJuly
 Author-email: caijie_hui@163.com
 Maintainer: TerraJuly
 Maintainer-email: caijie_hui@163.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+Requires-Dist: xlrd>=1.2.0
+Requires-Dist: openpyxl>=3.0.0
 
 # TerraLib
 
 #### 介绍
 python 常用lib
 
 #### 软件架构
@@ -36,9 +38,7 @@
 pip install TerraLib
 
 #### 使用说明
 
 安装后，可以根据自己的需要导入到自己项目中。
 
 #### 参与贡献
-
-
```

### Comparing `TerraLib-1.0.3/setup.py` & `TerraLib-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='TerraLib',  # 包名
-    version='1.0.3',  # 版本
+    version='1.0.4',  # 版本
     description="Common libs for use, include operation on excel, print and so on.",  # 包简介
     long_description=open('README.md', encoding="utf-8").read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='TerraJuly',  # 作者
     author_email='caijie_hui@163.com',  # 作者邮件
     maintainer='TerraJuly',  # 维护者
     maintainer_email='caijie_hui@163.com',  # 维护者邮件
@@ -20,12 +20,13 @@
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',  # 设置编写时的python版本
         'Programming Language :: Python :: 3.9',  # 设置编写时的python版本
+        'Programming Language :: Python :: 3.10',  # 设置编写时的python版本
     ],
     python_requires='>=3.6',  # 设置python版本要求
     install_requires=['xlrd>=1.2.0', 'openpyxl>=3.0.0']  # 安装所需要的库
 
 )
```

### Comparing `TerraLib-1.0.3/TerraLib/TerraExcel.py` & `TerraLib-1.0.4/TerraLib/TerraExcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         return (MySheet(x, self) for x in ws)
 
     def add_sheet(self, name):
         if self.excel_type == ExcelType.XLS:
             raise (f"Not support {ExcelType.XLS.value}.")
         else:
             ws = self.pre.create_sheet(title=name)
-        return MySheet(ws, self.pre)
+        return MySheet(ws, self)
 
     def remove_sheet(self, name):
         if self.excel_type == ExcelType.XLS:
             raise (f"Not support {ExcelType.XLS.value}.")
         else:
             ws = self.sheet_by_name(name).pre
             self.pre.remove(ws)
```

### Comparing `TerraLib-1.0.3/TerraLib.egg-info/PKG-INFO` & `TerraLib-1.0.4/TerraLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: TerraLib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common libs for use, include operation on excel, print and so on.
-Home-page: UNKNOWN
+Home-page: 
 Author: TerraJuly
 Author-email: caijie_hui@163.com
 Maintainer: TerraJuly
 Maintainer-email: caijie_hui@163.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+Requires-Dist: xlrd>=1.2.0
+Requires-Dist: openpyxl>=3.0.0
 
 # TerraLib
 
 #### 介绍
 python 常用lib
 
 #### 软件架构
@@ -36,9 +38,7 @@
 pip install TerraLib
 
 #### 使用说明
 
 安装后，可以根据自己的需要导入到自己项目中。
 
 #### 参与贡献
-
-
```

