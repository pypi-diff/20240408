# Comparing `tmp/passwordless-0.1.1.tar.gz` & `tmp/passwordless-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-0.1.1.tar", max compression
+gzip compressed data, was "passwordless-1.0.0.tar", max compression
```

## Comparing `passwordless-0.1.1.tar` & `passwordless-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-01-03 10:13:12.699613 passwordless-0.1.1/LICENSE
--rw-r--r--   0        0        0     2882 2024-01-03 10:13:12.699613 passwordless-0.1.1/README.md
--rw-r--r--   0        0        0     1869 2024-01-03 10:13:12.699613 passwordless-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      879 2024-01-03 10:13:12.699613 passwordless-0.1.1/src/passwordless/__init__.py
--rw-r--r--   0        0        0    11659 2024-01-03 10:13:12.699613 passwordless-0.1.1/src/passwordless/client.py
--rw-r--r--   0        0        0      497 2024-01-03 10:13:12.699613 passwordless-0.1.1/src/passwordless/config.py
--rw-r--r--   0        0        0     1083 2024-01-03 10:13:12.699613 passwordless-0.1.1/src/passwordless/errors.py
--rw-r--r--   0        0        0     2231 2024-01-03 10:13:12.699613 passwordless-0.1.1/src/passwordless/models.py
--rw-r--r--   0        0        0     5822 2024-01-03 10:13:12.699613 passwordless-0.1.1/src/passwordless/serialization.py
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 passwordless-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 07:45:36.813967 passwordless-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2882 2024-04-08 07:45:36.813967 passwordless-1.0.0/README.md
+-rw-r--r--   0        0        0     1996 2024-04-08 07:45:36.817967 passwordless-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1097 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/__init__.py
+-rw-r--r--   0        0        0    13669 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/client.py
+-rw-r--r--   0        0        0      497 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/config.py
+-rw-r--r--   0        0        0     1083 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/errors.py
+-rw-r--r--   0        0        0     2548 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/models.py
+-rw-r--r--   0        0        0     6653 2024-04-08 07:45:36.817967 passwordless-1.0.0/src/passwordless/serialization.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 passwordless-1.0.0/PKG-INFO
```

### Comparing `passwordless-0.1.1/LICENSE` & `passwordless-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `passwordless-0.1.1/README.md` & `passwordless-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `passwordless-0.1.1/pyproject.toml` & `passwordless-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 [tool.poetry]
 name = "passwordless"
-version = "0.1.1"
+version = "1.0.0"
 description = "Passwordless.dev Python SDK"
 authors = [
     "Bitwarden <hello@bitwarden.com>"
 ]
 maintainers = [
     "Maciej Zieniuk <zieniuk.maciej@gmail.com>"
 ]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Security",
     "Topic :: Software Development :: Libraries",
+    "Topic :: Communications :: FIDO",
     "License :: OSI Approved :: Apache Software License"
 ]
 keywords = ["passwordless", "bitwarden"]
 homepage = "https://bitwarden.com/products/passwordless"
 documentation = "https://docs.passwordless.dev/guide"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-requests = "^2"
-marshmallow = "^3"
-python-dateutil = "^2"
+python = "3.8.18"
+requests = "2.31.0"
+marshmallow = "3.21.1"
+python-dateutil = "2.9.0.post0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-python-dotenv = "*"
-flake8 = "*"
-black = "*"
-mypy = "*"
-isort = "*"
-pre-commit = "*"
-pre-commit-hooks = "*"
-types-requests = "^2"
-docformatter = {extras = ["tomli"], version = "^1.7.5"}
+python-dotenv = "1.0.1"
+flake8 = "5.0.4"
+black = "24.3.0"
+mypy = "1.9.0"
+isort = "5.13.2"
+pre-commit = "3.5.0"
+pre-commit-hooks = "4.5.0"
+types-requests = "2.31.0.20240406"
+docformatter = {extras = ["tomli"], version = "1.7.5"}
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "*"
-pytest-mock = "*"
-pytest-httpserver = "*"
+pytest = "8.0.2"
+pytest-mock = "3.12.0"
+pytest-httpserver = "1.0.10"
 
 [tool.mypy]
 python_version = "3.8"
 files = ["src/passwordless"]
 exclude = ["venv", "tests", "examples"]
 show_error_codes = true
 pretty = true
```

### Comparing `passwordless-0.1.1/src/passwordless/__init__.py` & `passwordless-1.0.0/src/passwordless/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,36 @@
 from .errors import PasswordlessError, PasswordlessProblemDetails
 from .models import (
     Alias,
     Credential,
     CredentialDescriptor,
     DeleteCredential,
     DeleteUser,
+    GenerateAuthenticationTokenOptions,
+    GeneratedAuthenticationToken,
     RegisteredToken,
     RegisterToken,
+    SendMagicLinkOptions,
     SetAlias,
     UpdateAppsFeature,
     UserSummary,
     VerifiedUser,
     VerifySignIn,
 )
 from .serialization import (
     AliasSchema,
     CredentialDescriptorSchema,
     CredentialSchema,
     DeleteCredentialSchema,
     DeleteUserSchema,
+    GenerateAuthenticationTokenOptionsSchema,
+    GeneratedAuthenticationTokenSchema,
     PasswordlessProblemDetailsSchema,
     RegisteredTokenSchema,
     RegisterTokenSchema,
+    SendMagicLinkOptionsSchema,
     SetAliasSchema,
     UpdateAppsFeatureSchema,
     UserSummarySchema,
     VerifiedUserSchema,
     VerifySignInSchema,
 )
```

### Comparing `passwordless-0.1.1/src/passwordless/client.py` & `passwordless-1.0.0/src/passwordless/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 from .config import PasswordlessOptions
 from .errors import PasswordlessError, PasswordlessProblemDetails
 from .models import (
     Alias,
     Credential,
     DeleteCredential,
     DeleteUser,
+    GenerateAuthenticationTokenOptions,
+    GeneratedAuthenticationToken,
     ListResponse,
     RegisteredToken,
     RegisterToken,
+    SendMagicLinkOptions,
     SetAlias,
     UpdateAppsFeature,
     UserSummary,
     VerifiedUser,
     VerifySignIn,
 )
 from .serialization import (
     AliasListResponseSchema,
     CredentialListResponseSchema,
     DeleteCredentialSchema,
     DeleteUserSchema,
+    GenerateAuthenticationTokenOptionsSchema,
+    GeneratedAuthenticationTokenSchema,
     PasswordlessProblemDetailsSchema,
     RegisteredTokenSchema,
     RegisterTokenSchema,
+    SendMagicLinkOptionsSchema,
     SetAliasSchema,
     UpdateAppsFeatureSchema,
     UserSummaryListResponseSchema,
     VerifiedUserSchema,
     VerifySignInSchema,
 )
 
@@ -148,14 +154,40 @@
         :param delete_user: `DeleteUser` containing details about the user
             to delete.
         :raises PasswordlessError: If the Passwordless Api responds with
             an error.
         """
         pass
 
+    @abstractmethod
+    def send_magic_link(self, options: SendMagicLinkOptions) -> None:
+        """Sends a magic link.
+
+        :param options: `SendMagicLinkOptions` containing details about the
+            magic link to send.
+        :raises PasswordlessError: If the Passwordless Api responds with
+            an error.
+        """
+        pass
+
+    @abstractmethod
+    def generate_authentication_token(
+        self, options: GenerateAuthenticationTokenOptions
+    ) -> GeneratedAuthenticationToken:
+        """Can be used to implement a "magic link"-style login and other
+        similar scenarios.
+
+        :param options: The options to generate an authentication token.
+        :return: User token details upon successful generation of the
+            token.
+        :raises PasswordlessError: If the Passwordless Api responds with
+            an error.
+        """
+        pass
+
 
 def handle_response_error(response: Response) -> None:
     problem_details = None
     if "Content-Type" in response.headers and response.headers[
         "Content-Type"
     ].startswith("application/problem+json"):
         problem_details_schema = PasswordlessProblemDetailsSchema()
@@ -270,14 +302,41 @@
         schema = DeleteUserSchema()
         request_data = schema.dumps(delete_user)
 
         request = self.__build_post_request("/users/delete", request_data)
 
         self.__send_request(request)
 
+    def send_magic_link(self, options: SendMagicLinkOptions) -> None:
+        request_schema = SendMagicLinkOptionsSchema()
+        request_data = request_schema.dumps(options)
+
+        request = self.__build_post_request("/magic-links/send", request_data)
+
+        self.__send_request(request)
+
+    def generate_authentication_token(
+        self, options: GenerateAuthenticationTokenOptions
+    ) -> GeneratedAuthenticationToken:
+        schema = GenerateAuthenticationTokenOptionsSchema()
+        request_data = schema.dumps(options)
+
+        request = self.__build_post_request(
+            "/signin/generate-token", request_data
+        )
+
+        response = self.__send_request(request)
+
+        response_schema = GeneratedAuthenticationTokenSchema()
+        response_data: GeneratedAuthenticationToken = response_schema.loads(
+            response.text
+        )
+
+        return response_data
+
     def __build_get_request(
         self,
         path: str,
         query_params: Optional[Dict[str, str]] = None,
     ) -> Request:
         if query_params is None:
             query_params = {}
```

### Comparing `passwordless-0.1.1/src/passwordless/errors.py` & `passwordless-1.0.0/src/passwordless/errors.py`

 * *Files identical despite different names*

### Comparing `passwordless-0.1.1/src/passwordless/models.py` & `passwordless-1.0.0/src/passwordless/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,7 +114,26 @@
     credentials_count: int
     last_used_at: datetime
 
 
 @dataclass
 class DeleteUser:
     user_id: str
+
+
+@dataclass
+class SendMagicLinkOptions:
+    email_address: str
+    url_template: str
+    user_id: str
+    time_to_live: Optional[int] = None
+
+
+@dataclass
+class GenerateAuthenticationTokenOptions:
+    user_id: str
+    time_to_live: Optional[int] = None
+
+
+@dataclass
+class GeneratedAuthenticationToken:
+    token: str
```

### Comparing `passwordless-0.1.1/src/passwordless/serialization.py` & `passwordless-1.0.0/src/passwordless/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from marshmallow import EXCLUDE, Schema, fields, post_load
 
 from .errors import PasswordlessProblemDetails
 from .models import (
     Alias,
     Credential,
     CredentialDescriptor,
+    GeneratedAuthenticationToken,
     ListResponse,
     RegisteredToken,
     UserSummary,
     VerifiedUser,
 )
 
 
@@ -215,7 +216,30 @@
 
     class Meta:
         unknown = EXCLUDE
 
 
 class DeleteUserSchema(Schema):
     user_id = fields.Str(data_key="userId", required=True)
+
+
+class SendMagicLinkOptionsSchema(Schema):
+    email_address = fields.Str(data_key="emailAddress", required=True)
+    url_template = fields.Str(data_key="urlTemplate", required=True)
+    user_id = fields.Str(data_key="userId", required=True)
+    time_to_live = fields.Int(data_key="timeToLive", allow_none=True)
+
+
+class GenerateAuthenticationTokenOptionsSchema(Schema):
+    user_id = fields.Str(data_key="userId", required=True)
+    time_to_live = fields.Int(data_key="timeToLive", allow_none=True)
+
+
+class GeneratedAuthenticationTokenSchema(Schema):
+    token = fields.Str(data_key="token", required=True)
+
+    @post_load
+    def make(self, data: Any, **kwargs: Any) -> GeneratedAuthenticationToken:
+        return GeneratedAuthenticationToken(**data)
+
+    class Meta:
+        unknown = EXCLUDE
```

### Comparing `passwordless-0.1.1/PKG-INFO` & `passwordless-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: passwordless
-Version: 0.1.1
+Version: 1.0.0
 Summary: Passwordless.dev Python SDK
 Home-page: https://bitwarden.com/products/passwordless
 License: Apache-2.0
 Keywords: passwordless,bitwarden
 Author: Bitwarden
 Author-email: hello@bitwarden.com
 Maintainer: Maciej Zieniuk
 Maintainer-email: zieniuk.maciej@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: ==3.8.18
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Communications :: FIDO
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: marshmallow (>=3,<4)
-Requires-Dist: python-dateutil (>=2,<3)
-Requires-Dist: requests (>=2,<3)
+Requires-Dist: marshmallow (==3.21.1)
+Requires-Dist: python-dateutil (==2.9.0.post0)
+Requires-Dist: requests (==2.31.0)
 Project-URL: Documentation, https://docs.passwordless.dev/guide
 Description-Content-Type: text/markdown
 
 # Passwordless Python SDK
 
 The official [Bitwarden Passwordless.dev](https://passwordless.dev/) Python library, for Python 3+.
```

