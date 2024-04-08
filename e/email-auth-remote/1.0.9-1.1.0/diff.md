# Comparing `tmp/email-auth-remote-1.0.9.tar.gz` & `tmp/email-auth-remote-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-auth-remote-1.0.9.tar", last modified: Tue Feb 13 15:47:34 2024, max compression
+gzip compressed data, was "email-auth-remote-1.1.0.tar", last modified: Mon Apr  8 14:58:07 2024, max compression
```

## Comparing `email-auth-remote-1.0.9.tar` & `email-auth-remote-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-02-13 15:47:34.922991 email-auth-remote-1.0.9/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     1568 2024-02-13 15:47:34.922991 email-auth-remote-1.0.9/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1034 2024-02-13 12:48:36.000000 email-auth-remote-1.0.9/README.md
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-02-13 15:47:34.922991 email-auth-remote-1.0.9/email_auth_remote/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      234 2024-02-13 13:42:40.000000 email-auth-remote-1.0.9/email_auth_remote/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2434 2024-02-13 14:32:43.000000 email-auth-remote-1.0.9/email_auth_remote/authentication.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      683 2024-02-13 15:46:55.000000 email-auth-remote-1.0.9/email_auth_remote/extensions.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     5258 2024-02-12 12:26:49.000000 email-auth-remote-1.0.9/email_auth_remote/models.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      527 2024-02-13 14:34:39.000000 email-auth-remote-1.0.9/email_auth_remote/settings.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-02-13 15:47:34.922991 email-auth-remote-1.0.9/email_auth_remote.egg-info/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     1568 2024-02-13 15:47:34.000000 email-auth-remote-1.0.9/email_auth_remote.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      384 2024-02-13 15:47:34.000000 email-auth-remote-1.0.9/email_auth_remote.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-02-13 15:47:34.000000 email-auth-remote-1.0.9/email_auth_remote.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       53 2024-02-13 15:47:34.000000 email-auth-remote-1.0.9/email_auth_remote.egg-info/requires.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-02-13 15:47:34.000000 email-auth-remote-1.0.9/email_auth_remote.egg-info/top_level.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      603 2024-02-13 15:47:26.000000 email-auth-remote-1.0.9/pyproject.toml
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-02-13 15:47:34.922991 email-auth-remote-1.0.9/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-08 14:58:07.736713 email-auth-remote-1.1.0/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     2044 2024-04-08 14:58:07.736713 email-auth-remote-1.1.0/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1510 2024-03-27 15:31:17.000000 email-auth-remote-1.1.0/README.md
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-08 14:58:07.732713 email-auth-remote-1.1.0/email_auth_remote/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-08 14:54:42.000000 email-auth-remote-1.1.0/email_auth_remote/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1437 2024-04-08 14:51:55.000000 email-auth-remote-1.1.0/email_auth_remote/authentication.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     2816 2024-04-08 14:53:29.000000 email-auth-remote-1.1.0/email_auth_remote/middleware.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1494 2024-04-08 14:45:35.000000 email-auth-remote-1.1.0/email_auth_remote/models.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-08 07:54:28.000000 email-auth-remote-1.1.0/email_auth_remote/schema.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      727 2024-04-08 14:10:11.000000 email-auth-remote-1.1.0/email_auth_remote/settings.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1330 2024-04-08 14:48:28.000000 email-auth-remote-1.1.0/email_auth_remote/utils.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1318 2024-04-08 14:46:48.000000 email-auth-remote-1.1.0/email_auth_remote/views.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-08 14:58:07.732713 email-auth-remote-1.1.0/email_auth_remote.egg-info/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     2044 2024-04-08 14:58:07.000000 email-auth-remote-1.1.0/email_auth_remote.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      466 2024-04-08 14:58:07.000000 email-auth-remote-1.1.0/email_auth_remote.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-04-08 14:58:07.000000 email-auth-remote-1.1.0/email_auth_remote.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       53 2024-04-08 14:58:07.000000 email-auth-remote-1.1.0/email_auth_remote.egg-info/requires.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-04-08 14:58:07.000000 email-auth-remote-1.1.0/email_auth_remote.egg-info/top_level.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      603 2024-04-08 14:56:07.000000 email-auth-remote-1.1.0/pyproject.toml
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-04-08 14:58:07.736713 email-auth-remote-1.1.0/setup.cfg
```

### Comparing `email-auth-remote-1.0.9/PKG-INFO` & `email-auth-remote-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.0.9
+Version: 1.1.0
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
@@ -31,41 +31,49 @@
 ```
 
 Установить переменную AUTH_ENDPOINT_URL
 
 ```python
 # File: settings.py
 
-AUTH_ENDPOINT_URL = "http://localhost:8000/api/auth/user/"  # Как пример
+AUTH_ENDPOINT_URL = "http://localhost:8000/api/v1/auth/user/"  # Как пример
 ```
 
 Добавить класс аутентификации
 
 ```python
 # File: settings.py
 
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": [
         "email_auth_remote.authentication.EndpointAuthentication",
     ],
 }
 ```
 
+**Важная информация:**
+При использовании библиотеки модель EmailUser, полученная через request.user не будет сохранена в
+БД. На эту модель невозможно ссылаться через ForeignKey и тд. Сохранение в БД также невозможно.
+
 ## Сборка
 
+***Необходимо только для сборки, для интеграции не надо.***
+
 Как собрать проект локально
 
 ```bash
 python3 -m pip install build
 python3 -m build 
 ```
 
 ### Проверка собранного пакета
+
 ```bash
 python3 -m pip install twine
 twine check dist/*
 ```
 
 ### Выкладывание проекта в PYPI
+
 ```bash
 twine upload dist/*
 ```
```

### Comparing `email-auth-remote-1.0.9/email_auth_remote.egg-info/PKG-INFO` & `email-auth-remote-1.1.0/email_auth_remote.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.0.9
+Version: 1.1.0
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
@@ -31,41 +31,49 @@
 ```
 
 Установить переменную AUTH_ENDPOINT_URL
 
 ```python
 # File: settings.py
 
-AUTH_ENDPOINT_URL = "http://localhost:8000/api/auth/user/"  # Как пример
+AUTH_ENDPOINT_URL = "http://localhost:8000/api/v1/auth/user/"  # Как пример
 ```
 
 Добавить класс аутентификации
 
 ```python
 # File: settings.py
 
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": [
         "email_auth_remote.authentication.EndpointAuthentication",
     ],
 }
 ```
 
+**Важная информация:**
+При использовании библиотеки модель EmailUser, полученная через request.user не будет сохранена в
+БД. На эту модель невозможно ссылаться через ForeignKey и тд. Сохранение в БД также невозможно.
+
 ## Сборка
 
+***Необходимо только для сборки, для интеграции не надо.***
+
 Как собрать проект локально
 
 ```bash
 python3 -m pip install build
 python3 -m build 
 ```
 
 ### Проверка собранного пакета
+
 ```bash
 python3 -m pip install twine
 twine check dist/*
 ```
 
 ### Выкладывание проекта в PYPI
+
 ```bash
 twine upload dist/*
 ```
```

### Comparing `email-auth-remote-1.0.9/pyproject.toml` & `email-auth-remote-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email-auth-remote"
-version = "1.0.9"
+version = "1.1.0"
 description = "Django app for an endpoint authentication."
 readme = "README.md"
 requires-python = ">=3.11"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
```

