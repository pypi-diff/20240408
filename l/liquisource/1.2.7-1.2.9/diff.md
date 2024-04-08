# Comparing `tmp/liquisource-1.2.7.tar.gz` & `tmp/liquisource-1.2.9.tar.gz`

## Comparing `liquisource-1.2.7.tar` & `liquisource-1.2.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liquisource-1.2.7/Dockerfile
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 liquisource-1.2.7/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/ck_client.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/config.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/es_client.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/mongo_client.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/mysql_client.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.2.7/liquiclient/redis_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.7/.gitignore
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 liquisource-1.2.7/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 liquisource-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 liquisource-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 liquisource-1.2.9/.DS_Store
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 liquisource-1.2.9/Dockerfile
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 liquisource-1.2.9/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/__init__.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/ck_client.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/config.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/es_client.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/mysql_client.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 liquisource-1.2.9/liquiclient/redis_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.9/.gitignore
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 liquisource-1.2.9/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 liquisource-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 liquisource-1.2.9/PKG-INFO
```

### Comparing `liquisource-1.2.7/liquiclient/config.py` & `liquisource-1.2.9/liquiclient/config.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.7/liquiclient/es_client.py` & `liquisource-1.2.9/liquiclient/es_client.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.7/liquiclient/mysql_client.py` & `liquisource-1.2.9/liquiclient/mysql_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     # 由于默认liquibase是jdbc的，这里解析对应的ip port
     params = parse_jdbc_dsn(get_property("url"))
     client = mysql.connector.connect(**params)
 
     return client
 
 
+# 获取mysql集群实例
+def get_mysql_cluster_client(cluster):
+    # 由于默认liquibase是jdbc的，这里解析对应的ip port
+    params = parse_jdbc_dsn(get_property(cluster+".url"))
+    client = mysql.connector.connect(**params)
+
+    return client
+
+
 def parse_jdbc_dsn(dsn):
     if not dsn.startswith("jdbc:"):
         raise ValueError("Invalid MySQL DSN")
     # 去除 "jdbc:" 前缀
     dsn = dsn[5:]
 
     # 当成url解析
```

### Comparing `liquisource-1.2.7/README.md` & `liquisource-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.7/pyproject.toml` & `liquisource-1.2.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build.targets.wheel]
+packages = ["liquiclient"]
+
 [project]
 name = "liquisource"
-version = "1.2.7"
+version = "1.2.9"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `liquisource-1.2.7/PKG-INFO` & `liquisource-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.2.7
+Version: 1.2.9
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

