# Comparing `tmp/rfstools-1.8.1.tar.gz` & `tmp/rfstools-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfstools-1.8.1.tar", last modified: Sat Jan 13 09:29:02 2024, max compression
+gzip compressed data, was "rfstools-1.8.2.tar", last modified: Mon Apr  8 13:06:20 2024, max compression
```

## Comparing `rfstools-1.8.1.tar` & `rfstools-1.8.2.tar`

### file list

```diff
@@ -1,45 +1,57 @@
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.930371 rfstools-1.8.1/
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     2069 2022-06-19 16:33:37.000000 rfstools-1.8.1/.gitignore
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     5964 2024-01-13 09:27:57.000000 rfstools-1.8.1/.gitlab-ci.yml
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)    35056 2022-06-19 16:33:37.000000 rfstools-1.8.1/LICENSE
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)       38 2022-06-19 16:33:37.000000 rfstools-1.8.1/MANIFEST.in
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     4986 2024-01-13 09:29:02.929371 rfstools-1.8.1/PKG-INFO
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     4549 2022-06-19 16:33:37.000000 rfstools-1.8.1/README.md
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.924371 rfstools-1.8.1/bin/
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     1014 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pcp
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      782 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pexist
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      782 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pisdir
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     4730 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pls
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      779 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pmkdir
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      900 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pmv
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      726 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/prm
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      590 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/prmdir
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     1038 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/pstat
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      581 2022-06-19 16:33:37.000000 rfstools-1.8.1/bin/ptouch
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      287 2022-06-19 16:33:37.000000 rfstools-1.8.1/deploy.sh
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.925371 rfstools-1.8.1/docs/
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)      634 2022-06-19 16:33:37.000000 rfstools-1.8.1/docs/Makefile
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     2024 2022-06-19 16:33:37.000000 rfstools-1.8.1/docs/conf.py
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      875 2022-06-19 16:33:37.000000 rfstools-1.8.1/docs/generate-docs.sh
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     1043 2022-06-19 16:33:37.000000 rfstools-1.8.1/docs/index.rst
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)       97 2022-06-19 16:33:37.000000 rfstools-1.8.1/requirements.txt
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)       38 2024-01-13 09:29:02.930371 rfstools-1.8.1/setup.cfg
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      892 2022-06-19 16:33:37.000000 rfstools-1.8.1/setup.py
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)       55 2024-01-13 09:27:57.000000 rfstools-1.8.1/sonar-project.properties
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.917371 rfstools-1.8.1/src/
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.926371 rfstools-1.8.1/src/_rfstools/
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)        0 2022-06-19 16:33:37.000000 rfstools-1.8.1/src/_rfstools/__init__.py
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     9012 2022-06-19 16:33:37.000000 rfstools-1.8.1/src/_rfstools/arg_parser.py
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     8246 2022-06-19 16:33:37.000000 rfstools-1.8.1/src/_rfstools/arg_processor.py
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.927371 rfstools-1.8.1/src/rfstools.egg-info/
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)     4986 2024-01-13 09:29:02.000000 rfstools-1.8.1/src/rfstools.egg-info/PKG-INFO
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)      614 2024-01-13 09:29:02.000000 rfstools-1.8.1/src/rfstools.egg-info/SOURCES.txt
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)        1 2024-01-13 09:29:02.000000 rfstools-1.8.1/src/rfstools.egg-info/dependency_links.txt
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)       62 2024-01-13 09:29:02.000000 rfstools-1.8.1/src/rfstools.egg-info/requires.txt
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)       10 2024-01-13 09:29:02.000000 rfstools-1.8.1/src/rfstools.egg-info/top_level.txt
-drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-01-13 09:29:02.928371 rfstools-1.8.1/tests/
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     2932 2022-06-19 16:33:37.000000 rfstools-1.8.1/tests/generic-tests
--rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      556 2022-06-19 16:33:37.000000 rfstools-1.8.1/tests/local-tests
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)      525 2022-06-19 16:33:37.000000 rfstools-1.8.1/tests/test-lib
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)      404 2022-06-19 16:33:37.000000 rfstools-1.8.1/tox.ini
--rw-r--r--   0 p-dev     (1001) p-dev     (1001)        6 2024-01-13 09:27:54.000000 rfstools-1.8.1/version.txt
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.778478 rfstools-1.8.2/
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     2069 2022-06-19 16:33:37.000000 rfstools-1.8.2/.gitignore
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     5686 2024-01-13 11:07:39.000000 rfstools-1.8.2/.gitlab-ci.yml
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)    35056 2022-06-19 16:33:37.000000 rfstools-1.8.2/LICENSE
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)       38 2022-06-19 16:33:37.000000 rfstools-1.8.2/MANIFEST.in
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     3805 2024-04-08 13:06:20.778478 rfstools-1.8.2/PKG-INFO
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     3265 2024-04-08 13:02:47.000000 rfstools-1.8.2/README.md
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.767478 rfstools-1.8.2/bin/
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     1014 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pcp
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      782 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pexist
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      782 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pisdir
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     4730 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pls
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      779 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pmkdir
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      900 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pmv
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      726 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/prm
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      590 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/prmdir
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     1038 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/pstat
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      581 2022-06-19 16:33:37.000000 rfstools-1.8.2/bin/ptouch
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      287 2022-06-19 16:33:37.000000 rfstools-1.8.2/deploy.sh
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.768478 rfstools-1.8.2/docs/
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)      634 2022-06-19 16:33:37.000000 rfstools-1.8.2/docs/Makefile
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     2024 2022-06-19 16:33:37.000000 rfstools-1.8.2/docs/conf.py
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      875 2022-06-19 16:33:37.000000 rfstools-1.8.2/docs/generate-docs.sh
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     2494 2024-04-08 12:08:32.000000 rfstools-1.8.2/docs/index.rst
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)       90 2024-04-08 12:08:32.000000 rfstools-1.8.2/requirements.txt
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)       38 2024-04-08 13:06:20.778478 rfstools-1.8.2/setup.cfg
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     1015 2024-01-13 10:16:25.000000 rfstools-1.8.2/setup.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)       55 2024-01-13 09:27:57.000000 rfstools-1.8.2/sonar-project.properties
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.759478 rfstools-1.8.2/src/
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.770478 rfstools-1.8.2/src/_rfstools/
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)        0 2022-06-19 16:33:37.000000 rfstools-1.8.2/src/_rfstools/__init__.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     9012 2022-06-19 16:33:37.000000 rfstools-1.8.2/src/_rfstools/arg_parser.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     8246 2022-06-19 16:33:37.000000 rfstools-1.8.2/src/_rfstools/arg_processor.py
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.774478 rfstools-1.8.2/src/rfslib/
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)       56 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/__init__.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)    29664 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/abstract_pconnection.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     1396 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/fs_pconnection.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     2901 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/ftp_pconnection.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     4834 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/path_utils.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     1639 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/pconnection_settings.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     6200 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/pglobber.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)      240 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/pinstance.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     3076 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/sftp_pconnection.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     3586 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/smb12_pconnection.py
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     4700 2024-01-13 10:16:25.000000 rfstools-1.8.2/src/rfslib/smb23_pconnection.py
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.777478 rfstools-1.8.2/src/rfstools.egg-info/
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)     3805 2024-04-08 13:06:20.000000 rfstools-1.8.2/src/rfstools.egg-info/PKG-INFO
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)      933 2024-04-08 13:06:20.000000 rfstools-1.8.2/src/rfstools.egg-info/SOURCES.txt
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)        1 2024-04-08 13:06:20.000000 rfstools-1.8.2/src/rfstools.egg-info/dependency_links.txt
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)      120 2024-04-08 13:06:20.000000 rfstools-1.8.2/src/rfstools.egg-info/requires.txt
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)       17 2024-04-08 13:06:20.000000 rfstools-1.8.2/src/rfstools.egg-info/top_level.txt
+drwxr-sr-x   0 p-dev     (1001) p-dev     (1001)        0 2024-04-08 13:06:20.777478 rfstools-1.8.2/tests/
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)     2932 2022-06-19 16:33:37.000000 rfstools-1.8.2/tests/generic-tests
+-rwxr-xr-x   0 p-dev     (1001) p-dev     (1001)      556 2022-06-19 16:33:37.000000 rfstools-1.8.2/tests/local-tests
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)      525 2022-06-19 16:33:37.000000 rfstools-1.8.2/tests/test-lib
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)      404 2022-06-19 16:33:37.000000 rfstools-1.8.2/tox.ini
+-rw-r--r--   0 p-dev     (1001) p-dev     (1001)        6 2024-04-08 13:05:53.000000 rfstools-1.8.2/version.txt
```

### Comparing `rfstools-1.8.1/.gitignore` & `rfstools-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/.gitlab-ci.yml` & `rfstools-1.8.2/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,22 @@
 
 image: debian:stable
 
 default:
   before_script:
     - apt update -y
     - apt dist-upgrade -y
-    - apt install -y python3-pip git
+    - apt install -y python3-pip python3-virtualenv git
 
-    - pip3 install --user -U virtualenv pip
     - export PATH=~/.local/bin:$PATH
     
     - virtualenv ~/venv
     - source ~/venv/bin/activate
 
-    - pip install -U pip
 
-    - mkdir -p ~/.pip
-    - |
-      cat > ~/.pip/pip.conf <<EOF
-      [global]
-      extra-index-url = https://rfstools-worker:${CI_RFSTOOLS_WORKER_TOKEN}@git.profinit.eu/api/v4/projects/552/packages/pypi/simple
-
-      EOF
 
 test-tox:
   stage: examine
   script: 
     - apt install -y libc6 dos2unix file
     - pip install tox
     - tox
@@ -198,15 +189,15 @@
 
       [ -n "$CI_COMMIT_TAG" ] && {
         echo Sleeping for 30 seconds to prevent race condition.
         sleep 30
       }
 
       pushd /tmp
-      git clone https://oauth2:${CI_DOCS_ACCESS_TOKEN}@git.profinit.eu/rfs/rfstools-docs/
+      git clone https://oauth2:${CI_DOCS_ACCESS_TOKEN}@gitlab.com/rfs4/rfstools-docs
       popd
 
       pushd $doc_repo
       rm -fr ./commands ./rfstools-dev-doc.pdf 2>/dev/null || :
       popd
 
       cp -r docs/_build/commands $doc_repo
```

### Comparing `rfstools-1.8.1/LICENSE` & `rfstools-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pcp` & `rfstools-1.8.2/bin/pcp`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pexist` & `rfstools-1.8.2/bin/pexist`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pisdir` & `rfstools-1.8.2/bin/pisdir`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pls` & `rfstools-1.8.2/bin/pls`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pmkdir` & `rfstools-1.8.2/bin/pmkdir`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pmv` & `rfstools-1.8.2/bin/pmv`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/prm` & `rfstools-1.8.2/bin/prm`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/prmdir` & `rfstools-1.8.2/bin/prmdir`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/pstat` & `rfstools-1.8.2/bin/pstat`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/bin/ptouch` & `rfstools-1.8.2/bin/ptouch`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/docs/Makefile` & `rfstools-1.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/docs/conf.py` & `rfstools-1.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/docs/generate-docs.sh` & `rfstools-1.8.2/docs/generate-docs.sh`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/setup.py` & `rfstools-1.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,21 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     author='Přemysl Šťastný',
     author_email='p-w@stty.cz',
     url='https://git.profinit.eu/pstastny/rfstools',
     package_dir={"": "src"},
-    packages=['_rfstools'],
+    packages=['_rfstools','rfslib'],
     install_requires=[
-      'rfslib>=3.1.8,<4',
       'ConfigArgParse>=1.4.1,<2',
-      'texttable>=1.6.4,<2'
+      'texttable>=1.6.4,<2',
+
+      # rfslib dependencies
+      'pysmb>=1.2.7,<2',
+      'paramiko>=2.7.2,<3',
+      'smbprotocol>=1.6.1,<2',
+      'ftputil>=5.0.1,<6'
       
     ],
     scripts=[*map(lambda x: 'bin/' + x, os.listdir('bin'))],
   )
```

### Comparing `rfstools-1.8.1/src/_rfstools/arg_parser.py` & `rfstools-1.8.2/src/_rfstools/arg_parser.py`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/src/_rfstools/arg_processor.py` & `rfstools-1.8.2/src/_rfstools/arg_processor.py`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/tests/generic-tests` & `rfstools-1.8.2/tests/generic-tests`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/tests/local-tests` & `rfstools-1.8.2/tests/local-tests`

 * *Files identical despite different names*

### Comparing `rfstools-1.8.1/tests/test-lib` & `rfstools-1.8.2/tests/test-lib`

 * *Files identical despite different names*

