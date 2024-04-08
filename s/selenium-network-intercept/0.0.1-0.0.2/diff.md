# Comparing `tmp/selenium-network-intercept-0.0.1.tar.gz` & `tmp/selenium-network-intercept-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-network-intercept-0.0.1.tar", last modified: Mon Apr  8 16:58:11 2024, max compression
+gzip compressed data, was "selenium-network-intercept-0.0.2.tar", last modified: Mon Apr  8 17:27:49 2024, max compression
```

## Comparing `selenium-network-intercept-0.0.1.tar` & `selenium-network-intercept-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:58:11.200960 selenium-network-intercept-0.0.1/
--rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-0.0.1/LICENCE
--rw-rw-rw-   0        0        0     6344 2024-04-08 16:58:11.199952 selenium-network-intercept-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5935 2024-04-08 16:41:42.000000 selenium-network-intercept-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 16:58:11.192446 selenium-network-intercept-0.0.1/network_intercept/
--rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-0.0.1/network_intercept/__init__.py
--rw-rw-rw-   0        0        0     3720 2024-04-08 16:33:17.000000 selenium-network-intercept-0.0.1/network_intercept/intercept.py
--rw-rw-rw-   0        0        0     3237 2024-03-04 14:19:54.000000 selenium-network-intercept-0.0.1/network_intercept/objected.py
--rw-rw-rw-   0        0        0     1798 2024-04-08 16:33:17.000000 selenium-network-intercept-0.0.1/network_intercept/request.py
--rw-rw-rw-   0        0        0     1571 2024-04-08 16:33:17.000000 selenium-network-intercept-0.0.1/network_intercept/response.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:58:11.198446 selenium-network-intercept-0.0.1/selenium_network_intercept.egg-info/
--rw-rw-rw-   0        0        0     6344 2024-04-08 16:58:11.000000 selenium-network-intercept-0.0.1/selenium_network_intercept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-04-08 16:58:11.000000 selenium-network-intercept-0.0.1/selenium_network_intercept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:58:11.000000 selenium-network-intercept-0.0.1/selenium_network_intercept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-08 16:58:11.000000 selenium-network-intercept-0.0.1/selenium_network_intercept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 16:58:11.200960 selenium-network-intercept-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2024-04-08 16:58:10.000000 selenium-network-intercept-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:27:49.285391 selenium-network-intercept-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0     6353 2024-04-08 17:27:49.284392 selenium-network-intercept-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5944 2024-04-08 17:26:13.000000 selenium-network-intercept-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 17:27:49.278392 selenium-network-intercept-0.0.2/selenium_network_intercept/
+-rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/__init__.py
+-rw-rw-rw-   0        0        0     3747 2024-04-08 17:26:28.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/intercept.py
+-rw-rw-rw-   0        0        0     3237 2024-03-04 14:19:54.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/objected.py
+-rw-rw-rw-   0        0        0     1807 2024-04-08 17:26:28.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/request.py
+-rw-rw-rw-   0        0        0     1580 2024-04-08 17:26:28.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/response.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:27:49.283391 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/
+-rw-rw-rw-   0        0        0     6353 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 17:27:49.285391 selenium-network-intercept-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      664 2024-04-08 17:27:46.000000 selenium-network-intercept-0.0.2/setup.py
```

### Comparing `selenium-network-intercept-0.0.1/LICENCE` & `selenium-network-intercept-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.1/PKG-INFO` & `selenium-network-intercept-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
 Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -57,15 +57,15 @@
 A partir desta configuração, é possível receber os LOGS que trarão todas requisições feitas durante a execução do navegador pela instância `driver`.
 
 ---
 
 Após realizada a instância, importe a função `intercept_http` do pacote network, e módulo intercept.
 
 ```python
-from network.intercept import intercept_http
+from selenium_network_intercept import intercept_http
 ```
 
 Feito isso, você já tem todas funcionalidades do pacote em uma chamada, apenas sendo necessários alterar parâmetros, vamos as explicações de como usá-la.
 
 ---
 
 ### Buscando as requisições
```

### Comparing `selenium-network-intercept-0.0.1/README.md` & `selenium-network-intercept-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 A partir desta configuração, é possível receber os LOGS que trarão todas requisições feitas durante a execução do navegador pela instância `driver`.
 
 ---
 
 Após realizada a instância, importe a função `intercept_http` do pacote network, e módulo intercept.
 
 ```python
-from network.intercept import intercept_http
+from selenium_network_intercept import intercept_http
 ```
 
 Feito isso, você já tem todas funcionalidades do pacote em uma chamada, apenas sendo necessários alterar parâmetros, vamos as explicações de como usá-la.
 
 ---
 
 ### Buscando as requisições
```

### Comparing `selenium-network-intercept-0.0.1/network_intercept/intercept.py` & `selenium-network-intercept-0.0.2/selenium_network_intercept/intercept.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import json
-from network_intercept.response import network_response
-from network_intercept.request import network_request
+from selenium_network_intercept.response import network_response
+from selenium_network_intercept.request import network_request
 from time import sleep
-from network_intercept.objected import ObjectIntercepted
+from selenium_network_intercept.objected import ObjectIntercepted
 
 
 def  _get_url(params,req_or_res): #falta teste unitario
     try:
         if req_or_res == 'response':
             url = _fix_url(params.get('response').get('url'))
         else:
```

### Comparing `selenium-network-intercept-0.0.1/network_intercept/objected.py` & `selenium-network-intercept-0.0.2/selenium_network_intercept/objected.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.1/network_intercept/request.py` & `selenium-network-intercept-0.0.2/selenium_network_intercept/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from network_intercept.objected import MethodError
+from selenium_network_intercept.objected import MethodError
 
 
 def network_request(
     params,
     message,
     route,
     url,
```

### Comparing `selenium-network-intercept-0.0.1/network_intercept/response.py` & `selenium-network-intercept-0.0.2/selenium_network_intercept/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from network_intercept.objected import ObjectIntercepted
+from selenium_network_intercept.objected import ObjectIntercepted
 
 
 def network_response(
     driver,
     params,
     message,
     route,
```

### Comparing `selenium-network-intercept-0.0.1/selenium_network_intercept.egg-info/PKG-INFO` & `selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
 Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -57,15 +57,15 @@
 A partir desta configuração, é possível receber os LOGS que trarão todas requisições feitas durante a execução do navegador pela instância `driver`.
 
 ---
 
 Após realizada a instância, importe a função `intercept_http` do pacote network, e módulo intercept.
 
 ```python
-from network.intercept import intercept_http
+from selenium_network_intercept import intercept_http
 ```
 
 Feito isso, você já tem todas funcionalidades do pacote em uma chamada, apenas sendo necessários alterar parâmetros, vamos as explicações de como usá-la.
 
 ---
 
 ### Buscando as requisições
```

### Comparing `selenium-network-intercept-0.0.1/setup.py` & `selenium-network-intercept-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 file = open('README.md', 'r',encoding='utf-8')
 readme = file.read()
 
 
 setup(
     name='selenium-network-intercept',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT License',
     author='Alexandre Mariano',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='alexandre_mariano@hotmail.com.br',
     keywords=['selenium', 'network', 'intercept','http','requests','selenium network intercept','selenium intercept'],
     description='Interceptador de requisições http não oficial do selenium 4',
-    packages=['network_intercept'],
+    packages=['selenium_network_intercept'],
     install_requires=[]
 )
 
 file.close()
```

