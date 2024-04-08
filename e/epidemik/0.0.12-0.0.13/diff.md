# Comparing `tmp/epidemik-0.0.12.tar.gz` & `tmp/epidemik-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.12.tar", last modified: Sun Apr  7 18:38:03 2024, max compression
+gzip compressed data, was "epidemik-0.0.13.tar", last modified: Mon Apr  8 18:30:29 2024, max compression
```

## Comparing `epidemik-0.0.12.tar` & `epidemik-0.0.13.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.579688 epidemik-0.0.12/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.12/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5232 2024-04-07 18:38:03.579496 epidemik-0.0.12/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)     4693 2024-04-07 18:32:21.000000 epidemik-0.0.12/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      683 2024-04-07 18:37:40.000000 epidemik-0.0.12/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-07 18:38:03.579727 epidemik-0.0.12/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.577886 epidemik-0.0.12/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.578595 epidemik-0.0.12/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    17904 2024-04-06 19:09:23.000000 epidemik-0.0.12/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.12/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-06 19:09:43.000000 epidemik-0.0.12/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.579302 epidemik-0.0.12/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5232 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:30:29.415266 epidemik-0.0.13/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.13/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5356 2024-04-08 18:30:29.415089 epidemik-0.0.13/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)     4678 2024-04-07 18:39:31.000000 epidemik-0.0.13/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      782 2024-04-08 18:30:25.000000 epidemik-0.0.13/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-08 18:30:29.415306 epidemik-0.0.13/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:30:29.413262 epidemik-0.0.13/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:30:29.414040 epidemik-0.0.13/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    17904 2024-04-06 19:09:23.000000 epidemik-0.0.13/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.13/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-08 18:28:40.000000 epidemik-0.0.13/src/epidemik/__init__.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:30:29.414873 epidemik-0.0.13/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5356 2024-04-08 18:30:29.000000 epidemik-0.0.13/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      293 2024-04-08 18:30:29.000000 epidemik-0.0.13/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-08 18:30:29.000000 epidemik-0.0.13/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       64 2024-04-08 18:30:29.000000 epidemik-0.0.13/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-08 18:30:29.000000 epidemik-0.0.13/src/epidemik.egg-info/top_level.txt
```

### Comparing `epidemik-0.0.12/LICENSE` & `epidemik-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.12/PKG-INFO` & `epidemik-0.0.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.12
+Version: 0.0.13
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib>=3.8
+Requires-Dist: networkx>=3
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=2.0
+Requires-Dist: scipy>=1.10
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
 
 ---
@@ -147,17 +152,16 @@
 ## Spread The Word[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#spread)
 
 If you want to say thank you and/or support active development of the `epidemik` package:
 
 - Add a GitHub star [![epidemik](https://img.shields.io/github/stars/DataForScience/epidemik.svg?style=social&label=Star%20epidemik)](https://github.com/DataForScience/epidemik/) to the repository to encourage contributors and helps to grow our community.
 - Tweet about the project on your Twitter!
 	- Tag [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://twitter.com/bgoncalves)
-- 
 
-Thank you so much for your interest in growing the reach of the Well app!
+Thank you so much for your interest in growing our community!
 
 
 ---
 
 ## License[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#license)
 
 `epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves. Please have a look at the [LICENSE.md](LICENSE) for more details.
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.12 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.13 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # epidemik Compartmental Epidemic Models in Python --- ## Table of
-contents[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/
-images/pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) -
-[Usage](#usage) - [Contributing](#contributing) - [License](#license) --- ##
+LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
+Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 #
+epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
+(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
+(#usage) - [Contributing](#contributing) - [License](#license) --- ##
 Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
 main/images/pin.svg)](#installation) Use the package manager [pip](https://
 pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
@@ -56,14 +58,14 @@
 epidemik/main/images/pin.svg)](#spread) If you want to say thank you and/or
 support active development of the `epidemik` package: - Add a GitHub star [!
 [epidemik](https://img.shields.io/github/stars/DataForScience/
 epidemik.svg?style=social&label=Star%20epidemik)](https://github.com/
 DataForScience/epidemik/) to the repository to encourage contributors and helps
 to grow our community. - Tweet about the project on your Twitter! - Tag
 [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://
-twitter.com/bgoncalves) - Thank you so much for your interest in growing the
-reach of the Well app! --- ## License[![](https://raw.githubusercontent.com/
-DataForScience/epidemik/main/images/pin.svg)](#license) `epidemik` is free and
-open-source software licensed under the [MIT License](https://
-choosealicense.com/licenses/mit/) [2024] - Bruno GonÃ§alves. Please have a look
-at the [LICENSE.md](LICENSE) for more details.
+twitter.com/bgoncalves) Thank you so much for your interest in growing our
+community! --- ## License[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#license) `epidemik` is free and open-source
+software licensed under the [MIT License](https://choosealicense.com/licenses/
+mit/) [2024] - Bruno GonÃ§alves. Please have a look at the [LICENSE.md]
+(LICENSE) for more details.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
```

### Comparing `epidemik-0.0.12/README.md` & `epidemik-0.0.13/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -133,17 +133,16 @@
 ## Spread The Word[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#spread)
 
 If you want to say thank you and/or support active development of the `epidemik` package:
 
 - Add a GitHub star [![epidemik](https://img.shields.io/github/stars/DataForScience/epidemik.svg?style=social&label=Star%20epidemik)](https://github.com/DataForScience/epidemik/) to the repository to encourage contributors and helps to grow our community.
 - Tweet about the project on your Twitter!
 	- Tag [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://twitter.com/bgoncalves)
-- 
 
-Thank you so much for your interest in growing the reach of the Well app!
+Thank you so much for your interest in growing our community!
 
 
 ---
 
 ## License[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#license)
 
 `epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves. Please have a look at the [LICENSE.md](LICENSE) for more details.
```

#### html2text {}

```diff
@@ -49,14 +49,14 @@
 epidemik/main/images/pin.svg)](#spread) If you want to say thank you and/or
 support active development of the `epidemik` package: - Add a GitHub star [!
 [epidemik](https://img.shields.io/github/stars/DataForScience/
 epidemik.svg?style=social&label=Star%20epidemik)](https://github.com/
 DataForScience/epidemik/) to the repository to encourage contributors and helps
 to grow our community. - Tweet about the project on your Twitter! - Tag
 [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://
-twitter.com/bgoncalves) - Thank you so much for your interest in growing the
-reach of the Well app! --- ## License[![](https://raw.githubusercontent.com/
-DataForScience/epidemik/main/images/pin.svg)](#license) `epidemik` is free and
-open-source software licensed under the [MIT License](https://
-choosealicense.com/licenses/mit/) [2024] - Bruno GonÃ§alves. Please have a look
-at the [LICENSE.md](LICENSE) for more details.
+twitter.com/bgoncalves) Thank you so much for your interest in growing our
+community! --- ## License[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#license) `epidemik` is free and open-source
+software licensed under the [MIT License](https://choosealicense.com/licenses/
+mit/) [2024] - Bruno GonÃ§alves. Please have a look at the [LICENSE.md]
+(LICENSE) for more details.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
```

### Comparing `epidemik-0.0.12/pyproject.toml` & `epidemik-0.0.13/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 [project]
 name = "epidemik"
-version = "0.0.12"
+dynamic = ["version"]
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
 description = "A pakage to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
+dependencies = [
+ "matplotlib>=3.8",
+ "networkx>=3",
+ "numpy>=1.20",
+ "pandas>=2.0",
+ "scipy>=1.10"
+]
 [project.urls]
 Homepage = "https://github.com/DataForScience/epidemik"
 Issues = "https://github.com/DataForScience/epidemik/issues"
 
 [build-system]
-requires = ["setuptools>=61.0","matplotlib>=3.8","networkx>=3","numpy>=1.20","pandas>=2.0","scipy>=1.10"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools.dynamic]
+version = {attr = "epidemik.__version__"}
```

### Comparing `epidemik-0.0.12/src/epidemik/EpiModel.py` & `epidemik-0.0.13/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.12/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.13/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.12/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.13/src/epidemik.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.12
+Version: 0.0.13
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib>=3.8
+Requires-Dist: networkx>=3
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=2.0
+Requires-Dist: scipy>=1.10
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
 
 ---
@@ -147,17 +152,16 @@
 ## Spread The Word[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#spread)
 
 If you want to say thank you and/or support active development of the `epidemik` package:
 
 - Add a GitHub star [![epidemik](https://img.shields.io/github/stars/DataForScience/epidemik.svg?style=social&label=Star%20epidemik)](https://github.com/DataForScience/epidemik/) to the repository to encourage contributors and helps to grow our community.
 - Tweet about the project on your Twitter!
 	- Tag [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://twitter.com/bgoncalves)
-- 
 
-Thank you so much for your interest in growing the reach of the Well app!
+Thank you so much for your interest in growing our community!
 
 
 ---
 
 ## License[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#license)
 
 `epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves. Please have a look at the [LICENSE.md](LICENSE) for more details.
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.12 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.13 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # epidemik Compartmental Epidemic Models in Python --- ## Table of
-contents[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/
-images/pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) -
-[Usage](#usage) - [Contributing](#contributing) - [License](#license) --- ##
+LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
+Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 #
+epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
+(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
+(#usage) - [Contributing](#contributing) - [License](#license) --- ##
 Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
 main/images/pin.svg)](#installation) Use the package manager [pip](https://
 pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
@@ -56,14 +58,14 @@
 epidemik/main/images/pin.svg)](#spread) If you want to say thank you and/or
 support active development of the `epidemik` package: - Add a GitHub star [!
 [epidemik](https://img.shields.io/github/stars/DataForScience/
 epidemik.svg?style=social&label=Star%20epidemik)](https://github.com/
 DataForScience/epidemik/) to the repository to encourage contributors and helps
 to grow our community. - Tweet about the project on your Twitter! - Tag
 [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://
-twitter.com/bgoncalves) - Thank you so much for your interest in growing the
-reach of the Well app! --- ## License[![](https://raw.githubusercontent.com/
-DataForScience/epidemik/main/images/pin.svg)](#license) `epidemik` is free and
-open-source software licensed under the [MIT License](https://
-choosealicense.com/licenses/mit/) [2024] - Bruno GonÃ§alves. Please have a look
-at the [LICENSE.md](LICENSE) for more details.
+twitter.com/bgoncalves) Thank you so much for your interest in growing our
+community! --- ## License[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#license) `epidemik` is free and open-source
+software licensed under the [MIT License](https://choosealicense.com/licenses/
+mit/) [2024] - Bruno GonÃ§alves. Please have a look at the [LICENSE.md]
+(LICENSE) for more details.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
```

