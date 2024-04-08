# Comparing `tmp/ccs-digitalmarketplace-test-utils-4.3.2.tar.gz` & `tmp/ccs-digitalmarketplace-test-utils-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-test-utils-4.3.2.tar", last modified: Wed Mar 27 11:41:49 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-test-utils-4.4.0.tar", last modified: Mon Apr  8 13:19:06 2024, max compression
```

## Comparing `ccs-digitalmarketplace-test-utils-4.3.2.tar` & `ccs-digitalmarketplace-test-utils-4.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:41:49.212865 ccs-digitalmarketplace-test-utils-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-27 11:41:49.212865 ccs-digitalmarketplace-test-utils-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:41:49.208865 ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-27 11:41:49.000000 ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-27 11:41:49.000000 ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:41:49.000000 ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-27 11:41:49.000000 ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 11:41:49.000000 ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:41:49.208865 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:41:49.212865 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/audit_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/brief.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/brief_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/framework_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/lot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/supplier_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 11:41:49.212865 ccs-digitalmarketplace-test-utils-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-27 11:41:32.000000 ccs-digitalmarketplace-test-utils-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.325380 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.325380 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/audit_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/lot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/setup.py
```

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/LICENCE` & `ccs-digitalmarketplace-test-utils-4.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/README.md` & `ccs-digitalmarketplace-test-utils-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/__init__.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .base import BaseAPIModelStub
 from .audit_event import AuditEventStub
 from .brief import BriefStub
 from .brief_response import BriefResponseStub
-from .communication import CommunicationStub
+from .communication import CommunicationStub, CommunicationMessageStub
 from .framework import FrameworkStub
 from .framework_agreement import FrameworkAgreementStub
 from .lot import LotStub, as_a_service_lots, cloud_lots, dos_lots
 from .services import ArchivedServiceStub, DraftServiceStub, ServiceStub
 from .supplier import SupplierStub
 from .supplier_framework import SupplierFrameworkStub
```

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/audit_event.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/audit_event.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/base.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/base.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/brief.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/brief_response.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief_response.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/communication.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/communication.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from datetime import datetime, timedelta
 
 from .base import BaseAPIModelStub
 
 
 DATETIME_FORMAT = '%Y-%m-%dT%H:%M:%S.%fZ'
+DEFAULT_TIME = datetime(2024, 3, 14, 14, 30)
 
 
 class CommunicationStub(BaseAPIModelStub):
     resource_name = 'communications'
 
     admin_user = {
         'id': 123,
         'email': 'test+123@digital.cabinet-office.gov.uk'
     }
     supplier_user = {
         'id': 456,
         'email': 'test+456@digital.gov.uk'
     }
-    default_time = datetime(2024, 3, 14, 14, 30)
     default_data = {
         'id': 1234,
         'subject': 'Communication Subject',
         'supplierId': 1234,
         'supplierName': "My Little Company",
         'frameworkSlug': 'g-cloud-14',
         'frameworkFramework': 'g-cloud',
         'frameworkFamily': 'g-cloud',
         'frameworkName': 'G-Cloud 14',
         'frameworkStatus': 'pending',
-        'createdAt': default_time.strftime(DATETIME_FORMAT),
-        'updatedAt': default_time.strftime(DATETIME_FORMAT),
+        'createdAt': DEFAULT_TIME.strftime(DATETIME_FORMAT),
+        'updatedAt': DEFAULT_TIME.strftime(DATETIME_FORMAT),
         'links': {},
         'messages': [],
     }
     optional_keys = [
         ('supplierName', 'supplier_name'),
     ]
 
@@ -46,56 +46,86 @@
                 'archivedByUserId': self.admin_user["id"]
             })
 
         message_data = {
             'id': int(f"{self.response_data['id']}1"),
             'communicationId': self.response_data["id"],
             'text': 'This is the communication message sent by CCS',
-            'sentAt': self.default_time.strftime(DATETIME_FORMAT),
+            'sentAt': DEFAULT_TIME.strftime(DATETIME_FORMAT),
             'sentByUserId': self.admin_user["id"],
             'sentByUserEmail': self.admin_user["email"],
             'target': 'for_supplier',
         }
 
         message_data['attachments'] = [
             {"id": int(f"{message_data['id']}{index + 1}")} | attachment
             for index, attachment in enumerate(kwargs.get('attachments', []))
         ]
 
         if kwargs.get('read') or kwargs.get('last_message_target', 'for_admin') == 'for_admin':
             message_data.update(**{
                 'readAt': (
-                    self.default_time
+                    DEFAULT_TIME
                     + timedelta(minutes=self.response_data['id'])
                 ).strftime(DATETIME_FORMAT),
                 'readByUserId': self.supplier_user["id"],
                 'readByUserEmail': self.supplier_user["email"]
             })
 
         self.response_data['messages'].append(message_data)
 
         if kwargs.get('last_message_target', 'for_admin') == 'for_admin':
             message_data = {
                 'id': int(f"{self.response_data['id']}2"),
                 'communicationId': self.response_data["id"],
                 'text': 'This is the communication message sent by Supplier',
                 'sentAt': (
-                    self.default_time
+                    DEFAULT_TIME
                     + timedelta(days=self.response_data['id'])
                 ).strftime(DATETIME_FORMAT),
                 'sentByUserId': self.supplier_user["id"],
                 'sentByUserEmail': self.supplier_user["email"],
                 'target': 'for_admin',
                 'attachments': []
             }
 
             if kwargs.get('read'):
                 message_data.update(**{
                     'readAt': (
-                        self.default_time
+                        DEFAULT_TIME
                         + timedelta(days=self.response_data['id'], minutes=self.response_data['id'])
                     ).strftime(DATETIME_FORMAT),
                     'readByUserId': self.admin_user["id"],
                     'readByUserEmail': self.admin_user["email"]
                 })
 
             self.response_data['messages'].append(message_data)
+
+
+class CommunicationMessageStub(BaseAPIModelStub):
+    resource_name = 'communicationMessages'
+
+    default_data = {
+        'id': 1231,
+        'communicationId': 123,
+        'text': 'This is the communication message',
+        'sentAt': DEFAULT_TIME.strftime(DATETIME_FORMAT),
+        'sentByUserId': 123,
+        'sentByUserEmail': 'test+123@digital.cabinet-office.gov.uk',
+        'target': 'for_supplier',
+    }
+    optional_keys = [
+        ('communicationId', 'communication_id'),
+        ('sentAt', 'sent_at'),
+        ('sentByUserId', 'sent_by_user_id'),
+        ('sentByUserEmail', 'sent_by_user_email'),
+        ('readAt', 'read_at'),
+        ('readByUserId', 'read_by_user_id'),
+        ('readByUserEmail', 'read_by_user_email'),
+    ]
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.response_data.update(attachments=[
+            {"id": int(f"{self.response_data['id']}{index + 1}")} | attachment
+            for index, attachment in enumerate(kwargs.get('attachments', []))
+        ])
```

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/framework.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/framework_agreement.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework_agreement.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/lot.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/lot.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/services.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/services.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/supplier.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/api_model_stubs/supplier_framework.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier_framework.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/comparisons.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/comparisons.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/fixtures.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/fixtures.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/login.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/login.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/dmtestutils/mocking.py` & `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/mocking.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.3.2/setup.py` & `ccs-digitalmarketplace-test-utils-4.4.0/setup.py`

 * *Files identical despite different names*

