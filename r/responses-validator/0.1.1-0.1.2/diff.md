# Comparing `tmp/responses_validator-0.1.1-cp312-cp312-win_amd64.whl.zip` & `tmp/responses_validator-0.1.2-cp312-cp312-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 58413 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1254 b- defN 16-Jan-01 00:00 responses_validator/__init__.pyi
--rw-rw-rw-  2.0 fat   124928 b- defN 16-Jan-01 00:00 responses_validator/__init__.cp312-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2433 b- defN 16-Jan-01 00:00 responses_validator-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      101 b- defN 16-Jan-01 00:00 responses_validator-0.1.1.dist-info/WHEEL
-?rw-------  2.0 fat      439 b- defN 16-Jan-01 00:00 responses_validator-0.1.1.dist-info/RECORD
-5 files, 129155 bytes uncompressed, 57597 bytes compressed:  55.4%
+Zip file size: 59273 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   126976 b- defN 16-Jan-01 00:00 responses_validator/__init__.cp312-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1300 b- defN 16-Jan-01 00:00 responses_validator/__init__.pyi
+-rw-rw-rw-  2.0 fat     2433 b- defN 16-Jan-01 00:00 responses_validator-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      101 b- defN 16-Jan-01 00:00 responses_validator-0.1.2.dist-info/WHEEL
+?rw-------  2.0 fat      439 b- defN 16-Jan-01 00:00 responses_validator-0.1.2.dist-info/RECORD
+5 files, 131249 bytes uncompressed, 58457 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: responses_validator/__init__.pyi
+Filename: responses_validator/__init__.cp312-win_amd64.pyd
 Comment: 
 
-Filename: responses_validator/__init__.cp312-win_amd64.pyd
+Filename: responses_validator/__init__.pyi
 Comment: 
 
-Filename: responses_validator-0.1.1.dist-info/METADATA
+Filename: responses_validator-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: responses_validator-0.1.1.dist-info/WHEEL
+Filename: responses_validator-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: responses_validator-0.1.1.dist-info/RECORD
+Filename: responses_validator-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## responses_validator/__init__.pyi

```diff
@@ -36,7 +36,9 @@
     def validate_text(self, resp_text): ...
     def validate_json(self, resp_json_func): ...
     @property
     def errors(self) -> dict[str, str]: ...
     def __init__(self, status_code, headers, text, json) -> None: ...
 
 class ResponseAssertionError(AssertionError): ...
+
+def validator(resp, **kwargs) -> None: ...
```

## Comparing `responses_validator-0.1.1.dist-info/METADATA` & `responses_validator-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responses-validator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Write response validation scripts for requests using flexible YAML syntax, including: status_code, headers, text, and json()
 License: MIT
 Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
 Requires-Python: ~=3.12
 Requires-Dist: genson~=1.2.2
 Requires-Dist: jsonpath~=0.82.2
 Requires-Dist: jsonschema~=4.21.1
```

