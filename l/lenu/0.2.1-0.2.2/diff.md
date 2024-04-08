# Comparing `tmp/lenu-0.2.1.tar.gz` & `tmp/lenu-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenu-0.2.1.tar", max compression
+gzip compressed data, was "lenu-0.2.2.tar", max compression
```

## Comparing `lenu-0.2.1.tar` & `lenu-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     7048 2022-05-10 15:15:50.116411 lenu-0.2.1/LICENSE
--rw-r--r--   0        0        0     4991 2023-01-30 16:06:56.652153 lenu-0.2.1/README.md
--rw-r--r--   0        0        0        0 2021-11-29 09:56:19.182000 lenu-0.2.1/lenu/__init__.py
--rw-r--r--   0        0        0     6399 2023-01-30 15:34:11.992507 lenu-0.2.1/lenu/console.py
--rw-r--r--   0        0        0   660062 2022-05-05 10:03:14.900000 lenu-0.2.1/lenu/data/2021-10-21-elf-code-list-v1.4.1.csv
--rw-r--r--   0        0        0     3457 2023-01-30 11:11:29.221047 lenu-0.2.1/lenu/data/__init__.py
--rw-r--r--   0        0        0     4151 2023-01-30 11:11:29.221366 lenu-0.2.1/lenu/data/elf_codes.py
--rw-r--r--   0        0        0     2250 2022-05-05 09:14:00.936000 lenu-0.2.1/lenu/data/goldencopyfiles.py
--rw-r--r--   0        0        0      960 2022-05-05 08:15:45.634000 lenu-0.2.1/lenu/data/lei.py
--rw-r--r--   0        0        0        0 2022-03-22 11:21:24.514000 lenu-0.2.1/lenu/ml/__init__.py
--rw-r--r--   0        0        0     2779 2022-05-05 08:43:53.478000 lenu-0.2.1/lenu/ml/cnames.py
--rw-r--r--   0        0        0      752 2022-05-10 19:31:30.806755 lenu-0.2.1/lenu/ml/eval.py
--rw-r--r--   0        0        0     1653 2023-01-30 11:11:29.221667 lenu-0.2.1/lenu/ml/features.py
--rw-r--r--   0        0        0     2134 2022-05-10 19:31:17.701763 lenu-0.2.1/lenu/ml/models.py
--rw-r--r--   0        0        0     5420 2023-01-30 15:34:11.976924 lenu-0.2.1/lenu/ml/pipelines.py
--rw-r--r--   0        0        0        0 2022-03-22 12:48:45.833000 lenu-0.2.1/lenu/ml/test/__init__.py
--rw-r--r--   0        0        0     1211 2022-05-10 16:11:22.422000 lenu-0.2.1/lenu/ml/test/test_features.py
--rw-r--r--   0        0        0     1031 2023-01-30 15:34:11.866522 lenu-0.2.1/lenu/modelhub.py
--rw-r--r--   0        0        0      820 2023-01-30 15:03:01.916598 lenu-0.2.1/lenu/util.py
--rw-r--r--   0        0        0      840 2023-01-30 16:06:56.652511 lenu-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6120 1970-01-01 00:00:00.000000 lenu-0.2.1/setup.py
--rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 lenu-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7048 2022-05-10 15:15:50.116411 lenu-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4991 2024-04-08 10:04:06.615367 lenu-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2021-11-29 09:56:19.182000 lenu-0.2.2/lenu/__init__.py
+-rw-r--r--   0        0        0     6399 2023-01-30 15:34:11.992507 lenu-0.2.2/lenu/console.py
+-rw-r--r--   0        0        0   660062 2022-05-05 10:03:14.900000 lenu-0.2.2/lenu/data/2021-10-21-elf-code-list-v1.4.1.csv
+-rw-r--r--   0        0        0     3457 2023-01-30 11:11:29.221047 lenu-0.2.2/lenu/data/__init__.py
+-rw-r--r--   0        0        0     4151 2023-01-30 11:11:29.221366 lenu-0.2.2/lenu/data/elf_codes.py
+-rw-r--r--   0        0        0     2250 2022-05-05 09:14:00.936000 lenu-0.2.2/lenu/data/goldencopyfiles.py
+-rw-r--r--   0        0        0      960 2022-05-05 08:15:45.634000 lenu-0.2.2/lenu/data/lei.py
+-rw-r--r--   0        0        0        0 2022-03-22 11:21:24.514000 lenu-0.2.2/lenu/ml/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-08 09:39:23.494396 lenu-0.2.2/lenu/ml/cnames.py
+-rw-r--r--   0        0        0      752 2022-05-10 19:31:30.806755 lenu-0.2.2/lenu/ml/eval.py
+-rw-r--r--   0        0        0     1653 2023-01-30 11:11:29.221667 lenu-0.2.2/lenu/ml/features.py
+-rw-r--r--   0        0        0     2134 2022-05-10 19:31:17.701763 lenu-0.2.2/lenu/ml/models.py
+-rw-r--r--   0        0        0     5420 2023-04-19 13:35:02.900444 lenu-0.2.2/lenu/ml/pipelines.py
+-rw-r--r--   0        0        0        0 2022-03-22 12:48:45.833000 lenu-0.2.2/lenu/ml/test/__init__.py
+-rw-r--r--   0        0        0     1211 2022-05-10 16:11:22.422000 lenu-0.2.2/lenu/ml/test/test_features.py
+-rw-r--r--   0        0        0     1031 2023-01-30 15:34:11.866522 lenu-0.2.2/lenu/modelhub.py
+-rw-r--r--   0        0        0      820 2023-01-30 15:03:01.916598 lenu-0.2.2/lenu/util.py
+-rw-r--r--   0        0        0      840 2024-04-08 10:06:53.881976 lenu-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6120 1970-01-01 00:00:00.000000 lenu-0.2.2/setup.py
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 lenu-0.2.2/PKG-INFO
```

### Comparing `lenu-0.2.1/LICENSE` & `lenu-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/README.md` & `lenu-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <h1 align="center">
-lenu - Legal Entity Name Understanding 
+LENU - Legal Entity Name Understanding 
 </h1>
 
 ---------------
 
 <h1 align="center">
 <a href="https://gleif.org">
 <img src="http://sdglabs.ai/wp-content/uploads/2022/07/gleif-logo-new.png" width="220" alt="">
@@ -20,15 +20,15 @@
 ---------------
 
 [![License](https://img.shields.io/github/license/Sociovestix/lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/LICENSE)
 ![](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-**lenu** is a python library that helps to understand and work with Legal Entity Names
+**LENU** is a python library that helps to understand and work with Legal Entity Names
 in the context of the [Legal Entity Identifier](https://www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei) (LEI) Standard (ISO 17441)
 as well as the [Entity Legal Form (ELF) Code List](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) Standard (ISO 20275).  
 
 The library utilizes Machine Learning with Transformers and scikit-learn. It provides and utilizes pre-trained ELF Detection models published at https://huggingface.co/Sociovestix. This code as well as the LEI data and models are distributed under Creative Commons Zero 1.0 Universal license.
 
 The project was started in November 2021 as a collaboration of the [Global Legal Entity Identifier Foundation](https://gleif.org) (GLEIF) and
 [Sociovestix Labs](https://sociovestix.com) with the goal to explore how Machine Learning can support in detecting the legal form (ELF Code) from a legal name. 
@@ -36,15 +36,15 @@
 It provides:
 - an interface to download [LEI](https://www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy#/) and [ELF Code](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) data from GLEIF's public website
 - an interface to train and make use of Machine Learning models to classify ELF Codes from given Legal Names
 - an interface to use pre-trained ELF Detection models published on https://huggingface.co/Sociovestix
 ---
 
 ## Dependencies
-**lenu** requires
+**LENU** requires
 - python (>=3.8, <3.10)
 - [scikit-learn](https://scikit-learn.org/) - Provides Machine Learning functionality for token based modelling
 - [transformers](https://huggingface.co/docs/transformers/index) - Download and applying Neural Network Models
 - [pytorch](https://pytorch.org/) - Machine Learning Framework to train Neural Network Models
 - [pandas](https://pandas.pydata.org/) - For reading and handling data
 - [Typer](https://typer.tiangolo.com/) - Adds the command line interface
 - [requests](https://docs.python-requests.org/en/latest/) and [pydantic](https://pydantic-docs.helpmanual.io/) - For downloading LEI data from GLEIF's website
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-             ************ lleennuu -- LLeeggaall EEnnttiittyy NNaammee UUnnddeerrssttaannddiinngg ************
+             ************ LLEENNUU -- LLeeggaall EEnnttiittyy NNaammee UUnnddeerrssttaannddiinngg ************
 ---------------
 
                         ******** iinn ccoollllaabboorraattiioonn wwiitthh ********
        ************ _[[_hh_tt_tt_pp_ss_::_//_//_ss_oo_cc_ii_oo_vv_ee_ss_tt_ii_xx_.._cc_oo_mm_//_ii_mm_gg_//_ss_vv_ll____ll_oo_gg_oo____cc_ee_nn_tt_ee_rr_ee_dd_.._ss_vv_gg_]] ************
 
 --------------- [![License](https://img.shields.io/github/license/Sociovestix/
 lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/LICENSE) ![](https://
 img.shields.io/badge/python-3.8%20%7C%203.9-blue) [![Code style: black](https:/
 /img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-black) **lenu** is a python library that helps to understand and work with
+black) **LENU** is a python library that helps to understand and work with
 Legal Entity Names in the context of the [Legal Entity Identifier](https://
 www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei) (LEI)
 Standard (ISO 17441) as well as the [Entity Legal Form (ELF) Code List](https:/
 /www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list)
 Standard (ISO 20275). The library utilizes Machine Learning with Transformers
 and scikit-learn. It provides and utilizes pre-trained ELF Detection models
 published at https://huggingface.co/Sociovestix. This code as well as the LEI
@@ -23,15 +23,15 @@
 Machine Learning can support in detecting the legal form (ELF Code) from a
 legal name. It provides: - an interface to download [LEI](https://
 www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy#/) and
 [ELF Code](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-
 legal-forms-code-list) data from GLEIF's public website - an interface to train
 and make use of Machine Learning models to classify ELF Codes from given Legal
 Names - an interface to use pre-trained ELF Detection models published on
-https://huggingface.co/Sociovestix --- ## Dependencies **lenu** requires -
+https://huggingface.co/Sociovestix --- ## Dependencies **LENU** requires -
 python (>=3.8, <3.10) - [scikit-learn](https://scikit-learn.org/) - Provides
 Machine Learning functionality for token based modelling - [transformers]
 (https://huggingface.co/docs/transformers/index) - Download and applying Neural
 Network Models - [pytorch](https://pytorch.org/) - Machine Learning Framework
 to train Neural Network Models - [pandas](https://pandas.pydata.org/) - For
 reading and handling data - [Typer](https://typer.tiangolo.com/) - Adds the
 command line interface - [requests](https://docs.python-requests.org/en/latest/
```

### Comparing `lenu-0.2.1/lenu/console.py` & `lenu-0.2.2/lenu/console.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/data/2021-10-21-elf-code-list-v1.4.1.csv` & `lenu-0.2.2/lenu/data/2021-10-21-elf-code-list-v1.4.1.csv`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/data/__init__.py` & `lenu-0.2.2/lenu/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/data/elf_codes.py` & `lenu-0.2.2/lenu/data/elf_codes.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/data/goldencopyfiles.py` & `lenu-0.2.2/lenu/data/goldencopyfiles.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/data/lei.py` & `lenu-0.2.2/lenu/data/lei.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/ml/cnames.py` & `lenu-0.2.2/lenu/ml/cnames.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 # coding=utf-8
 
 import unicodedata
 import numpy
 
 
+def _rmdiacritics(char):
+    '''
+    Return the base character of char, by "removing" any
+    diacritics like accents or curls and strokes and the like.
+    '''
+    # https://stackoverflow.com/a/15547803/3264997
+    desc = unicodedata.name(char)
+    cutoff = desc.find(' WITH ')
+    if cutoff != -1:
+        desc = desc[:cutoff]
+        try:
+            char = unicodedata.lookup(desc)
+        except KeyError:
+            pass  # removing "WITH ..." produced an invalid name
+    return char
+
+
 def _replace_diacritics(s):
-    # lambda x : x.replace(u'ø', u'o').replace(u'æ', u'ae'),
-    # what about ü,ö,ä,...
-    return unicodedata.normalize("NFKD", s).encode("ASCII", "ignore").decode("utf-8")
+    return "".join([_rmdiacritics(c) for c in s])
 
 
 def _replace_multi_spaces(s):
     while "  " in s:
         s = s.replace("  ", " ")
     return s
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lenu-0.2.1/lenu/ml/eval.py` & `lenu-0.2.2/lenu/ml/eval.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/ml/features.py` & `lenu-0.2.2/lenu/ml/features.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/ml/models.py` & `lenu-0.2.2/lenu/ml/models.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/ml/pipelines.py` & `lenu-0.2.2/lenu/ml/pipelines.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/ml/test/test_features.py` & `lenu-0.2.2/lenu/ml/test/test_features.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/modelhub.py` & `lenu-0.2.2/lenu/modelhub.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/lenu/util.py` & `lenu-0.2.2/lenu/util.py`

 * *Files identical despite different names*

### Comparing `lenu-0.2.1/pyproject.toml` & `lenu-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lenu"
-version = "0.2.1"
+version = "0.2.2"
 description = "Legal Entity Name Understanding"
 readme = "README.md"
 authors = [
     "aarimond <alexander.arimond@sociovestix.com>"
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `lenu-0.2.1/setup.py` & `lenu-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'types-requests>=2.27.16,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['lenu = lenu.console:app']}
 
 setup_kwargs = {
     'name': 'lenu',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Legal Entity Name Understanding',
-    'long_description': '\n<h1 align="center">\nlenu - Legal Entity Name Understanding \n</h1>\n\n---------------\n\n<h1 align="center">\n<a href="https://gleif.org">\n<img src="http://sdglabs.ai/wp-content/uploads/2022/07/gleif-logo-new.png" width="220" alt="">\n</a>\n</h1><br>\n<h3 align="center">in collaboration with</h3> \n<h1 align="center">\n<a href="https://sociovestix.com">\n<img src="https://sociovestix.com/img/svl_logo_centered.svg" width="700px">\n</a>\n</h1><br>\n\n---------------\n\n[![License](https://img.shields.io/github/license/Sociovestix/lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/LICENSE)\n![](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n**lenu** is a python library that helps to understand and work with Legal Entity Names\nin the context of the [Legal Entity Identifier](https://www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei) (LEI) Standard (ISO 17441)\nas well as the [Entity Legal Form (ELF) Code List](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) Standard (ISO 20275).  \n\nThe library utilizes Machine Learning with Transformers and scikit-learn. It provides and utilizes pre-trained ELF Detection models published at https://huggingface.co/Sociovestix. This code as well as the LEI data and models are distributed under Creative Commons Zero 1.0 Universal license.\n\nThe project was started in November 2021 as a collaboration of the [Global Legal Entity Identifier Foundation](https://gleif.org) (GLEIF) and\n[Sociovestix Labs](https://sociovestix.com) with the goal to explore how Machine Learning can support in detecting the legal form (ELF Code) from a legal name. \n\nIt provides:\n- an interface to download [LEI](https://www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy#/) and [ELF Code](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) data from GLEIF\'s public website\n- an interface to train and make use of Machine Learning models to classify ELF Codes from given Legal Names\n- an interface to use pre-trained ELF Detection models published on https://huggingface.co/Sociovestix\n---\n\n## Dependencies\n**lenu** requires\n- python (>=3.8, <3.10)\n- [scikit-learn](https://scikit-learn.org/) - Provides Machine Learning functionality for token based modelling\n- [transformers](https://huggingface.co/docs/transformers/index) - Download and applying Neural Network Models\n- [pytorch](https://pytorch.org/) - Machine Learning Framework to train Neural Network Models\n- [pandas](https://pandas.pydata.org/) - For reading and handling data\n- [Typer](https://typer.tiangolo.com/) - Adds the command line interface\n- [requests](https://docs.python-requests.org/en/latest/) and [pydantic](https://pydantic-docs.helpmanual.io/) - For downloading LEI data from GLEIF\'s website\n\n## Installation\n\nvia PyPI:\n```shell\npip install lenu\n```\n\nFrom github:\n```shell\npip install https://github.com/Sociovestix/lenu\n```\n\nEditable install from locally cloned repository\n```shell\ngit clone https://github.com/Sociovestix/lenu\npip install -e lenu\n```\n\n## Usage\n\nCreate folders for LEI and ELF Code data and to store your models\n\n```shell\nmkdir data\nmkdir models\n```\n\nDownload LEI data and ELF Code data into your `data` folder\n```shell\nlenu download\n```\n\nTrain a (default) ELF Code Classification model. An ELF Classification model is always Jurisdiction specific and \nwill be trained from Legal Names from this Jurisdiction.\n\nExamples: \n```shell\nlenu train DE       # Germany\nlenu train US-DE    # United States - Delaware\nlenu train IT       # Italy\n\n# enable logging to see more information like the number of samples and accuracy\nlenu --enable-logging train CH \n```\n\nIdentify ELF Code by using a model. The tool will return the best scoring ELF Codes. \n```shell\nlenu elf DE "Hans Müller KG"\n#   ELF Code                  Entity Legal Form name Local name     Score\n# 0     8Z6G                              Kommanditgesellschaft  0.979568\n# 1     V2YH                       Stiftung des privaten Rechts  0.001141\n# 2     OL20  Einzelunternehmen, eingetragener Kaufmann, ein...  0.000714\n```\n\nYou can also use pre-trained models, which is recommended in most cases:\n```shell\n# Model available at https://huggingface.co/Sociovestix/lenu_DE\nlenu elf Sociovestix/lenu_DE "Hans Müller KG"  \n#  ELF Code      Entity Legal Form name Local name     Score\n#0     8Z6G                  Kommanditgesellschaft  0.999445\n#1     2HBR  Gesellschaft mit beschränkter Haftung  0.000247\n#2     FR3V       Gesellschaft bürgerlichen Rechts  0.000071\n```\n\n## Support and Contributing\nFeel free to reach out to either [Sociovestix Labs](https://sociovestix.com/contact) or [GLEIF](https://www.gleif.org/contact/contact-information)\nif you need support in using this library, in utilizing LEI data in general, or in case you would like to contribute to this library in any form.\n',
+    'long_description': '\n<h1 align="center">\nLENU - Legal Entity Name Understanding \n</h1>\n\n---------------\n\n<h1 align="center">\n<a href="https://gleif.org">\n<img src="http://sdglabs.ai/wp-content/uploads/2022/07/gleif-logo-new.png" width="220" alt="">\n</a>\n</h1><br>\n<h3 align="center">in collaboration with</h3> \n<h1 align="center">\n<a href="https://sociovestix.com">\n<img src="https://sociovestix.com/img/svl_logo_centered.svg" width="700px">\n</a>\n</h1><br>\n\n---------------\n\n[![License](https://img.shields.io/github/license/Sociovestix/lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/LICENSE)\n![](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n**LENU** is a python library that helps to understand and work with Legal Entity Names\nin the context of the [Legal Entity Identifier](https://www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei) (LEI) Standard (ISO 17441)\nas well as the [Entity Legal Form (ELF) Code List](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) Standard (ISO 20275).  \n\nThe library utilizes Machine Learning with Transformers and scikit-learn. It provides and utilizes pre-trained ELF Detection models published at https://huggingface.co/Sociovestix. This code as well as the LEI data and models are distributed under Creative Commons Zero 1.0 Universal license.\n\nThe project was started in November 2021 as a collaboration of the [Global Legal Entity Identifier Foundation](https://gleif.org) (GLEIF) and\n[Sociovestix Labs](https://sociovestix.com) with the goal to explore how Machine Learning can support in detecting the legal form (ELF Code) from a legal name. \n\nIt provides:\n- an interface to download [LEI](https://www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy#/) and [ELF Code](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) data from GLEIF\'s public website\n- an interface to train and make use of Machine Learning models to classify ELF Codes from given Legal Names\n- an interface to use pre-trained ELF Detection models published on https://huggingface.co/Sociovestix\n---\n\n## Dependencies\n**LENU** requires\n- python (>=3.8, <3.10)\n- [scikit-learn](https://scikit-learn.org/) - Provides Machine Learning functionality for token based modelling\n- [transformers](https://huggingface.co/docs/transformers/index) - Download and applying Neural Network Models\n- [pytorch](https://pytorch.org/) - Machine Learning Framework to train Neural Network Models\n- [pandas](https://pandas.pydata.org/) - For reading and handling data\n- [Typer](https://typer.tiangolo.com/) - Adds the command line interface\n- [requests](https://docs.python-requests.org/en/latest/) and [pydantic](https://pydantic-docs.helpmanual.io/) - For downloading LEI data from GLEIF\'s website\n\n## Installation\n\nvia PyPI:\n```shell\npip install lenu\n```\n\nFrom github:\n```shell\npip install https://github.com/Sociovestix/lenu\n```\n\nEditable install from locally cloned repository\n```shell\ngit clone https://github.com/Sociovestix/lenu\npip install -e lenu\n```\n\n## Usage\n\nCreate folders for LEI and ELF Code data and to store your models\n\n```shell\nmkdir data\nmkdir models\n```\n\nDownload LEI data and ELF Code data into your `data` folder\n```shell\nlenu download\n```\n\nTrain a (default) ELF Code Classification model. An ELF Classification model is always Jurisdiction specific and \nwill be trained from Legal Names from this Jurisdiction.\n\nExamples: \n```shell\nlenu train DE       # Germany\nlenu train US-DE    # United States - Delaware\nlenu train IT       # Italy\n\n# enable logging to see more information like the number of samples and accuracy\nlenu --enable-logging train CH \n```\n\nIdentify ELF Code by using a model. The tool will return the best scoring ELF Codes. \n```shell\nlenu elf DE "Hans Müller KG"\n#   ELF Code                  Entity Legal Form name Local name     Score\n# 0     8Z6G                              Kommanditgesellschaft  0.979568\n# 1     V2YH                       Stiftung des privaten Rechts  0.001141\n# 2     OL20  Einzelunternehmen, eingetragener Kaufmann, ein...  0.000714\n```\n\nYou can also use pre-trained models, which is recommended in most cases:\n```shell\n# Model available at https://huggingface.co/Sociovestix/lenu_DE\nlenu elf Sociovestix/lenu_DE "Hans Müller KG"  \n#  ELF Code      Entity Legal Form name Local name     Score\n#0     8Z6G                  Kommanditgesellschaft  0.999445\n#1     2HBR  Gesellschaft mit beschränkter Haftung  0.000247\n#2     FR3V       Gesellschaft bürgerlichen Rechts  0.000071\n```\n\n## Support and Contributing\nFeel free to reach out to either [Sociovestix Labs](https://sociovestix.com/contact) or [GLEIF](https://www.gleif.org/contact/contact-information)\nif you need support in using this library, in utilizing LEI data in general, or in case you would like to contribute to this library in any form.\n',
     'author': 'aarimond',
     'author_email': 'alexander.arimond@sociovestix.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['lenu',
 'lenu.data', 'lenu.ml', 'lenu.ml.test'] package_data = \ {'': ['*']}
 install_requires = \ ['importlib-resources>=5.7.1,<6.0.0',
 'pandas>=1.4.2,<2.0.0', 'pydantic>=1.9.0,<2.0.0', 'requests>=2.27.1,<3.0.0',
 'scikit-learn>=1.0.2,<2.0.0', 'torch>=1.13.1,<2.0.0',
 'transformers>=4.26.0,<5.0.0', 'typer[all]>=0.4.1,<0.5.0', 'types-
 requests>=2.27.16,<3.0.0'] entry_points = \ {'console_scripts': ['lenu =
-lenu.console:app']} setup_kwargs = { 'name': 'lenu', 'version': '0.2.1',
+lenu.console:app']} setup_kwargs = { 'name': 'lenu', 'version': '0.2.2',
 'description': 'Legal Entity Name Understanding', 'long_description': '\n
-           ************ \\nnlleennuu -- LLeeggaall EEnnttiittyy NNaammee UUnnddeerrssttaannddiinngg \\nn ************
+           ************ \\nnLLEENNUU -- LLeeggaall EEnnttiittyy NNaammee UUnnddeerrssttaannddiinngg \\nn ************
 \n\n---------------\n\n
                                       \\nn
                                      _\\_nn_\\_nn
                                       \\nn
 
 \n
                         ******** iinn ccoollllaabboorraattiioonn wwiitthh ********
 \n
    ************ \\nn_\\_nn_[[_hh_tt_tt_pp_ss_::_//_//_ss_oo_cc_ii_oo_vv_ee_ss_tt_ii_xx_.._cc_oo_mm_//_ii_mm_gg_//_ss_vv_ll____ll_oo_gg_oo____cc_ee_nn_tt_ee_rr_ee_dd_.._ss_vv_gg_]]_\\_nn\\nn ************
 
 \n\n---------------\n\n[![License](https://img.shields.io/github/license/
 Sociovestix/lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/
 LICENSE)\n![](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)\n[!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black)\n\n\n**lenu** is a python library
+000000.svg)](https://github.com/psf/black)\n\n\n**LENU** is a python library
 that helps to understand and work with Legal Entity Names\nin the context of
 the [Legal Entity Identifier](https://www.gleif.org/en/about-lei/introducing-
 the-legal-entity-identifier-lei) (LEI) Standard (ISO 17441)\nas well as the
 [Entity Legal Form (ELF) Code List](https://www.gleif.org/en/about-lei/code-
 lists/iso-20275-entity-legal-forms-code-list) Standard (ISO 20275). \n\nThe
 library utilizes Machine Learning with Transformers and scikit-learn. It
 provides and utilizes pre-trained ELF Detection models published at https://
@@ -38,15 +38,15 @@
 support in detecting the legal form (ELF Code) from a legal name. \n\nIt
 provides:\n- an interface to download [LEI](https://www.gleif.org/en/lei-data/
 gleif-golden-copy/download-the-golden-copy#/) and [ELF Code](https://
 www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list)
 data from GLEIF\'s public website\n- an interface to train and make use of
 Machine Learning models to classify ELF Codes from given Legal Names\n- an
 interface to use pre-trained ELF Detection models published on https://
-huggingface.co/Sociovestix\n---\n\n## Dependencies\n**lenu** requires\n- python
+huggingface.co/Sociovestix\n---\n\n## Dependencies\n**LENU** requires\n- python
 (>=3.8, <3.10)\n- [scikit-learn](https://scikit-learn.org/) - Provides Machine
 Learning functionality for token based modelling\n- [transformers](https://
 huggingface.co/docs/transformers/index) - Download and applying Neural Network
 Models\n- [pytorch](https://pytorch.org/) - Machine Learning Framework to train
 Neural Network Models\n- [pandas](https://pandas.pydata.org/) - For reading and
 handling data\n- [Typer](https://typer.tiangolo.com/) - Adds the command line
 interface\n- [requests](https://docs.python-requests.org/en/latest/) and
```

### Comparing `lenu-0.2.1/PKG-INFO` & `lenu-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenu
-Version: 0.2.1
+Version: 0.2.2
 Summary: Legal Entity Name Understanding
 Author: aarimond
 Author-email: alexander.arimond@sociovestix.com
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Requires-Dist: transformers (>=4.26.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.4.1,<0.5.0)
 Requires-Dist: types-requests (>=2.27.16,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 <h1 align="center">
-lenu - Legal Entity Name Understanding 
+LENU - Legal Entity Name Understanding 
 </h1>
 
 ---------------
 
 <h1 align="center">
 <a href="https://gleif.org">
 <img src="http://sdglabs.ai/wp-content/uploads/2022/07/gleif-logo-new.png" width="220" alt="">
@@ -41,15 +41,15 @@
 ---------------
 
 [![License](https://img.shields.io/github/license/Sociovestix/lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/LICENSE)
 ![](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-**lenu** is a python library that helps to understand and work with Legal Entity Names
+**LENU** is a python library that helps to understand and work with Legal Entity Names
 in the context of the [Legal Entity Identifier](https://www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei) (LEI) Standard (ISO 17441)
 as well as the [Entity Legal Form (ELF) Code List](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) Standard (ISO 20275).  
 
 The library utilizes Machine Learning with Transformers and scikit-learn. It provides and utilizes pre-trained ELF Detection models published at https://huggingface.co/Sociovestix. This code as well as the LEI data and models are distributed under Creative Commons Zero 1.0 Universal license.
 
 The project was started in November 2021 as a collaboration of the [Global Legal Entity Identifier Foundation](https://gleif.org) (GLEIF) and
 [Sociovestix Labs](https://sociovestix.com) with the goal to explore how Machine Learning can support in detecting the legal form (ELF Code) from a legal name. 
@@ -57,15 +57,15 @@
 It provides:
 - an interface to download [LEI](https://www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy#/) and [ELF Code](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list) data from GLEIF's public website
 - an interface to train and make use of Machine Learning models to classify ELF Codes from given Legal Names
 - an interface to use pre-trained ELF Detection models published on https://huggingface.co/Sociovestix
 ---
 
 ## Dependencies
-**lenu** requires
+**LENU** requires
 - python (>=3.8, <3.10)
 - [scikit-learn](https://scikit-learn.org/) - Provides Machine Learning functionality for token based modelling
 - [transformers](https://huggingface.co/docs/transformers/index) - Download and applying Neural Network Models
 - [pytorch](https://pytorch.org/) - Machine Learning Framework to train Neural Network Models
 - [pandas](https://pandas.pydata.org/) - For reading and handling data
 - [Typer](https://typer.tiangolo.com/) - Adds the command line interface
 - [requests](https://docs.python-requests.org/en/latest/) and [pydantic](https://pydantic-docs.helpmanual.io/) - For downloading LEI data from GLEIF's website
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: lenu Version: 0.2.1 Summary: Legal Entity Name
+Metadata-Version: 2.1 Name: lenu Version: 0.2.2 Summary: Legal Entity Name
 Understanding Author: aarimond Author-email: alexander.arimond@sociovestix.com
 Requires-Python: >=3.8,<3.10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Requires-Dist: importlib-resources (>=5.7.1,<6.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0) Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: scikit-learn
 (>=1.0.2,<2.0.0) Requires-Dist: torch (>=1.13.1,<2.0.0) Requires-Dist:
 transformers (>=4.26.0,<5.0.0) Requires-Dist: typer[all] (>=0.4.1,<0.5.0)
 Requires-Dist: types-requests (>=2.27.16,<3.0.0) Description-Content-Type:
 text/markdown
-             ************ lleennuu -- LLeeggaall EEnnttiittyy NNaammee UUnnddeerrssttaannddiinngg ************
+             ************ LLEENNUU -- LLeeggaall EEnnttiittyy NNaammee UUnnddeerrssttaannddiinngg ************
 ---------------
 
                         ******** iinn ccoollllaabboorraattiioonn wwiitthh ********
        ************ _[[_hh_tt_tt_pp_ss_::_//_//_ss_oo_cc_ii_oo_vv_ee_ss_tt_ii_xx_.._cc_oo_mm_//_ii_mm_gg_//_ss_vv_ll____ll_oo_gg_oo____cc_ee_nn_tt_ee_rr_ee_dd_.._ss_vv_gg_]] ************
 
 --------------- [![License](https://img.shields.io/github/license/Sociovestix/
 lenu.svg)](https://github.com/Sociovestix/lenu/blob/main/LICENSE) ![](https://
 img.shields.io/badge/python-3.8%20%7C%203.9-blue) [![Code style: black](https:/
 /img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-black) **lenu** is a python library that helps to understand and work with
+black) **LENU** is a python library that helps to understand and work with
 Legal Entity Names in the context of the [Legal Entity Identifier](https://
 www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei) (LEI)
 Standard (ISO 17441) as well as the [Entity Legal Form (ELF) Code List](https:/
 /www.gleif.org/en/about-lei/code-lists/iso-20275-entity-legal-forms-code-list)
 Standard (ISO 20275). The library utilizes Machine Learning with Transformers
 and scikit-learn. It provides and utilizes pre-trained ELF Detection models
 published at https://huggingface.co/Sociovestix. This code as well as the LEI
@@ -34,15 +34,15 @@
 Machine Learning can support in detecting the legal form (ELF Code) from a
 legal name. It provides: - an interface to download [LEI](https://
 www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy#/) and
 [ELF Code](https://www.gleif.org/en/about-lei/code-lists/iso-20275-entity-
 legal-forms-code-list) data from GLEIF's public website - an interface to train
 and make use of Machine Learning models to classify ELF Codes from given Legal
 Names - an interface to use pre-trained ELF Detection models published on
-https://huggingface.co/Sociovestix --- ## Dependencies **lenu** requires -
+https://huggingface.co/Sociovestix --- ## Dependencies **LENU** requires -
 python (>=3.8, <3.10) - [scikit-learn](https://scikit-learn.org/) - Provides
 Machine Learning functionality for token based modelling - [transformers]
 (https://huggingface.co/docs/transformers/index) - Download and applying Neural
 Network Models - [pytorch](https://pytorch.org/) - Machine Learning Framework
 to train Neural Network Models - [pandas](https://pandas.pydata.org/) - For
 reading and handling data - [Typer](https://typer.tiangolo.com/) - Adds the
 command line interface - [requests](https://docs.python-requests.org/en/latest/
```

