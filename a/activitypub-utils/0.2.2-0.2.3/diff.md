# Comparing `tmp/activitypub-utils-0.2.2.tar.gz` & `tmp/activitypub-utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitypub-utils-0.2.2.tar", last modified: Wed Apr  3 17:56:20 2024, max compression
+gzip compressed data, was "activitypub-utils-0.2.3.tar", last modified: Mon Apr  8 19:25:11 2024, max compression
```

## Comparing `activitypub-utils-0.2.2.tar` & `activitypub-utils-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-03 17:56:20.362771 activitypub-utils-0.2.2/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-14 16:23:17.000000 activitypub-utils-0.2.2/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1944 2024-04-03 17:56:20.362771 activitypub-utils-0.2.2/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      418 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-03 17:56:20.358771 activitypub-utils-0.2.2/activitypub_utils.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1944 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      452 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        8 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/top_level.txt
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-03 17:56:20.358771 activitypub-utils-0.2.2/aputils/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      742 2024-04-03 17:18:25.000000 activitypub-utils-0.2.2/aputils/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9467 2024-04-03 17:43:36.000000 activitypub-utils-0.2.2/aputils/__main__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9997 2024-04-03 15:10:57.000000 activitypub-utils-0.2.2/aputils/algorithms.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6095 2024-03-31 15:43:20.000000 activitypub-utils-0.2.2/aputils/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)      395 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/aputils/errors.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    16530 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/aputils/message.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    12394 2024-04-03 15:56:22.000000 activitypub-utils-0.2.2/aputils/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9208 2024-03-31 15:45:56.000000 activitypub-utils-0.2.2/aputils/objects.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/aputils/py.typed
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4140 2024-03-28 03:37:58.000000 activitypub-utils-0.2.2/aputils/request_classes.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9975 2024-03-31 15:44:34.000000 activitypub-utils-0.2.2/aputils/signer.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1996 2024-04-03 15:11:20.000000 activitypub-utils-0.2.2/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-03 17:56:20.362771 activitypub-utils-0.2.2/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:25:11.131593 activitypub-utils-0.2.3/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-14 16:23:17.000000 activitypub-utils-0.2.3/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1944 2024-04-08 19:25:11.131593 activitypub-utils-0.2.3/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      418 2024-03-27 17:16:45.000000 activitypub-utils-0.2.3/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:25:11.131593 activitypub-utils-0.2.3/activitypub_utils.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1944 2024-04-08 19:25:11.000000 activitypub-utils-0.2.3/activitypub_utils.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      452 2024-04-08 19:25:11.000000 activitypub-utils-0.2.3/activitypub_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-08 19:25:11.000000 activitypub-utils-0.2.3/activitypub_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-08 19:25:11.000000 activitypub-utils-0.2.3/activitypub_utils.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        8 2024-04-08 19:25:11.000000 activitypub-utils-0.2.3/activitypub_utils.egg-info/top_level.txt
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:25:11.131593 activitypub-utils-0.2.3/aputils/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      742 2024-04-08 19:13:22.000000 activitypub-utils-0.2.3/aputils/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    11091 2024-04-08 19:16:27.000000 activitypub-utils-0.2.3/aputils/__main__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    10027 2024-04-08 19:03:42.000000 activitypub-utils-0.2.3/aputils/algorithms.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6095 2024-03-31 15:43:20.000000 activitypub-utils-0.2.3/aputils/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      395 2024-03-27 17:16:45.000000 activitypub-utils-0.2.3/aputils/errors.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    16993 2024-04-08 19:14:33.000000 activitypub-utils-0.2.3/aputils/message.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    12582 2024-04-07 13:54:10.000000 activitypub-utils-0.2.3/aputils/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9208 2024-03-31 15:45:56.000000 activitypub-utils-0.2.3/aputils/objects.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-27 17:16:45.000000 activitypub-utils-0.2.3/aputils/py.typed
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4140 2024-03-28 03:37:58.000000 activitypub-utils-0.2.3/aputils/request_classes.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9975 2024-03-31 15:44:34.000000 activitypub-utils-0.2.3/aputils/signer.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1996 2024-04-03 15:11:20.000000 activitypub-utils-0.2.3/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-08 19:25:11.131593 activitypub-utils-0.2.3/setup.cfg
```

### Comparing `activitypub-utils-0.2.2/LICENSE.md` & `activitypub-utils-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.2/PKG-INFO` & `activitypub-utils-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activitypub-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Various classes and functions for ActivityPub servers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/aputils
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/aputils/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/aputils
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/aputils
```

### Comparing `activitypub-utils-0.2.2/activitypub_utils.egg-info/PKG-INFO` & `activitypub-utils-0.2.3/activitypub_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activitypub-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Various classes and functions for ActivityPub servers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/aputils
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/aputils/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/aputils
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/aputils
```

### Comparing `activitypub-utils-0.2.2/aputils/__init__.py` & `activitypub-utils-0.2.3/aputils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from .algorithms import Algorithm, HS2019, RsaSha256
 from .algorithms import get as get_algorithm, register as register_algorithm
 from .errors import InvalidKeyError, SignatureFailureError
 from .message import Attachment, Message, Property
 from .misc import Digest, HttpDate, JsonBase, MessageDate, Signature
 from .objects import HostMeta, HostMetaJson, Nodeinfo, Webfinger, WellKnownNodeinfo
```

### Comparing `activitypub-utils-0.2.2/aputils/algorithms.py` & `activitypub-utils-0.2.3/aputils/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,21 +302,24 @@
 				body = bytes(body, encoding = "utf-8")
 
 		headers = {key.lower(): value for key, value in headers.items()}
 
 		if host:
 			headers["host"] = host
 
-		date: HttpDate | datetime | str = headers.get("date", HttpDate.new_utc())
+		raw_date: HttpDate | datetime | str = headers.get("date", HttpDate.new_utc())
 
-		if isinstance(date, str):
-			date = HttpDate.parse(date)
+		if isinstance(raw_date, str):
+			date = HttpDate.parse(raw_date)
 
-		elif isinstance(date, datetime) and not isinstance(date, HttpDate):
-			date = HttpDate.new_from_datetime(date)
+		elif isinstance(raw_date, datetime) and not isinstance(raw_date, HttpDate):
+			date = HttpDate.new_from_datetime(raw_date)
+
+		else:
+			date = raw_date
 
 		if date + timedelta(hours = 6) >= (new_date := HttpDate.new_utc()):
 			date = new_date
 
 		headers.update({
 			"date": date.to_string(),
 			"(request-target)": f"{method.lower()} {path}",
@@ -340,22 +343,20 @@
 			headers: dict[str, str],
 			signature: Signature) -> dict[str, str]:
 
 		headers = {key.lower(): value for key, value in headers.items()}
 		headers["(request-target)"] = f"{method.lower()} {path}"
 
 		if signature.created is not None:
+			if signature.created_date > HttpDate.new_utc():
+				raise SignatureFailureError("Signature creation date is in the future")
+
 			headers["(created)"] = str(signature.created)
 
 		if signature.expires is not None:
-			current = HttpDate.new_utc()
-
-			if signature.created_date > current:
-				raise SignatureFailureError("Signature creation date is in the future")
-
 			if signature.expires_date < HttpDate.new_utc():
 				raise SignatureFailureError("Signature has expired")
 
 			headers["(expires)"] = str(signature.expires)
 
 		return headers
```

### Comparing `activitypub-utils-0.2.2/aputils/enums.py` & `activitypub-utils-0.2.3/aputils/enums.py`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.2/aputils/message.py` & `activitypub-utils-0.2.3/aputils/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,22 +384,24 @@
 			value = [Attachment(item) for item in value] if value else []
 
 		else:
 			try:
 				prop = getattr(Message, key)
 				vtype = TYPES[prop.type_name]
 
-				if vtype == TYPES["object"] and isinstance(value, str):
+				if isinstance(value, datetime) and not isinstance(value, MessageDate):
+					value = MessageDate.parse(value)
+
+				elif vtype == TYPES["object"] and isinstance(value, str):
 					pass
 
 				else:
 					vtype = vtype[0] if isinstance(vtype, tuple) else vtype
 
 					if not isinstance(value, vtype):
-						print(key, type(value), vtype)
 						value = CONVERTERS[vtype][0](value)
 
 			except (KeyError, AttributeError):
 				pass
 
 		dict.__setitem__(self, dict_key, value)
 
@@ -463,14 +465,31 @@
 		data.media_type = mimetype
 		data.url = url
 		return data
 
 
 	# general properties
 	@property
+	def actor_id(self) -> str:
+		"Get the url of the actor associated with the message"
+
+		if "actor" not in self:
+			raise AttributeError("Message does not have an 'actor' key")
+
+		if isinstance(self["actor"], str):
+			return self["actor"]
+
+		try:
+			return self["actor"]["id"]
+
+		except KeyError:
+			raise AttributeError("Message does not have an 'actor' key") from None
+
+
+	@property
 	def domain(self) -> str:
 		"Get the domain of the object origin"
 		return urlparse(self["id"]).hostname
 
 
 	@property
 	def object_id(self) -> str:
@@ -596,25 +615,25 @@
 
 		data = cls.new(
 			actor_type,
 			data = {
 				"id": actor,
 				"preferred_username": handle,
 				"inbox": inbox or f"{actor}/inbox",
-				"outbox": inbox or f"{actor}/outbox",
+				"outbox": outbox or f"{actor}/outbox",
 				"attachment": [],
+				**kwargs,
 				"endpoints": {
 					"sharedInbox": shared_inbox or f"{proto}://{domain}/inbox"
 				},
 				"public_key": {
 					"id": f"{actor}#main-key",
 					"owner": actor,
 					"publicKeyPem": pubkey
-				},
-				**kwargs
+				}
 			},
 			context = [
 				{
 					"toot": "http://joinmastodon.org/ns#",
 					"publicKeyBase64": "toot:publicKeyBase64",
 				}
 			]
```

### Comparing `activitypub-utils-0.2.2/aputils/misc.py` & `activitypub-utils-0.2.3/aputils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,31 +194,38 @@
 
 
 	def __str__(self) -> str:
 		return self.to_string()
 
 
 	@classmethod
-	def parse(cls: type[Self], date: str | int | float) -> Self:
+	def parse(cls: type[Self], date: datetime | str | int | float) -> Self:
 		"""
 			Parse a unix timestamp or HTTP date in string format
 
 			:param date: Unix timestamp or string from an HTTP Date header
 		"""
 
-		if isinstance(date, (int | float)):
+		if isinstance(date, cls):
+			return date
+
+		elif isinstance(date, datetime):
+			return cls.fromisoformat(date.isoformat())
+
+		elif isinstance(date, (int | float)):
 			data = cls.fromtimestamp(float(date) if type(date) is int else date)
 
 		else:
 			data = cls.strptime(date, cls.FORMAT)
 
 		return data.replace(tzinfo=timezone.utc)
 
 
 	@classmethod
+	@deprecated("HttpDate.parse", "0.2.3", "0.3.0")
 	def new_from_datetime(cls: type[Self], date: datetime) -> Self:
 		"""
 			Create a new ``HttpDate`` object from a ``datetime`` object
 
 			:param date: ``datetime`` object to convert
 		"""
 		return cls.fromisoformat(date.isoformat())
```

### Comparing `activitypub-utils-0.2.2/aputils/objects.py` & `activitypub-utils-0.2.3/aputils/objects.py`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.2/aputils/request_classes.py` & `activitypub-utils-0.2.3/aputils/request_classes.py`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.2/aputils/signer.py` & `activitypub-utils-0.2.3/aputils/signer.py`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.2/pyproject.toml` & `activitypub-utils-0.2.3/pyproject.toml`

 * *Files identical despite different names*

