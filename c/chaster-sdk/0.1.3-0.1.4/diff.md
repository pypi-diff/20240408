# Comparing `tmp/chaster-sdk-0.1.3.tar.gz` & `tmp/chaster-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaster-sdk-0.1.3.tar", last modified: Sun Mar 31 16:28:52 2024, max compression
+gzip compressed data, was "chaster-sdk-0.1.4.tar", last modified: Mon Apr  8 01:24:04 2024, max compression
```

## Comparing `chaster-sdk-0.1.3.tar` & `chaster-sdk-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-03-31 16:28:52.714543 chaster-sdk-0.1.3/
--rwxrwxrwx   0 max       (1000) max       (1000)    11357 2023-12-26 18:30:11.000000 chaster-sdk-0.1.3/LICENSE
--rwxrwxrwx   0 max       (1000) max       (1000)     1092 2024-03-31 16:28:52.699544 chaster-sdk-0.1.3/PKG-INFO
--rwxrwxrwx   0 max       (1000) max       (1000)      534 2024-02-02 18:04:23.000000 chaster-sdk-0.1.3/README.md
--rwxrwxrwx   0 max       (1000) max       (1000)      682 2024-03-31 16:28:16.000000 chaster-sdk-0.1.3/pyproject.toml
--rwxrwxrwx   0 max       (1000) max       (1000)       38 2024-03-31 16:28:52.714543 chaster-sdk-0.1.3/setup.cfg
-drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-03-31 16:28:52.125322 chaster-sdk-0.1.3/src/
-drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-03-31 16:28:52.516087 chaster-sdk-0.1.3/src/chaster/
--rwxrwxrwx   0 max       (1000) max       (1000)        0 2024-01-23 17:43:23.000000 chaster-sdk-0.1.3/src/chaster/__init__.py
--rwxrwxrwx   0 max       (1000) max       (1000)    50391 2024-02-17 17:14:33.000000 chaster-sdk-0.1.3/src/chaster/api.py
--rwxrwxrwx   0 max       (1000) max       (1000)     3496 2024-02-10 05:22:28.000000 chaster-sdk-0.1.3/src/chaster/conversation.py
--rwxrwxrwx   0 max       (1000) max       (1000)    22424 2024-02-10 05:22:28.000000 chaster-sdk-0.1.3/src/chaster/extensions.py
--rwxrwxrwx   0 max       (1000) max       (1000)    23045 2024-03-07 22:34:09.000000 chaster-sdk-0.1.3/src/chaster/lock.py
--rwxrwxrwx   0 max       (1000) max       (1000)       89 2024-02-10 05:22:28.000000 chaster-sdk-0.1.3/src/chaster/setup.py
--rwxrwxrwx   0 max       (1000) max       (1000)     5310 2024-02-10 05:22:28.000000 chaster-sdk-0.1.3/src/chaster/triggers.py
--rwxrwxrwx   0 max       (1000) max       (1000)    18012 2024-02-10 05:22:28.000000 chaster-sdk-0.1.3/src/chaster/user.py
--rwxrwxrwx   0 max       (1000) max       (1000)      848 2024-01-23 17:43:23.000000 chaster-sdk-0.1.3/src/chaster/util.py
-drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-03-31 16:28:52.699544 chaster-sdk-0.1.3/src/chaster_sdk.egg-info/
--rwxrwxrwx   0 max       (1000) max       (1000)     1092 2024-03-31 16:28:51.000000 chaster-sdk-0.1.3/src/chaster_sdk.egg-info/PKG-INFO
--rwxrwxrwx   0 max       (1000) max       (1000)      507 2024-03-31 16:28:52.000000 chaster-sdk-0.1.3/src/chaster_sdk.egg-info/SOURCES.txt
--rwxrwxrwx   0 max       (1000) max       (1000)        1 2024-03-31 16:28:51.000000 chaster-sdk-0.1.3/src/chaster_sdk.egg-info/dependency_links.txt
--rwxrwxrwx   0 max       (1000) max       (1000)       25 2024-03-31 16:28:51.000000 chaster-sdk-0.1.3/src/chaster_sdk.egg-info/requires.txt
--rwxrwxrwx   0 max       (1000) max       (1000)        8 2024-03-31 16:28:51.000000 chaster-sdk-0.1.3/src/chaster_sdk.egg-info/top_level.txt
-drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-03-31 16:28:52.669539 chaster-sdk-0.1.3/tests/
--rwxrwxrwx   0 max       (1000) max       (1000)    27513 2024-02-17 17:14:33.000000 chaster-sdk-0.1.3/tests/test_api_integration.py
--rwxrwxrwx   0 max       (1000) max       (1000)    27822 2024-03-07 22:34:09.000000 chaster-sdk-0.1.3/tests/test_api_mock_chaster.py
--rwxrwxrwx   0 max       (1000) max       (1000)     8961 2024-01-23 17:43:23.000000 chaster-sdk-0.1.3/tests/test_dto.py
+drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-04-08 01:24:04.424689 chaster-sdk-0.1.4/
+-rwxrwxrwx   0 max       (1000) max       (1000)    11357 2023-12-26 18:30:11.000000 chaster-sdk-0.1.4/LICENSE
+-rwxrwxrwx   0 max       (1000) max       (1000)     1092 2024-04-08 01:24:04.408640 chaster-sdk-0.1.4/PKG-INFO
+-rwxrwxrwx   0 max       (1000) max       (1000)      534 2024-02-02 18:04:23.000000 chaster-sdk-0.1.4/README.md
+-rwxrwxrwx   0 max       (1000) max       (1000)      682 2024-04-08 01:23:39.000000 chaster-sdk-0.1.4/pyproject.toml
+-rwxrwxrwx   0 max       (1000) max       (1000)       38 2024-04-08 01:24:04.426686 chaster-sdk-0.1.4/setup.cfg
+drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-04-08 01:24:03.644572 chaster-sdk-0.1.4/src/
+drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-04-08 01:24:04.045079 chaster-sdk-0.1.4/src/chaster/
+-rwxrwxrwx   0 max       (1000) max       (1000)        0 2024-01-23 17:43:23.000000 chaster-sdk-0.1.4/src/chaster/__init__.py
+-rwxrwxrwx   0 max       (1000) max       (1000)    50786 2024-04-06 18:22:36.000000 chaster-sdk-0.1.4/src/chaster/api.py
+-rwxrwxrwx   0 max       (1000) max       (1000)     3516 2024-04-06 03:10:46.000000 chaster-sdk-0.1.4/src/chaster/conversation.py
+-rwxrwxrwx   0 max       (1000) max       (1000)    22607 2024-04-07 00:26:50.000000 chaster-sdk-0.1.4/src/chaster/extensions.py
+-rwxrwxrwx   0 max       (1000) max       (1000)    23239 2024-04-08 01:22:01.000000 chaster-sdk-0.1.4/src/chaster/lock.py
+-rwxrwxrwx   0 max       (1000) max       (1000)       89 2024-02-10 05:22:28.000000 chaster-sdk-0.1.4/src/chaster/setup.py
+-rwxrwxrwx   0 max       (1000) max       (1000)     5315 2024-04-06 03:10:46.000000 chaster-sdk-0.1.4/src/chaster/triggers.py
+-rwxrwxrwx   0 max       (1000) max       (1000)    18072 2024-04-06 03:10:46.000000 chaster-sdk-0.1.4/src/chaster/user.py
+-rwxrwxrwx   0 max       (1000) max       (1000)      853 2024-04-06 03:10:46.000000 chaster-sdk-0.1.4/src/chaster/util.py
+drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-04-08 01:24:04.390352 chaster-sdk-0.1.4/src/chaster_sdk.egg-info/
+-rwxrwxrwx   0 max       (1000) max       (1000)     1092 2024-04-08 01:24:03.000000 chaster-sdk-0.1.4/src/chaster_sdk.egg-info/PKG-INFO
+-rwxrwxrwx   0 max       (1000) max       (1000)      507 2024-04-08 01:24:03.000000 chaster-sdk-0.1.4/src/chaster_sdk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 max       (1000) max       (1000)        1 2024-04-08 01:24:03.000000 chaster-sdk-0.1.4/src/chaster_sdk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 max       (1000) max       (1000)       25 2024-04-08 01:24:03.000000 chaster-sdk-0.1.4/src/chaster_sdk.egg-info/requires.txt
+-rwxrwxrwx   0 max       (1000) max       (1000)        8 2024-04-08 01:24:03.000000 chaster-sdk-0.1.4/src/chaster_sdk.egg-info/top_level.txt
+drwxrwxrwx   0 max       (1000) max       (1000)        0 2024-04-08 01:24:04.330906 chaster-sdk-0.1.4/tests/
+-rwxrwxrwx   0 max       (1000) max       (1000)    28527 2024-04-06 18:22:36.000000 chaster-sdk-0.1.4/tests/test_api_integration.py
+-rwxrwxrwx   0 max       (1000) max       (1000)    27822 2024-04-06 17:56:21.000000 chaster-sdk-0.1.4/tests/test_api_mock_chaster.py
+-rwxrwxrwx   0 max       (1000) max       (1000)     8961 2024-01-23 17:43:23.000000 chaster-sdk-0.1.4/tests/test_dto.py
```

### Comparing `chaster-sdk-0.1.3/LICENSE` & `chaster-sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chaster-sdk-0.1.3/PKG-INFO` & `chaster-sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaster-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Chaster python sdk
 Author-email: Poofy <poofy.enigma@gmail.com>
 Project-URL: Homepage, https://github.com/PoofyEnigma/chaster-python-sdk
 Project-URL: Issues, https://github.com/PoofyEnigma/chaster-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `chaster-sdk-0.1.3/README.md` & `chaster-sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chaster-sdk-0.1.3/pyproject.toml` & `chaster-sdk-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "chaster-sdk"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "Poofy", email = "poofy.enigma@gmail.com" },
 ]
 description = "Chaster python sdk"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `chaster-sdk-0.1.3/src/chaster/api.py` & `chaster-sdk-0.1.4/src/chaster/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 import time
 from types import SimpleNamespace
 from urllib.parse import urlparse, urljoin
 
 
 class ChasterAPI:
 
-    def __init__(self, bearer, user_agent='ChasterPythonSDK/1.0', delay=5, root_api='https://api.chaster.app/'):
+    def __init__(self, bearer,
+                 user_agent='ChasterPythonSDK/1.0',
+                 delay=0,
+                 root_api='https://api.chaster.app/',
+                 request_hook=None):
         """
         Not thread safe. Will need a ChasterAPI object per thread.
         :param bearer: bearer token for authentication
         :param user_agent: the value assigned to the User-Agent http header
         :param delay: the amount of seconds to wait after a request
         :param root_api: the url to the api endpoint
+        :param request_hook: a function or list of functions with params (response: requests.models.Response, *args, **kwargs) that is called after every chaster api request.
         """
 
         super().__init__()
         self.logger = logging.getLogger(self.__class__.__name__)
         self.root_api = urlparse(root_api)
         self.delay = delay
         self.session = requests.Session()  # generally not multithread safe https://github.com/psf/requests/issues/1871
@@ -36,14 +41,20 @@
         # The retries are left here as a good measure but is not a proven necessary component of the class.
         retries = Retry(total=3,
                         backoff_factor=0.1,
                         status_forcelist=[500, 502, 503, 504],
                         respect_retry_after_header=True)
         self.session.mount('http://', HTTPAdapter(max_retries=retries))
         self.session.mount('https://', HTTPAdapter(max_retries=retries))
+        self._hooks = [self._request_logger, self._post_request_handler]
+        if request_hook is not None:
+            if type(request_hook) is list:
+                self._hooks.extend(request_hook)
+            else:
+                self._hooks.append(request_hook)
 
     def _request_logger(self, response: requests.models.Response, *args, **kwargs):
         chaster_transaction_id = ''
         if 'x-chaster-transaction-id' in response.headers:
             chaster_transaction_id = response.headers['x-chaster-transaction-id']
             pass
 
@@ -57,39 +68,39 @@
             f'{response.status_code} {response.request.method} {response.request.url}  chaster_transaction_id:{chaster_transaction_id} {response.content}')
 
     def _post_request_handler(self, response: requests.models.Response, *args, **kwargs):
         time.sleep(self.delay)
 
     def _get(self, path: str) -> requests.models.Response:
         response = self.session.get(urljoin(self.root_api.geturl(), path),
-                                    hooks={'response': [self._post_request_handler, self._request_logger]})
+                                    hooks={'response': self._hooks})
         return response
 
     def _post(self, path: str, data) -> requests.models.Response:
         response = self.session.post(urljoin(self.root_api.geturl(), path),
                                      data=json.dumps(data),
-                                     hooks={'response': [self._post_request_handler, self._request_logger]},
+                                     hooks={'response': self._hooks},
                                      headers={'Content-Type': 'application/json'})
         return response
 
     def _post_form(self, path: str, form) -> requests.models.Response:
         response = self.session.post(urljoin(self.root_api.geturl(), path),
-                                     hooks={'response': [self._post_request_handler, self._request_logger]},
+                                     hooks={'response': self._hooks},
                                      files=form)
         return response
 
     def _put(self, path: str, data) -> requests.models.Response:
         response = self.session.put(urljoin(self.root_api.geturl(), path),
-                                    data=json.dumps(data), hooks={'response': self._post_request_handler},
+                                    data=json.dumps(data), hooks={'response': self._hooks},
                                     headers={'Content-Type': 'application/json'})
         return response
 
     def _delete(self, path: str):
         response = self.session.delete(urljoin(self.root_api.geturl(), path),
-                                       hooks={'response': self._post_request_handler})
+                                       hooks={'response': self._hooks})
         return response
 
     def _tester_get_wrapper(self, path, func):
         response = self._get(path)
         data = None
         if response.status_code == 200:
             data = response.json(object_hook=lambda d: SimpleNamespace(**d))
```

### Comparing `chaster-sdk-0.1.3/src/chaster/conversation.py` & `chaster-sdk-0.1.4/src/chaster/conversation.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         self.createdAt = isoparse(obj.createdAt)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
         obj['users'] = user.User.dump_array(self.users)
         util.safe_dump_parameter(self, 'lastMessage', obj)
-        util.dump_time(self, 'lastMessageAt', obj)
-        util.dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'lastMessageAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [Conversation().update(item) for item in obj_list]
 
     @staticmethod
@@ -69,16 +69,16 @@
         self.__dict__ = obj.__dict__
         self.createdAt = isoparse(obj.updatedAt)
         self.updatedAt = isoparse(obj.updatedAt)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
-        util.dump_time(self, 'createdAt', obj)
-        util.dump_time(self, 'updatedAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'updatedAt', obj)
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [Message().update(item) for item in obj_list]
 
     @staticmethod
```

### Comparing `chaster-sdk-0.1.3/src/chaster/extensions.py` & `chaster-sdk-0.1.4/src/chaster/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,14 +541,17 @@
         return self.__dict__.copy()
 
 
 class Penalty:
     def __init__(self):
         self.prefix: str = 'default'
         self.name: str = 'tasks'
+        """
+        options: tasks, tasks_do_task, verification_picture_verify, dice_roll, wheel_of_fortune_turns, temporary_opening_open, temporary_opening_time_limit
+        """
         self.params: PenaltyParams = PenaltyParams()
         self.punishments: list[Punishment] = []
 
     def update(self, obj):
         self.__dict__ = obj.__dict__.copy()
         self.punishments = Punishment.generate_array(obj.punishments)
         return self
```

### Comparing `chaster-sdk-0.1.3/src/chaster/lock.py` & `chaster-sdk-0.1.4/src/chaster/lock.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,46 +26,46 @@
         obj['extensions'] = eh.dump()
         return obj
 
 
 class Lock:
     def __init__(self):
         self._id: str = ''
-        self.startDate: str = ''
-        self.endDate: str = ''
-        self.minDate: str = ''
-        self.maxDate: str = ''
-        self.maxLimitDate: datetime.datetime = None
+        self.startDate: datetime.datetime = None
+        self.endDate: datetime.datetime = None
+        self.minDate: datetime.datetime = None
+        self.maxDate: datetime.datetime = None
+        self.maxLimitDate: datetime.datetime | None = None
         self.displayRemainingTime: bool = True
         self.limitLockTime: bool = False
         self.status: str = ''
         self.combination: str = ''
-        self.sharedLock: SharedLock = None
-        self.createdAt: str = ''
-        self.updatedAt: str = ''
-        self.unlockedAt: datetime.datetime = None
-        self.archivedAt: datetime.datetime = None
-        self.frozenAt: str = ''
+        self.sharedLock: SharedLock | None = None
+        self.createdAt: datetime.datetime = None
+        self.updatedAt: datetime.datetime = None
+        self.unlockedAt: datetime.datetime | None = None
+        self.archivedAt: datetime.datetime | None = None
+        self.frozenAt: datetime.datetime | None = None
         self.keyholderArchivedAt: datetime.datetime = None
         self.totalDuration: int = 235422887
         self.allowSessionOffer: bool = False
         self.isTestLock: bool = False
         self.offerToken: str = ''
         self.hideTimeLogs: bool = True
         self.trusted: bool = False
-        self.user = user.User()
-        self.keyholder = None
+        self.user: user.User = None
+        self.keyholder: user.User = None
         self.isAllowedToViewTime: bool = True
         self.canBeUnlocked: bool = False
         self.canBeUnlockedByMaxLimitDate: bool = False
         self.isFrozen: bool = True
         self.extensions = []
         self.role: str = ''
         self.title: str = ''
-        self.lastVerificationPicture = None
+        self.lastVerificationPicture: LastVerificationPicture = None
         self.availableHomeActions: list[AvailableHomeAction] = []
         self.reasonsPreventingUnlocking = []
         self.extensionsAllowUnlocking: bool = True
         self.deletedAt: datetime.datetime = None
 
     def dump(self):
         obj = self.__dict__.copy()
@@ -79,19 +79,31 @@
         if self.keyholder is not None:
             obj['keyholder'] = self.keyholder.dump()
         if self.lastVerificationPicture is not None:
             obj['lastVerificationPicture'] = self.lastVerificationPicture.dump()
         if self.sharedLock is not None:
             obj['sharedLock'] = self.sharedLock.dump()
 
-        util.dump_time(self, 'maxLimitDate', obj)
-        util.dump_time(self, 'unlockedAt', obj)
-        util.dump_time(self, 'archivedAt', obj)
-        util.dump_time(self, 'keyholderArchivedAt', obj)
-        util.dump_time(self, 'deletedAt', obj)
+        times = [
+            'startDate',
+            'endDate',
+            'minDate',
+            'maxDate',
+            'maxLimitDate',
+            'createdAt',
+            'updatedAt',
+            'unlockedAt',
+            'archivedAt',
+            'frozenAt',
+            'keyholderArchivedAt',
+            'deletedAt'
+        ]
+
+        for time in times:
+            util.safe_dump_time(self, time, obj)
         return obj
 
     def update(self, obj):
         self.__dict__ = obj.__dict__.copy()
         self.user = user.User().update(obj.user)
         if 'extensions' in obj.__dict__:
             self.extensions = extensions.Extension.generate_array(obj.extensions)
@@ -99,24 +111,32 @@
             self.availableHomeActions = AvailableHomeAction.generate_array(obj.availableHomeActions)
         if 'keyholder' in obj.__dict__ and obj.keyholder is not None:
             self.keyholder = user.User().update(obj.keyholder)
         if 'lastVerificationPicture' in obj.__dict__ and obj.lastVerificationPicture is not None:
             self.lastVerificationPicture = LastVerificationPicture().update(obj.lastVerificationPicture)
         if 'sharedLock' in obj.__dict__ and obj.sharedLock is not None:
             self.sharedLock = SharedLock().update(obj.sharedLock)
-        if 'maxLimitDate' in obj.__dict__ and obj.maxLimitDate is not None:
-            self.maxLimitDate = isoparse(obj.maxLimitDate)
-        if 'unlockedAt' in obj.__dict__ and obj.unlockedAt is not None:
-            self.unlockedAt = isoparse(obj.unlockedAt)
-        if 'archivedAt' in obj.__dict__ and obj.archivedAt is not None:
-            self.archivedAt = isoparse(obj.archivedAt)
-        if 'keyholderArchivedAt' in obj.__dict__ and obj.keyholderArchivedAt is not None:
-            self.keyholderArchivedAt = isoparse(obj.keyholderArchivedAt)
-        if 'deletedAt' in obj.__dict__ and obj.deletedAt is not None:
-            self.deletedAt = isoparse(obj.deletedAt)
+
+        times = [
+            'startDate',
+            'endDate',
+            'minDate',
+            'maxDate',
+            'maxLimitDate',
+            'createdAt',
+            'updatedAt',
+            'unlockedAt',
+            'archivedAt',
+            'frozenAt',
+            'keyholderArchivedAt',
+            'deletedAt'
+        ]
+
+        for time in times:
+            util.safe_update_time(obj, time, self)
         return self
 
     @staticmethod
     def generate_array(obj_list):
         return [Lock().update(lock) for lock in obj_list]
 
     @staticmethod
@@ -204,15 +224,15 @@
             self.createdAt = dateutil.parser.isoparse(obj.createdAt)
         util.safe_update_parameter(obj, 'user', self, user.User().update)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
         obj['user'] = self.user.dump()
-        util.dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
         obj['payload'] = self.payload.__dict__.copy()
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [ActionLog().update(item) for item in obj_list]
 
@@ -304,17 +324,17 @@
         self.description: str = ''
         self.photoId: str = ''
         self.hideTimeLogs: bool = False
         self.isFindom: bool = False
 
     def dump(self):
         dictionary = self.__dict__.copy()
-        util.dump_time(self, 'maxDate', dictionary)
-        util.dump_time(self, 'minDate', dictionary)
-        util.dump_time(self, 'maxLimitDate', dictionary)
+        util.safe_dump_time(self, 'maxDate', dictionary)
+        util.safe_dump_time(self, 'minDate', dictionary)
+        util.safe_dump_time(self, 'maxLimitDate', dictionary)
         return dictionary
 
     def update(self, obj):
         self.__dict__ = obj.__dict__
         if obj.maxDate is not None:
             self.maxDate = isoparse(obj.maxDate)
         if obj.minDate is not None:
@@ -383,18 +403,18 @@
             eh.load_defined(self.extensions)
             obj['extensions'] = eh.dump()
         if self.unsplashPhoto is not None:
             obj['unsplashPhoto'] = self.unsplashPhoto.dump()
         util.safe_dump_parameter(self, 'user', obj)
         if 'joinRules' in self.__dict__ and self.joinRules is not None:
             obj['joinRules'] = self.joinRules.dump()
-        util.dump_time(self, 'maxDate', obj)
-        util.dump_time(self, 'minDate', obj)
-        util.dump_time(self, 'maxLimitDate', obj)
-        util.dump_time(self, 'lastSavedAt', obj)
+        util.safe_dump_time(self, 'maxDate', obj)
+        util.safe_dump_time(self, 'minDate', obj)
+        util.safe_dump_time(self, 'maxLimitDate', obj)
+        util.safe_dump_time(self, 'lastSavedAt', obj)
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [SharedLock().update(entry) for entry in obj_list]
 
     @staticmethod
@@ -502,22 +522,22 @@
         obj['joinRules'] = self.joinRules.dump()
         obj['user'] = self.user.dump()
         eh = extensions.ExtensionsHandler()
         eh.load_defined(self.extensions)
         obj['extensions'] = eh.dump()
         if 'locks' in self.__dict__:
             obj['locks'] = Lock.dump_array(self.locks)
-        util.dump_time(self, 'maxDate', obj)
-        util.dump_time(self, 'minDate', obj)
-        util.dump_time(self, 'maxLimitDate', obj)
-        util.dump_time(self, 'lastSavedAt', obj)
-        util.dump_time(self, 'createdAt', obj)
-        util.dump_time(self, 'updatedAt', obj)
-        util.dump_time(self, 'unlockedAt', obj)
-        util.dump_time(self, 'deletedAt', obj)
+        util.safe_dump_time(self, 'maxDate', obj)
+        util.safe_dump_time(self, 'minDate', obj)
+        util.safe_dump_time(self, 'maxLimitDate', obj)
+        util.safe_dump_time(self, 'lastSavedAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'updatedAt', obj)
+        util.safe_dump_time(self, 'unlockedAt', obj)
+        util.safe_dump_time(self, 'deletedAt', obj)
         return obj
 
 
 class ExplorePageLock:
     def __init__(self):
         self.locks: list[Lock] = []
         self._id: str = ''
@@ -659,14 +679,14 @@
         self.submittedAt = dateutil.parser.isoparse(obj.submittedAt)
         if obj.votes is not None:
             self.votes = VerificationPhotoHistoryVotes().update(obj.votes)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
-        util.dump_time(self, 'submittedAt', obj)
+        util.safe_dump_time(self, 'submittedAt', obj)
         obj['votes'] = self.votes.dump()
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [VerificationPhotoHistory().update(account) for account in obj_list]
```

### Comparing `chaster-sdk-0.1.3/src/chaster/triggers.py` & `chaster-sdk-0.1.4/src/chaster/triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.__dict__ = obj.__dict__.copy()
         if obj.createdAt is not None:
             self.createdAt = dateutil.parser.isoparse(obj.createdAt)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
-        util.dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [Vote().update(vote) for vote in obj_list]
 
     @staticmethod
```

### Comparing `chaster-sdk-0.1.3/src/chaster/user.py` & `chaster-sdk-0.1.4/src/chaster/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,16 @@
             self.createdAt = dateutil.parser.isoparse(obj.createdAt)
         if obj.updatedAt is not None:
             self.updatedAt = dateutil.parser.isoparse(obj.updatedAt)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
-        util.dump_time(self, 'createdAt', obj)
-        util.dump_time(self, 'updatedAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'updatedAt', obj)
         return obj
 
 
 class Stats:
     def __init__(self):
         self.nbStartedLocks: int = 0
         self.nbEndedLocks: int = 0
@@ -344,17 +344,17 @@
     def dump(self):
         obj = self.__dict__.copy()
         obj['settings'] = self.settings.dump()
         obj['metadata'] = self.metadata.dump()
         obj['country'] = self.country.dump()
         obj['region'] = self.region.dump()
         obj['privateMetadata'] = self.privateMetadata.dump()
-        util.dump_time(self, 'subscriptionEnd', obj)
-        util.dump_time(self, 'customSubscriptionEnd', obj)
-        util.dump_time(self, 'birthDate', obj)
+        util.safe_dump_time(self, 'subscriptionEnd', obj)
+        util.safe_dump_time(self, 'customSubscriptionEnd', obj)
+        util.safe_dump_time(self, 'birthDate', obj)
         return obj
 
 
 class KeyholderOfferEntry:
     def __init__(self):
         self._id: str = ''
         self.keyholder: User = None
@@ -377,18 +377,18 @@
         if obj.updatedAt is not None:
             self.updatedAt = dateutil.parser.isoparse(obj.updatedAt)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
         obj['keyholder'] = self.keyholder.dump()
-        util.dump_time(self, 'validatedAt', obj)
-        util.dump_time(self, 'archivedAt', obj)
-        util.dump_time(self, 'createdAt', obj)
-        util.dump_time(self, 'updatedAt', obj)
+        util.safe_dump_time(self, 'validatedAt', obj)
+        util.safe_dump_time(self, 'archivedAt', obj)
+        util.safe_dump_time(self, 'createdAt', obj)
+        util.safe_dump_time(self, 'updatedAt', obj)
         return obj
 
     @staticmethod
     def generate_array(obj_list):
         return [KeyholderOfferEntry().update(item) for item in obj_list]
 
 
@@ -482,16 +482,16 @@
         self.__dict__ = obj.__dict__.copy()
         self.start = dateutil.parser.isoparse(obj.start)
         self.end = dateutil.parser.isoparse(obj.end)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
-        util.dump_time(self, 'start', obj)
-        util.dump_time(self, 'end', obj)
+        util.safe_dump_time(self, 'start', obj)
+        util.safe_dump_time(self, 'end', obj)
         return obj
 
 
 class CommunityEventTier:
     def __init__(self):
         self.name: str = ''
         self.requiredPoints: int = 0
@@ -554,9 +554,9 @@
         self.time = dateutil.parser.isoparse(obj.time)
         return self
 
     def dump(self):
         obj = self.__dict__.copy()
         if self.communityEvent is not None:
             obj['communityEvent'] = self.communityEvent.dump()
-        util.dump_time(self, 'time', obj)
+        util.safe_dump_time(self, 'time', obj)
         return obj
```

### Comparing `chaster-sdk-0.1.3/src/chaster/util.py` & `chaster-sdk-0.1.4/src/chaster/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def datetime_to_chaster_format(d: datetime.datetime) -> str:
     d.replace(tzinfo=datetime.timezone.utc).astimezone(tz=None)
     return d.strftime('%Y-%m-%dT%H:%M:%S.%f')[:-len('000')] + 'Z'
 
 
-def dump_time(src, key, out):
+def safe_dump_time(src, key, out):
     if key in src.__dict__ and src.__dict__[key] is not None:
         out[key] = datetime_to_chaster_format(src.__dict__[key])
 
 
 def safe_dump_parameter(src, key, out):
     if key in src.__dict__ and src.__dict__[key] is not None:
         out[key] = src.__dict__[key].dump()
```

### Comparing `chaster-sdk-0.1.3/src/chaster_sdk.egg-info/PKG-INFO` & `chaster-sdk-0.1.4/src/chaster_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaster-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Chaster python sdk
 Author-email: Poofy <poofy.enigma@gmail.com>
 Project-URL: Homepage, https://github.com/PoofyEnigma/chaster-python-sdk
 Project-URL: Issues, https://github.com/PoofyEnigma/chaster-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `chaster-sdk-0.1.3/tests/test_api_integration.py` & `chaster-sdk-0.1.4/tests/test_api_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import datetime
 import time
 
+import requests
+
 import src.chaster.api as api
 import src.chaster.lock as lock
 import src.chaster.extensions as extensions
 import unittest
 import uuid
 import logging
 import os
@@ -15,14 +17,40 @@
 
 
 class ApiTestCases(unittest.TestCase):
 
     def out_test(self, response, data):
         time.sleep(0)
 
+    @unittest.SkipTest
+    def test_request_hook(self):
+        count = 0
+
+        def func_count(response: requests.models.Response, *args, **kwargs):
+            nonlocal count
+            count += 1
+
+        chaster_api_temp = api.ChasterAPI(os.environ.get('CHASTER_BEARER_TOKEN'),
+                                          user_agent='PythonSDKDeveloplment/1.0', request_hook=func_count)
+        chaster_api_temp.get_user_shared_locks()
+        self.assertEqual(count, 1)
+
+    @unittest.SkipTest
+    def test_request_hooks(self):
+        count = 0
+
+        def func_count(response: requests.models.Response, *args, **kwargs):
+            nonlocal count
+            count += 1
+
+        chaster_api_temp = api.ChasterAPI(os.environ.get('CHASTER_BEARER_TOKEN'),
+                                          user_agent='PythonSDKDeveloplment/1.0', request_hook=[func_count, func_count])
+        chaster_api_temp.get_user_shared_locks()
+        self.assertEqual(count, 2)
+
     """
     Shared Locks
     """
 
     @unittest.SkipTest
     def test_get_shared_locks_active(self):
         response, data = chaster_api.get_user_shared_locks()
```

### Comparing `chaster-sdk-0.1.3/tests/test_api_mock_chaster.py` & `chaster-sdk-0.1.4/tests/test_api_mock_chaster.py`

 * *Files identical despite different names*

### Comparing `chaster-sdk-0.1.3/tests/test_dto.py` & `chaster-sdk-0.1.4/tests/test_dto.py`

 * *Files identical despite different names*

