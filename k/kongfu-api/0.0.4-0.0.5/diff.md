# Comparing `tmp/kongfu-api-0.0.4.tar.gz` & `tmp/kongfu-api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kongfu-api-0.0.4.tar", last modified: Tue Feb 20 01:54:08 2024, max compression
+gzip compressed data, was "kongfu-api-0.0.5.tar", last modified: Mon Apr  8 05:42:36 2024, max compression
```

## Comparing `kongfu-api-0.0.4.tar` & `kongfu-api-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-02-20 01:54:08.061435 kongfu-api-0.0.4/
--rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-02-20 01:54:08.060239 kongfu-api-0.0.4/PKG-INFO
--rw-r--r--   0 zhudelong   (501) staff       (20)      103 2024-02-20 01:47:07.000000 kongfu-api-0.0.4/README.md
-drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-02-20 01:54:08.049275 kongfu-api-0.0.4/kongfu_api/
--rw-r--r--   0 zhudelong   (501) staff       (20)       21 2024-02-08 03:09:34.000000 kongfu-api-0.0.4/kongfu_api/__init__.py
--rw-r--r--   0 zhudelong   (501) staff       (20)     1514 2024-02-08 03:09:34.000000 kongfu-api-0.0.4/kongfu_api/db.py
--rw-r--r--   0 zhudelong   (501) staff       (20)    45905 2024-02-20 01:36:44.000000 kongfu-api-0.0.4/kongfu_api/kongfu.py
--rw-r--r--   0 zhudelong   (501) staff       (20)     7419 2024-02-20 00:55:31.000000 kongfu-api-0.0.4/kongfu_api/tool.py
-drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-02-20 01:54:08.057649 kongfu-api-0.0.4/kongfu_api.egg-info/
--rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-02-20 01:54:07.000000 kongfu-api-0.0.4/kongfu_api.egg-info/PKG-INFO
--rw-r--r--   0 zhudelong   (501) staff       (20)      304 2024-02-20 01:54:08.000000 kongfu-api-0.0.4/kongfu_api.egg-info/SOURCES.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)        1 2024-02-20 01:54:07.000000 kongfu-api-0.0.4/kongfu_api.egg-info/dependency_links.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       48 2024-02-20 01:54:07.000000 kongfu-api-0.0.4/kongfu_api.egg-info/entry_points.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       67 2024-02-20 01:54:08.000000 kongfu-api-0.0.4/kongfu_api.egg-info/requires.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       11 2024-02-20 01:54:08.000000 kongfu-api-0.0.4/kongfu_api.egg-info/top_level.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       38 2024-02-20 01:54:08.061637 kongfu-api-0.0.4/setup.cfg
--rw-r--r--   0 zhudelong   (501) staff       (20)     1500 2024-02-20 01:47:58.000000 kongfu-api-0.0.4/setup.py
+drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-08 05:42:36.927946 kongfu-api-0.0.5/
+-rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-04-08 05:42:36.927332 kongfu-api-0.0.5/PKG-INFO
+-rw-r--r--   0 zhudelong   (501) staff       (20)      103 2024-02-20 01:47:07.000000 kongfu-api-0.0.5/README.md
+drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-08 05:42:36.921602 kongfu-api-0.0.5/kongfu_api/
+-rw-r--r--   0 zhudelong   (501) staff       (20)       21 2024-03-15 02:22:53.000000 kongfu-api-0.0.5/kongfu_api/__init__.py
+-rw-r--r--   0 zhudelong   (501) staff       (20)     1514 2024-03-15 02:22:53.000000 kongfu-api-0.0.5/kongfu_api/db.py
+-rw-r--r--   0 zhudelong   (501) staff       (20)    45684 2024-03-25 05:12:32.000000 kongfu-api-0.0.5/kongfu_api/kongfu.py
+-rw-r--r--   0 zhudelong   (501) staff       (20)     7419 2024-03-15 02:22:53.000000 kongfu-api-0.0.5/kongfu_api/tool.py
+drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-08 05:42:36.926728 kongfu-api-0.0.5/kongfu_api.egg-info/
+-rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-04-08 05:42:36.000000 kongfu-api-0.0.5/kongfu_api.egg-info/PKG-INFO
+-rw-r--r--   0 zhudelong   (501) staff       (20)      304 2024-04-08 05:42:36.000000 kongfu-api-0.0.5/kongfu_api.egg-info/SOURCES.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)        1 2024-04-08 05:42:36.000000 kongfu-api-0.0.5/kongfu_api.egg-info/dependency_links.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       48 2024-04-08 05:42:36.000000 kongfu-api-0.0.5/kongfu_api.egg-info/entry_points.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       67 2024-04-08 05:42:36.000000 kongfu-api-0.0.5/kongfu_api.egg-info/requires.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       11 2024-04-08 05:42:36.000000 kongfu-api-0.0.5/kongfu_api.egg-info/top_level.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       38 2024-04-08 05:42:36.928063 kongfu-api-0.0.5/setup.cfg
+-rw-r--r--   0 zhudelong   (501) staff       (20)     1500 2024-04-08 05:40:09.000000 kongfu-api-0.0.5/setup.py
```

### Comparing `kongfu-api-0.0.4/PKG-INFO` & `kongfu-api-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kongfu-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: sample wsgi server
 Author: smart_long
 Author-email: smart_long@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kongfu-api-0.0.4/kongfu_api/db.py` & `kongfu-api-0.0.5/kongfu_api/db.py`

 * *Files identical despite different names*

### Comparing `kongfu-api-0.0.4/kongfu_api/kongfu.py` & `kongfu-api-0.0.5/kongfu_api/kongfu.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 # region tools
 
 def get_mapping_model(resource):
     if resource not in MODEL_MAPPING:
         return None
-    if type(MODEL_MAPPING[resource]) == dict:
+    if type(MODEL_MAPPING[resource]) == tuple:
         return MODEL_MAPPING[resource][0]
     else:
         return MODEL_MAPPING[resource]
 
 
 def get_mapping_operation(resource):
     if resource not in MODEL_MAPPING:
@@ -297,53 +297,53 @@
     #     __day 时间或日期字段的日
     #     __date 时间或日期字段的日期部分
     #     __startswith 以…开头
     #     __endswith 以…结尾
     #     """
 
     arr_where = []
-    param_where = dict()
+    param_where = []
     for key in dict_where.keys():
         if dict_where[key] != '':
             arr_k = key.split("__")
             if len(arr_k) == 1:
-                arr_where.append(key + " = {" + key + "}")
-                param_where[arr_k[0]] = dict_where[key]
+                arr_where.append(key + " = %s")
+                param_where.append(dict_where[key])
             if len(arr_k) == 2:
                 field = arr_k[0]
                 operation = str(arr_k[1]).lower()
                 if operation == "exact":
-                    arr_where.append(field + " = {" + field + "}")
-                    param_where[arr_k[0]] = dict_where[key]
+                    arr_where.append(field + " = %s")
+                    param_where.append(dict_where[key])
                 if operation == "contains":
-                    arr_where.append(field + " like {" + field + "}")
-                    param_where[arr_k[0]] = "%" + dict_where[key] + "%"
+                    arr_where.append(field + " like %s")
+                    param_where.append("%" + dict_where[key] + "%")
                 if operation == "gt":
-                    arr_where.append(field + " > {" + field + "}")
-                    param_where[arr_k[0]] = dict_where[key]
+                    arr_where.append(field + " > %s")
+                    param_where.append(dict_where[key])
                 if operation == "gte":
-                    arr_where.append(field + " >= {" + field + "}")
-                    param_where[arr_k[0]] = dict_where[key]
+                    arr_where.append(field + " >= %s")
+                    param_where.append(dict_where[key])
                 if operation == "lt":
-                    arr_where.append(field + " < {" + field + "}")
-                    param_where[arr_k[0]] = dict_where[key]
+                    arr_where.append(field + " < %s")
+                    param_where.append(dict_where[key])
                 if operation == "lte":
-                    arr_where.append(field + " <= {" + field + "}")
-                    param_where[arr_k[0]] = dict_where[key]
+                    arr_where.append(field + " <= %s")
+                    param_where.append(dict_where[key])
                 if operation == "in" and len(dict_where[key]) > 0:
-                    arr_where.append(field + " in (" + ",".join(['\'' + item + '\'' if isinstance(item, str) else str(item) for item in dict_where[key]]) + ") ")
-                    # param_where[arr_k[0]] = dict_where[key]
+                    arr_where.append(field + " in (" + ",".join(['%s' for item in dict_where[key]]) + ") ")
+                    if isinstance(dict_where[key], list):
+                        for  item in dict_where[key]:
+                            param_where.append(item)
                 if operation == "isnull" and dict_where[key] == True:
                     arr_where.append("ISNULL(" + field + ")")
-                    # param_where[arr_k[0]] = dict_where[key]
                 if operation == "isnull" and dict_where[key] == False:
                     arr_where.append("NOT ISNULL(" + field + ")")
-                    # param_where[arr_k[0]] = dict_where[key]
 
-    return arr_where, param_where
+    return arr_where, tuple(param_where)
 
 
 def auto_list(request, table_name):
     select = request.data.get('select', '*')
     where = request.data.get('where', '{}')
     order_by = request.data.get('order_by', '')
 
@@ -373,34 +373,34 @@
     if len(arr_where) > 0:
         str_sql += " where " + " and ".join(arr_where)
 
     if order_by:
         str_sql += " order by " + order_by
 
     data_sql = "select * from (" + str_sql + ") t limit " + str((page - 1) * size) + "," + str(size)
-    data_cursor = db.execute_sql(data_sql.format(**param_where))
+    data_cursor = db.execute_sql(data_sql, param_where)
     data = data_cursor.fetchall()
 
     count_sql = "select count(*) from (" + str_sql + ") t "
-    count_cursor = db.execute_sql(count_sql.format(**param_where))
+    count_cursor = db.execute_sql(count_sql,param_where)
     count = count_cursor.fetchall()
 
     return {
         "code": 200,
         "data": [row_to_dict(data_cursor, row) for row in data],
         "total": count[0][0],
         "msg": "Success"
     }
 
 
 def auto_get(request, table_name, pk):
     select = request.data.get('select', '*')
-    str_sql = "select " + select + " from " + table_name + " where id = '{id}' "
+    str_sql = "select " + select + " from " + table_name + " where id = %s "
 
-    cursor = db.execute_sql(str_sql.format(**{"id": pk}))
+    cursor = db.execute_sql(str_sql, (pk,))
     row = cursor.fetchone()
 
     if not row:
         return {
             "code": 404,
             "msg": "Not Found"
         }
@@ -488,15 +488,15 @@
 
 # endregion
 
 
 # region file_view
 
 def file_file(request, operation):
-    field_storage = request.FILES.get("file")
+    field_storage = request.files.get("file")
 
     allow_file_type = APP_SETTING["file"][operation]
     file_type = field_storage.filename.split('.')[-1]
     if str(file_type).lower() not in allow_file_type:
         return {
             "code": 400,
             "msg": "File Type Error!"
@@ -1144,16 +1144,16 @@
             star_response('200 OK', [('Content-Type', mimetype)])
             return '' if request.method == 'HEAD' else open(file_path, 'rb')
         else:
             if not request.path_resource or not request.path_operation:
                 star_response('200 OK', [('Content-Type', 'text/html')])
                 return ['''<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>Title</title></head><body>接口不存在</body></html>'''.encode('utf-8'), ]
 
-            star_response('200 OK', [('Content-Type', 'text/html')])
-            return ['''<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>Title</title></head><body>接口页面</body></html>'''.encode('utf-8'), ]
+            # star_response('200 OK', [('Content-Type', 'text/html')])
+            # return ['''<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><title>Title</title></head><body>接口页面</body></html>'''.encode('utf-8'), ]
 
     # endregion
 
     # 资源
     path_resource = request.path_resource
     # 方法
     path_operation = request.path_operation
```

### Comparing `kongfu-api-0.0.4/kongfu_api/tool.py` & `kongfu-api-0.0.5/kongfu_api/tool.py`

 * *Files identical despite different names*

### Comparing `kongfu-api-0.0.4/kongfu_api.egg-info/PKG-INFO` & `kongfu-api-0.0.5/kongfu_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kongfu-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: sample wsgi server
 Author: smart_long
 Author-email: smart_long@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kongfu-api-0.0.4/setup.py` & `kongfu-api-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'sample wsgi server'
 
 setup(
     name="kongfu-api",
     version=VERSION,
     author="smart_long",
     author_email="smart_long@outlook.com",
```

