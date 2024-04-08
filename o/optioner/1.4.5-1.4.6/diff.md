# Comparing `tmp/optioner-1.4.5.tar.gz` & `tmp/optioner-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.5.tar", last modified: Wed Apr  3 21:25:51 2024, max compression
+gzip compressed data, was "optioner-1.4.6.tar", last modified: Mon Apr  8 12:05:14 2024, max compression
```

## Comparing `optioner-1.4.5.tar` & `optioner-1.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:25:51.342683 optioner-1.4.5/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 21:17:25.000000 optioner-1.4.5/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 21:25:51.342313 optioner-1.4.5/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3910 2024-04-03 21:25:18.000000 optioner-1.4.5/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-03 21:17:34.000000 optioner-1.4.5/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:25:51.342752 optioner-1.4.5/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:25:51.335663 optioner-1.4.5/src/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 21:17:25.000000 optioner-1.4.5/src/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:25:51.341920 optioner-1.4.5/src/optioner.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 d33pster   (501) staff       (20)     6973 2024-04-03 21:24:07.000000 optioner-1.4.5/src/optioner.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:05:14.468043 optioner-1.4.6/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 21:17:25.000000 optioner-1.4.6/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-08 12:05:14.467644 optioner-1.4.6/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3910 2024-04-08 12:04:40.000000 optioner-1.4.6/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-08 12:04:56.000000 optioner-1.4.6/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-08 12:05:14.468110 optioner-1.4.6/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:05:14.464171 optioner-1.4.6/src/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 21:17:25.000000 optioner-1.4.6/src/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:05:14.467042 optioner-1.4.6/src/optioner.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)     6973 2024-04-03 21:24:07.000000 optioner-1.4.6/src/optioner.py
```

### Comparing `optioner-1.4.5/LICENSE` & `optioner-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.5/PKG-INFO` & `optioner-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.5
+Version: 1.4.6
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -35,27 +35,27 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # optioner
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.5
+v1.4.6
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.5 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.6 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -21,26 +21,26 @@
 d33pster,optioner,argument-parser,argument,parser,argparse Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.9 Description-Content-Type: text/markdown License-File: LICENSE # optioner
+>=3.0 Description-Content-Type: text/markdown License-File: LICENSE # optioner
 ![Static Badge](https://img.shields.io/badge/pypi-available-
 brightgreen?style=flat&logo=python&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.5
+v1.4.6
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.5/README.md` & `optioner-1.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.5
+v1.4.6
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.5
+v1.4.6
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.5/pyproject.toml` & `optioner-1.4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.5"
+version = "1.4.6"
 description = "Argument Parser"
-requires-python = ">=3.9"
+requires-python = ">=3.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `optioner-1.4.5/src/optioner.egg-info/PKG-INFO` & `optioner-1.4.6/src/optioner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.5
+Version: 1.4.6
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -35,27 +35,27 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # optioner
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.5
+v1.4.6
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.5 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.6 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -21,26 +21,26 @@
 d33pster,optioner,argument-parser,argument,parser,argparse Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.9 Description-Content-Type: text/markdown License-File: LICENSE # optioner
+>=3.0 Description-Content-Type: text/markdown License-File: LICENSE # optioner
 ![Static Badge](https://img.shields.io/badge/pypi-available-
 brightgreen?style=flat&logo=python&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.5
+v1.4.6
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.5/src/optioner.py` & `optioner-1.4.6/src/optioner.py`

 * *Files identical despite different names*

