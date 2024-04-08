# Comparing `tmp/ctqkit-0.1.1b3.tar.gz` & `tmp/ctqkit-0.1.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctqkit-0.1.1b3.tar", max compression
+gzip compressed data, was "ctqkit-0.1.1b4.tar", max compression
```

## Comparing `ctqkit-0.1.1b3.tar` & `ctqkit-0.1.1b4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b3/LICENSE.txt
--rw-r--r--   0        0        0      946 2024-04-02 11:14:50.769219 ctqkit-0.1.1b3/pyproject.toml
--rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b3/README.md
--rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b3/src/CtqKit/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b3/src/CtqKit/account.py
--rw-r--r--   0        0        0    31174 2024-04-02 11:12:51.377421 ctqkit-0.1.1b3/src/CtqKit/platform.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 ctqkit-0.1.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b4/LICENSE.txt
+-rw-r--r--   0        0        0      953 2024-04-08 02:27:27.634900 ctqkit-0.1.1b4/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b4/README.md
+-rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b4/src/CtqKit/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b4/src/CtqKit/account.py
+-rw-r--r--   0        0        0    31334 2024-04-08 02:25:24.690537 ctqkit-0.1.1b4/src/CtqKit/platform.py
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ctqkit-0.1.1b4/PKG-INFO
```

### Comparing `ctqkit-0.1.1b3/LICENSE.txt` & `ctqkit-0.1.1b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b3/pyproject.toml` & `ctqkit-0.1.1b4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "CtqKit"
-version = "0.1.1-beta.3"
+version = "0.1.1-beta.4"
 description = "中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)"
 authors = ["Gao Jianjian <jianjian001@outlook.com>"]
 readme = "README.md"
-license = "MIT"
+license = "Apache 2.0"
 documentation = "https://qc.zdxlz.com/informationSpace"
 homepage = "https://qc.zdxlz.com/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ctqkit-0.1.1b3/src/CtqKit/account.py` & `ctqkit-0.1.1b4/src/CtqKit/account.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b3/src/CtqKit/platform.py` & `ctqkit-0.1.1b4/src/CtqKit/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,21 +384,21 @@
         else:
             new_circuit = circuit
         data = [{
             "exp_id": exp_id,
             "experimentId": collection_id,
             "inputCode": c,
             "languageCode": language,
-            "name": exp_name,
+            "name": f'{exp_name}.{i}',
             "shots": num_shots,
             "source": "sdk",
             "computerCode": self.machine,
             "experimentDetailName": version,
             "is_verify": is_verify
-        } for c in new_circuit]
+        } for i, c in enumerate(new_circuit)]
         return self._batch_run_experiment(data)
 
     def _batch_run_experiment(self, data):
         """
         批量提交任务，返回任务 id 列表，并后台排队运行
         todo: 接口未完成
 
@@ -613,15 +613,18 @@
             raise Exception(f'下载实验参数失败接口请求失败, status_code:{status_code}')
         result = res.json()
         code = result.get('code')
         if code != self.SUCCESS_CODE:
             msg = result.get('msg', '下载实验参数失败')
             raise RequestError(f'下载实验参数失败:{msg}')
         data = result.get('data')
-
+        try:
+            data = json.loads(data)
+        except Exception as e:
+            raise Exception("config file parse error")
         if save_file:
             with open(f'./{self.machine}_config_param_{self.current_datetime()}.json', 'w') as f:
                 f.write(json.dumps(data))
         return data
 
     @staticmethod
     def current_datetime(fmt='%Y-%m-%d %H:%M:%S'):
```

### Comparing `ctqkit-0.1.1b3/PKG-INFO` & `ctqkit-0.1.1b4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: CtqKit
-Version: 0.1.1b3
+Version: 0.1.1b4
 Summary: 中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)
 Home-page: https://qc.zdxlz.com/
-License: MIT
+License: Apache 2.0
 Author: Gao Jianjian
 Author-email: jianjian001@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

