# Comparing `tmp/dynamic-rest-client-0.1.9.tar.gz` & `tmp/dynamic-rest-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynamic-rest-client-0.1.9.tar", last modified: Wed Mar 27 23:59:33 2024, max compression
+gzip compressed data, was "dynamic-rest-client-0.2.0.tar", last modified: Mon Apr  8 21:55:46 2024, max compression
```

## Comparing `dynamic-rest-client-0.1.9.tar` & `dynamic-rest-client-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/
--rw-r--r--   0 savinay    (501) staff       (20)     1677 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/CONTRIBUTING.md
--rw-r--r--   0 savinay    (501) staff       (20)     1081 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/LICENSE.md
--rw-r--r--   0 savinay    (501) staff       (20)     1081 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/LICENSE.txt
--rw-r--r--   0 savinay    (501) staff       (20)       41 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/MANIFEST.in
--rw-r--r--   0 savinay    (501) staff       (20)      335 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/PKG-INFO
--rw-r--r--   0 savinay    (501) staff       (20)       92 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/README.md
--rw-r--r--   0 savinay    (501) staff       (20)       95 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/README.rst
-drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/
--rw-r--r--   0 savinay    (501) staff       (20)       40 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/__init__.py
--rw-r--r--   0 savinay    (501) staff       (20)     7879 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/client.py
--rw-r--r--   0 savinay    (501) staff       (20)      172 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/exceptions.py
--rw-r--r--   0 savinay    (501) staff       (20)     4686 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/query.py
--rw-r--r--   0 savinay    (501) staff       (20)     3448 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/record.py
--rw-r--r--   0 savinay    (501) staff       (20)     2937 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/resource.py
--rw-r--r--   0 savinay    (501) staff       (20)      207 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/dynamic_rest_client/utils.py
-drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/
--rw-r--r--   0 savinay    (501) staff       (20)      335 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/PKG-INFO
--rw-r--r--   0 savinay    (501) staff       (20)      600 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/SOURCES.txt
--rw-r--r--   0 savinay    (501) staff       (20)        1 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/dependency_links.txt
--rw-r--r--   0 savinay    (501) staff       (20)       46 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/requires.txt
--rw-r--r--   0 savinay    (501) staff       (20)       20 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/top_level.txt
--rw-r--r--   0 savinay    (501) staff       (20)       46 2024-03-27 23:04:59.000000 dynamic-rest-client-0.1.9/install_requires.txt
--rw-r--r--   0 savinay    (501) staff       (20)      133 2024-03-27 23:04:59.000000 dynamic-rest-client-0.1.9/requirements.txt
--rw-r--r--   0 savinay    (501) staff       (20)       38 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/setup.cfg
--rw-r--r--   0 savinay    (501) staff       (20)      514 2024-03-27 23:27:24.000000 dynamic-rest-client-0.1.9/setup.py
-drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-03-27 23:59:33.000000 dynamic-rest-client-0.1.9/tests/
--rw-r--r--   0 savinay    (501) staff       (20)     6412 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/tests/test_client.py
--rw-r--r--   0 savinay    (501) staff       (20)      598 2024-03-27 22:57:22.000000 dynamic-rest-client-0.1.9/tests/test_deepcopy.py
--rw-r--r--   0 savinay    (501) staff       (20)      298 2024-03-27 23:04:59.000000 dynamic-rest-client-0.1.9/tox.ini
+drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-04-08 21:55:46.405340 dynamic-rest-client-0.2.0/
+-rw-r--r--   0 savinay    (501) staff       (20)     1677 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 savinay    (501) staff       (20)     1081 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/LICENSE.md
+-rw-r--r--   0 savinay    (501) staff       (20)     1081 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/LICENSE.txt
+-rw-r--r--   0 savinay    (501) staff       (20)       41 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/MANIFEST.in
+-rw-r--r--   0 savinay    (501) staff       (20)      441 2024-04-08 21:55:46.405068 dynamic-rest-client-0.2.0/PKG-INFO
+-rw-r--r--   0 savinay    (501) staff       (20)       92 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/README.md
+-rw-r--r--   0 savinay    (501) staff       (20)       95 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/README.rst
+drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-04-08 21:55:46.403334 dynamic-rest-client-0.2.0/dynamic_rest_client/
+-rw-r--r--   0 savinay    (501) staff       (20)       40 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/__init__.py
+-rw-r--r--   0 savinay    (501) staff       (20)     7879 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/client.py
+-rw-r--r--   0 savinay    (501) staff       (20)      172 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/exceptions.py
+-rw-r--r--   0 savinay    (501) staff       (20)     4686 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/query.py
+-rw-r--r--   0 savinay    (501) staff       (20)     3448 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/record.py
+-rw-r--r--   0 savinay    (501) staff       (20)     2937 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/resource.py
+-rw-r--r--   0 savinay    (501) staff       (20)      207 2024-03-27 22:57:22.000000 dynamic-rest-client-0.2.0/dynamic_rest_client/utils.py
+drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-04-08 21:55:46.404730 dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/
+-rw-r--r--   0 savinay    (501) staff       (20)      441 2024-04-08 21:55:46.000000 dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/PKG-INFO
+-rw-r--r--   0 savinay    (501) staff       (20)      600 2024-04-08 21:55:46.000000 dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/SOURCES.txt
+-rw-r--r--   0 savinay    (501) staff       (20)        1 2024-04-08 21:55:46.000000 dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/dependency_links.txt
+-rw-r--r--   0 savinay    (501) staff       (20)       46 2024-04-08 21:55:46.000000 dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/requires.txt
+-rw-r--r--   0 savinay    (501) staff       (20)       20 2024-04-08 21:55:46.000000 dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/top_level.txt
+-rw-r--r--   0 savinay    (501) staff       (20)       46 2024-04-08 21:50:44.000000 dynamic-rest-client-0.2.0/install_requires.txt
+-rw-r--r--   0 savinay    (501) staff       (20)       92 2024-04-08 21:50:44.000000 dynamic-rest-client-0.2.0/requirements.txt
+-rw-r--r--   0 savinay    (501) staff       (20)       38 2024-04-08 21:55:46.405404 dynamic-rest-client-0.2.0/setup.cfg
+-rw-r--r--   0 savinay    (501) staff       (20)      514 2024-04-08 21:50:44.000000 dynamic-rest-client-0.2.0/setup.py
+drwxr-xr-x   0 savinay    (501) staff       (20)        0 2024-04-08 21:55:46.404501 dynamic-rest-client-0.2.0/tests/
+-rw-r--r--   0 savinay    (501) staff       (20)     6358 2024-04-08 21:50:44.000000 dynamic-rest-client-0.2.0/tests/test_client.py
+-rw-r--r--   0 savinay    (501) staff       (20)      595 2024-04-08 21:50:44.000000 dynamic-rest-client-0.2.0/tests/test_deepcopy.py
+-rw-r--r--   0 savinay    (501) staff       (20)      299 2024-04-08 21:50:44.000000 dynamic-rest-client-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dynamic-rest-client-0.1.9/CONTRIBUTING.md` & `dynamic-rest-client-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/LICENSE.md` & `dynamic-rest-client-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/LICENSE.txt` & `dynamic-rest-client-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/dynamic_rest_client/client.py` & `dynamic-rest-client-0.2.0/dynamic_rest_client/client.py`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/dynamic_rest_client/query.py` & `dynamic-rest-client-0.2.0/dynamic_rest_client/query.py`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/dynamic_rest_client/record.py` & `dynamic-rest-client-0.2.0/dynamic_rest_client/record.py`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/dynamic_rest_client/resource.py` & `dynamic-rest-client-0.2.0/dynamic_rest_client/resource.py`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/dynamic_rest_client.egg-info/SOURCES.txt` & `dynamic-rest-client-0.2.0/dynamic_rest_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-rest-client-0.1.9/setup.py` & `dynamic-rest-client-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 NAME = 'dynamic-rest-client'
 DESCRIPTION = 'Python client for dynamic-rest with minimal dependencies'
 URL = 'http://github.com/AltSchool/dynamic-rest-client'
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 SCRIPTS = []
 
 setup(
     description=DESCRIPTION,
     include_package_data=True,
     install_requires=open('install_requires.txt').readlines(),
     long_description=open('README.rst').read(),
```

### Comparing `dynamic-rest-client-0.1.9/tests/test_client.py` & `dynamic-rest-client-0.2.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import
 import json
 from rest_framework.test import APITestCase, APIClient
 from dynamic_rest_client import DRESTClient
 from dynamic_rest_client.exceptions import (
     BadRequest, DoesNotExist
 )
 from six import string_types
@@ -48,43 +47,43 @@
         self.fixture = create_fixture()
         self.drest = DRESTClient(
             'test', client=MockSession(self.client)
         )
 
     def test_get_all(self):
         users = self.drest.Users.all().list()
-        self.assertEquals(len(users), len(self.fixture.users))
-        self.assertEquals(
+        self.assertEqual(len(users), len(self.fixture.users))
+        self.assertEqual(
             {user.name for user in users},
             {user.name for user in self.fixture.users}
         )
 
     def test_get_filter(self):
         users = self.drest.Users.filter(id=self.fixture.users[0].id).list()
-        self.assertEquals(1, len(users))
-        self.assertEquals(users[0].name, self.fixture.users[0].name)
+        self.assertEqual(1, len(users))
+        self.assertEqual(users[0].name, self.fixture.users[0].name)
 
     def test_get_one(self):
         fixed_user = self.fixture.users[0]
         pk = fixed_user.pk
         user = self.drest.Users.get(pk)
-        self.assertEquals(user.name, fixed_user.name)
+        self.assertEqual(user.name, fixed_user.name)
         # test dict get
-        self.assertEquals(user['name'], fixed_user.name)
-        self.assertEquals(user.get('name'), fixed_user.name)
-        self.assertEquals(user.get('foobar'), None)
+        self.assertEqual(user['name'], fixed_user.name)
+        self.assertEqual(user.get('name'), fixed_user.name)
+        self.assertEqual(user.get('foobar'), None)
 
     def test_get_include(self):
         users = self.drest.Users.including('location.*').list()
-        self.assertEquals(users[0].location.name, '0')
+        self.assertEqual(users[0].location.name, '0')
 
     def test_get_map(self):
         users = self.drest.Users.map()
         id = self.fixture.users[0].pk
-        self.assertEquals(users[id].id, id)
+        self.assertEqual(users[id].id, id)
 
     def test_get_exclude(self):
         user = self.fixture.users[0]
         users = self.drest.Users.exclude(name=user.name).map()
         self.assertTrue(user.pk not in users)
 
     def test_get_including_related_save(self):
@@ -100,15 +99,15 @@
         location.reload()
         self.assertTrue(_location.name, location.name)
         self.assertTrue(location.name, 'foo')
 
     def test_get_excluding(self):
         users = self.drest.Users.excluding('*').map()
         pk = self.fixture.users[0].pk
-        self.assertEquals(users[pk].id, pk)
+        self.assertEqual(users[pk].id, pk)
 
     def test_update(self):
         user = self.drest.Users.first()
         user.name = 'foo'
         user.save()
         user = self.drest.Users.first()
         self.assertTrue(user.name, 'foo')
@@ -149,40 +148,40 @@
     def test_get_invalid_data(self):
         with self.assertRaises(DoesNotExist):
             self.drest.Users.get('does-not-exist')
 
     def test_extra_pagination(self):
         users = list(self.drest.Users.all().extra(per_page=1))
         users2 = list(self.drest.Users.all())
-        self.assertEquals(users, users2)
+        self.assertEqual(users, users2)
 
         name = users[0].name
         users_named = list(self.drest.Users.extra(name=name))
         self.assertTrue(len(users_named), 1)
         self.assertTrue(users_named[0].name, name)
 
     def test_save_deferred(self):
         user = self.drest.Users.excluding('*').first()
         user.name = 'foo'
         user.save()
 
         user2 = self.drest.Users.filter(name='foo').first()
         self.assertIsNotNone(user2)
-        self.assertEquals(user2.id, user.id)
+        self.assertEqual(user2.id, user.id)
 
     def test_delete(self):
         user = self.drest.Users.first()
         id = user.id
         user.delete()
         self.assertIsNone(user.id)
         self.assertIsNone(self.drest.Users.filter(id=id).first())
 
     def test_sort(self):
         users = self.drest.Users.sort('name').list()
-        self.assertEquals(
+        self.assertEqual(
             users,
             list(sorted(users, key=lambda x: x.name))
         )
 
     def test_mocks(self):
         mock_users = [{
             'id': 1,
@@ -196,8 +195,8 @@
             }
         )
         users = drest.users.list()
         try:
             mus = [u.dict for u in users]
         except AttributeError:
             mus = [u for u in users]
-        self.assertEquals(mus, mock_users)
+        self.assertEqual(mus, mock_users)
```

### Comparing `dynamic-rest-client-0.1.9/tests/test_deepcopy.py` & `dynamic-rest-client-0.2.0/tests/test_deepcopy.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 class DeepcopyTestCase(APITestCase):
     def test_cat(self):
         home = Location(name='Home', blob='ILUVU')
         papa = Cat(name='Papa')
         kitkat = Cat(name='KitKat', home=home, parent=papa)
         kitkat_clone = copy.deepcopy(kitkat)
 
-        self.assertEquals(kitkat.name, kitkat_clone.name)
-        self.assertEquals(kitkat.home.name, kitkat_clone.home.name)
-        self.assertEquals(kitkat.parent.name, kitkat_clone.parent.name)
+        self.assertEqual(kitkat.name, kitkat_clone.name)
+        self.assertEqual(kitkat.home.name, kitkat_clone.home.name)
+        self.assertEqual(kitkat.parent.name, kitkat_clone.parent.name)
```

