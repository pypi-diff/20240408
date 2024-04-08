# Comparing `tmp/dwh_oppfolging-0.0.90.tar.gz` & `tmp/dwh_oppfolging-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwh_oppfolging-0.0.90.tar", max compression
+gzip compressed data, was "dwh_oppfolging-0.0.91.tar", max compression
```

## Comparing `dwh_oppfolging-0.0.90.tar` & `dwh_oppfolging-0.0.91.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/LICENSE
--rw-r--r--   0        0        0      325 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/README.md
--rw-r--r--   0        0        0       22 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/README.md
--rw-r--r--   0        0        0        0 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/__init__.py
--rw-r--r--   0        0        0       14 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/airflow_api_v1.py
--rw-r--r--   0        0        0     8543 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1.py
--rw-r--r--   0        0        0     4051 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1_types.py
--rw-r--r--   0        0        0    17798 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v2.py
--rw-r--r--   0        0        0     2163 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/dbt_oracle_api_v1.py
--rw-r--r--   0        0        0      422 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/generic_api_v1.py
--rw-r--r--   0        0        0      741 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/kafka_api_v1.py
--rw-r--r--   0        0        0    24608 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/kafka_api_v1_types.py
--rw-r--r--   0        0        0    11838 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/oracle_api_v1.py
--rw-r--r--   0        0        0      125 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/oracle_api_v1_types.py
--rw-r--r--   0        0        0     2371 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/secrets_api_v1.py
--rw-r--r--   0        0        0     6831 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/ssb_api_v1.py
--rw-r--r--   0        0        0    11693 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/ssb_api_v1_types.py
--rw-r--r--   0        0        0        0 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/__init__.py
--rw-r--r--   0        0        0     9224 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/datatypes.py
--rw-r--r--   0        0        0     9521 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/functions.py
--rw-r--r--   0        0        0     1661 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/pyproject.toml
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.90/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-08 10:48:41.589381 dwh_oppfolging-0.0.91/LICENSE
+-rw-r--r--   0        0        0      325 2024-04-08 10:48:41.589381 dwh_oppfolging-0.0.91/README.md
+-rw-r--r--   0        0        0       22 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/__init__.py
+-rw-r--r--   0        0        0       14 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/airflow_api_v1.py
+-rw-r--r--   0        0        0     8543 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1.py
+-rw-r--r--   0        0        0     4051 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1_types.py
+-rw-r--r--   0        0        0    17798 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v2.py
+-rw-r--r--   0        0        0     2179 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/dbt_oracle_api_v1.py
+-rw-r--r--   0        0        0      422 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/generic_api_v1.py
+-rw-r--r--   0        0        0      741 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1.py
+-rw-r--r--   0        0        0    24608 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1_types.py
+-rw-r--r--   0        0        0    11838 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/oracle_api_v1.py
+-rw-r--r--   0        0        0      125 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/oracle_api_v1_types.py
+-rw-r--r--   0        0        0     2371 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/secrets_api_v1.py
+-rw-r--r--   0        0        0     6831 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1.py
+-rw-r--r--   0        0        0    11693 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1_types.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/__init__.py
+-rw-r--r--   0        0        0     9224 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/datatypes.py
+-rw-r--r--   0        0        0     9521 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/functions.py
+-rw-r--r--   0        0        0     1661 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/pyproject.toml
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.91/PKG-INFO
```

### Comparing `dwh_oppfolging-0.0.90/LICENSE` & `dwh_oppfolging-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1_types.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v2.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v2.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/dbt_oracle_api_v1.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/dbt_oracle_api_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         - schema, str: the schema the dbt project operates in.
     
     yields:
         - None
     """
     creds = get_oracle_user_credentials(schema)
     dbt_env_params = {
-        "DBT_ENV_SECRET_USER": creds["user"],
+        "DBT_ENV_SECRET_USER": creds["user"] + f"[{schema}]",
         "DBT_ENV_SECRET_PASS": creds["pwd"],
         "DBT_ENV_SECRET_HOST": creds["host"],
         "DBT_ENV_SECRET_PORT": creds["port"],
         "DBT_ENV_SECRET_SERVICE": creds["service"],
         "DBT_ENV_SECRET_DATABASE": creds["database"],
         "DBT_ENV_SECRET_SCHEMA": schema,
         "ORA_PYTHON_DRIVER_TYPE": "thin",
```

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/kafka_api_v1.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/kafka_api_v1_types.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/oracle_api_v1.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/oracle_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/secrets_api_v1.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/secrets_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/ssb_api_v1.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/ssb_api_v1_types.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/datatypes.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/datatypes.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/functions.py` & `dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/functions.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.90/pyproject.toml` & `dwh_oppfolging-0.0.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dwh-oppfolging"
-version = "0.0.90"
+version = "0.0.91"
 description = "Oppfolging python package for DWH ETL"
 authors = ["Team Oppfølging"]
 packages = [{include = "dwh_oppfolging"}]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `dwh_oppfolging-0.0.90/PKG-INFO` & `dwh_oppfolging-0.0.91/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwh-oppfolging
-Version: 0.0.90
+Version: 0.0.91
 Summary: Oppfolging python package for DWH ETL
 Author: Team Oppfølging
 Requires-Python: ==3.11.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: confluent-kafka (==2.3.0)
 Requires-Dist: dbt-oracle (==1.7.3)
```

