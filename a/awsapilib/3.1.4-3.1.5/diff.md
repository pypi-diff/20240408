# Comparing `tmp/awsapilib-3.1.4.tar.gz` & `tmp/awsapilib-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsapilib-3.1.4.tar", last modified: Wed Nov 29 04:49:21 2023, max compression
+gzip compressed data, was "awsapilib-3.1.5.tar", last modified: Mon Apr  8 18:31:45 2024, max compression
```

## Comparing `awsapilib-3.1.4.tar` & `awsapilib-3.1.5.tar`

### file list

```diff
@@ -1,88 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.172630 awsapilib-3.1.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)        5 2023-11-29 04:48:07.000000 awsapilib-3.1.4/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (127)      315 2023-11-29 04:48:07.000000 awsapilib-3.1.4/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2023-11-29 04:48:07.000000 awsapilib-3.1.4/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4204 2023-11-29 04:48:07.000000 awsapilib-3.1.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-29 04:48:07.000000 awsapilib-3.1.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2023-11-29 04:48:07.000000 awsapilib-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2023-11-29 04:49:21.172630 awsapilib-3.1.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      765 2023-11-29 04:48:07.000000 awsapilib-3.1.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    86576 2023-11-29 04:49:20.000000 awsapilib-3.1.4/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2023-11-29 04:48:07.000000 awsapilib-3.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.164630 awsapilib-3.1.4/awsapilib/
--rwxr-xr-x   0 runner    (1001) docker     (127)        5 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (127)      315 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4204 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)      765 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    86576 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/USAGE_BILLING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/USAGE_CONTROL_TOWER.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/USAGE_SSO.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     2200 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.164630 awsapilib-3.1.4/awsapilib/authentication/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2263 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/authentication/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25652 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/authentication/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/authentication/authenticationexceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/authentication/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1878 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/awsapilib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/awsapilibexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/billing/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2158 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/billing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18573 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/billing/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/billing/billingexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/captcha/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2038 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/captcha/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5882 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/captcha/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/captcha/captchaexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/cloudformation/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/cloudformation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4763 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/cloudformation/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/cloudformation/cloudformationexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/console/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3080 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/console/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34297 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/console/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/console/consoleexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/controltower/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3128 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/controltower/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    62213 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/controltower/controltower.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/controltower/controltowerexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/controltower/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2684 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/controltower/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/controltower/resources/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21054 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/controltower/resources/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-11-29 04:49:20.000000 awsapilib-3.1.4/awsapilib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/sso/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2312 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.168630 awsapilib-3.1.4/awsapilib/sso/entities/
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/sso/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20644 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/sso/entities/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27520 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/sso/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2023-11-29 04:48:07.000000 awsapilib-3.1.4/awsapilib/sso/ssoexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.164630 awsapilib-3.1.4/awsapilib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2023-11-29 04:49:21.000000 awsapilib-3.1.4/awsapilib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2023-11-29 04:49:21.000000 awsapilib-3.1.4/awsapilib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 04:49:21.000000 awsapilib-3.1.4/awsapilib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 04:49:21.000000 awsapilib-3.1.4/awsapilib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-11-29 04:49:21.000000 awsapilib-3.1.4/awsapilib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-29 04:49:21.000000 awsapilib-3.1.4/awsapilib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-11-29 04:49:20.000000 awsapilib-3.1.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.172630 awsapilib-3.1.4/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6774 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     8908 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       33 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      501 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2023-11-29 04:48:07.000000 awsapilib-3.1.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-11-29 04:49:20.000000 awsapilib-3.1.4/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      149 2023-11-29 04:49:21.172630 awsapilib-3.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2009 2023-11-29 04:48:07.000000 awsapilib-3.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:49:21.172630 awsapilib-3.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-11-29 04:48:07.000000 awsapilib-3.1.4/tests/test_awsapilib.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.167293 awsapilib-3.1.5/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2024-04-08 18:30:30.000000 awsapilib-3.1.5/.VERSION
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      315 2022-05-05 14:41:57.000000 awsapilib-3.1.5/AUTHORS.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1262 2021-04-26 12:49:21.000000 awsapilib-3.1.5/CONTRIBUTING.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     4272 2024-04-08 18:30:41.000000 awsapilib-3.1.5/HISTORY.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1063 2021-04-26 12:49:21.000000 awsapilib-3.1.5/LICENSE
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      392 2021-04-26 12:49:21.000000 awsapilib-3.1.5/MANIFEST.in
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     7266 2024-04-08 18:31:45.167488 awsapilib-3.1.5/PKG-INFO
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      765 2023-11-27 12:34:11.000000 awsapilib-3.1.5/Pipfile
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    79703 2024-04-08 18:31:43.000000 awsapilib-3.1.5/Pipfile.lock
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2388 2021-05-11 12:13:20.000000 awsapilib-3.1.5/README.rst
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.839922 awsapilib-3.1.5/awsapilib/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/.VERSION
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      315 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/AUTHORS.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1262 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/CONTRIBUTING.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     4272 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/HISTORY.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1063 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/LICENSE
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      765 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/Pipfile
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    79703 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/Pipfile.lock
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2388 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/README.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      783 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/USAGE_BILLING.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3291 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/USAGE_CONTROL_TOWER.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      250 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/USAGE_SSO.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2200 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.867397 awsapilib-3.1.5/awsapilib/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1105 2022-03-04 12:46:25.000000 awsapilib-3.1.5/awsapilib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1093 2023-11-29 04:43:03.000000 awsapilib-3.1.5/awsapilib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      940 2021-05-05 14:11:04.000000 awsapilib-3.1.5/awsapilib/__pycache__/_version.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1017 2023-11-29 04:43:03.000000 awsapilib-3.1.5/awsapilib/__pycache__/_version.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5879 2023-08-25 14:08:08.000000 awsapilib-3.1.5/awsapilib/__pycache__/awsapilib.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1471 2023-08-22 10:14:39.000000 awsapilib-3.1.5/awsapilib/__pycache__/awsapilibexceptions.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2144 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/_version.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.883115 awsapilib-3.1.5/awsapilib/authentication/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2263 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/authentication/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.905545 awsapilib-3.1.5/awsapilib/authentication/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      995 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      983 2023-11-29 04:43:03.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19927 2022-10-11 17:52:57.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/authentication.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19559 2023-11-29 04:43:03.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/authentication.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1301 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/authenticationexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1283 2023-11-29 04:43:05.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/authenticationexceptions.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    16923 2023-08-24 10:23:02.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/metadata.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6769 2021-12-28 14:03:43.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6889 2023-03-30 15:02:25.000000 awsapilib-3.1.5/awsapilib/authentication/__pycache__/utils.cpython-39.pyc
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    25652 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/authentication/authentication.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2020 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/authentication/authenticationexceptions.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     7016 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/authentication/utils.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1878 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/awsapilib.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1720 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/awsapilibexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.919342 awsapilib-3.1.5/awsapilib/billing/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2158 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/billing/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.932077 awsapilib-3.1.5/awsapilib/billing/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      919 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/billing/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      907 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/billing/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    16523 2022-04-29 09:08:11.000000 awsapilib-3.1.5/awsapilib/billing/__pycache__/billing.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    16227 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/billing/__pycache__/billing.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1675 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/billing/__pycache__/billingexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1631 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/billing/__pycache__/billingexceptions.cpython-39.pyc
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    19259 2024-04-08 18:12:31.000000 awsapilib-3.1.5/awsapilib/billing/billing.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2195 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/billing/billingexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.945871 awsapilib-3.1.5/awsapilib/captcha/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2038 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/captcha/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.966601 awsapilib-3.1.5/awsapilib/captcha/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      940 2021-12-20 15:26:28.000000 awsapilib-3.1.5/awsapilib/captcha/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      928 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/captcha/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5112 2021-12-20 15:26:28.000000 awsapilib-3.1.5/awsapilib/captcha/__pycache__/captcha.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5210 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/captcha/__pycache__/captcha.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1330 2021-12-20 15:26:28.000000 awsapilib-3.1.5/awsapilib/captcha/__pycache__/captchaexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1312 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/captcha/__pycache__/captchaexceptions.cpython-39.pyc
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     5882 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/captcha/captcha.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2056 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/captcha/captchaexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.977546 awsapilib-3.1.5/awsapilib/cloudformation/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1884 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/cloudformation/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.991295 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      797 2021-12-01 10:24:10.000000 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      785 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3893 2021-11-29 11:00:06.000000 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/cloudformation.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3904 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/cloudformation.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      880 2021-11-29 11:00:06.000000 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/cloudformationexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      888 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/cloudformation/__pycache__/cloudformationexceptions.cpython-39.pyc
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     4763 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/cloudformation/cloudformation.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1805 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/cloudformation/cloudformationexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.001914 awsapilib-3.1.5/awsapilib/console/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     3080 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/console/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.017388 awsapilib-3.1.5/awsapilib/console/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1397 2021-12-03 09:35:33.000000 awsapilib-3.1.5/awsapilib/console/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1385 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/console/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    25372 2022-10-11 07:59:27.000000 awsapilib-3.1.5/awsapilib/console/__pycache__/console.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    24915 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/console/__pycache__/console.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3591 2021-12-03 08:12:34.000000 awsapilib-3.1.5/awsapilib/console/__pycache__/consoleexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3377 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/console/__pycache__/consoleexceptions.cpython-39.pyc
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    34297 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/console/console.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3081 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/console/consoleexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.028570 awsapilib-3.1.5/awsapilib/controltower/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     3128 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/controltower/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.046910 awsapilib-3.1.5/awsapilib/controltower/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1383 2022-03-04 12:46:26.000000 awsapilib-3.1.5/awsapilib/controltower/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1371 2023-11-29 04:43:05.000000 awsapilib-3.1.5/awsapilib/controltower/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    51141 2022-10-11 17:54:08.000000 awsapilib-3.1.5/awsapilib/controltower/__pycache__/controltower.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    50794 2023-11-29 04:43:05.000000 awsapilib-3.1.5/awsapilib/controltower/__pycache__/controltower.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3964 2021-12-29 13:35:25.000000 awsapilib-3.1.5/awsapilib/controltower/__pycache__/controltowerexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3777 2023-11-29 04:43:05.000000 awsapilib-3.1.5/awsapilib/controltower/__pycache__/controltowerexceptions.cpython-39.pyc
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    62213 2023-11-29 04:40:45.000000 awsapilib-3.1.5/awsapilib/controltower/controltower.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3346 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/controltower/controltowerexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.056613 awsapilib-3.1.5/awsapilib/controltower/resources/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2684 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.073452 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1235 2022-03-21 09:46:14.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1223 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1039 2022-03-21 09:46:14.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/configuration.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1043 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/configuration.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    22070 2022-09-20 08:39:21.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/resources.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    21757 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/controltower/resources/__pycache__/resources.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2064 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/controltower/resources/configuration.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    21054 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/controltower/resources/resources.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1208 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/dev-requirements.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      676 2024-04-08 18:31:43.000000 awsapilib-3.1.5/awsapilib/requirements.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.087237 awsapilib-3.1.5/awsapilib/sso/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2312 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/sso/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.107367 awsapilib-3.1.5/awsapilib/sso/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1072 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/sso/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1060 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/sso/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    18998 2021-11-29 11:00:06.000000 awsapilib-3.1.5/awsapilib/sso/__pycache__/sso.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    18192 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/sso/__pycache__/sso.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1918 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/sso/__pycache__/ssoexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1861 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/sso/__pycache__/ssoexceptions.cpython-39.pyc
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.115064 awsapilib-3.1.5/awsapilib/sso/entities/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1974 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/sso/entities/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.124427 awsapilib-3.1.5/awsapilib/sso/entities/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      967 2021-06-04 07:35:03.000000 awsapilib-3.1.5/awsapilib/sso/entities/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      955 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/sso/entities/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    17649 2021-11-29 11:00:06.000000 awsapilib-3.1.5/awsapilib/sso/entities/__pycache__/entities.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    17370 2023-11-29 04:43:06.000000 awsapilib-3.1.5/awsapilib/sso/entities/__pycache__/entities.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    20644 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/sso/entities/entities.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    27520 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/sso/sso.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2338 2023-11-27 12:34:11.000000 awsapilib-3.1.5/awsapilib/sso/ssoexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:44.851426 awsapilib-3.1.5/awsapilib.egg-info/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     7266 2024-04-08 18:31:44.000000 awsapilib-3.1.5/awsapilib.egg-info/PKG-INFO
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5920 2024-04-08 18:31:44.000000 awsapilib-3.1.5/awsapilib.egg-info/SOURCES.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2024-04-08 18:31:44.000000 awsapilib-3.1.5/awsapilib.egg-info/dependency_links.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2021-05-11 08:20:21.000000 awsapilib-3.1.5/awsapilib.egg-info/not-zip-safe
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      301 2024-04-08 18:31:44.000000 awsapilib-3.1.5/awsapilib.egg-info/requires.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       10 2024-04-08 18:31:44.000000 awsapilib-3.1.5/awsapilib.egg-info/top_level.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1208 2024-04-08 18:31:43.000000 awsapilib-3.1.5/dev-requirements.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.164006 awsapilib-3.1.5/docs/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6774 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/Makefile
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/authors.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      840 2021-05-11 08:51:06.000000 awsapilib-3.1.5/docs/awsapilib.authentication.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      556 2021-05-11 08:51:06.000000 awsapilib-3.1.5/docs/awsapilib.billing.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      556 2021-12-02 14:32:09.000000 awsapilib-3.1.5/docs/awsapilib.captcha.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      661 2021-12-02 14:32:09.000000 awsapilib-3.1.5/docs/awsapilib.cloudformation.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      556 2021-12-02 14:32:09.000000 awsapilib-3.1.5/docs/awsapilib.console.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      685 2021-05-11 08:51:06.000000 awsapilib-3.1.5/docs/awsapilib.controltower.resources.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      707 2021-05-11 08:51:06.000000 awsapilib-3.1.5/docs/awsapilib.controltower.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      698 2021-12-02 14:32:09.000000 awsapilib-3.1.5/docs/awsapilib.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      395 2021-05-11 08:51:06.000000 awsapilib-3.1.5/docs/awsapilib.sso.entities.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      562 2021-05-11 08:51:06.000000 awsapilib-3.1.5/docs/awsapilib.sso.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     8908 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/conf.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       33 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/contributing.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/history.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      501 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/index.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       33 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/installation.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       64 2022-04-29 09:08:53.000000 awsapilib-3.1.5/docs/modules.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       27 2021-04-26 12:49:21.000000 awsapilib-3.1.5/docs/readme.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      168 2023-11-27 12:34:11.000000 awsapilib-3.1.5/docs/usage.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      676 2024-04-08 18:31:43.000000 awsapilib-3.1.5/requirements.txt
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      149 2024-04-08 18:31:45.169352 awsapilib-3.1.5/setup.cfg
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2009 2024-04-08 18:13:41.000000 awsapilib-3.1.5/setup.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2024-04-08 18:31:45.166925 awsapilib-3.1.5/tests/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2249 2021-04-26 12:49:21.000000 awsapilib-3.1.5/tests/test_awsapilib.py
```

### Comparing `awsapilib-3.1.4/CONTRIBUTING.rst` & `awsapilib-3.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/HISTORY.rst` & `awsapilib-3.1.5/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -231,7 +231,13 @@
 * Bump and loosen dependencies.
 
 
 3.1.4 (29-11-2023)
 ------------------
 
 * Remove gov regions from Control Tower. Bump dependencies.
+
+
+3.1.5 (08-04-2024)
+------------------
+
+* Fix billing api changes.
```

### Comparing `awsapilib-3.1.4/LICENSE` & `awsapilib-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/PKG-INFO` & `awsapilib-3.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: awsapilib
-Version: 3.1.4
+Version: 3.1.5
 Summary: A python library that exposes AWS services that are not covered by boto3, through the usage of undocumented APIs.
 Home-page: https://github.com/schubergphilis/awsapilib
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsapilib AWS api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: requests>=2.31.0; python_version >= "3.7"
-Requires-Dist: boto3>=1.33.2; python_version >= "3.7"
-Requires-Dist: beautifulsoup4>=4.12.2; python_full_version >= "3.6.0"
-Requires-Dist: opnieuw>=1.2.1; python_version >= "3.7"
-Requires-Dist: boto3-type-annotations>=0.3.1
-Requires-Dist: cachetools>=4.2.4; python_version ~= "3.5"
-Requires-Dist: pyotp>=2.9.0; python_version >= "3.7"
-Requires-Dist: 2captcha-python>=1.2.2; python_version >= "3.6"
 
 =========
 awsapilib
 =========
 
 A python library that exposes AWS services that are not covered by boto3, through the usage of undocumented APIs.
 
@@ -326,7 +318,13 @@
 * Bump and loosen dependencies.
 
 
 3.1.4 (29-11-2023)
 ------------------
 
 * Remove gov regions from Control Tower. Bump dependencies.
+
+
+3.1.5 (08-04-2024)
+------------------
+
+* Fix billing api changes.
```

### Comparing `awsapilib-3.1.4/Pipfile` & `awsapilib-3.1.5/Pipfile`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/Pipfile.lock` & `awsapilib-3.1.5/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9626166384139717%*

 * *Differences: {"'default'": "{'2captcha-python': {'hashes': "*

 * *              "['sha256:b9331618ef323d74200843cb7090a155b8d5b45dd06a20445c45101cbf20170f', "*

 * *              "'sha256:e52237e28c91959a795e6f7f101bd94763ee36dcd54b93ebf5da8813570ade4b'], "*

 * *              "'version': '==1.2.4'}, 'beautifulsoup4': {'hashes': "*

 * *              "['sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051', "*

 * *              "'sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed'], "*

 * *              "'version […]*

```diff
@@ -12,71 +12,71 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "2captcha-python": {
             "hashes": [
-                "sha256:3775b743cde9ee9e393aeff42811278f7ba28a99c3a39915f02b6962f7c297ad",
-                "sha256:b81b78c1b4aed51a373d724675675267d6af6f1b636393479e23cfb5d2ca7b55"
+                "sha256:b9331618ef323d74200843cb7090a155b8d5b45dd06a20445c45101cbf20170f",
+                "sha256:e52237e28c91959a795e6f7f101bd94763ee36dcd54b93ebf5da8813570ade4b"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.6'",
-            "version": "==1.2.2"
+            "version": "==1.2.4"
         },
         "beautifulsoup4": {
             "hashes": [
-                "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da",
-                "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"
+                "sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051",
+                "sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed"
             ],
             "index": "pypi",
             "markers": "python_full_version >= '3.6.0'",
-            "version": "==4.12.2"
+            "version": "==4.12.3"
         },
         "boto3": {
             "hashes": [
-                "sha256:70626598dd6698d6da8f2854a1ae5010f175572e2a465b2aa86685c745c1013c",
-                "sha256:fc7c0dd5fa74ae0d57e11747695bdba4ad164e62dee35db15b43762c392fbd92"
+                "sha256:139dd2d94eaa0e3213ff37ba7cf4cb2e3823269178fe8f3e33c965f680a9ddde",
+                "sha256:265b0b4865e8c07e27abb32a31d2bd9129bb009b1d89ca0783776ec084886123"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==1.33.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.34.79"
         },
         "boto3-type-annotations": {
             "hashes": [
                 "sha256:52e007ac2ab792abee42aaac3019c2acc9781a84e79e1283a5bc64164225435e",
                 "sha256:e5682093d035e935c8189f24c601ef6eaccedfcd1e642ba7922429d093b1b885"
             ],
             "index": "pypi",
             "version": "==0.3.1"
         },
         "botocore": {
             "hashes": [
-                "sha256:16a30faac6e6f17961c009defb74ab1a3508b8abc58fab98e7cf96af0d91ea84",
-                "sha256:5c46b7e8450efbf7ddc2a0016eee7225a5564583122e25a20ca92a29a105225c"
+                "sha256:6b59b0f7de219d383a2a633f6718c2600642ebcb707749dc6c67a6a436474b7a",
+                "sha256:a42a014d3dbaa9ef123810592af69f9e55b456c5be3ac9efc037325685519e83"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.33.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.34.79"
         },
         "cachetools": {
             "hashes": [
                 "sha256:89ea6f1b638d5a73a4f9226be57ac5e4f399d22770b92355f92dcb0f7f001693",
                 "sha256:92971d3cb7d2a97efff7c7bb1657f21a8f5fb309a37530537c71b1774189f2d1"
             ],
             "index": "pypi",
             "markers": "python_version ~= '3.5'",
             "version": "==4.2.4"
         },
         "certifi": {
             "hashes": [
-                "sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1",
-                "sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.11.17"
+            "version": "==2024.2.2"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027",
                 "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087",
                 "sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786",
                 "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8",
@@ -202,36 +202,36 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.9.0"
         },
         "python-dateutil": {
             "hashes": [
-                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
-                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+                "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3",
+                "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.2"
+            "version": "==2.9.0.post0"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.31.0"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:d1c52af7bceca1650d0f27728b29bb4925184aead7b55bccacf893b79a108604",
-                "sha256:e6cafd5643fc7b44fddfba1e5b521005675b0e07533ddad958a3554bc87d7330"
+                "sha256:5683916b4c724f799e600f41dd9e10a9ff19871bf87623cc8f491cb4f5fa0a19",
+                "sha256:ceb252b11bcf87080fb7850a224fb6e05c8a776bab8f2b64b7f25b969464839d"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.8.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.10.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -243,61 +243,70 @@
                 "sha256:eaa337ff55a1579b6549dc679565eac1e3d000563bcb1c8ab0d0fefbc0c2cdc7"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.5"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0",
-                "sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==4.8.0"
+            "version": "==4.11.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:34b97092d7e0a3a8cf7cd10e386f401b3737364026c45e622aa02903dffe0f07",
                 "sha256:f8ecc1bba5667413457c529ab955bf8c67b45db799d159066261719e328580a0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.18"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
-                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
+                "sha256:75a8b99c28a5dad50dd7f8ccdd447a121ddb3892da9e53d1ca5cca3106d58d65",
+                "sha256:b46733c07dce03ae4e150330b975c75737fa60f0a7c591b6c8bf4928a28e2c92"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.7.13"
+            "markers": "python_version >= '3.9'",
+            "version": "==0.7.16"
         },
         "astroid": {
             "hashes": [
                 "sha256:1aa149fc5c6589e3d0ece885b4491acd80af4f087baafa3fb5203b113e68cd3c",
                 "sha256:6c107453dffee9055899705de3c9ead36e74119cee151e5a9aaf7f0b0e020a6a"
             ],
             "markers": "python_full_version >= '3.7.2'",
             "version": "==2.15.8"
         },
         "babel": {
             "hashes": [
-                "sha256:33e0952d7dd6374af8dbf6768cc4ddf3ccfefc244f9986d4074704f2fbd18900",
-                "sha256:7077a4984b02b6727ac10f1f7294484f737443d7e2e66c5e4380e41a3ae0b4ed"
+                "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363",
+                "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.13.1"
+            "version": "==2.14.0"
+        },
+        "backports.tarfile": {
+            "hashes": [
+                "sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75",
+                "sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4"
+            ],
+            "markers": "python_version < '3.12'",
+            "version": "==1.0.0"
         },
         "betamax": {
             "hashes": [
-                "sha256:5bf004ceffccae881213fb722f34517166b84a34919b92ffc14d1dbd050b71c2",
-                "sha256:aa5ad34cc8d018b35814fb0557d15c78ced9ac56fdc43ccacdb882aa7a5217c1"
+                "sha256:82316e1679bc6879e3c83318d016b54b7c9225ff08c4462de4813e22038d5f94",
+                "sha256:880d6da87eaf7e61c42bdc4240f0ac04ab5365bd7f2798784c18d37d8cf747bc"
             ],
             "index": "pypi",
-            "version": "==0.8.1"
+            "markers": "python_full_version >= '3.8.1'",
+            "version": "==0.9.0"
         },
         "betamax-serializers": {
             "hashes": [
                 "sha256:1b23c46429c40a8873682854c88d805c787c72d252f3fa0c858e9c300682ceac",
                 "sha256:345c419b1b73171f2951c62ac3c701775ac4b76e13e86464ebf0ff2a978e4949"
             ],
             "index": "pypi",
@@ -318,77 +327,19 @@
             ],
             "index": "pypi",
             "markers": "python_version ~= '3.5'",
             "version": "==4.2.4"
         },
         "certifi": {
             "hashes": [
-                "sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1",
-                "sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.11.17"
-        },
-        "cffi": {
-            "hashes": [
-                "sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc",
-                "sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a",
-                "sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417",
-                "sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab",
-                "sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520",
-                "sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36",
-                "sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743",
-                "sha256:3686dffb02459559c74dd3d81748269ffb0eb027c39a6fc99502de37d501faa8",
-                "sha256:582215a0e9adbe0e379761260553ba11c58943e4bbe9c36430c4ca6ac74b15ed",
-                "sha256:5b50bf3f55561dac5438f8e70bfcdfd74543fd60df5fa5f62d94e5867deca684",
-                "sha256:5bf44d66cdf9e893637896c7faa22298baebcd18d1ddb6d2626a6e39793a1d56",
-                "sha256:6602bc8dc6f3a9e02b6c22c4fc1e47aa50f8f8e6d3f78a5e16ac33ef5fefa324",
-                "sha256:673739cb539f8cdaa07d92d02efa93c9ccf87e345b9a0b556e3ecc666718468d",
-                "sha256:68678abf380b42ce21a5f2abde8efee05c114c2fdb2e9eef2efdb0257fba1235",
-                "sha256:68e7c44931cc171c54ccb702482e9fc723192e88d25a0e133edd7aff8fcd1f6e",
-                "sha256:6b3d6606d369fc1da4fd8c357d026317fbb9c9b75d36dc16e90e84c26854b088",
-                "sha256:748dcd1e3d3d7cd5443ef03ce8685043294ad6bd7c02a38d1bd367cfd968e000",
-                "sha256:7651c50c8c5ef7bdb41108b7b8c5a83013bfaa8a935590c5d74627c047a583c7",
-                "sha256:7b78010e7b97fef4bee1e896df8a4bbb6712b7f05b7ef630f9d1da00f6444d2e",
-                "sha256:7e61e3e4fa664a8588aa25c883eab612a188c725755afff6289454d6362b9673",
-                "sha256:80876338e19c951fdfed6198e70bc88f1c9758b94578d5a7c4c91a87af3cf31c",
-                "sha256:8895613bcc094d4a1b2dbe179d88d7fb4a15cee43c052e8885783fac397d91fe",
-                "sha256:88e2b3c14bdb32e440be531ade29d3c50a1a59cd4e51b1dd8b0865c54ea5d2e2",
-                "sha256:8f8e709127c6c77446a8c0a8c8bf3c8ee706a06cd44b1e827c3e6a2ee6b8c098",
-                "sha256:9cb4a35b3642fc5c005a6755a5d17c6c8b6bcb6981baf81cea8bfbc8903e8ba8",
-                "sha256:9f90389693731ff1f659e55c7d1640e2ec43ff725cc61b04b2f9c6d8d017df6a",
-                "sha256:a09582f178759ee8128d9270cd1344154fd473bb77d94ce0aeb2a93ebf0feaf0",
-                "sha256:a6a14b17d7e17fa0d207ac08642c8820f84f25ce17a442fd15e27ea18d67c59b",
-                "sha256:a72e8961a86d19bdb45851d8f1f08b041ea37d2bd8d4fd19903bc3083d80c896",
-                "sha256:abd808f9c129ba2beda4cfc53bde801e5bcf9d6e0f22f095e45327c038bfe68e",
-                "sha256:ac0f5edd2360eea2f1daa9e26a41db02dd4b0451b48f7c318e217ee092a213e9",
-                "sha256:b29ebffcf550f9da55bec9e02ad430c992a87e5f512cd63388abb76f1036d8d2",
-                "sha256:b2ca4e77f9f47c55c194982e10f058db063937845bb2b7a86c84a6cfe0aefa8b",
-                "sha256:b7be2d771cdba2942e13215c4e340bfd76398e9227ad10402a8767ab1865d2e6",
-                "sha256:b84834d0cf97e7d27dd5b7f3aca7b6e9263c56308ab9dc8aae9784abb774d404",
-                "sha256:b86851a328eedc692acf81fb05444bdf1891747c25af7529e39ddafaf68a4f3f",
-                "sha256:bcb3ef43e58665bbda2fb198698fcae6776483e0c4a631aa5647806c25e02cc0",
-                "sha256:c0f31130ebc2d37cdd8e44605fb5fa7ad59049298b3f745c74fa74c62fbfcfc4",
-                "sha256:c6a164aa47843fb1b01e941d385aab7215563bb8816d80ff3a363a9f8448a8dc",
-                "sha256:d8a9d3ebe49f084ad71f9269834ceccbf398253c9fac910c4fd7053ff1386936",
-                "sha256:db8e577c19c0fda0beb7e0d4e09e0ba74b1e4c092e0e40bfa12fe05b6f6d75ba",
-                "sha256:dc9b18bf40cc75f66f40a7379f6a9513244fe33c0e8aa72e2d56b0196a7ef872",
-                "sha256:e09f3ff613345df5e8c3667da1d918f9149bd623cd9070c983c013792a9a62eb",
-                "sha256:e4108df7fe9b707191e55f33efbcb2d81928e10cea45527879a4749cbe472614",
-                "sha256:e6024675e67af929088fda399b2094574609396b1decb609c55fa58b028a32a1",
-                "sha256:e70f54f1796669ef691ca07d046cd81a29cb4deb1e5f942003f401c0c4a2695d",
-                "sha256:e715596e683d2ce000574bae5d07bd522c781a822866c20495e52520564f0969",
-                "sha256:e760191dd42581e023a68b758769e2da259b5d52e3103c6060ddc02c9edb8d7b",
-                "sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4",
-                "sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627",
-                "sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956",
-                "sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357"
-            ],
-            "markers": "python_version >= '3.8'",
-            "version": "==1.16.0"
+            "version": "==2024.2.2"
         },
         "chardet": {
             "hashes": [
                 "sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7",
                 "sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970"
             ],
             "markers": "python_version >= '3.7'",
@@ -505,114 +456,85 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:0cbf38419fb1a347aaf63481c00f0bdc86889d9fbf3f25109cf96c26b403fda1",
-                "sha256:12d15ab5833a997716d76f2ac1e4b4d536814fc213c85ca72756c19e5a6b3d63",
-                "sha256:149de1d2401ae4655c436a3dced6dd153f4c3309f599c3d4bd97ab172eaf02d9",
-                "sha256:1981f785239e4e39e6444c63a98da3a1db8e971cb9ceb50a945ba6296b43f312",
-                "sha256:2443cbda35df0d35dcfb9bf8f3c02c57c1d6111169e3c85fc1fcc05e0c9f39a3",
-                "sha256:289fe43bf45a575e3ab10b26d7b6f2ddb9ee2dba447499f5401cfb5ecb8196bb",
-                "sha256:2f11cc3c967a09d3695d2a6f03fb3e6236622b93be7a4b5dc09166a861be6d25",
-                "sha256:307adb8bd3abe389a471e649038a71b4eb13bfd6b7dd9a129fa856f5c695cf92",
-                "sha256:310b3bb9c91ea66d59c53fa4989f57d2436e08f18fb2f421a1b0b6b8cc7fffda",
-                "sha256:315a989e861031334d7bee1f9113c8770472db2ac484e5b8c3173428360a9148",
-                "sha256:3a4006916aa6fee7cd38db3bfc95aa9c54ebb4ffbfc47c677c8bba949ceba0a6",
-                "sha256:3c7bba973ebee5e56fe9251300c00f1579652587a9f4a5ed8404b15a0471f216",
-                "sha256:4175e10cc8dda0265653e8714b3174430b07c1dca8957f4966cbd6c2b1b8065a",
-                "sha256:43668cabd5ca8258f5954f27a3aaf78757e6acf13c17604d89648ecc0cc66640",
-                "sha256:4cbae1051ab791debecc4a5dcc4a1ff45fc27b91b9aee165c8a27514dd160836",
-                "sha256:5c913b556a116b8d5f6ef834038ba983834d887d82187c8f73dec21049abd65c",
-                "sha256:5f7363d3b6a1119ef05015959ca24a9afc0ea8a02c687fe7e2d557705375c01f",
-                "sha256:630b13e3036e13c7adc480ca42fa7afc2a5d938081d28e20903cf7fd687872e2",
-                "sha256:72c0cfa5250f483181e677ebc97133ea1ab3eb68645e494775deb6a7f6f83901",
-                "sha256:7dbc3ed60e8659bc59b6b304b43ff9c3ed858da2839c78b804973f613d3e92ed",
-                "sha256:88ed2c30a49ea81ea3b7f172e0269c182a44c236eb394718f976239892c0a27a",
-                "sha256:89a937174104339e3a3ffcf9f446c00e3a806c28b1841c63edb2b369310fd074",
-                "sha256:9028a3871280110d6e1aa2df1afd5ef003bab5fb1ef421d6dc748ae1c8ef2ebc",
-                "sha256:99b89d9f76070237975b315b3d5f4d6956ae354a4c92ac2388a5695516e47c84",
-                "sha256:9f805d62aec8eb92bab5b61c0f07329275b6f41c97d80e847b03eb894f38d083",
-                "sha256:a889ae02f43aa45032afe364c8ae84ad3c54828c2faa44f3bfcafecb5c96b02f",
-                "sha256:aa72dbaf2c2068404b9870d93436e6d23addd8bbe9295f49cbca83f6e278179c",
-                "sha256:ac8c802fa29843a72d32ec56d0ca792ad15a302b28ca6203389afe21f8fa062c",
-                "sha256:ae97af89f0fbf373400970c0a21eef5aa941ffeed90aee43650b81f7d7f47637",
-                "sha256:af3d828d2c1cbae52d34bdbb22fcd94d1ce715d95f1a012354a75e5913f1bda2",
-                "sha256:b4275802d16882cf9c8b3d057a0839acb07ee9379fa2749eca54efbce1535b82",
-                "sha256:b4767da59464bb593c07afceaddea61b154136300881844768037fd5e859353f",
-                "sha256:b631c92dfe601adf8f5ebc7fc13ced6bb6e9609b19d9a8cd59fa47c4186ad1ce",
-                "sha256:be32ad29341b0170e795ca590e1c07e81fc061cb5b10c74ce7203491484404ef",
-                "sha256:beaa5c1b4777f03fc63dfd2a6bd820f73f036bfb10e925fce067b00a340d0f3f",
-                "sha256:c0ba320de3fb8c6ec16e0be17ee1d3d69adcda99406c43c0409cb5c41788a611",
-                "sha256:c9eacf273e885b02a0273bb3a2170f30e2d53a6d53b72dbe02d6701b5296101c",
-                "sha256:cb536f0dcd14149425996821a168f6e269d7dcd2c273a8bff8201e79f5104e76",
-                "sha256:d1bc430677773397f64a5c88cb522ea43175ff16f8bfcc89d467d974cb2274f9",
-                "sha256:d1c88ec1a7ff4ebca0219f5b1ef863451d828cccf889c173e1253aa84b1e07ce",
-                "sha256:d3d9df4051c4a7d13036524b66ecf7a7537d14c18a384043f30a303b146164e9",
-                "sha256:d51ac2a26f71da1b57f2dc81d0e108b6ab177e7d30e774db90675467c847bbdf",
-                "sha256:d872145f3a3231a5f20fd48500274d7df222e291d90baa2026cc5152b7ce86bf",
-                "sha256:d8f17966e861ff97305e0801134e69db33b143bbfb36436efb9cfff6ec7b2fd9",
-                "sha256:dbc1b46b92186cc8074fee9d9fbb97a9dd06c6cbbef391c2f59d80eabdf0faa6",
-                "sha256:e10c39c0452bf6e694511c901426d6b5ac005acc0f78ff265dbe36bf81f808a2",
-                "sha256:e267e9e2b574a176ddb983399dec325a80dbe161f1a32715c780b5d14b5f583a",
-                "sha256:f47d39359e2c3779c5331fc740cf4bce6d9d680a7b4b4ead97056a0ae07cb49a",
-                "sha256:f6e9589bd04d0461a417562649522575d8752904d35c12907d8c9dfeba588faf",
-                "sha256:f94b734214ea6a36fe16e96a70d941af80ff3bfd716c141300d95ebc85339738",
-                "sha256:fa28e909776dc69efb6ed975a63691bc8172b64ff357e663a1bb06ff3c9b589a",
-                "sha256:fe494faa90ce6381770746077243231e0b83ff3f17069d748f645617cefe19d4"
+                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
+                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
+                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
+                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
+                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
+                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
+                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
+                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
+                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
+                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
+                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
+                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
+                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
+                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
+                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
+                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
+                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
+                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
+                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
+                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
+                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
+                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
+                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
+                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
+                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
+                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
+                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
+                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
+                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
+                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
+                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
+                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
+                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
+                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
+                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
+                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
+                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
+                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
+                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
+                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
+                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
+                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
+                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
+                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
+                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
+                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
+                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
+                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
+                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
+                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
+                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
+                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==7.3.2"
-        },
-        "cryptography": {
-            "hashes": [
-                "sha256:079b85658ea2f59c4f43b70f8119a52414cdb7be34da5d019a77bf96d473b960",
-                "sha256:09616eeaef406f99046553b8a40fbf8b1e70795a91885ba4c96a70793de5504a",
-                "sha256:13f93ce9bea8016c253b34afc6bd6a75993e5c40672ed5405a9c832f0d4a00bc",
-                "sha256:37a138589b12069efb424220bf78eac59ca68b95696fc622b6ccc1c0a197204a",
-                "sha256:3c78451b78313fa81607fa1b3f1ae0a5ddd8014c38a02d9db0616133987b9cdf",
-                "sha256:43f2552a2378b44869fe8827aa19e69512e3245a219104438692385b0ee119d1",
-                "sha256:48a0476626da912a44cc078f9893f292f0b3e4c739caf289268168d8f4702a39",
-                "sha256:49f0805fc0b2ac8d4882dd52f4a3b935b210935d500b6b805f321addc8177406",
-                "sha256:5429ec739a29df2e29e15d082f1d9ad683701f0ec7709ca479b3ff2708dae65a",
-                "sha256:5a1b41bc97f1ad230a41657d9155113c7521953869ae57ac39ac7f1bb471469a",
-                "sha256:68a2dec79deebc5d26d617bfdf6e8aab065a4f34934b22d3b5010df3ba36612c",
-                "sha256:7a698cb1dac82c35fcf8fe3417a3aaba97de16a01ac914b89a0889d364d2f6be",
-                "sha256:841df4caa01008bad253bce2a6f7b47f86dc9f08df4b433c404def869f590a15",
-                "sha256:90452ba79b8788fa380dfb587cca692976ef4e757b194b093d845e8d99f612f2",
-                "sha256:928258ba5d6f8ae644e764d0f996d61a8777559f72dfeb2eea7e2fe0ad6e782d",
-                "sha256:af03b32695b24d85a75d40e1ba39ffe7db7ffcb099fe507b39fd41a565f1b157",
-                "sha256:b640981bf64a3e978a56167594a0e97db71c89a479da8e175d8bb5be5178c003",
-                "sha256:c5ca78485a255e03c32b513f8c2bc39fedb7f5c5f8535545bdc223a03b24f248",
-                "sha256:c7f3201ec47d5207841402594f1d7950879ef890c0c495052fa62f58283fde1a",
-                "sha256:d5ec85080cce7b0513cfd233914eb8b7bbd0633f1d1703aa28d1dd5a72f678ec",
-                "sha256:d6c391c021ab1f7a82da5d8d0b3cee2f4b2c455ec86c8aebbc84837a631ff309",
-                "sha256:e3114da6d7f95d2dee7d3f4eec16dacff819740bbab931aff8648cb13c5ff5e7",
-                "sha256:f983596065a18a2183e7f79ab3fd4c475205b839e02cbc0efbbf9666c4b3083d"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==41.0.7"
+            "version": "==7.4.4"
         },
         "dill": {
             "hashes": [
-                "sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e",
-                "sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03"
+                "sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca",
+                "sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==0.3.7"
+            "version": "==0.3.8"
         },
         "distlib": {
             "hashes": [
-                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
-                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
+                "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784",
+                "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"
             ],
-            "version": "==0.3.7"
+            "version": "==0.3.8"
         },
         "docutils": {
             "hashes": [
                 "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -623,28 +545,28 @@
                 "sha256:28323cbfc9352139fdd3d316fa17f325cc0e9ac74438cbba51d70f9b48f86c3a",
                 "sha256:51f54c0fd886fa3854387f354b19f429d38c04f984f38bc572558b703c0542a6"
             ],
             "version": "==0.2.1"
         },
         "emoji": {
             "hashes": [
-                "sha256:8d8b5dec3c507444b58890e598fc895fcec022b3f5acb49497c6ccc5208b8b00",
-                "sha256:a8468fd836b7ecb6d1eac054c9a591701ce0ccd6c6f7779ad71b66f76664df90"
+                "sha256:63fc9107f06c6c2e48e5078ce9575cef98518f5ac09474f6148a43e989989582",
+                "sha256:772eaa30f4e0b1ce95148a092df4c7dc97644532c03225326b0fd05e8a9f72a3"
             ],
             "index": "pypi",
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.0"
+            "version": "==2.11.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e",
-                "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"
+                "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb",
+                "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.13.1"
+            "version": "==3.13.3"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -663,27 +585,26 @@
                 "sha256:bf5421126136d6d0af55bc1e7c1af1c397a34f5b7bd79e776cd3e89785c2b04b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.0.11"
         },
         "gitpython": {
             "hashes": [
-                "sha256:22b126e9ffb671fdd0c129796343a02bf67bf2994b35449ffc9321aa755e18a4",
-                "sha256:cf14627d5a8049ffbf49915732e5eddbe8134c3bdb9d476e6182b676fc573f8a"
+                "sha256:35f314a9f878467f5453cc1fee295c3e18e52f1b99f10f6cf5b1682e968a9e7c",
+                "sha256:eec7ec56b92aad751f9912a73404bc02ba212a23adb2c7098ee668417051a1ff"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.40"
+            "version": "==3.1.43"
         },
         "gitwrapperlib": {
             "hashes": [
-                "sha256:2f1c5e0fc69168dde3cd141f56b7714c6841ebe886956c1cd302c5867b640db7",
-                "sha256:90b33ad4568e5ce056d0058b98dd850a6dee2473d3bfc115f35c721e62f95078"
+                "sha256:f4b0adc0f91a568dd6c385306fa88af02221fef3e7ccf9000d428ace5aafe086"
             ],
             "index": "pypi",
-            "version": "==1.0.3"
+            "version": "==1.0.4"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -703,175 +624,184 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
-                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==6.8.0"
+            "markers": "python_version < '3.10'",
+            "version": "==7.1.0"
         },
         "isort": {
             "hashes": [
-                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
-                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
+                "sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109",
+                "sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6"
             ],
             "markers": "python_full_version >= '3.8.0'",
-            "version": "==5.12.0"
+            "version": "==5.13.2"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb",
-                "sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621"
+                "sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd",
+                "sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.3.0"
+            "version": "==3.4.0"
         },
-        "jeepney": {
+        "jaraco.context": {
             "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+                "sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266",
+                "sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.3.0"
+        },
+        "jaraco.functools": {
+            "hashes": [
+                "sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925",
+                "sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.0"
         },
         "jinja2": {
             "hashes": [
-                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
-                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
+                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.2"
+            "version": "==3.1.3"
         },
         "keyring": {
             "hashes": [
-                "sha256:4446d35d636e6a10b8bce7caa66913dd9eca5fd222ca03a3d42c38608ac30836",
-                "sha256:e730ecffd309658a08ee82535a3b5ec4b4c8669a9be11efb66249d8e0aeb9a25"
+                "sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427",
+                "sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==24.3.0"
+            "version": "==25.1.0"
         },
         "lazy-object-proxy": {
             "hashes": [
-                "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
-                "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
-                "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
-                "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
-                "sha256:1aa3de4088c89a1b69f8ec0dcc169aa725b0ff017899ac568fe44ddc1396df46",
-                "sha256:212774e4dfa851e74d393a2370871e174d7ff0ebc980907723bb67d25c8a7c30",
-                "sha256:2d0daa332786cf3bb49e10dc6a17a52f6a8f9601b4cf5c295a4f85854d61de63",
-                "sha256:5f83ac4d83ef0ab017683d715ed356e30dd48a93746309c8f3517e1287523ef4",
-                "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae",
-                "sha256:660c94ea760b3ce47d1855a30984c78327500493d396eac4dfd8bd82041b22be",
-                "sha256:66a3de4a3ec06cd8af3f61b8e1ec67614fbb7c995d02fa224813cb7afefee701",
-                "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd",
-                "sha256:7322c3d6f1766d4ef1e51a465f47955f1e8123caee67dd641e67d539a534d006",
-                "sha256:79a31b086e7e68b24b99b23d57723ef7e2c6d81ed21007b6281ebcd1688acb0a",
-                "sha256:81fc4d08b062b535d95c9ea70dbe8a335c45c04029878e62d744bdced5141586",
-                "sha256:8fa02eaab317b1e9e03f69aab1f91e120e7899b392c4fc19807a8278a07a97e8",
-                "sha256:9090d8e53235aa280fc9239a86ae3ea8ac58eff66a705fa6aa2ec4968b95c821",
-                "sha256:946d27deaff6cf8452ed0dba83ba38839a87f4f7a9732e8f9fd4107b21e6ff07",
-                "sha256:9990d8e71b9f6488e91ad25f322898c136b008d87bf852ff65391b004da5e17b",
-                "sha256:9cd077f3d04a58e83d04b20e334f678c2b0ff9879b9375ed107d5d07ff160171",
-                "sha256:9e7551208b2aded9c1447453ee366f1c4070602b3d932ace044715d89666899b",
-                "sha256:9f5fa4a61ce2438267163891961cfd5e32ec97a2c444e5b842d574251ade27d2",
-                "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7",
-                "sha256:bfb38f9ffb53b942f2b5954e0f610f1e721ccebe9cce9025a38c8ccf4a5183a4",
-                "sha256:cbf9b082426036e19c6924a9ce90c740a9861e2bdc27a4834fd0a910742ac1e8",
-                "sha256:d9e25ef10a39e8afe59a5c348a4dbf29b4868ab76269f81ce1674494e2565a6e",
-                "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f",
-                "sha256:e7c21c95cae3c05c14aafffe2865bbd5e377cfc1348c4f7751d9dc9a48ca4bda",
-                "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4",
-                "sha256:ea806fd4c37bf7e7ad82537b0757999264d5f70c45468447bb2b91afdbe73a6e",
-                "sha256:edd20c5a55acb67c7ed471fa2b5fb66cb17f61430b7a6b9c3b4a1e40293b1671",
-                "sha256:f0117049dd1d5635bbff65444496c90e0baa48ea405125c088e93d9cf4525b11",
-                "sha256:f0705c376533ed2a9e5e97aacdbfe04cecd71e0aa84c7c0595d02ef93b6e4455",
-                "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
-                "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
-                "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
+                "sha256:009e6bb1f1935a62889ddc8541514b6a9e1fcf302667dcb049a0be5c8f613e56",
+                "sha256:02c83f957782cbbe8136bee26416686a6ae998c7b6191711a04da776dc9e47d4",
+                "sha256:0aefc7591920bbd360d57ea03c995cebc204b424524a5bd78406f6e1b8b2a5d8",
+                "sha256:127a789c75151db6af398b8972178afe6bda7d6f68730c057fbbc2e96b08d282",
+                "sha256:18dd842b49456aaa9a7cf535b04ca4571a302ff72ed8740d06b5adcd41fe0757",
+                "sha256:217138197c170a2a74ca0e05bddcd5f1796c735c37d0eee33e43259b192aa424",
+                "sha256:2297f08f08a2bb0d32a4265e98a006643cd7233fb7983032bd61ac7a02956b3b",
+                "sha256:2fc0a92c02fa1ca1e84fc60fa258458e5bf89d90a1ddaeb8ed9cc3147f417255",
+                "sha256:30b339b2a743c5288405aa79a69e706a06e02958eab31859f7f3c04980853b70",
+                "sha256:366c32fe5355ef5fc8a232c5436f4cc66e9d3e8967c01fb2e6302fd6627e3d94",
+                "sha256:3ad54b9ddbe20ae9f7c1b29e52f123120772b06dbb18ec6be9101369d63a4074",
+                "sha256:5ad9e6ed739285919aa9661a5bbed0aaf410aa60231373c5579c6b4801bd883c",
+                "sha256:5faf03a7d8942bb4476e3b62fd0f4cf94eaf4618e304a19865abf89a35c0bbee",
+                "sha256:75fc59fc450050b1b3c203c35020bc41bd2695ed692a392924c6ce180c6f1dc9",
+                "sha256:76a095cfe6045c7d0ca77db9934e8f7b71b14645f0094ffcd842349ada5c5fb9",
+                "sha256:78247b6d45f43a52ef35c25b5581459e85117225408a4128a3daf8bf9648ac69",
+                "sha256:782e2c9b2aab1708ffb07d4bf377d12901d7a1d99e5e410d648d892f8967ab1f",
+                "sha256:7ab7004cf2e59f7c2e4345604a3e6ea0d92ac44e1c2375527d56492014e690c3",
+                "sha256:80b39d3a151309efc8cc48675918891b865bdf742a8616a337cb0090791a0de9",
+                "sha256:80fa48bd89c8f2f456fc0765c11c23bf5af827febacd2f523ca5bc1893fcc09d",
+                "sha256:855e068b0358ab916454464a884779c7ffa312b8925c6f7401e952dcf3b89977",
+                "sha256:92f09ff65ecff3108e56526f9e2481b8116c0b9e1425325e13245abfd79bdb1b",
+                "sha256:952c81d415b9b80ea261d2372d2a4a2332a3890c2b83e0535f263ddfe43f0d43",
+                "sha256:9a3a87cf1e133e5b1994144c12ca4aa3d9698517fe1e2ca82977781b16955658",
+                "sha256:9e4ed0518a14dd26092614412936920ad081a424bdcb54cc13349a8e2c6d106a",
+                "sha256:a899b10e17743683b293a729d3a11f2f399e8a90c73b089e29f5d0fe3509f0dd",
+                "sha256:b1f711e2c6dcd4edd372cf5dec5c5a30d23bba06ee012093267b3376c079ec83",
+                "sha256:b4f87d4ed9064b2628da63830986c3d2dca7501e6018347798313fcf028e2fd4",
+                "sha256:cb73507defd385b7705c599a94474b1d5222a508e502553ef94114a143ec6696",
+                "sha256:dc0d2fc424e54c70c4bc06787e4072c4f3b1aa2f897dfdc34ce1013cf3ceef05",
+                "sha256:e221060b701e2aa2ea991542900dd13907a5c90fa80e199dbf5a03359019e7a3",
+                "sha256:e271058822765ad5e3bca7f05f2ace0de58a3f4e62045a8c90a0dfd2f8ad8cc6",
+                "sha256:e2adb09778797da09d2b5ebdbceebf7dd32e2c96f79da9052b2e87b6ea495895",
+                "sha256:e333e2324307a7b5d86adfa835bb500ee70bfcd1447384a822e96495796b0ca4",
+                "sha256:e98c8af98d5707dcdecc9ab0863c0ea6e88545d42ca7c3feffb6b4d1e370c7ba",
+                "sha256:edb45bb8278574710e68a6b021599a10ce730d156e5b254941754a9cc0b17d03",
+                "sha256:fec03caabbc6b59ea4a638bee5fce7117be8e99a4103d9d5ad77f15d6f81020c"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.9.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.10.0"
         },
         "markdown-it-py": {
             "hashes": [
                 "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
                 "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
-                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
-                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
-                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
-                "sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c",
-                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
-                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
-                "sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb",
-                "sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939",
-                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
-                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
-                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
-                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
-                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
-                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
-                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
-                "sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd",
-                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
-                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
-                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
-                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
-                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
-                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
-                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
-                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
-                "sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007",
-                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
-                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
-                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
-                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
-                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
-                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
-                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
-                "sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1",
-                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
-                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
-                "sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c",
-                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
-                "sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823",
-                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
-                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
-                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
-                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
-                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
-                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
-                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
-                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
-                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
-                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
-                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
-                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
-                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
-                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
-                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
-                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
-                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
-                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
-                "sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc",
-                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2",
-                "sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11"
+                "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf",
+                "sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff",
+                "sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f",
+                "sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3",
+                "sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532",
+                "sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f",
+                "sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617",
+                "sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df",
+                "sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4",
+                "sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906",
+                "sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f",
+                "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4",
+                "sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8",
+                "sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371",
+                "sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2",
+                "sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465",
+                "sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52",
+                "sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6",
+                "sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169",
+                "sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad",
+                "sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2",
+                "sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0",
+                "sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029",
+                "sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f",
+                "sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a",
+                "sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced",
+                "sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5",
+                "sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c",
+                "sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf",
+                "sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9",
+                "sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb",
+                "sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad",
+                "sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3",
+                "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1",
+                "sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46",
+                "sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc",
+                "sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a",
+                "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee",
+                "sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900",
+                "sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5",
+                "sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea",
+                "sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f",
+                "sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5",
+                "sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e",
+                "sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a",
+                "sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f",
+                "sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50",
+                "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a",
+                "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b",
+                "sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4",
+                "sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff",
+                "sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2",
+                "sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46",
+                "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b",
+                "sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf",
+                "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5",
+                "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5",
+                "sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab",
+                "sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd",
+                "sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.3"
+            "version": "==2.1.5"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -883,40 +813,40 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a",
-                "sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6"
+                "sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684",
+                "sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==10.1.0"
+            "version": "==10.2.0"
         },
         "nh3": {
             "hashes": [
-                "sha256:116c9515937f94f0057ef50ebcbcc10600860065953ba56f14473ff706371873",
-                "sha256:18415df36db9b001f71a42a3a5395db79cf23d556996090d293764436e98e8ad",
-                "sha256:203cac86e313cf6486704d0ec620a992c8bc164c86d3a4fd3d761dd552d839b5",
-                "sha256:2b0be5c792bd43d0abef8ca39dd8acb3c0611052ce466d0401d51ea0d9aa7525",
-                "sha256:377aaf6a9e7c63962f367158d808c6a1344e2b4f83d071c43fbd631b75c4f0b2",
-                "sha256:525846c56c2bcd376f5eaee76063ebf33cf1e620c1498b2a40107f60cfc6054e",
-                "sha256:5529a3bf99402c34056576d80ae5547123f1078da76aa99e8ed79e44fa67282d",
-                "sha256:7771d43222b639a4cd9e341f870cee336b9d886de1ad9bec8dddab22fe1de450",
-                "sha256:88c753efbcdfc2644a5012938c6b9753f1c64a5723a67f0301ca43e7b85dcf0e",
-                "sha256:93a943cfd3e33bd03f77b97baa11990148687877b74193bf777956b67054dcc6",
-                "sha256:9be2f68fb9a40d8440cbf34cbf40758aa7f6093160bfc7fb018cce8e424f0c3a",
-                "sha256:a0c509894fd4dccdff557068e5074999ae3b75f4c5a2d6fb5415e782e25679c4",
-                "sha256:ac8056e937f264995a82bf0053ca898a1cb1c9efc7cd68fa07fe0060734df7e4",
-                "sha256:aed56a86daa43966dd790ba86d4b810b219f75b4bb737461b6886ce2bde38fd6",
-                "sha256:e8986f1dd3221d1e741fda0a12eaa4a273f1d80a35e31a1ffe579e7c621d069e",
-                "sha256:f99212a81c62b5f22f9e7c3e347aa00491114a5647e1f13bbebd79c3e5f08d75"
+                "sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a",
+                "sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911",
+                "sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb",
+                "sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a",
+                "sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc",
+                "sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028",
+                "sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9",
+                "sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3",
+                "sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351",
+                "sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10",
+                "sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71",
+                "sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f",
+                "sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b",
+                "sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a",
+                "sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062",
+                "sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a"
             ],
-            "version": "==0.2.14"
+            "version": "==0.2.17"
         },
         "nose": {
             "hashes": [
                 "sha256:9ff7c6cc443f8c51994b34a667bbcf45afd6d945be7477b52e97516fd17c53ac",
                 "sha256:dadcddc0aefbf99eea214e0f1232b94f2fa9bd98fa8353711dacb112bfcbbb2a",
                 "sha256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98"
             ],
@@ -929,50 +859,50 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
-                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
+                "sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297",
+                "sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.9.6"
+            "version": "==1.10.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:118c954d7e949b35437270383a3f2531e99dd93cf7ce4dc8340d3356d30f173b",
-                "sha256:cb633b2bcf10c51af60beb0ab06d2f1d69064b43abf4c185ca6b28865f3f9731"
+                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
+                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==4.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12",
-                "sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7"
+                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
+                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.3.0"
+            "version": "==1.4.0"
         },
         "poetry-semver": {
             "hashes": [
                 "sha256:4e6349bd7231cc657f0e1930f7b204e87e33dfd63eef5cac869363969515083a",
                 "sha256:d809b612aa27b39bf2d0fc9d31b4f4809b0e972646c5f19cfa46c725b7638810"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -991,21 +921,14 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
-            ],
-            "version": "==2.21"
-        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -1096,14 +1019,15 @@
                 "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
                 "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
                 "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
                 "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28",
                 "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4",
                 "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
                 "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef",
                 "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
                 "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
                 "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
                 "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
                 "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
                 "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
                 "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
@@ -1123,19 +1047,19 @@
                 "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0.1"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:13d039515c1f24de668e2c93f2e877b9dbe6c6c32328b90a40a49d8b2b85f36d",
-                "sha256:2d55489f83be4992fe4454939d1a051c33edbab778e82761d060c9fc6b308cd1"
+                "sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311",
+                "sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==42.0"
+            "version": "==43.0"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
@@ -1164,27 +1088,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa",
-                "sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235"
+                "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222",
+                "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.7.0"
-        },
-        "secretstorage": {
-            "hashes": [
-                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
-                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.3"
+            "version": "==13.7.1"
         },
         "semver": {
             "hashes": [
                 "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4",
                 "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"
             ],
             "index": "pypi",
@@ -1199,15 +1115,15 @@
             "version": "==0.3.1"
         },
         "sh": {
             "hashes": [
                 "sha256:9b2998f313f201c777e2c0061f0b1367497097ef13388595be147e2a00bf7ba1",
                 "sha256:ced8f2e081a858b66a46ace3703dec243779abbd5a1887ba7e3c34f34da70cd2"
             ],
-            "markers": "sys_platform != 'win32'",
+            "markers": "python_version < '4.0' and python_full_version >= '3.8.1'",
             "version": "==2.0.6"
         },
         "smmap": {
             "hashes": [
                 "sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62",
                 "sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da"
             ],
@@ -1237,35 +1153,35 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.3.0"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:094c4d56209d1734e7d252f6e0b3ccc090bd52ee56807a5d9315b19c122ab15d",
-                "sha256:39fdc8d762d33b01a7d8f026a3b7d71563ea3b72787d5f00ad8465bd9d6dfbfa"
+                "sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619",
+                "sha256:cb61eb0ec1b61f349e5cc36b2028e9e7ca765be05e49641c97241274753067b4"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.0.7"
+            "version": "==1.0.8"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
-                "sha256:63b41e0d38207ca40ebbeabcf4d8e51f76c03e78cd61abe118cf4435c73d4212",
-                "sha256:fe8009aed765188f08fcaadbb3ea0d90ce8ae2d76710b7e29ea7d047177dae2f"
+                "sha256:6485d09629944511c893fa11355bda18b742b83a2b181f9a009f7e500595c90f",
+                "sha256:9893fd3f90506bc4b97bdb977ceb8fbd823989f4316b28c3841ec128544372d3"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.0.5"
+            "version": "==1.0.6"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:6c26a118a05b76000738429b724a0568dbde5b72391a688577da08f11891092a",
-                "sha256:8001661c077a73c29beaf4a79968d0726103c5605e27db92b9ebed8bab1359e9"
+                "sha256:0dc87637d5de53dd5eec3a6a01753b1ccf99494bd756aafecd74b4fa9e729015",
+                "sha256:393f04f112b4d2f53d93448d4bce35842f62b307ccdc549ec1585e950bc35e04"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==2.0.4"
+            "version": "==2.0.5"
         },
         "sphinxcontrib-jquery": {
             "hashes": [
                 "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
                 "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
             ],
             "markers": "python_version >= '2.7'",
@@ -1277,27 +1193,27 @@
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.1"
         },
         "sphinxcontrib-qthelp": {
             "hashes": [
-                "sha256:62b9d1a186ab7f5ee3356d906f648cacb7a6bdb94d201ee7adf26db55092982d",
-                "sha256:bf76886ee7470b934e363da7a954ea2825650013d367728588732c7350f49ea4"
+                "sha256:053dedc38823a80a7209a80860b16b722e9e0209e32fea98c90e4e6624588ed6",
+                "sha256:e2ae3b5c492d58fcbd73281fbd27e34b8393ec34a073c792642cd8e529288182"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.0.6"
+            "version": "==1.0.7"
         },
         "sphinxcontrib-serializinghtml": {
             "hashes": [
-                "sha256:0c64ff898339e1fac29abd2bf5f11078f3ec413cfe9c046d3120d7ca65530b54",
-                "sha256:9b36e503703ff04f20e9675771df105e58aa029cfcbc23b8ed716019b7416ae1"
+                "sha256:326369b8df80a7d2d8d7f99aa5ac577f51ea51556ed974e7716cfd4fca3f6cb7",
+                "sha256:93f3f5dc458b91b192fe10c397e324f262cf163d79f3282c158e8436a2c4511f"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.1.9"
+            "version": "==1.1.10"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
@@ -1310,19 +1226,19 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:75baf5012d06501f07bee5bf8e801b9f343e7aac5a92581f20f80ce632e6b5a4",
-                "sha256:b0a645a9156dc7cb5d3a1f0d4bab66db287fcb8e0430bdd4664a095ea16414ba"
+                "sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b",
+                "sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.12.3"
+            "version": "==0.12.4"
         },
         "tox": {
             "hashes": [
                 "sha256:445fb1fe5d0b0e8ea59a66c7d03e4b829e3524e61d5905cf3387b56161484eb8",
                 "sha256:78efc716e760390b5129bdf4f46662ff771d767085377f2d623894096f5320ea"
             ],
             "index": "pypi",
@@ -1336,35 +1252,35 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0",
-                "sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==4.8.0"
+            "version": "==4.11.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:34b97092d7e0a3a8cf7cd10e386f401b3737364026c45e622aa02903dffe0f07",
                 "sha256:f8ecc1bba5667413457c529ab955bf8c67b45db799d159066261719e328580a0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.18"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:69050ffb42419c91f6c1284a7b24e0475d793447e35929b488bf6a0aade39353",
-                "sha256:a18b3fd0314ca59a2e9f4b556819ed07183b3e9a3702ecfe213f593d44f7b3fd"
+                "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a",
+                "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.24.7"
+            "version": "==20.25.1"
         },
         "wrapt": {
             "hashes": [
                 "sha256:0d2691979e93d06a95a26257adb7bfd0c93818e89b1406f5a28f36e0d8c1e1fc",
                 "sha256:14d7dc606219cdd7405133c713f2c218d4252f2a469003f8c46bb92d5d095d81",
                 "sha256:1a5db485fe2de4403f13fafdc231b0dbae5eca4359232d2efc79025527375b09",
                 "sha256:1acd723ee2a8826f3d53910255643e33673e1d11db84ce5880675954183ec47e",
@@ -1436,15 +1352,15 @@
                 "sha256:ffa565331890b90056c01db69c0fe634a776f8019c143a5ae265f9c6bc4bd6d4"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.16.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31",
-                "sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0"
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.17.0"
+            "version": "==3.18.1"
         }
     }
 }
```

### Comparing `awsapilib-3.1.4/README.rst` & `awsapilib-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/CONTRIBUTING.rst` & `awsapilib-3.1.5/awsapilib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/HISTORY.rst` & `awsapilib-3.1.5/awsapilib/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -231,7 +231,13 @@
 * Bump and loosen dependencies.
 
 
 3.1.4 (29-11-2023)
 ------------------
 
 * Remove gov regions from Control Tower. Bump dependencies.
+
+
+3.1.5 (08-04-2024)
+------------------
+
+* Fix billing api changes.
```

### Comparing `awsapilib-3.1.4/awsapilib/LICENSE` & `awsapilib-3.1.5/awsapilib/LICENSE`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/Pipfile` & `awsapilib-3.1.5/awsapilib/Pipfile`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/Pipfile.lock` & `awsapilib-3.1.5/awsapilib/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9626166384139717%*

 * *Differences: {"'default'": "{'2captcha-python': {'hashes': "*

 * *              "['sha256:b9331618ef323d74200843cb7090a155b8d5b45dd06a20445c45101cbf20170f', "*

 * *              "'sha256:e52237e28c91959a795e6f7f101bd94763ee36dcd54b93ebf5da8813570ade4b'], "*

 * *              "'version': '==1.2.4'}, 'beautifulsoup4': {'hashes': "*

 * *              "['sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051', "*

 * *              "'sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed'], "*

 * *              "'version […]*

```diff
@@ -12,71 +12,71 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "2captcha-python": {
             "hashes": [
-                "sha256:3775b743cde9ee9e393aeff42811278f7ba28a99c3a39915f02b6962f7c297ad",
-                "sha256:b81b78c1b4aed51a373d724675675267d6af6f1b636393479e23cfb5d2ca7b55"
+                "sha256:b9331618ef323d74200843cb7090a155b8d5b45dd06a20445c45101cbf20170f",
+                "sha256:e52237e28c91959a795e6f7f101bd94763ee36dcd54b93ebf5da8813570ade4b"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.6'",
-            "version": "==1.2.2"
+            "version": "==1.2.4"
         },
         "beautifulsoup4": {
             "hashes": [
-                "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da",
-                "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"
+                "sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051",
+                "sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed"
             ],
             "index": "pypi",
             "markers": "python_full_version >= '3.6.0'",
-            "version": "==4.12.2"
+            "version": "==4.12.3"
         },
         "boto3": {
             "hashes": [
-                "sha256:70626598dd6698d6da8f2854a1ae5010f175572e2a465b2aa86685c745c1013c",
-                "sha256:fc7c0dd5fa74ae0d57e11747695bdba4ad164e62dee35db15b43762c392fbd92"
+                "sha256:139dd2d94eaa0e3213ff37ba7cf4cb2e3823269178fe8f3e33c965f680a9ddde",
+                "sha256:265b0b4865e8c07e27abb32a31d2bd9129bb009b1d89ca0783776ec084886123"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==1.33.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.34.79"
         },
         "boto3-type-annotations": {
             "hashes": [
                 "sha256:52e007ac2ab792abee42aaac3019c2acc9781a84e79e1283a5bc64164225435e",
                 "sha256:e5682093d035e935c8189f24c601ef6eaccedfcd1e642ba7922429d093b1b885"
             ],
             "index": "pypi",
             "version": "==0.3.1"
         },
         "botocore": {
             "hashes": [
-                "sha256:16a30faac6e6f17961c009defb74ab1a3508b8abc58fab98e7cf96af0d91ea84",
-                "sha256:5c46b7e8450efbf7ddc2a0016eee7225a5564583122e25a20ca92a29a105225c"
+                "sha256:6b59b0f7de219d383a2a633f6718c2600642ebcb707749dc6c67a6a436474b7a",
+                "sha256:a42a014d3dbaa9ef123810592af69f9e55b456c5be3ac9efc037325685519e83"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.33.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.34.79"
         },
         "cachetools": {
             "hashes": [
                 "sha256:89ea6f1b638d5a73a4f9226be57ac5e4f399d22770b92355f92dcb0f7f001693",
                 "sha256:92971d3cb7d2a97efff7c7bb1657f21a8f5fb309a37530537c71b1774189f2d1"
             ],
             "index": "pypi",
             "markers": "python_version ~= '3.5'",
             "version": "==4.2.4"
         },
         "certifi": {
             "hashes": [
-                "sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1",
-                "sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.11.17"
+            "version": "==2024.2.2"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027",
                 "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087",
                 "sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786",
                 "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8",
@@ -202,36 +202,36 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.9.0"
         },
         "python-dateutil": {
             "hashes": [
-                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
-                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+                "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3",
+                "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.2"
+            "version": "==2.9.0.post0"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.31.0"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:d1c52af7bceca1650d0f27728b29bb4925184aead7b55bccacf893b79a108604",
-                "sha256:e6cafd5643fc7b44fddfba1e5b521005675b0e07533ddad958a3554bc87d7330"
+                "sha256:5683916b4c724f799e600f41dd9e10a9ff19871bf87623cc8f491cb4f5fa0a19",
+                "sha256:ceb252b11bcf87080fb7850a224fb6e05c8a776bab8f2b64b7f25b969464839d"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.8.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.10.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -243,61 +243,70 @@
                 "sha256:eaa337ff55a1579b6549dc679565eac1e3d000563bcb1c8ab0d0fefbc0c2cdc7"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.5"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0",
-                "sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==4.8.0"
+            "version": "==4.11.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:34b97092d7e0a3a8cf7cd10e386f401b3737364026c45e622aa02903dffe0f07",
                 "sha256:f8ecc1bba5667413457c529ab955bf8c67b45db799d159066261719e328580a0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.18"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
-                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
+                "sha256:75a8b99c28a5dad50dd7f8ccdd447a121ddb3892da9e53d1ca5cca3106d58d65",
+                "sha256:b46733c07dce03ae4e150330b975c75737fa60f0a7c591b6c8bf4928a28e2c92"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.7.13"
+            "markers": "python_version >= '3.9'",
+            "version": "==0.7.16"
         },
         "astroid": {
             "hashes": [
                 "sha256:1aa149fc5c6589e3d0ece885b4491acd80af4f087baafa3fb5203b113e68cd3c",
                 "sha256:6c107453dffee9055899705de3c9ead36e74119cee151e5a9aaf7f0b0e020a6a"
             ],
             "markers": "python_full_version >= '3.7.2'",
             "version": "==2.15.8"
         },
         "babel": {
             "hashes": [
-                "sha256:33e0952d7dd6374af8dbf6768cc4ddf3ccfefc244f9986d4074704f2fbd18900",
-                "sha256:7077a4984b02b6727ac10f1f7294484f737443d7e2e66c5e4380e41a3ae0b4ed"
+                "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363",
+                "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.13.1"
+            "version": "==2.14.0"
+        },
+        "backports.tarfile": {
+            "hashes": [
+                "sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75",
+                "sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4"
+            ],
+            "markers": "python_version < '3.12'",
+            "version": "==1.0.0"
         },
         "betamax": {
             "hashes": [
-                "sha256:5bf004ceffccae881213fb722f34517166b84a34919b92ffc14d1dbd050b71c2",
-                "sha256:aa5ad34cc8d018b35814fb0557d15c78ced9ac56fdc43ccacdb882aa7a5217c1"
+                "sha256:82316e1679bc6879e3c83318d016b54b7c9225ff08c4462de4813e22038d5f94",
+                "sha256:880d6da87eaf7e61c42bdc4240f0ac04ab5365bd7f2798784c18d37d8cf747bc"
             ],
             "index": "pypi",
-            "version": "==0.8.1"
+            "markers": "python_full_version >= '3.8.1'",
+            "version": "==0.9.0"
         },
         "betamax-serializers": {
             "hashes": [
                 "sha256:1b23c46429c40a8873682854c88d805c787c72d252f3fa0c858e9c300682ceac",
                 "sha256:345c419b1b73171f2951c62ac3c701775ac4b76e13e86464ebf0ff2a978e4949"
             ],
             "index": "pypi",
@@ -318,77 +327,19 @@
             ],
             "index": "pypi",
             "markers": "python_version ~= '3.5'",
             "version": "==4.2.4"
         },
         "certifi": {
             "hashes": [
-                "sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1",
-                "sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.11.17"
-        },
-        "cffi": {
-            "hashes": [
-                "sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc",
-                "sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a",
-                "sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417",
-                "sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab",
-                "sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520",
-                "sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36",
-                "sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743",
-                "sha256:3686dffb02459559c74dd3d81748269ffb0eb027c39a6fc99502de37d501faa8",
-                "sha256:582215a0e9adbe0e379761260553ba11c58943e4bbe9c36430c4ca6ac74b15ed",
-                "sha256:5b50bf3f55561dac5438f8e70bfcdfd74543fd60df5fa5f62d94e5867deca684",
-                "sha256:5bf44d66cdf9e893637896c7faa22298baebcd18d1ddb6d2626a6e39793a1d56",
-                "sha256:6602bc8dc6f3a9e02b6c22c4fc1e47aa50f8f8e6d3f78a5e16ac33ef5fefa324",
-                "sha256:673739cb539f8cdaa07d92d02efa93c9ccf87e345b9a0b556e3ecc666718468d",
-                "sha256:68678abf380b42ce21a5f2abde8efee05c114c2fdb2e9eef2efdb0257fba1235",
-                "sha256:68e7c44931cc171c54ccb702482e9fc723192e88d25a0e133edd7aff8fcd1f6e",
-                "sha256:6b3d6606d369fc1da4fd8c357d026317fbb9c9b75d36dc16e90e84c26854b088",
-                "sha256:748dcd1e3d3d7cd5443ef03ce8685043294ad6bd7c02a38d1bd367cfd968e000",
-                "sha256:7651c50c8c5ef7bdb41108b7b8c5a83013bfaa8a935590c5d74627c047a583c7",
-                "sha256:7b78010e7b97fef4bee1e896df8a4bbb6712b7f05b7ef630f9d1da00f6444d2e",
-                "sha256:7e61e3e4fa664a8588aa25c883eab612a188c725755afff6289454d6362b9673",
-                "sha256:80876338e19c951fdfed6198e70bc88f1c9758b94578d5a7c4c91a87af3cf31c",
-                "sha256:8895613bcc094d4a1b2dbe179d88d7fb4a15cee43c052e8885783fac397d91fe",
-                "sha256:88e2b3c14bdb32e440be531ade29d3c50a1a59cd4e51b1dd8b0865c54ea5d2e2",
-                "sha256:8f8e709127c6c77446a8c0a8c8bf3c8ee706a06cd44b1e827c3e6a2ee6b8c098",
-                "sha256:9cb4a35b3642fc5c005a6755a5d17c6c8b6bcb6981baf81cea8bfbc8903e8ba8",
-                "sha256:9f90389693731ff1f659e55c7d1640e2ec43ff725cc61b04b2f9c6d8d017df6a",
-                "sha256:a09582f178759ee8128d9270cd1344154fd473bb77d94ce0aeb2a93ebf0feaf0",
-                "sha256:a6a14b17d7e17fa0d207ac08642c8820f84f25ce17a442fd15e27ea18d67c59b",
-                "sha256:a72e8961a86d19bdb45851d8f1f08b041ea37d2bd8d4fd19903bc3083d80c896",
-                "sha256:abd808f9c129ba2beda4cfc53bde801e5bcf9d6e0f22f095e45327c038bfe68e",
-                "sha256:ac0f5edd2360eea2f1daa9e26a41db02dd4b0451b48f7c318e217ee092a213e9",
-                "sha256:b29ebffcf550f9da55bec9e02ad430c992a87e5f512cd63388abb76f1036d8d2",
-                "sha256:b2ca4e77f9f47c55c194982e10f058db063937845bb2b7a86c84a6cfe0aefa8b",
-                "sha256:b7be2d771cdba2942e13215c4e340bfd76398e9227ad10402a8767ab1865d2e6",
-                "sha256:b84834d0cf97e7d27dd5b7f3aca7b6e9263c56308ab9dc8aae9784abb774d404",
-                "sha256:b86851a328eedc692acf81fb05444bdf1891747c25af7529e39ddafaf68a4f3f",
-                "sha256:bcb3ef43e58665bbda2fb198698fcae6776483e0c4a631aa5647806c25e02cc0",
-                "sha256:c0f31130ebc2d37cdd8e44605fb5fa7ad59049298b3f745c74fa74c62fbfcfc4",
-                "sha256:c6a164aa47843fb1b01e941d385aab7215563bb8816d80ff3a363a9f8448a8dc",
-                "sha256:d8a9d3ebe49f084ad71f9269834ceccbf398253c9fac910c4fd7053ff1386936",
-                "sha256:db8e577c19c0fda0beb7e0d4e09e0ba74b1e4c092e0e40bfa12fe05b6f6d75ba",
-                "sha256:dc9b18bf40cc75f66f40a7379f6a9513244fe33c0e8aa72e2d56b0196a7ef872",
-                "sha256:e09f3ff613345df5e8c3667da1d918f9149bd623cd9070c983c013792a9a62eb",
-                "sha256:e4108df7fe9b707191e55f33efbcb2d81928e10cea45527879a4749cbe472614",
-                "sha256:e6024675e67af929088fda399b2094574609396b1decb609c55fa58b028a32a1",
-                "sha256:e70f54f1796669ef691ca07d046cd81a29cb4deb1e5f942003f401c0c4a2695d",
-                "sha256:e715596e683d2ce000574bae5d07bd522c781a822866c20495e52520564f0969",
-                "sha256:e760191dd42581e023a68b758769e2da259b5d52e3103c6060ddc02c9edb8d7b",
-                "sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4",
-                "sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627",
-                "sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956",
-                "sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357"
-            ],
-            "markers": "python_version >= '3.8'",
-            "version": "==1.16.0"
+            "version": "==2024.2.2"
         },
         "chardet": {
             "hashes": [
                 "sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7",
                 "sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970"
             ],
             "markers": "python_version >= '3.7'",
@@ -505,114 +456,85 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:0cbf38419fb1a347aaf63481c00f0bdc86889d9fbf3f25109cf96c26b403fda1",
-                "sha256:12d15ab5833a997716d76f2ac1e4b4d536814fc213c85ca72756c19e5a6b3d63",
-                "sha256:149de1d2401ae4655c436a3dced6dd153f4c3309f599c3d4bd97ab172eaf02d9",
-                "sha256:1981f785239e4e39e6444c63a98da3a1db8e971cb9ceb50a945ba6296b43f312",
-                "sha256:2443cbda35df0d35dcfb9bf8f3c02c57c1d6111169e3c85fc1fcc05e0c9f39a3",
-                "sha256:289fe43bf45a575e3ab10b26d7b6f2ddb9ee2dba447499f5401cfb5ecb8196bb",
-                "sha256:2f11cc3c967a09d3695d2a6f03fb3e6236622b93be7a4b5dc09166a861be6d25",
-                "sha256:307adb8bd3abe389a471e649038a71b4eb13bfd6b7dd9a129fa856f5c695cf92",
-                "sha256:310b3bb9c91ea66d59c53fa4989f57d2436e08f18fb2f421a1b0b6b8cc7fffda",
-                "sha256:315a989e861031334d7bee1f9113c8770472db2ac484e5b8c3173428360a9148",
-                "sha256:3a4006916aa6fee7cd38db3bfc95aa9c54ebb4ffbfc47c677c8bba949ceba0a6",
-                "sha256:3c7bba973ebee5e56fe9251300c00f1579652587a9f4a5ed8404b15a0471f216",
-                "sha256:4175e10cc8dda0265653e8714b3174430b07c1dca8957f4966cbd6c2b1b8065a",
-                "sha256:43668cabd5ca8258f5954f27a3aaf78757e6acf13c17604d89648ecc0cc66640",
-                "sha256:4cbae1051ab791debecc4a5dcc4a1ff45fc27b91b9aee165c8a27514dd160836",
-                "sha256:5c913b556a116b8d5f6ef834038ba983834d887d82187c8f73dec21049abd65c",
-                "sha256:5f7363d3b6a1119ef05015959ca24a9afc0ea8a02c687fe7e2d557705375c01f",
-                "sha256:630b13e3036e13c7adc480ca42fa7afc2a5d938081d28e20903cf7fd687872e2",
-                "sha256:72c0cfa5250f483181e677ebc97133ea1ab3eb68645e494775deb6a7f6f83901",
-                "sha256:7dbc3ed60e8659bc59b6b304b43ff9c3ed858da2839c78b804973f613d3e92ed",
-                "sha256:88ed2c30a49ea81ea3b7f172e0269c182a44c236eb394718f976239892c0a27a",
-                "sha256:89a937174104339e3a3ffcf9f446c00e3a806c28b1841c63edb2b369310fd074",
-                "sha256:9028a3871280110d6e1aa2df1afd5ef003bab5fb1ef421d6dc748ae1c8ef2ebc",
-                "sha256:99b89d9f76070237975b315b3d5f4d6956ae354a4c92ac2388a5695516e47c84",
-                "sha256:9f805d62aec8eb92bab5b61c0f07329275b6f41c97d80e847b03eb894f38d083",
-                "sha256:a889ae02f43aa45032afe364c8ae84ad3c54828c2faa44f3bfcafecb5c96b02f",
-                "sha256:aa72dbaf2c2068404b9870d93436e6d23addd8bbe9295f49cbca83f6e278179c",
-                "sha256:ac8c802fa29843a72d32ec56d0ca792ad15a302b28ca6203389afe21f8fa062c",
-                "sha256:ae97af89f0fbf373400970c0a21eef5aa941ffeed90aee43650b81f7d7f47637",
-                "sha256:af3d828d2c1cbae52d34bdbb22fcd94d1ce715d95f1a012354a75e5913f1bda2",
-                "sha256:b4275802d16882cf9c8b3d057a0839acb07ee9379fa2749eca54efbce1535b82",
-                "sha256:b4767da59464bb593c07afceaddea61b154136300881844768037fd5e859353f",
-                "sha256:b631c92dfe601adf8f5ebc7fc13ced6bb6e9609b19d9a8cd59fa47c4186ad1ce",
-                "sha256:be32ad29341b0170e795ca590e1c07e81fc061cb5b10c74ce7203491484404ef",
-                "sha256:beaa5c1b4777f03fc63dfd2a6bd820f73f036bfb10e925fce067b00a340d0f3f",
-                "sha256:c0ba320de3fb8c6ec16e0be17ee1d3d69adcda99406c43c0409cb5c41788a611",
-                "sha256:c9eacf273e885b02a0273bb3a2170f30e2d53a6d53b72dbe02d6701b5296101c",
-                "sha256:cb536f0dcd14149425996821a168f6e269d7dcd2c273a8bff8201e79f5104e76",
-                "sha256:d1bc430677773397f64a5c88cb522ea43175ff16f8bfcc89d467d974cb2274f9",
-                "sha256:d1c88ec1a7ff4ebca0219f5b1ef863451d828cccf889c173e1253aa84b1e07ce",
-                "sha256:d3d9df4051c4a7d13036524b66ecf7a7537d14c18a384043f30a303b146164e9",
-                "sha256:d51ac2a26f71da1b57f2dc81d0e108b6ab177e7d30e774db90675467c847bbdf",
-                "sha256:d872145f3a3231a5f20fd48500274d7df222e291d90baa2026cc5152b7ce86bf",
-                "sha256:d8f17966e861ff97305e0801134e69db33b143bbfb36436efb9cfff6ec7b2fd9",
-                "sha256:dbc1b46b92186cc8074fee9d9fbb97a9dd06c6cbbef391c2f59d80eabdf0faa6",
-                "sha256:e10c39c0452bf6e694511c901426d6b5ac005acc0f78ff265dbe36bf81f808a2",
-                "sha256:e267e9e2b574a176ddb983399dec325a80dbe161f1a32715c780b5d14b5f583a",
-                "sha256:f47d39359e2c3779c5331fc740cf4bce6d9d680a7b4b4ead97056a0ae07cb49a",
-                "sha256:f6e9589bd04d0461a417562649522575d8752904d35c12907d8c9dfeba588faf",
-                "sha256:f94b734214ea6a36fe16e96a70d941af80ff3bfd716c141300d95ebc85339738",
-                "sha256:fa28e909776dc69efb6ed975a63691bc8172b64ff357e663a1bb06ff3c9b589a",
-                "sha256:fe494faa90ce6381770746077243231e0b83ff3f17069d748f645617cefe19d4"
+                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
+                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
+                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
+                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
+                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
+                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
+                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
+                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
+                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
+                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
+                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
+                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
+                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
+                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
+                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
+                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
+                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
+                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
+                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
+                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
+                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
+                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
+                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
+                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
+                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
+                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
+                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
+                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
+                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
+                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
+                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
+                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
+                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
+                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
+                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
+                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
+                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
+                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
+                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
+                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
+                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
+                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
+                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
+                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
+                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
+                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
+                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
+                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
+                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
+                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
+                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
+                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==7.3.2"
-        },
-        "cryptography": {
-            "hashes": [
-                "sha256:079b85658ea2f59c4f43b70f8119a52414cdb7be34da5d019a77bf96d473b960",
-                "sha256:09616eeaef406f99046553b8a40fbf8b1e70795a91885ba4c96a70793de5504a",
-                "sha256:13f93ce9bea8016c253b34afc6bd6a75993e5c40672ed5405a9c832f0d4a00bc",
-                "sha256:37a138589b12069efb424220bf78eac59ca68b95696fc622b6ccc1c0a197204a",
-                "sha256:3c78451b78313fa81607fa1b3f1ae0a5ddd8014c38a02d9db0616133987b9cdf",
-                "sha256:43f2552a2378b44869fe8827aa19e69512e3245a219104438692385b0ee119d1",
-                "sha256:48a0476626da912a44cc078f9893f292f0b3e4c739caf289268168d8f4702a39",
-                "sha256:49f0805fc0b2ac8d4882dd52f4a3b935b210935d500b6b805f321addc8177406",
-                "sha256:5429ec739a29df2e29e15d082f1d9ad683701f0ec7709ca479b3ff2708dae65a",
-                "sha256:5a1b41bc97f1ad230a41657d9155113c7521953869ae57ac39ac7f1bb471469a",
-                "sha256:68a2dec79deebc5d26d617bfdf6e8aab065a4f34934b22d3b5010df3ba36612c",
-                "sha256:7a698cb1dac82c35fcf8fe3417a3aaba97de16a01ac914b89a0889d364d2f6be",
-                "sha256:841df4caa01008bad253bce2a6f7b47f86dc9f08df4b433c404def869f590a15",
-                "sha256:90452ba79b8788fa380dfb587cca692976ef4e757b194b093d845e8d99f612f2",
-                "sha256:928258ba5d6f8ae644e764d0f996d61a8777559f72dfeb2eea7e2fe0ad6e782d",
-                "sha256:af03b32695b24d85a75d40e1ba39ffe7db7ffcb099fe507b39fd41a565f1b157",
-                "sha256:b640981bf64a3e978a56167594a0e97db71c89a479da8e175d8bb5be5178c003",
-                "sha256:c5ca78485a255e03c32b513f8c2bc39fedb7f5c5f8535545bdc223a03b24f248",
-                "sha256:c7f3201ec47d5207841402594f1d7950879ef890c0c495052fa62f58283fde1a",
-                "sha256:d5ec85080cce7b0513cfd233914eb8b7bbd0633f1d1703aa28d1dd5a72f678ec",
-                "sha256:d6c391c021ab1f7a82da5d8d0b3cee2f4b2c455ec86c8aebbc84837a631ff309",
-                "sha256:e3114da6d7f95d2dee7d3f4eec16dacff819740bbab931aff8648cb13c5ff5e7",
-                "sha256:f983596065a18a2183e7f79ab3fd4c475205b839e02cbc0efbbf9666c4b3083d"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==41.0.7"
+            "version": "==7.4.4"
         },
         "dill": {
             "hashes": [
-                "sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e",
-                "sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03"
+                "sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca",
+                "sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==0.3.7"
+            "version": "==0.3.8"
         },
         "distlib": {
             "hashes": [
-                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
-                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
+                "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784",
+                "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"
             ],
-            "version": "==0.3.7"
+            "version": "==0.3.8"
         },
         "docutils": {
             "hashes": [
                 "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -623,28 +545,28 @@
                 "sha256:28323cbfc9352139fdd3d316fa17f325cc0e9ac74438cbba51d70f9b48f86c3a",
                 "sha256:51f54c0fd886fa3854387f354b19f429d38c04f984f38bc572558b703c0542a6"
             ],
             "version": "==0.2.1"
         },
         "emoji": {
             "hashes": [
-                "sha256:8d8b5dec3c507444b58890e598fc895fcec022b3f5acb49497c6ccc5208b8b00",
-                "sha256:a8468fd836b7ecb6d1eac054c9a591701ce0ccd6c6f7779ad71b66f76664df90"
+                "sha256:63fc9107f06c6c2e48e5078ce9575cef98518f5ac09474f6148a43e989989582",
+                "sha256:772eaa30f4e0b1ce95148a092df4c7dc97644532c03225326b0fd05e8a9f72a3"
             ],
             "index": "pypi",
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.0"
+            "version": "==2.11.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e",
-                "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"
+                "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb",
+                "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.13.1"
+            "version": "==3.13.3"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -663,27 +585,26 @@
                 "sha256:bf5421126136d6d0af55bc1e7c1af1c397a34f5b7bd79e776cd3e89785c2b04b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.0.11"
         },
         "gitpython": {
             "hashes": [
-                "sha256:22b126e9ffb671fdd0c129796343a02bf67bf2994b35449ffc9321aa755e18a4",
-                "sha256:cf14627d5a8049ffbf49915732e5eddbe8134c3bdb9d476e6182b676fc573f8a"
+                "sha256:35f314a9f878467f5453cc1fee295c3e18e52f1b99f10f6cf5b1682e968a9e7c",
+                "sha256:eec7ec56b92aad751f9912a73404bc02ba212a23adb2c7098ee668417051a1ff"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.40"
+            "version": "==3.1.43"
         },
         "gitwrapperlib": {
             "hashes": [
-                "sha256:2f1c5e0fc69168dde3cd141f56b7714c6841ebe886956c1cd302c5867b640db7",
-                "sha256:90b33ad4568e5ce056d0058b98dd850a6dee2473d3bfc115f35c721e62f95078"
+                "sha256:f4b0adc0f91a568dd6c385306fa88af02221fef3e7ccf9000d428ace5aafe086"
             ],
             "index": "pypi",
-            "version": "==1.0.3"
+            "version": "==1.0.4"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -703,175 +624,184 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
-                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==6.8.0"
+            "markers": "python_version < '3.10'",
+            "version": "==7.1.0"
         },
         "isort": {
             "hashes": [
-                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
-                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
+                "sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109",
+                "sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6"
             ],
             "markers": "python_full_version >= '3.8.0'",
-            "version": "==5.12.0"
+            "version": "==5.13.2"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb",
-                "sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621"
+                "sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd",
+                "sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.3.0"
+            "version": "==3.4.0"
         },
-        "jeepney": {
+        "jaraco.context": {
             "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+                "sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266",
+                "sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.3.0"
+        },
+        "jaraco.functools": {
+            "hashes": [
+                "sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925",
+                "sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.0"
         },
         "jinja2": {
             "hashes": [
-                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
-                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
+                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.2"
+            "version": "==3.1.3"
         },
         "keyring": {
             "hashes": [
-                "sha256:4446d35d636e6a10b8bce7caa66913dd9eca5fd222ca03a3d42c38608ac30836",
-                "sha256:e730ecffd309658a08ee82535a3b5ec4b4c8669a9be11efb66249d8e0aeb9a25"
+                "sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427",
+                "sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==24.3.0"
+            "version": "==25.1.0"
         },
         "lazy-object-proxy": {
             "hashes": [
-                "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
-                "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
-                "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
-                "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
-                "sha256:1aa3de4088c89a1b69f8ec0dcc169aa725b0ff017899ac568fe44ddc1396df46",
-                "sha256:212774e4dfa851e74d393a2370871e174d7ff0ebc980907723bb67d25c8a7c30",
-                "sha256:2d0daa332786cf3bb49e10dc6a17a52f6a8f9601b4cf5c295a4f85854d61de63",
-                "sha256:5f83ac4d83ef0ab017683d715ed356e30dd48a93746309c8f3517e1287523ef4",
-                "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae",
-                "sha256:660c94ea760b3ce47d1855a30984c78327500493d396eac4dfd8bd82041b22be",
-                "sha256:66a3de4a3ec06cd8af3f61b8e1ec67614fbb7c995d02fa224813cb7afefee701",
-                "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd",
-                "sha256:7322c3d6f1766d4ef1e51a465f47955f1e8123caee67dd641e67d539a534d006",
-                "sha256:79a31b086e7e68b24b99b23d57723ef7e2c6d81ed21007b6281ebcd1688acb0a",
-                "sha256:81fc4d08b062b535d95c9ea70dbe8a335c45c04029878e62d744bdced5141586",
-                "sha256:8fa02eaab317b1e9e03f69aab1f91e120e7899b392c4fc19807a8278a07a97e8",
-                "sha256:9090d8e53235aa280fc9239a86ae3ea8ac58eff66a705fa6aa2ec4968b95c821",
-                "sha256:946d27deaff6cf8452ed0dba83ba38839a87f4f7a9732e8f9fd4107b21e6ff07",
-                "sha256:9990d8e71b9f6488e91ad25f322898c136b008d87bf852ff65391b004da5e17b",
-                "sha256:9cd077f3d04a58e83d04b20e334f678c2b0ff9879b9375ed107d5d07ff160171",
-                "sha256:9e7551208b2aded9c1447453ee366f1c4070602b3d932ace044715d89666899b",
-                "sha256:9f5fa4a61ce2438267163891961cfd5e32ec97a2c444e5b842d574251ade27d2",
-                "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7",
-                "sha256:bfb38f9ffb53b942f2b5954e0f610f1e721ccebe9cce9025a38c8ccf4a5183a4",
-                "sha256:cbf9b082426036e19c6924a9ce90c740a9861e2bdc27a4834fd0a910742ac1e8",
-                "sha256:d9e25ef10a39e8afe59a5c348a4dbf29b4868ab76269f81ce1674494e2565a6e",
-                "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f",
-                "sha256:e7c21c95cae3c05c14aafffe2865bbd5e377cfc1348c4f7751d9dc9a48ca4bda",
-                "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4",
-                "sha256:ea806fd4c37bf7e7ad82537b0757999264d5f70c45468447bb2b91afdbe73a6e",
-                "sha256:edd20c5a55acb67c7ed471fa2b5fb66cb17f61430b7a6b9c3b4a1e40293b1671",
-                "sha256:f0117049dd1d5635bbff65444496c90e0baa48ea405125c088e93d9cf4525b11",
-                "sha256:f0705c376533ed2a9e5e97aacdbfe04cecd71e0aa84c7c0595d02ef93b6e4455",
-                "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
-                "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
-                "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
+                "sha256:009e6bb1f1935a62889ddc8541514b6a9e1fcf302667dcb049a0be5c8f613e56",
+                "sha256:02c83f957782cbbe8136bee26416686a6ae998c7b6191711a04da776dc9e47d4",
+                "sha256:0aefc7591920bbd360d57ea03c995cebc204b424524a5bd78406f6e1b8b2a5d8",
+                "sha256:127a789c75151db6af398b8972178afe6bda7d6f68730c057fbbc2e96b08d282",
+                "sha256:18dd842b49456aaa9a7cf535b04ca4571a302ff72ed8740d06b5adcd41fe0757",
+                "sha256:217138197c170a2a74ca0e05bddcd5f1796c735c37d0eee33e43259b192aa424",
+                "sha256:2297f08f08a2bb0d32a4265e98a006643cd7233fb7983032bd61ac7a02956b3b",
+                "sha256:2fc0a92c02fa1ca1e84fc60fa258458e5bf89d90a1ddaeb8ed9cc3147f417255",
+                "sha256:30b339b2a743c5288405aa79a69e706a06e02958eab31859f7f3c04980853b70",
+                "sha256:366c32fe5355ef5fc8a232c5436f4cc66e9d3e8967c01fb2e6302fd6627e3d94",
+                "sha256:3ad54b9ddbe20ae9f7c1b29e52f123120772b06dbb18ec6be9101369d63a4074",
+                "sha256:5ad9e6ed739285919aa9661a5bbed0aaf410aa60231373c5579c6b4801bd883c",
+                "sha256:5faf03a7d8942bb4476e3b62fd0f4cf94eaf4618e304a19865abf89a35c0bbee",
+                "sha256:75fc59fc450050b1b3c203c35020bc41bd2695ed692a392924c6ce180c6f1dc9",
+                "sha256:76a095cfe6045c7d0ca77db9934e8f7b71b14645f0094ffcd842349ada5c5fb9",
+                "sha256:78247b6d45f43a52ef35c25b5581459e85117225408a4128a3daf8bf9648ac69",
+                "sha256:782e2c9b2aab1708ffb07d4bf377d12901d7a1d99e5e410d648d892f8967ab1f",
+                "sha256:7ab7004cf2e59f7c2e4345604a3e6ea0d92ac44e1c2375527d56492014e690c3",
+                "sha256:80b39d3a151309efc8cc48675918891b865bdf742a8616a337cb0090791a0de9",
+                "sha256:80fa48bd89c8f2f456fc0765c11c23bf5af827febacd2f523ca5bc1893fcc09d",
+                "sha256:855e068b0358ab916454464a884779c7ffa312b8925c6f7401e952dcf3b89977",
+                "sha256:92f09ff65ecff3108e56526f9e2481b8116c0b9e1425325e13245abfd79bdb1b",
+                "sha256:952c81d415b9b80ea261d2372d2a4a2332a3890c2b83e0535f263ddfe43f0d43",
+                "sha256:9a3a87cf1e133e5b1994144c12ca4aa3d9698517fe1e2ca82977781b16955658",
+                "sha256:9e4ed0518a14dd26092614412936920ad081a424bdcb54cc13349a8e2c6d106a",
+                "sha256:a899b10e17743683b293a729d3a11f2f399e8a90c73b089e29f5d0fe3509f0dd",
+                "sha256:b1f711e2c6dcd4edd372cf5dec5c5a30d23bba06ee012093267b3376c079ec83",
+                "sha256:b4f87d4ed9064b2628da63830986c3d2dca7501e6018347798313fcf028e2fd4",
+                "sha256:cb73507defd385b7705c599a94474b1d5222a508e502553ef94114a143ec6696",
+                "sha256:dc0d2fc424e54c70c4bc06787e4072c4f3b1aa2f897dfdc34ce1013cf3ceef05",
+                "sha256:e221060b701e2aa2ea991542900dd13907a5c90fa80e199dbf5a03359019e7a3",
+                "sha256:e271058822765ad5e3bca7f05f2ace0de58a3f4e62045a8c90a0dfd2f8ad8cc6",
+                "sha256:e2adb09778797da09d2b5ebdbceebf7dd32e2c96f79da9052b2e87b6ea495895",
+                "sha256:e333e2324307a7b5d86adfa835bb500ee70bfcd1447384a822e96495796b0ca4",
+                "sha256:e98c8af98d5707dcdecc9ab0863c0ea6e88545d42ca7c3feffb6b4d1e370c7ba",
+                "sha256:edb45bb8278574710e68a6b021599a10ce730d156e5b254941754a9cc0b17d03",
+                "sha256:fec03caabbc6b59ea4a638bee5fce7117be8e99a4103d9d5ad77f15d6f81020c"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.9.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.10.0"
         },
         "markdown-it-py": {
             "hashes": [
                 "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
                 "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
-                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
-                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
-                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
-                "sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c",
-                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
-                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
-                "sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb",
-                "sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939",
-                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
-                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
-                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
-                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
-                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
-                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
-                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
-                "sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd",
-                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
-                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
-                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
-                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
-                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
-                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
-                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
-                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
-                "sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007",
-                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
-                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
-                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
-                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
-                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
-                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
-                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
-                "sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1",
-                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
-                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
-                "sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c",
-                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
-                "sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823",
-                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
-                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
-                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
-                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
-                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
-                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
-                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
-                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
-                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
-                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
-                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
-                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
-                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
-                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
-                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
-                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
-                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
-                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
-                "sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc",
-                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2",
-                "sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11"
+                "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf",
+                "sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff",
+                "sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f",
+                "sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3",
+                "sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532",
+                "sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f",
+                "sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617",
+                "sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df",
+                "sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4",
+                "sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906",
+                "sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f",
+                "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4",
+                "sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8",
+                "sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371",
+                "sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2",
+                "sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465",
+                "sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52",
+                "sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6",
+                "sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169",
+                "sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad",
+                "sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2",
+                "sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0",
+                "sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029",
+                "sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f",
+                "sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a",
+                "sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced",
+                "sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5",
+                "sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c",
+                "sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf",
+                "sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9",
+                "sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb",
+                "sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad",
+                "sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3",
+                "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1",
+                "sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46",
+                "sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc",
+                "sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a",
+                "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee",
+                "sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900",
+                "sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5",
+                "sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea",
+                "sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f",
+                "sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5",
+                "sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e",
+                "sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a",
+                "sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f",
+                "sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50",
+                "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a",
+                "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b",
+                "sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4",
+                "sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff",
+                "sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2",
+                "sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46",
+                "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b",
+                "sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf",
+                "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5",
+                "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5",
+                "sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab",
+                "sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd",
+                "sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.3"
+            "version": "==2.1.5"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -883,40 +813,40 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a",
-                "sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6"
+                "sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684",
+                "sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==10.1.0"
+            "version": "==10.2.0"
         },
         "nh3": {
             "hashes": [
-                "sha256:116c9515937f94f0057ef50ebcbcc10600860065953ba56f14473ff706371873",
-                "sha256:18415df36db9b001f71a42a3a5395db79cf23d556996090d293764436e98e8ad",
-                "sha256:203cac86e313cf6486704d0ec620a992c8bc164c86d3a4fd3d761dd552d839b5",
-                "sha256:2b0be5c792bd43d0abef8ca39dd8acb3c0611052ce466d0401d51ea0d9aa7525",
-                "sha256:377aaf6a9e7c63962f367158d808c6a1344e2b4f83d071c43fbd631b75c4f0b2",
-                "sha256:525846c56c2bcd376f5eaee76063ebf33cf1e620c1498b2a40107f60cfc6054e",
-                "sha256:5529a3bf99402c34056576d80ae5547123f1078da76aa99e8ed79e44fa67282d",
-                "sha256:7771d43222b639a4cd9e341f870cee336b9d886de1ad9bec8dddab22fe1de450",
-                "sha256:88c753efbcdfc2644a5012938c6b9753f1c64a5723a67f0301ca43e7b85dcf0e",
-                "sha256:93a943cfd3e33bd03f77b97baa11990148687877b74193bf777956b67054dcc6",
-                "sha256:9be2f68fb9a40d8440cbf34cbf40758aa7f6093160bfc7fb018cce8e424f0c3a",
-                "sha256:a0c509894fd4dccdff557068e5074999ae3b75f4c5a2d6fb5415e782e25679c4",
-                "sha256:ac8056e937f264995a82bf0053ca898a1cb1c9efc7cd68fa07fe0060734df7e4",
-                "sha256:aed56a86daa43966dd790ba86d4b810b219f75b4bb737461b6886ce2bde38fd6",
-                "sha256:e8986f1dd3221d1e741fda0a12eaa4a273f1d80a35e31a1ffe579e7c621d069e",
-                "sha256:f99212a81c62b5f22f9e7c3e347aa00491114a5647e1f13bbebd79c3e5f08d75"
+                "sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a",
+                "sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911",
+                "sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb",
+                "sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a",
+                "sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc",
+                "sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028",
+                "sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9",
+                "sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3",
+                "sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351",
+                "sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10",
+                "sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71",
+                "sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f",
+                "sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b",
+                "sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a",
+                "sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062",
+                "sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a"
             ],
-            "version": "==0.2.14"
+            "version": "==0.2.17"
         },
         "nose": {
             "hashes": [
                 "sha256:9ff7c6cc443f8c51994b34a667bbcf45afd6d945be7477b52e97516fd17c53ac",
                 "sha256:dadcddc0aefbf99eea214e0f1232b94f2fa9bd98fa8353711dacb112bfcbbb2a",
                 "sha256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98"
             ],
@@ -929,50 +859,50 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
-                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
+                "sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297",
+                "sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.9.6"
+            "version": "==1.10.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:118c954d7e949b35437270383a3f2531e99dd93cf7ce4dc8340d3356d30f173b",
-                "sha256:cb633b2bcf10c51af60beb0ab06d2f1d69064b43abf4c185ca6b28865f3f9731"
+                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
+                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==4.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12",
-                "sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7"
+                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
+                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.3.0"
+            "version": "==1.4.0"
         },
         "poetry-semver": {
             "hashes": [
                 "sha256:4e6349bd7231cc657f0e1930f7b204e87e33dfd63eef5cac869363969515083a",
                 "sha256:d809b612aa27b39bf2d0fc9d31b4f4809b0e972646c5f19cfa46c725b7638810"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -991,21 +921,14 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
-            ],
-            "version": "==2.21"
-        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -1096,14 +1019,15 @@
                 "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
                 "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
                 "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
                 "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28",
                 "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4",
                 "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
                 "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef",
                 "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
                 "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
                 "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
                 "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
                 "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
                 "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
                 "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
@@ -1123,19 +1047,19 @@
                 "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0.1"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:13d039515c1f24de668e2c93f2e877b9dbe6c6c32328b90a40a49d8b2b85f36d",
-                "sha256:2d55489f83be4992fe4454939d1a051c33edbab778e82761d060c9fc6b308cd1"
+                "sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311",
+                "sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==42.0"
+            "version": "==43.0"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
@@ -1164,27 +1088,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa",
-                "sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235"
+                "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222",
+                "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.7.0"
-        },
-        "secretstorage": {
-            "hashes": [
-                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
-                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.3"
+            "version": "==13.7.1"
         },
         "semver": {
             "hashes": [
                 "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4",
                 "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"
             ],
             "index": "pypi",
@@ -1199,15 +1115,15 @@
             "version": "==0.3.1"
         },
         "sh": {
             "hashes": [
                 "sha256:9b2998f313f201c777e2c0061f0b1367497097ef13388595be147e2a00bf7ba1",
                 "sha256:ced8f2e081a858b66a46ace3703dec243779abbd5a1887ba7e3c34f34da70cd2"
             ],
-            "markers": "sys_platform != 'win32'",
+            "markers": "python_version < '4.0' and python_full_version >= '3.8.1'",
             "version": "==2.0.6"
         },
         "smmap": {
             "hashes": [
                 "sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62",
                 "sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da"
             ],
@@ -1237,35 +1153,35 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.3.0"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:094c4d56209d1734e7d252f6e0b3ccc090bd52ee56807a5d9315b19c122ab15d",
-                "sha256:39fdc8d762d33b01a7d8f026a3b7d71563ea3b72787d5f00ad8465bd9d6dfbfa"
+                "sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619",
+                "sha256:cb61eb0ec1b61f349e5cc36b2028e9e7ca765be05e49641c97241274753067b4"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.0.7"
+            "version": "==1.0.8"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
-                "sha256:63b41e0d38207ca40ebbeabcf4d8e51f76c03e78cd61abe118cf4435c73d4212",
-                "sha256:fe8009aed765188f08fcaadbb3ea0d90ce8ae2d76710b7e29ea7d047177dae2f"
+                "sha256:6485d09629944511c893fa11355bda18b742b83a2b181f9a009f7e500595c90f",
+                "sha256:9893fd3f90506bc4b97bdb977ceb8fbd823989f4316b28c3841ec128544372d3"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.0.5"
+            "version": "==1.0.6"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:6c26a118a05b76000738429b724a0568dbde5b72391a688577da08f11891092a",
-                "sha256:8001661c077a73c29beaf4a79968d0726103c5605e27db92b9ebed8bab1359e9"
+                "sha256:0dc87637d5de53dd5eec3a6a01753b1ccf99494bd756aafecd74b4fa9e729015",
+                "sha256:393f04f112b4d2f53d93448d4bce35842f62b307ccdc549ec1585e950bc35e04"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==2.0.4"
+            "version": "==2.0.5"
         },
         "sphinxcontrib-jquery": {
             "hashes": [
                 "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
                 "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
             ],
             "markers": "python_version >= '2.7'",
@@ -1277,27 +1193,27 @@
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.1"
         },
         "sphinxcontrib-qthelp": {
             "hashes": [
-                "sha256:62b9d1a186ab7f5ee3356d906f648cacb7a6bdb94d201ee7adf26db55092982d",
-                "sha256:bf76886ee7470b934e363da7a954ea2825650013d367728588732c7350f49ea4"
+                "sha256:053dedc38823a80a7209a80860b16b722e9e0209e32fea98c90e4e6624588ed6",
+                "sha256:e2ae3b5c492d58fcbd73281fbd27e34b8393ec34a073c792642cd8e529288182"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.0.6"
+            "version": "==1.0.7"
         },
         "sphinxcontrib-serializinghtml": {
             "hashes": [
-                "sha256:0c64ff898339e1fac29abd2bf5f11078f3ec413cfe9c046d3120d7ca65530b54",
-                "sha256:9b36e503703ff04f20e9675771df105e58aa029cfcbc23b8ed716019b7416ae1"
+                "sha256:326369b8df80a7d2d8d7f99aa5ac577f51ea51556ed974e7716cfd4fca3f6cb7",
+                "sha256:93f3f5dc458b91b192fe10c397e324f262cf163d79f3282c158e8436a2c4511f"
             ],
             "markers": "python_version >= '3.9'",
-            "version": "==1.1.9"
+            "version": "==1.1.10"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
@@ -1310,19 +1226,19 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:75baf5012d06501f07bee5bf8e801b9f343e7aac5a92581f20f80ce632e6b5a4",
-                "sha256:b0a645a9156dc7cb5d3a1f0d4bab66db287fcb8e0430bdd4664a095ea16414ba"
+                "sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b",
+                "sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.12.3"
+            "version": "==0.12.4"
         },
         "tox": {
             "hashes": [
                 "sha256:445fb1fe5d0b0e8ea59a66c7d03e4b829e3524e61d5905cf3387b56161484eb8",
                 "sha256:78efc716e760390b5129bdf4f46662ff771d767085377f2d623894096f5320ea"
             ],
             "index": "pypi",
@@ -1336,35 +1252,35 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0",
-                "sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==4.8.0"
+            "version": "==4.11.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:34b97092d7e0a3a8cf7cd10e386f401b3737364026c45e622aa02903dffe0f07",
                 "sha256:f8ecc1bba5667413457c529ab955bf8c67b45db799d159066261719e328580a0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.18"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:69050ffb42419c91f6c1284a7b24e0475d793447e35929b488bf6a0aade39353",
-                "sha256:a18b3fd0314ca59a2e9f4b556819ed07183b3e9a3702ecfe213f593d44f7b3fd"
+                "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a",
+                "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.24.7"
+            "version": "==20.25.1"
         },
         "wrapt": {
             "hashes": [
                 "sha256:0d2691979e93d06a95a26257adb7bfd0c93818e89b1406f5a28f36e0d8c1e1fc",
                 "sha256:14d7dc606219cdd7405133c713f2c218d4252f2a469003f8c46bb92d5d095d81",
                 "sha256:1a5db485fe2de4403f13fafdc231b0dbae5eca4359232d2efc79025527375b09",
                 "sha256:1acd723ee2a8826f3d53910255643e33673e1d11db84ce5880675954183ec47e",
@@ -1436,15 +1352,15 @@
                 "sha256:ffa565331890b90056c01db69c0fe634a776f8019c143a5ae265f9c6bc4bd6d4"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.16.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31",
-                "sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0"
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.17.0"
+            "version": "==3.18.1"
         }
     }
 }
```

### Comparing `awsapilib-3.1.4/awsapilib/README.rst` & `awsapilib-3.1.5/awsapilib/README.rst`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/USAGE_BILLING.rst` & `awsapilib-3.1.5/awsapilib/USAGE_BILLING.rst`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/USAGE_CONTROL_TOWER.rst` & `awsapilib-3.1.5/awsapilib/USAGE_CONTROL_TOWER.rst`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/__init__.py` & `awsapilib-3.1.5/awsapilib/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/_version.py` & `awsapilib-3.1.5/awsapilib/_version.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/authentication/__init__.py` & `awsapilib-3.1.5/awsapilib/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/authentication/authentication.py` & `awsapilib-3.1.5/awsapilib/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/authentication/authenticationexceptions.py` & `awsapilib-3.1.5/awsapilib/authentication/authenticationexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/authentication/utils.py` & `awsapilib-3.1.5/awsapilib/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/awsapilib.py` & `awsapilib-3.1.5/awsapilib/awsapilib.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/awsapilibexceptions.py` & `awsapilib-3.1.5/awsapilib/awsapilibexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/billing/__init__.py` & `awsapilib-3.1.5/awsapilib/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/billing/billing.py` & `awsapilib-3.1.5/awsapilib/billing/billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 .. _Google Python Style Guide:
    http://google.github.io/styleguide/pyguide.html
 
 """
 
 import logging
 import time
+import json
 from datetime import datetime, timedelta
 
 from bs4 import BeautifulSoup as Bfs
 
 from awsapilib.authentication import Authenticator, LoggerMixin
 from awsapilib.authentication import InvalidCredentials
 
 from .billingexceptions import (InvalidCountryCode,
                                 NonEditableSetting,
                                 IAMAccessDenied,
                                 InvalidCurrency,
                                 ServerError)
 
-
 __author__ = '''Costas Tyfoxylos <ctyfoxylos@schubergphilis.com>'''
 __docformat__ = '''google'''
 __date__ = '''30-03-2021'''
 __copyright__ = '''Copyright 2021, Costas Tyfoxylos'''
 __credits__ = ["Costas Tyfoxylos"]
 __license__ = '''MIT'''
 __maintainer__ = '''Costas Tyfoxylos'''
@@ -65,14 +65,15 @@
 
 class Tax(LoggerMixin):
     """Models the tax settings of the billing console."""
 
     def __init__(self, billing):
         self._billing = billing
         self._endpoint = f'{self._billing.rest_api}/taxexemption/heritage'
+        self._endpointV2 = f'{self._billing.rest_api}/taxexemption/heritage.v2'
         self._available_country_codes = None
 
     @property
     def available_country_codes_eu(self):
         """The available country codes of the tax settings for eu.
 
         Returns:
@@ -113,24 +114,26 @@
         Returns:
             None
 
         """
         if self.inheritance == value:
             return
         self._is_editable()
-        parameters = {'heritageStatus': 'OptIn' if value else 'OptOut'}
-        response = self._billing.session.post(self._endpoint, params=parameters)
+        payload = {'heritageStatus': 'OptIn' if value else 'OptOut'}
+        response = self._billing.session.post(self._endpointV2, json=payload)
         if not response.ok:
             self.logger.error(f'Failed to retrieve inheritance state, response: {response.text}')
 
     def _is_editable(self):
         parameters = {'heritageStatus': 'OptIn'}
         response = self._billing.session.get(self._endpoint, params=parameters)
         if not response.json().get('heritageStatusEditable'):
             timestamp = response.json().get('effectiveTimestamp')
+            if not timestamp:
+                raise NonEditableSetting(f'API is not enabled: {response.json()}')
             unlock_time = (datetime.fromtimestamp(timestamp / 1000) + timedelta(minutes=15))
             wait_time = unlock_time - datetime.now()
             raise NonEditableSetting(f'API is not enabled for {wait_time} more.')
         return True
 
     #  pylint: disable=too-many-arguments
     def set_information(self, address, city, postal_code, legal_name, vat_number, country_code, state=None):
@@ -140,29 +143,36 @@
             None
 
         """
         country_code = country_code.upper()
         if country_code not in self.available_country_codes_eu:
             raise InvalidCountryCode(f'{country_code} provided is not valid. '
                                      f'Valid ones are {self.available_country_codes_eu}')
-        payload = {'address': {'addressLine1': address,
-                               'addressLine2': None,
-                               'city': city,
-                               'countryCode': country_code,
-                               'postalCode': postal_code,
-                               'state': state,
-                               },
-                   'authority': {'country': country_code,
-                                 'state': None},
-                   'legalName': legal_name,
-                   'localTaxRegistration': False,
-                   'registrationId': vat_number,
+        payload = {'linkedAccounts': [{self.account_id}],
+                   'taxRegistration': {'address': {'addressLine1': address,
+                                                   'addressLine2': None,
+                                                   'city': city,
+                                                   'countryCode': country_code,
+                                                   'postalCode': postal_code,
+                                                   'state': state,
+                                                   },
+                                       'authority': {'country': country_code,
+                                                     'state': None},
+                                       'legalName': legal_name,
+                                       'localTaxRegistration': False,
+                                       'registrationId': vat_number,
+                                       }
                    }
-        url = f'{self._billing.rest_api}/taxexemption/eu/vat/information'
-        response = self._billing.session.put(url, json=payload)
+
+        files = {
+            'details': ('blob', json.dumps(payload), 'application/json'),
+        }
+
+        url = f'{self._billing.rest_api}/taxexemption/taxregistration.v2'
+        response = self._billing.session.put(url, files=files)
         if not response.ok:
             self.logger.error(f'Failed to set information, response: {response.text}')
         return response.ok
 
 
 class Preferences(LoggerMixin):
     """Models the preferences of the billing console."""
@@ -226,28 +236,28 @@
         Returns:
             None.
 
         """
         if self.credit_sharing == value:
             return
         endpoint = f'{self._billing.rest_api}/sharingpreferences/setcreditsharing'
-        payload = {'creditEnabled': bool(value)}
+        payload = {'creditEnabled': bool(value), 'creditShareAccountExceptions': []}
         response = self._billing.session.put(endpoint, json=payload)
         if not response.ok:
             self.logger.error(f'Failed to retrieve credit sharing state, response: {response.text}')
 
 
 class Billing(LoggerMixin):
     """Models Control Tower by wrapping around service catalog."""
 
     def __init__(self, arn, region=None):
         self.aws_authenticator = Authenticator(arn)
         self.session = self._get_authenticated_session()
         self.region = region or self.aws_authenticator.region
-        self.rest_api = 'https://console.aws.amazon.com/billing/rest/v1.0'
+        self.rest_api = 'https://us-east-1.console.aws.amazon.com/billing/rest/v1.0'
         self._sor_info_ = None
         self._payment_instrument_ids = None
         self._marketplace_id = None
 
     def _get_authenticated_session(self):
         return self.aws_authenticator.get_billing_authenticated_session()
```

### Comparing `awsapilib-3.1.4/awsapilib/billing/billingexceptions.py` & `awsapilib-3.1.5/awsapilib/billing/billingexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/captcha/__init__.py` & `awsapilib-3.1.5/awsapilib/captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/captcha/captcha.py` & `awsapilib-3.1.5/awsapilib/captcha/captcha.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/captcha/captchaexceptions.py` & `awsapilib-3.1.5/awsapilib/captcha/captchaexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/cloudformation/__init__.py` & `awsapilib-3.1.5/awsapilib/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/cloudformation/cloudformation.py` & `awsapilib-3.1.5/awsapilib/cloudformation/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/cloudformation/cloudformationexceptions.py` & `awsapilib-3.1.5/awsapilib/cloudformation/cloudformationexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/console/__init__.py` & `awsapilib-3.1.5/awsapilib/console/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/console/console.py` & `awsapilib-3.1.5/awsapilib/console/console.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/console/consoleexceptions.py` & `awsapilib-3.1.5/awsapilib/console/consoleexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/controltower/__init__.py` & `awsapilib-3.1.5/awsapilib/controltower/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/controltower/controltower.py` & `awsapilib-3.1.5/awsapilib/controltower/controltower.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/controltower/controltowerexceptions.py` & `awsapilib-3.1.5/awsapilib/controltower/controltowerexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/controltower/resources/__init__.py` & `awsapilib-3.1.5/awsapilib/controltower/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/controltower/resources/configuration.py` & `awsapilib-3.1.5/awsapilib/controltower/resources/configuration.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/controltower/resources/resources.py` & `awsapilib-3.1.5/awsapilib/controltower/resources/resources.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/dev-requirements.txt` & `awsapilib-3.1.5/awsapilib/dev-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
 sphinx>=6.2.1 ; python_version >= '3.8'
 sphinx-rtd-theme>=1.3.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 prospector>=1.9.0 ; python_version < '4.0' and python_full_version >= '3.7.2'
-coverage>=7.3.2 ; python_version >= '3.8'
+coverage>=7.4.4 ; python_version >= '3.8'
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox>=4.0.0b2 ; python_version >= '3.7'
-betamax>=0.8.1
+betamax>=0.9.0 ; python_full_version >= '3.8.1'
 betamax-serializers~=0.2.1
 semver>=2.13.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-gitwrapperlib>=1.0.3
+gitwrapperlib>=1.0.4
 twine>=4.0.2 ; python_version >= '3.7'
 coloredlogs>=15.0.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-emoji>=2.8.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+emoji>=2.11.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 toml>=0.10.2 ; python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'
 boto3-type-annotations-with-docs>=0.3.1
```

### Comparing `awsapilib-3.1.4/awsapilib/sso/__init__.py` & `awsapilib-3.1.5/awsapilib/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/sso/entities/__init__.py` & `awsapilib-3.1.5/awsapilib/sso/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/sso/entities/entities.py` & `awsapilib-3.1.5/awsapilib/sso/entities/entities.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/sso/sso.py` & `awsapilib-3.1.5/awsapilib/sso/sso.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib/sso/ssoexceptions.py` & `awsapilib-3.1.5/awsapilib/sso/ssoexceptions.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/awsapilib.egg-info/PKG-INFO` & `awsapilib-3.1.5/awsapilib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: awsapilib
-Version: 3.1.4
+Version: 3.1.5
 Summary: A python library that exposes AWS services that are not covered by boto3, through the usage of undocumented APIs.
 Home-page: https://github.com/schubergphilis/awsapilib
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsapilib AWS api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: requests>=2.31.0; python_version >= "3.7"
-Requires-Dist: boto3>=1.33.2; python_version >= "3.7"
-Requires-Dist: beautifulsoup4>=4.12.2; python_full_version >= "3.6.0"
-Requires-Dist: opnieuw>=1.2.1; python_version >= "3.7"
-Requires-Dist: boto3-type-annotations>=0.3.1
-Requires-Dist: cachetools>=4.2.4; python_version ~= "3.5"
-Requires-Dist: pyotp>=2.9.0; python_version >= "3.7"
-Requires-Dist: 2captcha-python>=1.2.2; python_version >= "3.6"
 
 =========
 awsapilib
 =========
 
 A python library that exposes AWS services that are not covered by boto3, through the usage of undocumented APIs.
 
@@ -326,7 +318,13 @@
 * Bump and loosen dependencies.
 
 
 3.1.4 (29-11-2023)
 ------------------
 
 * Remove gov regions from Control Tower. Bump dependencies.
+
+
+3.1.5 (08-04-2024)
+------------------
+
+* Fix billing api changes.
```

### Comparing `awsapilib-3.1.4/dev-requirements.txt` & `awsapilib-3.1.5/dev-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
 sphinx>=6.2.1 ; python_version >= '3.8'
 sphinx-rtd-theme>=1.3.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 prospector>=1.9.0 ; python_version < '4.0' and python_full_version >= '3.7.2'
-coverage>=7.3.2 ; python_version >= '3.8'
+coverage>=7.4.4 ; python_version >= '3.8'
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox>=4.0.0b2 ; python_version >= '3.7'
-betamax>=0.8.1
+betamax>=0.9.0 ; python_full_version >= '3.8.1'
 betamax-serializers~=0.2.1
 semver>=2.13.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-gitwrapperlib>=1.0.3
+gitwrapperlib>=1.0.4
 twine>=4.0.2 ; python_version >= '3.7'
 coloredlogs>=15.0.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-emoji>=2.8.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+emoji>=2.11.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 toml>=0.10.2 ; python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'
 boto3-type-annotations-with-docs>=0.3.1
```

### Comparing `awsapilib-3.1.4/docs/Makefile` & `awsapilib-3.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/docs/conf.py` & `awsapilib-3.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsapilib-3.1.4/setup.py` & `awsapilib-3.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     zip_safe=False,
     keywords='''awsapilib AWS api ''',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
         ],
     test_suite='tests',
     tests_require=test_requirements
 )
```

### Comparing `awsapilib-3.1.4/tests/test_awsapilib.py` & `awsapilib-3.1.5/tests/test_awsapilib.py`

 * *Files identical despite different names*

