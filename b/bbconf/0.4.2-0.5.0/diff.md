# Comparing `tmp/bbconf-0.4.2.tar.gz` & `tmp/bbconf-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbconf-0.4.2.tar", last modified: Wed Mar 13 03:28:15 2024, max compression
+gzip compressed data, was "bbconf-0.5.0.tar", last modified: Mon Apr  8 17:10:29 2024, max compression
```

## Comparing `bbconf-0.4.2.tar` & `bbconf-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:28:15.306209 bbconf-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-13 03:28:06.000000 bbconf-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-13 03:28:06.000000 bbconf-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-13 03:28:15.306209 bbconf-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-13 03:28:06.000000 bbconf-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:28:15.302209 bbconf-0.4.2/bbconf/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25911 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/bbconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:28:15.302209 bbconf-0.4.2/bbconf/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/schemas/bedfiles_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-13 03:28:06.000000 bbconf-0.4.2/bbconf/schemas/bedsets_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:28:15.302209 bbconf-0.4.2/bbconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-13 03:28:15.000000 bbconf-0.4.2/bbconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-13 03:28:15.000000 bbconf-0.4.2/bbconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 03:28:15.000000 bbconf-0.4.2/bbconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-13 03:28:15.000000 bbconf-0.4.2/bbconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 03:28:15.000000 bbconf-0.4.2/bbconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:28:15.302209 bbconf-0.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-13 03:28:06.000000 bbconf-0.4.2/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 03:28:06.000000 bbconf-0.4.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-13 03:28:06.000000 bbconf-0.4.2/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 03:28:15.306209 bbconf-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-13 03:28:06.000000 bbconf-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:28:15.302209 bbconf-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-03-13 03:28:06.000000 bbconf-0.4.2/tests/test_bbconf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-08 17:10:21.000000 bbconf-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 17:10:21.000000 bbconf-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 17:10:29.360425 bbconf-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-08 17:10:21.000000 bbconf-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.356425 bbconf-0.5.0/bbconf/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/bbagent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.356425 bbconf-0.5.0/bbconf/config_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/bedbaseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/bbconf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/bed_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/bedset_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/drs_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/bbconf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/bedfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15252 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/bedsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/bbconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 17:10:21.000000 bbconf-0.5.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:10:21.000000 bbconf-0.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 17:10:21.000000 bbconf-0.5.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:10:29.360425 bbconf-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-08 17:10:21.000000 bbconf-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-08 17:10:21.000000 bbconf-0.5.0/tests/test_bedfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-08 17:10:21.000000 bbconf-0.5.0/tests/test_bedset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-08 17:10:21.000000 bbconf-0.5.0/tests/test_objects.py
```

### Comparing `bbconf-0.4.2/LICENSE.txt` & `bbconf-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bbconf-0.4.2/PKG-INFO` & `bbconf-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbconf
-Version: 0.4.2
+Version: 0.5.0
 Summary: Configuration package for bedbase project
 Home-page: https://databio.org
 Author: Michal Stolarczyk, Oleksandr Khoroshevskyi
 Author-email: khorosh@virginia.edu
 License: BSD2
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -12,18 +12,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: yacman>=0.9.1
-Requires-Dist: pipestat[dbbackend]>=0.8.0
-Requires-Dist: geniml>=0.2.0
+Requires-Dist: sqlalchemy>=2.0.0
+Requires-Dist: geniml>=0.3.0
 Requires-Dist: psycopg>=3.1.15
 Requires-Dist: colorlogs
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: botocore>=1.34.54
+Requires-Dist: boto3>=1.34.54
+Requires-Dist: pephubclient>=0.4.1
+Requires-Dist: sqlalchemy_schemadisplay
+Requires-Dist: scipy<=1.11.0
 
 <h1 align="center">bbconf</h1>
 
 ![Run pytests](https://github.com/databio/bbconf/workflows/Run%20pytests/badge.svg)
 [![pypi-badge](https://img.shields.io/pypi/v/bbconf?color=%2334D058)](https://pypi.org/project/bbconf/)
 [![pypi-version](https://img.shields.io/pypi/pyversions/bbconf.svg?color=%2334D058)](https://pypi.org/project/bbconf)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -32,15 +38,15 @@
 
 
 *BEDBASE* project configuration package (agent)
 
 ## What is this?
 
 `bbconf` is a configuration and management tool for BEDbase, facilitating the reading of configuration files, 
-setting up connections to PostgreSQL and Qdrant databases, managing file paths, and storing transformer models. 
+setting up connections to PostgreSQL, PEPhub, S3, and Qdrant databases, managing file paths, and storing transformer models. 
 It formalizes communication pathways for pipelines and downstream tools, ensuring seamless interaction."
 
 ---
 
 **Documentation**: <a href="https://docs.bedbase.org/bedboss" target="_blank">https://docs.bedbase.org/bedboss</a>
 
 **Source Code**: <a href="https://github.com/databio/bbconf" target="_blank">https://github.com/databio/bbconf</a>
```

#### html2text {}

```diff
@@ -1,32 +1,35 @@
-Metadata-Version: 2.1 Name: bbconf Version: 0.4.2 Summary: Configuration
+Metadata-Version: 2.1 Name: bbconf Version: 0.5.0 Summary: Configuration
 package for bedbase project Home-page: https://databio.org Author: Michal
 Stolarczyk, Oleksandr Khoroshevskyi Author-email: khorosh@virginia.edu License:
 BSD2 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Description-
 Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist:
-yacman>=0.9.1 Requires-Dist: pipestat[dbbackend]>=0.8.0 Requires-Dist:
-geniml>=0.2.0 Requires-Dist: psycopg>=3.1.15 Requires-Dist: colorlogs
+yacman>=0.9.1 Requires-Dist: sqlalchemy>=2.0.0 Requires-Dist: geniml>=0.3.0
+Requires-Dist: psycopg>=3.1.15 Requires-Dist: colorlogs Requires-Dist:
+pydantic>=2.6.4 Requires-Dist: botocore>=1.34.54 Requires-Dist: boto3>=1.34.54
+Requires-Dist: pephubclient>=0.4.1 Requires-Dist: sqlalchemy_schemadisplay
+Requires-Dist: scipy<=1.11.0
                              ************ bbbbccoonnff ************
 ![Run pytests](https://github.com/databio/bbconf/workflows/Run%20pytests/
 badge.svg) [![pypi-badge](https://img.shields.io/pypi/v/
 bbconf?color=%2334D058)](https://pypi.org/project/bbconf/) [![pypi-version]
 (https://img.shields.io/pypi/pyversions/bbconf.svg?color=%2334D058)](https://
 pypi.org/project/bbconf) [![Code style: black](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) [![Github badge]
 (https://img.shields.io/badge/source-github-354a75?logo=github)](https://
 github.com/databio/bbconf) [![coverage](https://coverage-
 badge.samuelcolvin.workers.dev/databio/bbconf.svg)](https://coverage-
 badge.samuelcolvin.workers.dev/redirect/databio/bbconf) *BEDBASE* project
 configuration package (agent) ## What is this? `bbconf` is a configuration and
 management tool for BEDbase, facilitating the reading of configuration files,
-setting up connections to PostgreSQL and Qdrant databases, managing file paths,
-and storing transformer models. It formalizes communication pathways for
-pipelines and downstream tools, ensuring seamless interaction." --
-- **Documentation**: _h_t_t_p_s_:_/_/_d_o_c_s_._b_e_d_b_a_s_e_._o_r_g_/_b_e_d_b_o_s_s **Source Code**: _h_t_t_p_s_:_/_/
-_g_i_t_h_u_b_._c_o_m_/_d_a_t_a_b_i_o_/_b_b_c_o_n_f --- ## Installation To install `bbclient` use this
-command: ``` pip install bbclient ``` or install the latest version from the
-GitHub repository: ``` pip install git+https://github.com/databio/bbconf.git
-```
+setting up connections to PostgreSQL, PEPhub, S3, and Qdrant databases,
+managing file paths, and storing transformer models. It formalizes
+communication pathways for pipelines and downstream tools, ensuring seamless
+interaction." --- **Documentation**: _h_t_t_p_s_:_/_/_d_o_c_s_._b_e_d_b_a_s_e_._o_r_g_/_b_e_d_b_o_s_s **Source
+Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_a_t_a_b_i_o_/_b_b_c_o_n_f --- ## Installation To install
+`bbclient` use this command: ``` pip install bbclient ``` or install the latest
+version from the GitHub repository: ``` pip install git+https://github.com/
+databio/bbconf.git ```
```

### Comparing `bbconf-0.4.2/README.md` & `bbconf-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 *BEDBASE* project configuration package (agent)
 
 ## What is this?
 
 `bbconf` is a configuration and management tool for BEDbase, facilitating the reading of configuration files, 
-setting up connections to PostgreSQL and Qdrant databases, managing file paths, and storing transformer models. 
+setting up connections to PostgreSQL, PEPhub, S3, and Qdrant databases, managing file paths, and storing transformer models. 
 It formalizes communication pathways for pipelines and downstream tools, ensuring seamless interaction."
 
 ---
 
 **Documentation**: <a href="https://docs.bedbase.org/bedboss" target="_blank">https://docs.bedbase.org/bedboss</a>
 
 **Source Code**: <a href="https://github.com/databio/bbconf" target="_blank">https://github.com/databio/bbconf</a>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 code%20style-black-000000.svg)](https://github.com/psf/black) [![Github badge]
 (https://img.shields.io/badge/source-github-354a75?logo=github)](https://
 github.com/databio/bbconf) [![coverage](https://coverage-
 badge.samuelcolvin.workers.dev/databio/bbconf.svg)](https://coverage-
 badge.samuelcolvin.workers.dev/redirect/databio/bbconf) *BEDBASE* project
 configuration package (agent) ## What is this? `bbconf` is a configuration and
 management tool for BEDbase, facilitating the reading of configuration files,
-setting up connections to PostgreSQL and Qdrant databases, managing file paths,
-and storing transformer models. It formalizes communication pathways for
-pipelines and downstream tools, ensuring seamless interaction." --
-- **Documentation**: _h_t_t_p_s_:_/_/_d_o_c_s_._b_e_d_b_a_s_e_._o_r_g_/_b_e_d_b_o_s_s **Source Code**: _h_t_t_p_s_:_/_/
-_g_i_t_h_u_b_._c_o_m_/_d_a_t_a_b_i_o_/_b_b_c_o_n_f --- ## Installation To install `bbclient` use this
-command: ``` pip install bbclient ``` or install the latest version from the
-GitHub repository: ``` pip install git+https://github.com/databio/bbconf.git
-```
+setting up connections to PostgreSQL, PEPhub, S3, and Qdrant databases,
+managing file paths, and storing transformer models. It formalizes
+communication pathways for pipelines and downstream tools, ensuring seamless
+interaction." --- **Documentation**: _h_t_t_p_s_:_/_/_d_o_c_s_._b_e_d_b_a_s_e_._o_r_g_/_b_e_d_b_o_s_s **Source
+Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_a_t_a_b_i_o_/_b_b_c_o_n_f --- ## Installation To install
+`bbclient` use this command: ``` pip install bbclient ``` or install the latest
+version from the GitHub repository: ``` pip install git+https://github.com/
+databio/bbconf.git ```
```

### Comparing `bbconf-0.4.2/bbconf/models.py` & `bbconf-0.5.0/bbconf/models/drs_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
-from typing import Optional, List
+from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
 
+# DRS Models
 class AccessURL(BaseModel):
     url: str
     headers: Optional[dict] = None
 
 
 class AccessMethod(BaseModel):
     type: str
@@ -16,13 +17,13 @@
     region: Optional[str] = None
 
 
 class DRSModel(BaseModel):
     id: str
     name: Optional[str] = None
     self_uri: str
-    size: str
+    size: Union[int, None] = None
     created_time: Optional[datetime.datetime] = None
     updated_time: Optional[datetime.datetime] = None
     checksums: str
     access_methods: List[AccessMethod]
     description: Optional[str] = None
```

### Comparing `bbconf-0.4.2/bbconf.egg-info/PKG-INFO` & `bbconf-0.5.0/bbconf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbconf
-Version: 0.4.2
+Version: 0.5.0
 Summary: Configuration package for bedbase project
 Home-page: https://databio.org
 Author: Michal Stolarczyk, Oleksandr Khoroshevskyi
 Author-email: khorosh@virginia.edu
 License: BSD2
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -12,18 +12,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: yacman>=0.9.1
-Requires-Dist: pipestat[dbbackend]>=0.8.0
-Requires-Dist: geniml>=0.2.0
+Requires-Dist: sqlalchemy>=2.0.0
+Requires-Dist: geniml>=0.3.0
 Requires-Dist: psycopg>=3.1.15
 Requires-Dist: colorlogs
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: botocore>=1.34.54
+Requires-Dist: boto3>=1.34.54
+Requires-Dist: pephubclient>=0.4.1
+Requires-Dist: sqlalchemy_schemadisplay
+Requires-Dist: scipy<=1.11.0
 
 <h1 align="center">bbconf</h1>
 
 ![Run pytests](https://github.com/databio/bbconf/workflows/Run%20pytests/badge.svg)
 [![pypi-badge](https://img.shields.io/pypi/v/bbconf?color=%2334D058)](https://pypi.org/project/bbconf/)
 [![pypi-version](https://img.shields.io/pypi/pyversions/bbconf.svg?color=%2334D058)](https://pypi.org/project/bbconf)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -32,15 +38,15 @@
 
 
 *BEDBASE* project configuration package (agent)
 
 ## What is this?
 
 `bbconf` is a configuration and management tool for BEDbase, facilitating the reading of configuration files, 
-setting up connections to PostgreSQL and Qdrant databases, managing file paths, and storing transformer models. 
+setting up connections to PostgreSQL, PEPhub, S3, and Qdrant databases, managing file paths, and storing transformer models. 
 It formalizes communication pathways for pipelines and downstream tools, ensuring seamless interaction."
 
 ---
 
 **Documentation**: <a href="https://docs.bedbase.org/bedboss" target="_blank">https://docs.bedbase.org/bedboss</a>
 
 **Source Code**: <a href="https://github.com/databio/bbconf" target="_blank">https://github.com/databio/bbconf</a>
```

#### html2text {}

```diff
@@ -1,32 +1,35 @@
-Metadata-Version: 2.1 Name: bbconf Version: 0.4.2 Summary: Configuration
+Metadata-Version: 2.1 Name: bbconf Version: 0.5.0 Summary: Configuration
 package for bedbase project Home-page: https://databio.org Author: Michal
 Stolarczyk, Oleksandr Khoroshevskyi Author-email: khorosh@virginia.edu License:
 BSD2 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Description-
 Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist:
-yacman>=0.9.1 Requires-Dist: pipestat[dbbackend]>=0.8.0 Requires-Dist:
-geniml>=0.2.0 Requires-Dist: psycopg>=3.1.15 Requires-Dist: colorlogs
+yacman>=0.9.1 Requires-Dist: sqlalchemy>=2.0.0 Requires-Dist: geniml>=0.3.0
+Requires-Dist: psycopg>=3.1.15 Requires-Dist: colorlogs Requires-Dist:
+pydantic>=2.6.4 Requires-Dist: botocore>=1.34.54 Requires-Dist: boto3>=1.34.54
+Requires-Dist: pephubclient>=0.4.1 Requires-Dist: sqlalchemy_schemadisplay
+Requires-Dist: scipy<=1.11.0
                              ************ bbbbccoonnff ************
 ![Run pytests](https://github.com/databio/bbconf/workflows/Run%20pytests/
 badge.svg) [![pypi-badge](https://img.shields.io/pypi/v/
 bbconf?color=%2334D058)](https://pypi.org/project/bbconf/) [![pypi-version]
 (https://img.shields.io/pypi/pyversions/bbconf.svg?color=%2334D058)](https://
 pypi.org/project/bbconf) [![Code style: black](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) [![Github badge]
 (https://img.shields.io/badge/source-github-354a75?logo=github)](https://
 github.com/databio/bbconf) [![coverage](https://coverage-
 badge.samuelcolvin.workers.dev/databio/bbconf.svg)](https://coverage-
 badge.samuelcolvin.workers.dev/redirect/databio/bbconf) *BEDBASE* project
 configuration package (agent) ## What is this? `bbconf` is a configuration and
 management tool for BEDbase, facilitating the reading of configuration files,
-setting up connections to PostgreSQL and Qdrant databases, managing file paths,
-and storing transformer models. It formalizes communication pathways for
-pipelines and downstream tools, ensuring seamless interaction." --
-- **Documentation**: _h_t_t_p_s_:_/_/_d_o_c_s_._b_e_d_b_a_s_e_._o_r_g_/_b_e_d_b_o_s_s **Source Code**: _h_t_t_p_s_:_/_/
-_g_i_t_h_u_b_._c_o_m_/_d_a_t_a_b_i_o_/_b_b_c_o_n_f --- ## Installation To install `bbclient` use this
-command: ``` pip install bbclient ``` or install the latest version from the
-GitHub repository: ``` pip install git+https://github.com/databio/bbconf.git
-```
+setting up connections to PostgreSQL, PEPhub, S3, and Qdrant databases,
+managing file paths, and storing transformer models. It formalizes
+communication pathways for pipelines and downstream tools, ensuring seamless
+interaction." --- **Documentation**: _h_t_t_p_s_:_/_/_d_o_c_s_._b_e_d_b_a_s_e_._o_r_g_/_b_e_d_b_o_s_s **Source
+Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_a_t_a_b_i_o_/_b_b_c_o_n_f --- ## Installation To install
+`bbclient` use this command: ``` pip install bbclient ``` or install the latest
+version from the GitHub repository: ``` pip install git+https://github.com/
+databio/bbconf.git ```
```

### Comparing `bbconf-0.4.2/setup.py` & `bbconf-0.5.0/setup.py`

 * *Files identical despite different names*

