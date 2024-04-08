# Comparing `tmp/Drumpler-1.0.7.tar.gz` & `tmp/Drumpler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.7.tar", last modified: Fri Apr  5 21:43:29 2024, max compression
+gzip compressed data, was "Drumpler-1.0.8.tar", last modified: Mon Apr  8 20:51:13 2024, max compression
```

## Comparing `Drumpler-1.0.7.tar` & `Drumpler-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.533457 Drumpler-1.0.7/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.531896 Drumpler-1.0.7/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.7/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:43:29.532624 Drumpler-1.0.7/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.7/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.526579 Drumpler-1.0.7/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.7/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.7/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     6982 2024-04-05 21:43:17.000000 Drumpler-1.0.7/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.7/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.7/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-05 21:43:29.533637 Drumpler-1.0.7/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-05 21:43:22.000000 Drumpler-1.0.7/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.530959 Drumpler-1.0.7/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.7/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.566760 Drumpler-1.0.8/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.565359 Drumpler-1.0.8/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.8/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-08 20:51:13.566139 Drumpler-1.0.8/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.8/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.560543 Drumpler-1.0.8/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.8/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.8/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6945 2024-04-08 20:50:43.000000 Drumpler-1.0.8/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.8/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.8/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-08 20:51:13.566880 Drumpler-1.0.8/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-08 20:50:49.000000 Drumpler-1.0.8/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.564461 Drumpler-1.0.8/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.8/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.7/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.0.8/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.7/LICENSE` & `Drumpler-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.7/PKG-INFO` & `Drumpler-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.7/README.md` & `Drumpler-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.7/drumpler/constants.py` & `Drumpler-1.0.8/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.7/drumpler/drumpler.py` & `Drumpler-1.0.8/drumpler/drumpler.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,17 +33,20 @@
         self.host = os.environ.get("DRUMPLER_HOST", DRUMPLER_HOST)
         self.port = os.environ.get("DRUMPLER_PORT", DRUMPLER_PORT)
         self.debug = os.environ.get("DRUMPLER_DEBUG",DRUMPLER_DEBUG)
         
         self.app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
-        # Initialize SQLAlchemy with the current Flask app
+        # Initialize SQLAlchemy with the Flask app here instead of global scope
         db.init_app(self.app)
 
+        with self.app.app_context():
+            db.create_all()  # Move database initialization here
+        
         self.__setup_routes()
 
     def __setup_routes(self):
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
         self.app.add_url_rule('/request/next-unhandled', view_func=self.__get_next_unhandled_request, methods=['GET'])
@@ -149,16 +152,12 @@
             db.session.delete(request_entry)
             db.session.commit()
             return jsonify({"message": "Request deleted successfully"}), 200
         else:
             return jsonify({"message": "Request not found"}), 404
 
     def run(self):
-        with app.app_context():
-            db.create_all()  # Initialize the database tables within an application context
-            db.session.commit()
-            
         app.run(host=self.host, port=self.port, debug=self.debug)
 
 if __name__ == '__main__':
     drumpler = Drumpler()
     drumpler.run()
```

### Comparing `Drumpler-1.0.7/drumpler/mammoth.py` & `Drumpler-1.0.8/drumpler/mammoth.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.7/drumpler/request.py` & `Drumpler-1.0.8/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.7/setup.py` & `Drumpler-1.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.7',
+    version='1.0.8',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.7/test/test_drumpler.py` & `Drumpler-1.0.8/test/test_drumpler.py`

 * *Files identical despite different names*

