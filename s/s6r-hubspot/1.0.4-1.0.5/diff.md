# Comparing `tmp/s6r-hubspot-1.0.4.tar.gz` & `tmp/s6r-hubspot-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s6r-hubspot-1.0.4.tar", last modified: Fri Mar 15 08:51:35 2024, max compression
+gzip compressed data, was "s6r-hubspot-1.0.5.tar", last modified: Mon Apr  8 10:24:15 2024, max compression
```

## Comparing `s6r-hubspot-1.0.4.tar` & `s6r-hubspot-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:35.125976 s6r-hubspot-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-15 08:51:30.000000 s6r-hubspot-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-03-15 08:51:35.125976 s6r-hubspot-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-15 08:51:30.000000 s6r-hubspot-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-15 08:51:30.000000 s6r-hubspot-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 08:51:35.125976 s6r-hubspot-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:35.121976 s6r-hubspot-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:35.121976 s6r-hubspot-1.0.4/src/s6r_hubspot/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-15 08:51:30.000000 s6r-hubspot-1.0.4/src/s6r_hubspot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28230 2024-03-15 08:51:30.000000 s6r-hubspot-1.0.4/src/s6r_hubspot/hubspot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:35.125976 s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-03-15 08:51:35.000000 s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-15 08:51:35.000000 s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 08:51:35.000000 s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-15 08:51:35.000000 s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 08:51:35.000000 s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:35.125976 s6r-hubspot-1.0.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-03-15 08:51:30.000000 s6r-hubspot-1.0.4/src/tests/unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:24:15.421438 s6r-hubspot-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-08 10:24:09.000000 s6r-hubspot-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-08 10:24:15.421438 s6r-hubspot-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 10:24:09.000000 s6r-hubspot-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 10:24:09.000000 s6r-hubspot-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:24:15.421438 s6r-hubspot-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:24:15.417438 s6r-hubspot-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:24:15.421438 s6r-hubspot-1.0.5/src/s6r_hubspot/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 10:24:09.000000 s6r-hubspot-1.0.5/src/s6r_hubspot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35953 2024-04-08 10:24:09.000000 s6r-hubspot-1.0.5/src/s6r_hubspot/hubspot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:24:15.421438 s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-08 10:24:15.000000 s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 10:24:15.000000 s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:24:15.000000 s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 10:24:15.000000 s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 10:24:15.000000 s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:24:15.421438 s6r-hubspot-1.0.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-08 10:24:09.000000 s6r-hubspot-1.0.5/src/tests/unit_test.py
```

### Comparing `s6r-hubspot-1.0.4/LICENSE` & `s6r-hubspot-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s6r-hubspot-1.0.4/PKG-INFO` & `s6r-hubspot-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s6r-hubspot
-Version: 1.0.4
+Version: 1.0.5
 Summary: Hubspot API client
 Author-email: Michel Perrocheau <michel@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -197,33 +197,36 @@
 ```python
 from s6r_hubspot import HubspotConnection
 
 hubspot = HubspotConnection('your_access_token')
 owners = hubspot.get_owners()
 ```
 
+
+### Unit tests
+
+To run unit_test file, you need to set up a token of an empty hubspot base in an environnement variable name 
+HUBSPOT_TOKEN:
+```bash
+    export HUBSPOT_TOKEN='your_token'
+```
+
+
 ## License
 
 This project is licensed under the [GNU Lesser General Public License (LGPL) Version 3](https://www.gnu.org/licenses/lgpl-3.0.html).
 
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements,
 please open an issue or submit a pull request.
 
 - GitHub Repository: [ScalizerOrg/s6r-hubspot](https://github.com/ScalizerOrg/s6r-hubspot)
 
-### Unit test
-
-To run unit_test file, you need to set up a token of an empty hubspot base in an environnement variable name 
-HUBSPOT_TOKEN:
-```bash
-    export HUBSPOT_TOKEN='your_token'
-```
 
 ## Contributors
 
 * David Halgand - [GitHub](https://github.com/halgandd)
 * Morgane Goujon - [GitHub](https://github.com/MorganeGoujon)
 * Khalid Bentaleb - [GitHub](https://github.com/kbentaleb)
 * Michel Perrocheau - [GitHub](https://github.com/myrrkel)
```

### Comparing `s6r-hubspot-1.0.4/README.md` & `s6r-hubspot-1.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,33 +11,36 @@
 ```python
 from s6r_hubspot import HubspotConnection
 
 hubspot = HubspotConnection('your_access_token')
 owners = hubspot.get_owners()
 ```
 
+
+### Unit tests
+
+To run unit_test file, you need to set up a token of an empty hubspot base in an environnement variable name 
+HUBSPOT_TOKEN:
+```bash
+    export HUBSPOT_TOKEN='your_token'
+```
+
+
 ## License
 
 This project is licensed under the [GNU Lesser General Public License (LGPL) Version 3](https://www.gnu.org/licenses/lgpl-3.0.html).
 
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements,
 please open an issue or submit a pull request.
 
 - GitHub Repository: [ScalizerOrg/s6r-hubspot](https://github.com/ScalizerOrg/s6r-hubspot)
 
-### Unit test
-
-To run unit_test file, you need to set up a token of an empty hubspot base in an environnement variable name 
-HUBSPOT_TOKEN:
-```bash
-    export HUBSPOT_TOKEN='your_token'
-```
 
 ## Contributors
 
 * David Halgand - [GitHub](https://github.com/halgandd)
 * Morgane Goujon - [GitHub](https://github.com/MorganeGoujon)
 * Khalid Bentaleb - [GitHub](https://github.com/kbentaleb)
 * Michel Perrocheau - [GitHub](https://github.com/myrrkel)
```

### Comparing `s6r-hubspot-1.0.4/pyproject.toml` & `s6r-hubspot-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s6r-hubspot"
-version = "1.0.4"
+version = "1.0.5"
 description = "Hubspot API client"
 readme = "README.md"
 authors = [{ name = "Michel Perrocheau", email = "michel@scalizer.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
```

### Comparing `s6r-hubspot-1.0.4/src/s6r_hubspot/hubspot.py` & `s6r-hubspot-1.0.5/src/s6r_hubspot/hubspot.py`

 * *Files 21% similar despite different names*

```diff
@@ -71,14 +71,24 @@
         set header to connect to Hubspot api
         """
         self._headers = {
             "Authorization": "Bearer %s" % (self._token,),
             "content-type": "application/json"
         }
 
+    def get_limit_error(self, data):
+        condition =  (
+            'errorType' in data and
+            data['errorType'] == 'RATE_LIMIT' and
+            data['message'] != 'You have reached your daily limit.'
+        )
+        if condition:
+            return True
+        return False
+
     def retrieve(self, model, params={}, limit=100, after=0, cc=0):
 
         url = '%s/crm/v3/objects/%s' % (self._url, model)
         params['limit'] = limit
         if after != '{}':
             params['after'] = after
         data = requests.get(url, params=params, headers=self._headers).json()
@@ -106,15 +116,15 @@
             if data['status'] == 'COMPLETE':
                 result += data['results']
             else:
                 self.logger.error(data['message'])
                 if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                     self._renew_token()
                     return self.create(model, vals_list)
-                elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+                elif self.get_limit_error(data):
                     time.sleep(1.5)
                     data = requests.post(url, data=json.dumps(params), headers=self._headers).json()
                     if data['status'] == 'COMPLETE':
                         result += data['results']
                 else:
                     raise Exception(data['message'])
         return result
@@ -148,15 +158,15 @@
             if data['status'] == 'COMPLETE':
                 result += data['results']
             else:
                 self.logger.error(data['message'])
                 if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                     self._renew_token()
                     return self.update(model, vals_list)
-                elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+                elif self.get_limit_error(data):
                     time.sleep(1.5)
                     data = requests.post(url, data=json.dumps(params), headers=self._headers).json()
                     if data['status'] == 'COMPLETE':
                         result += data['results']
                 else:
                     raise Exception(data['message'])
         return result
@@ -176,38 +186,63 @@
         if properties:
             params["properties"] = properties
         url = "%s/crm/v3/objects/%s/search" % (self._url, model)
         data = requests.post(url, data=json.dumps(params), headers=self._headers).json()
         if ('status' in data and data['status'] == 'COMPLETE') or ('total' in data):
             results += data['results']
             after = data.get('paging', {}).get('next', {}).get('after', {})
-            if after:
-                return self.search(model, filters=filters, after=after, cc=cc + 1, properties=properties, associations=associations, results=results)
+            # The condition "cc < 5" is added to avoid the timeout exceed
+            # of "real_time_limit" parameter in odoo.sh which is 15 minutes
+            if after and cc < 5:
+                return self.search(
+                    model,
+                    filters=filters,
+                    after=after,
+                    cc=cc + 1,
+                    properties=properties,
+                    associations=associations,
+                    results=results
+                )
         else:
             self.logger.error(data['message'])
             if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
-                return self.search(model, filters=filters, after=after, cc=cc, properties=properties, associations=associations, results=results)
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+                return self.search(
+                    model,
+                    filters=filters,
+                    after=after,
+                    cc=cc,
+                    properties=properties,
+                    associations=associations,
+                    results=results)
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
-                return self.search(model, filters=filters, after=after, cc=cc, properties=properties,
-                                   associations=associations, results=results)
+                return self.search(
+                    model,
+                    filters=filters,
+                    after=after,
+                    cc=cc,
+                    properties=properties,
+                    associations=associations,
+                    results=results
+                )
             else:
                 raise Exception(data['message'])
         association_result = {}
         for association in associations:
-            association_result[association] = {i['from']['id']: i for i in
-                                               self.get_association(model, association, [i['id'] for i in results])}
+            association_result[association] = {
+                i['from']['id']: i for i in self.get_association(model, association, [i['id'] for i in results])
+            }
         for result in results:
             for association in associations:
                 if result['id'] in association_result[association]:
-                    result["_%s" % association] = [{'id': i['toObjectId'],
-                                                    'label': [i['associationTypes'][j]['label'] for j in
-                                                              range(len(i['associationTypes']))]}
-                                                   for i in association_result[association][result['id']]['to']]
+                    result["_%s" % association] = [{
+                        'id': i['toObjectId'],
+                        'label': [i['associationTypes'][j]['label'] for j in range(len(i['associationTypes']))]
+                    } for i in association_result[association][result['id']]['to']]
         if load_associations:
             results = self._load_associations_properties(associations, results)
         return results
 
     def _load_associations_properties(self, associations, results):
         for association in associations:
             ids = []
@@ -255,15 +290,15 @@
             if after:
                 return self.get_association(model_from, model_to, ids, after=after, cc=cc + 1, results=results)
         else:
             self.logger.error(data['message'])
             if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
                 return self.get_association(model_from, model_to, ids, after=after, cc=cc, results=results)
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
                 return self.get_association(model_from, model_to, ids, after=after, cc=cc, results=results)
             else:
                 raise Exception(data['message'])
         return results
 
     # TODO : deux reads différents à uniformiser
@@ -300,64 +335,95 @@
             data = requests.post(url, data=json.dumps(params), headers=self._headers).json()
             if data['status'] == 'COMPLETE':
                 results += data['results']
             else:
                 self.logger.error(data['message'])
                 if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                     self._renew_token()
-                    return self.read(model, ids, properties, associations=associations,
-                                     propertiesWithHistory=propertiesWithHistory,  props_name=props_name, after=after, cc=cc)
-                elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+                    return self.read(
+                        model,
+                        ids,
+                        properties,
+                        associations=associations,
+                        propertiesWithHistory=propertiesWithHistory,
+                        props_name=props_name,
+                        after=after,
+                        cc=cc
+                    )
+                elif self.get_limit_error(data):
                     time.sleep(1.5)
                     data = requests.post(url, data=json.dumps(params), headers=self._headers).json()
                     if data['status'] == 'COMPLETE':
                         results += data['results']
                 else:
                     raise Exception(data['message'])
         association_result = {}
         for association in associations:
             association_result[association] = {i['from']['id']: i for i in
                                                self.get_association(model, association, [i['id'] for i in results])}
         for result in results:
             for association in associations:
                 if result['id'] in association_result[association]:
-                    result["_%s" % (association)] = [{'id': i['toObjectId'],
-                                                      'label': [i['associationTypes'][j]['label'] for j in range(len(i['associationTypes']))]}
-                                                     for i in association_result[association][result['id']]['to']]
+                    result["_%s" % (association)] = [{
+                        'id': i['toObjectId'],
+                        'label': [i['associationTypes'][j]['label'] for j in range(len(i['associationTypes']))]
+                    } for i in association_result[association][result['id']]['to']]
         return results
 
     def get_all(self, model, properties, associations=[], after=0, cc=0, results=[]):
         results = []
         url = "%s/crm/v3/objects/%s?limit=100&after=%s&properties=%s" % (self._url, model, after, ','.join(properties))
         data = requests.get(url, headers=self._headers).json()
         if 'results' in data:
             results += data['results']
             association_result = {}
             for association in associations:
-                association_result[association] = {i['from']['id']: i for i in
-                                                   self.get_association(model, association, [i['id'] for i in results])}
+                association_result[association] = {
+                    i['from']['id']: i for i in
+                    self.get_association(model, association, [i['id'] for i in results])
+                }
             for result in results:
                 for association in associations:
                     if result['id'] in association_result[association]:
-                        result["_%s" % (association)] = [{'id': i['toObjectId'],
-                                                          'label': [i['associationTypes'][j]['label'] for j in
-                                                                    range(len(i['associationTypes']))]}
-                                                         for i in association_result[association][result['id']]['to']]
+                        result["_%s" % (association)] = [{
+                            'id': i['toObjectId'],
+                            'label': [i['associationTypes'][j]['label'] for j in range(len(i['associationTypes']))]
+                        } for i in association_result[association][result['id']]['to']]
             after = data.get('paging', {}).get('next', {}).get('after', {})
             if after:
-                return self.get_all(model, properties, associations=associations, after=after, cc=cc + 1, results=results)
+                return self.get_all(
+                    model,
+                    properties,
+                    associations=associations,
+                    after=after,
+                    cc=cc + 1,
+                    results=results
+                )
         else:
             self.logger.error(data['message'])
             if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
-                return results + self.get_all(model=model, properties=properties, associations=associations, after=after, cc=cc, results=results)
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+                return results + self.get_all(
+                    model=model,
+                    properties=properties,
+                    associations=associations,
+                    after=after,
+                    cc=cc,
+                    results=results
+                )
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
-                return self.get_all(model=model, properties=properties, associations=associations,
-                                                  after=after, cc=cc, results=results)
+                return self.get_all(
+                    model=model,
+                    properties=properties,
+                    associations=associations,
+                    after=after,
+                    cc=cc,
+                    results=results
+                )
             else:
                 raise Exception(data['message'])
         return results
 
     def archive(self, model, ids):
         """
         archive object in hubspot identify by model and ids
@@ -425,15 +491,17 @@
         if 'status' not in result:
             return result
         else:
             self.logger.error(result['message'])
             if result['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
                 return self.get_owner(owner_id)
-            elif 'errorType' in result and result['errorType'] == 'RATE_LIMIT' and result['message'] != 'You have reached your daily limit.':
+            elif ('errorType' in result and
+                  result['errorType'] == 'RATE_LIMIT' and
+                  result['message'] != 'You have reached your daily limit.'):
                 time.sleep(1.5)
                 return self.get_owner(owner_id)
             else:
                 raise Exception(result['message'])
 
     def get_owners(self):
         """
@@ -444,15 +512,15 @@
         if 'status' not in data:
             return data['results']
         else:
             self.logger.error(data['message'])
             if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
                 return self.get_owners()
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
                 return self.get_owners()
             else:
                 raise Exception(data['message'])
 
     def create_association(self, model_from, model_to, vals):
         """
@@ -483,15 +551,15 @@
             if data['status'] == 'COMPLETE':
                 result.append(data)
             else:
                 self.logger.error(data['message'])
                 if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                     self._renew_token()
                     return self.create_association(model_from, model_to, split_val_list)
-                elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+                elif self.get_limit_error(data):
                     time.sleep(1.5)
                     data = requests.post(url, data=json.dumps(params), headers=self._headers).json()
                     if data['status'] == 'COMPLETE':
                         result.append(data)
                 else:
                     raise Exception(data['message'])
         return result
@@ -506,15 +574,15 @@
         url = "%s/crm/v3/pipelines/%s/%s/stages/%s" % (self._url, model, pipeline_id, stage_id)
         data = requests.get(url, headers=self._headers).json()
         if 'status' in data:
             self.logger.error(data['message'])
             if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
                 return self.get_stage(model, pipeline_id, stage_id)
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
                 return self.get_stage(model, pipeline_id, stage_id)
             else:
                 raise Exception(data['message'])
         else:
             return data
 
@@ -527,15 +595,15 @@
         url = "%s/crm/v3/pipelines/%s/%s" % (self._url, model, pipeline_id)
         data = requests.get(url, headers=self._headers).json()
         if 'status' in data:
             self.logger.error(data['message'])
             if 'category' in data and data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
                 return self.get_stage(model, pipeline_id)
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
                 return self.get_stage(model, pipeline_id)
             else:
                 raise Exception(data['message'])
         else:
             return data
 
@@ -548,15 +616,15 @@
         if 'status' not in data:
             return data
         else:
             self.logger.error(data['message'])
             if data['category'] == 'EXPIRED_AUTHENTICATION':
                 self._renew_token()
                 return self.get_association_label()
-            elif 'errorType' in data and data['errorType'] == 'RATE_LIMIT' and data['message'] != 'You have reached your daily limit.':
+            elif self.get_limit_error(data):
                 time.sleep(1.5)
                 return self.get_association_label()
             else:
                 raise Exception(data['message'])
 
     def delete_notes(self, note_id):
         url = "%s/crm/v3/objects/notes/%s" % (self._url, note_id)
@@ -617,17 +685,216 @@
         params = {
             'folderId': folder_id,
             'options': options,
             'fileName': name,
         }
         headers = {
             "authorization": "Bearer %s" % (self._token,)
-            }
+        }
 
         hubspot_data = requests.post(url, files=files, data=params, headers=headers)
         return json.loads(hubspot_data.text)
 
     def retrieve_owner(self, user_id):
         url = "%s/crm/v3/owners/%s" % (self._url, user_id)
         params = {}
         data = requests.get(url, params=params, headers=self._headers).json()
         return data
+
+    def get_hub_db(self):
+        """
+        method call to get all hubdb tables
+        """
+        url = "%s/hubdb/api/v2/tables" % (self._url)
+        response = requests.get(url, headers=self._headers)
+        if response.status_code in [200, 201]:
+            data = response.json()
+            return data.get('objects', [])
+        return response
+
+    def delete_hub_db(self, table_id, row_id):
+        """
+        :param table_id: HubDB table ID
+        :param row_id: Row ID
+        :return: Delete the row in the hubdb table
+        """
+        url = "%s/cms/v3/hubdb/tables/%s/rows/%s/draft" % (self._url, table_id, row_id)
+        response = requests.delete(url, headers=self._headers)
+        if response.status_code == 204:
+            return 'The row ID %s has been deleted successfully from the table %s' % (row_id, table_id)
+        return response
+
+    def update_hub_db(self, table_id, row_id, params):
+        """
+        Method calls to update a specific row in the HubDB table
+        :param table_id: HubDB table ID
+        :param row_id: Row ID
+        :param row: dict of values to update
+        """
+        url = "%s/cms/v3/hubdb/tables/%s/rows/%s/draft" % (self._url, table_id, row_id)
+        response = requests.patch(url, data=json.dumps(params), headers=self._headers)
+
+        if response.status_code in [200, 201]:
+            data = response.json()
+            return 'The data has been updated successfully \n %s' % (data,)
+        else:
+            _logger.info("Failed to Update row: {} on table: {}. Status code: {}, Response: {}".format(
+                row_id,
+                table_id,
+                response.status_code,
+                response.content
+            ))
+        return True
+
+    def publish_hub_db(self, table_id):
+        """
+        Method calls to publish hubdb data after update/create
+        :param table_id: The Id of table to publish
+        :return: Hubdb table data published
+        """
+        url = "%s/cms/v3/hubdb/tables/%s/draft/publish" % (self._url, table_id)
+        response = requests.post(url, data=json.dumps({}), headers=self._headers)
+        if response.status_code in [200, 201]:
+            _logger.info("Draft table {} published successfully.".format(table_id))
+        else:
+            _logger.info("Failed to publish draft table. Status code: {}, Response: {}".format(
+                response.status_code,
+                response.text
+            ))
+        return True
+
+    def create_hub_db(self, table_id, params):
+        """
+        Method call to create new row in the HubDB table on Hubspot
+        :param table_id: string Id of table pn hubspot
+        :param params: Dict of values
+        """
+        url = "%s/cms/v3/hubdb/tables/%s/rows" % (self._url, table_id)
+        response = requests.post(url, data=json.dumps(params), headers=self._headers)
+        if response.status_code in [200, 201]:
+            return response.json()
+        else:
+            _logger.info("Failed to Create product on table: {}. Status code: {}, Response: {}".format(
+                table_id,
+                response.status_code,
+                response.json()
+            ))
+
+        return False
+
+    def create_table_hub_db(self, label, name):
+        """
+        Method calls to create a new HubDB table
+        :param label: string table label
+        :param name: string table name
+        :return:
+        """
+        params = {
+            "name": name,
+            "label": label,
+        }
+        url = "%s/hubdb/api/v2/tables" % (self._url)
+        response = requests.post(url, data=json.dumps(params), headers=self._headers)
+        if response.status_code in [200, 201]:
+            return response.json()
+        return False
+
+    def update_table_hub_db(self, table_id, label, name, columns):
+        """
+        Method calls to add new columns to the HubDB table
+        :param table_id: string id of table
+        :param label: string table label
+        :param name: string the table name
+        :param columns: list of columns names
+        :return:
+        """
+        params = {
+            "name": name,
+            "label": label,
+        }
+        if columns:
+            params['columns'] = columns
+        url = "%s/hubdb/api/v2/tables/%s" % (self._url, table_id)
+        response = requests.put(url, data=json.dumps(params), headers=self._headers)
+        if response.status_code in [200, 201]:
+            return response.json()
+        return False
+
+    def fetch_all_draft_rows(self, table_id):
+        """
+        Fetch all rows from the draft version of a HubDB table.
+        :param table_id: ID of the HubDB table.
+        :return: List of row IDs.
+        """
+        url = f"%s/cms/v3/hubdb/tables/%s/rows/draft" % (self._url, table_id)
+        response = requests.get(url, headers=self._headers)
+        if response.status_code == 200:
+            data = response.json()
+            rows = data.get('results', [])
+            return [row['id'] for row in rows]
+        else:
+            print(f"Failed to fetch rows. Response: {response.text}")
+            return []
+
+    def delete_all_draft_rows(self, table_id):
+        """
+        Delete all rows a HubDB table.
+        :param table_id: string ID of the HubDB table.
+        """
+        row_ids = self.fetch_all_draft_rows(table_id)
+        for row_id in row_ids:
+            self.delete_hub_db(table_id, row_id)
+        return True
+
+    def import_file(self, model, datas, keys):
+        """
+        Method call to import a csv file into an object
+        :param model: string, hubspot object ID
+        :param datas: list of dict that contains the lines of the csv file
+        :param keys: list of tuple that contains the (variable_name, variable label)
+        :return:
+        """
+        name = "%s_%s" % (model, datetime.datetime.now().strftime('%Y%m%d_%H%M'))
+        filename = "%s.csv" % (name)
+        params = {
+            "name": name,
+            "files": [{
+                "fileName": filename,
+                "importOperations": {
+                    "0-1": "UPDATE"
+                },
+                "fileFormat": "CSV",
+                "fileImportPage": {
+                    "hasHeader": True,
+                    "columnMappings": [{
+                        "ignored": False,
+                        "columnName": j,
+                        "idColumnType": 'HUBSPOT_ALTERNATE_ID' if i == 'id_odoo' else None,
+                        "propertyName": i,
+                        "foreignKeyType": None,
+                        "columnObjectTypeId": model,
+                        "associationIdentifiedColumn": False
+                        } for i,j in keys
+                    ]
+                }
+            }]
+        }
+
+        with open('/tmp/%s'%(filename),'w', newline='') as csvfile:
+            fieldnames = [i for i,j in keys]
+            writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
+            writer.writeheader()
+            for data in datas:
+                writer.writerow(data)
+
+        files = {
+            'importRequest': (None, json.dumps(params), 'application/json'),
+            'files': open('/tmp/%s'%(filename), 'rb')
+        }
+        url = "%s/crm/v3/imports" % (self._url)
+        response = requests.post(url, headers=self._headers_import, files=files)
+        if response.status_code == 200:
+            data = response.json()
+            return data
+        else:
+            _logger.info(f"Failed to fetch rows. Response: %s", response.text)
+            return []
```

### Comparing `s6r-hubspot-1.0.4/src/s6r_hubspot.egg-info/PKG-INFO` & `s6r-hubspot-1.0.5/src/s6r_hubspot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s6r-hubspot
-Version: 1.0.4
+Version: 1.0.5
 Summary: Hubspot API client
 Author-email: Michel Perrocheau <michel@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -197,33 +197,36 @@
 ```python
 from s6r_hubspot import HubspotConnection
 
 hubspot = HubspotConnection('your_access_token')
 owners = hubspot.get_owners()
 ```
 
+
+### Unit tests
+
+To run unit_test file, you need to set up a token of an empty hubspot base in an environnement variable name 
+HUBSPOT_TOKEN:
+```bash
+    export HUBSPOT_TOKEN='your_token'
+```
+
+
 ## License
 
 This project is licensed under the [GNU Lesser General Public License (LGPL) Version 3](https://www.gnu.org/licenses/lgpl-3.0.html).
 
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements,
 please open an issue or submit a pull request.
 
 - GitHub Repository: [ScalizerOrg/s6r-hubspot](https://github.com/ScalizerOrg/s6r-hubspot)
 
-### Unit test
-
-To run unit_test file, you need to set up a token of an empty hubspot base in an environnement variable name 
-HUBSPOT_TOKEN:
-```bash
-    export HUBSPOT_TOKEN='your_token'
-```
 
 ## Contributors
 
 * David Halgand - [GitHub](https://github.com/halgandd)
 * Morgane Goujon - [GitHub](https://github.com/MorganeGoujon)
 * Khalid Bentaleb - [GitHub](https://github.com/kbentaleb)
 * Michel Perrocheau - [GitHub](https://github.com/myrrkel)
```

### Comparing `s6r-hubspot-1.0.4/src/tests/unit_test.py` & `s6r-hubspot-1.0.5/src/tests/unit_test.py`

 * *Files identical despite different names*

