# Comparing `tmp/descope-1.6.4.tar.gz` & `tmp/descope-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.6.4.tar", max compression
+gzip compressed data, was "descope-1.6.5.tar", max compression
```

## Comparing `descope-1.6.4.tar` & `descope-1.6.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1064 2024-03-14 15:10:58.493838 descope-1.6.4/LICENSE
--rw-r--r--   0        0        0    49684 2024-03-14 15:10:58.493838 descope-1.6.4/README.md
--rw-r--r--   0        0        0     1027 2024-03-14 15:10:58.493838 descope-1.6.4/descope/__init__.py
--rw-r--r--   0        0        0      211 2024-03-14 15:10:58.493838 descope-1.6.4/descope/_auth_base.py
--rw-r--r--   0        0        0    23149 2024-03-14 15:10:58.493838 descope-1.6.4/descope/auth.py
--rw-r--r--   0        0        0        0 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     6427 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     7613 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1578 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    12512 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8970 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/password.py
--rw-r--r--   0        0        0     1596 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/saml.py
--rw-r--r--   0        0        0     1610 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/sso.py
--rw-r--r--   0        0        0     5236 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6806 2024-03-14 15:10:58.493838 descope-1.6.4/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     5890 2024-03-14 15:10:58.493838 descope-1.6.4/descope/common.py
--rw-r--r--   0        0        0    19080 2024-03-14 15:10:58.493838 descope-1.6.4/descope/descope_client.py
--rw-r--r--   0        0        0     1529 2024-03-14 15:10:58.493838 descope-1.6.4/descope/exceptions.py
--rw-r--r--   0        0        0    14840 2024-03-14 15:10:58.493838 descope-1.6.4/descope/flask/__init__.py
--rw-r--r--   0        0        0     6441 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/access_key.py
--rw-r--r--   0        0        0     4759 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/audit.py
--rw-r--r--   0        0        0    14709 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/authz.py
--rw-r--r--   0        0        0    10136 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/common.py
--rw-r--r--   0        0        0     4415 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/flow.py
--rw-r--r--   0        0        0     4001 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/group.py
--rw-r--r--   0        0        0     2245 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/jwt.py
--rw-r--r--   0        0        0     2584 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/permission.py
--rw-r--r--   0        0        0     3003 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/project.py
--rw-r--r--   0        0        0     4864 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/role.py
--rw-r--r--   0        0        0    16808 2024-03-14 15:10:58.493838 descope-1.6.4/descope/management/sso_application.py
--rw-r--r--   0        0        0    20223 2024-03-14 15:10:58.497839 descope-1.6.4/descope/management/sso_settings.py
--rw-r--r--   0        0        0     6456 2024-03-14 15:10:58.497839 descope-1.6.4/descope/management/tenant.py
--rw-r--r--   0        0        0    53833 2024-03-14 15:10:58.497839 descope-1.6.4/descope/management/user.py
--rw-r--r--   0        0        0     3143 2024-03-14 15:10:58.497839 descope-1.6.4/descope/management/user_pwd.py
--rw-r--r--   0        0        0     2242 2024-03-14 15:10:58.497839 descope-1.6.4/descope/mgmt.py
--rw-r--r--   0        0        0        0 2024-03-14 15:10:58.497839 descope-1.6.4/descope/py.typed
--rw-r--r--   0        0        0     2707 2024-03-14 15:11:16.126063 descope-1.6.4/pyproject.toml
--rw-r--r--   0        0        0    51219 1970-01-01 00:00:00.000000 descope-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-08 20:29:41.873686 descope-1.6.5/LICENSE
+-rw-r--r--   0        0        0    49751 2024-04-08 20:29:41.873686 descope-1.6.5/README.md
+-rw-r--r--   0        0        0     1027 2024-04-08 20:29:41.873686 descope-1.6.5/descope/__init__.py
+-rw-r--r--   0        0        0      211 2024-04-08 20:29:41.873686 descope-1.6.5/descope/_auth_base.py
+-rw-r--r--   0        0        0    23684 2024-04-08 20:29:41.873686 descope-1.6.5/descope/auth.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:29:41.873686 descope-1.6.5/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     6427 2024-04-08 20:29:41.873686 descope-1.6.5/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     7613 2024-04-08 20:29:41.873686 descope-1.6.5/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1578 2024-04-08 20:29:41.873686 descope-1.6.5/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    12587 2024-04-08 20:29:41.873686 descope-1.6.5/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8970 2024-04-08 20:29:41.877686 descope-1.6.5/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1596 2024-04-08 20:29:41.877686 descope-1.6.5/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     1610 2024-04-08 20:29:41.877686 descope-1.6.5/descope/authmethod/sso.py
+-rw-r--r--   0        0        0     5236 2024-04-08 20:29:41.877686 descope-1.6.5/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6806 2024-04-08 20:29:41.877686 descope-1.6.5/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     5904 2024-04-08 20:29:41.877686 descope-1.6.5/descope/common.py
+-rw-r--r--   0        0        0    19080 2024-04-08 20:29:41.877686 descope-1.6.5/descope/descope_client.py
+-rw-r--r--   0        0        0     1529 2024-04-08 20:29:41.877686 descope-1.6.5/descope/exceptions.py
+-rw-r--r--   0        0        0    16150 2024-04-08 20:29:41.877686 descope-1.6.5/descope/flask/__init__.py
+-rw-r--r--   0        0        0     6441 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/access_key.py
+-rw-r--r--   0        0        0     4759 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/audit.py
+-rw-r--r--   0        0        0    14709 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/authz.py
+-rw-r--r--   0        0        0    10136 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/common.py
+-rw-r--r--   0        0        0     4415 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/flow.py
+-rw-r--r--   0        0        0     4001 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/group.py
+-rw-r--r--   0        0        0     2245 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/jwt.py
+-rw-r--r--   0        0        0     2584 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/permission.py
+-rw-r--r--   0        0        0     3003 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/project.py
+-rw-r--r--   0        0        0     4864 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/role.py
+-rw-r--r--   0        0        0    16808 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/sso_application.py
+-rw-r--r--   0        0        0    20223 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     6456 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/tenant.py
+-rw-r--r--   0        0        0    53883 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/user.py
+-rw-r--r--   0        0        0     3143 2024-04-08 20:29:41.877686 descope-1.6.5/descope/management/user_pwd.py
+-rw-r--r--   0        0        0     2242 2024-04-08 20:29:41.877686 descope-1.6.5/descope/mgmt.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:29:41.877686 descope-1.6.5/descope/py.typed
+-rw-r--r--   0        0        0     2707 2024-04-08 20:30:02.329649 descope-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0    51286 1970-01-01 00:00:00.000000 descope-1.6.5/PKG-INFO
```

### Comparing `descope-1.6.4/LICENSE` & `descope-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/README.md` & `descope-1.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 If you're performing end-to-end testing, check out the [Utils for your end to end (e2e) tests and integration tests](#utils-for-your-end-to-end-e2e-tests-and-integration-tests) section. You will need to use the `DescopeClient` object created under [Setup](#setup-1) guide.
 
 For rate limiting information, please confer to the [API Rate Limits](#api-rate-limits) section.
 
 ### OTP Authentication
 
-Send a user a one-time password (OTP) using your preferred delivery method (_email / SMS_). An email address or phone number must be provided accordingly.
+Send a user a one-time password (OTP) using your preferred delivery method (_email / SMS / Voice call / WhatsApp_). An email address or phone number must be provided accordingly.
 
 The user can either `sign up`, `sign in` or `sign up or in`
 
 ```python
 from descope import DeliveryMethod
 
 # Every user must have a login ID. All other user information is optional
@@ -104,15 +104,15 @@
 refresh_token = jwt_response[REFRESH_SESSION_TOKEN_NAME].get("jwt")
 ```
 
 The session and refresh JWTs should be returned to the caller, and passed with every request in the session. Read more on [session validation](#session-validation)
 
 ### Magic Link
 
-Send a user a Magic Link using your preferred delivery method (_email / SMS_).
+Send a user a Magic Link using your preferred delivery method (_email / SMS / Voice call / WhatsApp_).
 The Magic Link will redirect the user to page where the its token needs to be verified.
 This redirection can be configured in code, or generally in the [Descope Console](https://app.descope.com/settings/authentication/magiclink)
 
 The user can either `sign up`, `sign in` or `sign up or in`
 
 ```python
 from descope import DeliveryMethod
@@ -1325,15 +1325,15 @@
 apps = apps_resp["apps"]
     for app in apps:
         # Do something
 
 ### Utils for your end to end (e2e) tests and integration tests
 
 To ease your e2e tests, we exposed dedicated management methods,
-that way, you don't need to use 3rd party messaging services in order to receive sign-in/up Emails or SMS, and avoid the need of parsing the code and token from them.
+that way, you don't need to use 3rd party messaging services in order to receive sign-in/up Email, SMS, Voice call, WhatsApp, and avoid the need of parsing the code and token from them.
 
 ```Python
 # User for test can be created, this user will be able to generate code/link without
 # the need of 3rd party messaging services.
 # Test user must have a loginId, other fields are optional.
 # Roles should be set directly if no tenants exist, otherwise set
 # on a per-tenant basis.
```

### Comparing `descope-1.6.4/descope/__init__.py` & `descope-1.6.5/descope/__init__.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/auth.py` & `descope-1.6.5/descope/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,19 @@
             except EmailNotValidError:
                 return False
         elif method == DeliveryMethod.SMS:
             if not user.get("phone", None):
                 user["phone"] = login_id
             if not re.match(PHONE_REGEX, user["phone"]):
                 return False
+        elif method == DeliveryMethod.VOICE:
+            if not user.get("phone", None):
+                user["phone"] = login_id
+            if not re.match(PHONE_REGEX, user["phone"]):
+                return False
         elif method == DeliveryMethod.WHATSAPP:
             if not user.get("phone", None):
                 user["phone"] = login_id
             if not re.match(PHONE_REGEX, user["phone"]):
                 return False
         else:
             return False
@@ -226,14 +231,15 @@
         return True
 
     @staticmethod
     def compose_url(base: str, method: DeliveryMethod) -> str:
         suffix = {
             DeliveryMethod.EMAIL: "email",
             DeliveryMethod.SMS: "sms",
+            DeliveryMethod.VOICE: "voice",
             DeliveryMethod.WHATSAPP: "whatsapp",
         }.get(method)
 
         if not suffix:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
             )
@@ -241,14 +247,15 @@
         return f"{base}/{suffix}"
 
     @staticmethod
     def get_login_id_by_method(method: DeliveryMethod, user: dict) -> tuple[str, str]:
         login_id = {
             DeliveryMethod.EMAIL: ("email", user.get("email", "")),
             DeliveryMethod.SMS: ("phone", user.get("phone", "")),
+            DeliveryMethod.VOICE: ("voice", user.get("phone", "")),
             DeliveryMethod.WHATSAPP: ("whatsapp", user.get("phone", "")),
         }.get(method)
 
         if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
             )
@@ -256,14 +263,15 @@
         return login_id
 
     @staticmethod
     def get_method_string(method: DeliveryMethod) -> str:
         name = {
             DeliveryMethod.EMAIL: "email",
             DeliveryMethod.SMS: "sms",
+            DeliveryMethod.VOICE: "voice",
             DeliveryMethod.WHATSAPP: "whatsapp",
             DeliveryMethod.EMBEDDED: "Embedded",
         }.get(method)
 
         if not name:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
@@ -297,15 +305,19 @@
             )
 
         if not re.match(PHONE_REGEX, phone):
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Invalid phone number"
             )
 
-        if method != DeliveryMethod.SMS and method != DeliveryMethod.WHATSAPP:
+        if (
+            method != DeliveryMethod.SMS
+            and method != DeliveryMethod.VOICE
+            and method != DeliveryMethod.WHATSAPP
+        ):
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Invalid delivery method"
             )
 
     def exchange_access_key(
         self,
         access_key: str,
@@ -665,12 +677,16 @@
         jwt_response = self.generate_jwt_response(
             resp, response.cookies.get(REFRESH_SESSION_COOKIE_NAME, None), None
         )
         return jwt_response
 
     @staticmethod
     def extract_masked_address(response: dict, method: DeliveryMethod) -> str:
-        if method == DeliveryMethod.SMS or method == DeliveryMethod.WHATSAPP:
+        if (
+            method == DeliveryMethod.SMS
+            or method == DeliveryMethod.VOICE
+            or method == DeliveryMethod.WHATSAPP
+        ):
             return response["maskedPhone"]
         elif method == DeliveryMethod.EMAIL:
             return response["maskedEmail"]
         return ""
```

### Comparing `descope-1.6.4/descope/authmethod/enchantedlink.py` & `descope-1.6.5/descope/authmethod/enchantedlink.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/magiclink.py` & `descope-1.6.5/descope/authmethod/magiclink.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/oauth.py` & `descope-1.6.5/descope/authmethod/oauth.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/otp.py` & `descope-1.6.5/descope/authmethod/otp.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         Sign in (log in) an existing user with the unique login_id you provide. (See 'sign_up' function for an explanation of the
             login_id field.) Provide the DeliveryMethod required for this user. If the login_id value cannot be used for the
             DeliverMethod selected (for example, 'login_id = 4567qq445km' and 'DeliveryMethod = email')
 
         Args:
         method (DeliveryMethod): The method to use for delivering the OTP verification code to the user, for example
-            email, SMS, or WhatsApp
+            Email, SMS, Voice call, or WhatsApp
         login_id (str): The login ID of the user being validated for example phone or email
         login_options (LoginOptions): Optional advanced controls over login parameters
         refresh_token: Optional refresh token is needed for specific login options
 
         Raise:
         AuthException: raised if sign-in operation fails
         """
@@ -54,15 +54,15 @@
         method: DeliveryMethod,
         login_id: str,
         user: dict | None = None,
         signup_options: SignUpOptions | None = None,
     ) -> str:
         """
         Sign up (create) a new user using their email or phone number. Choose a delivery method for OTP
-            verification, for example email, SMS, or WhatsApp.
+            verification, for example Email, SMS, Voice call, or WhatsApp.
             (optional) Include additional user metadata that you wish to preserve.
 
         Args:
         method (DeliveryMethod): The method to use for delivering the OTP verification code, for example phone or email
         login_id (str): The login ID of the user being validated
         user (dict) optional: Preserve additional user metadata in the form of
              {"name": "Joe Person", "phone": "2125551212", "email": "joe@somecompany.com"}
@@ -95,15 +95,15 @@
         """
         Sign_up_or_in lets you handle both sign up and sign in with a single call. Sign-up_or_in will first determine if
             login_id is a new or existing end user. If login_id is new, a new end user user will be created and then
             authenticated using the OTP DeliveryMethod specified. If login_id exists, the end user will be authenticated
             using the OTP DeliveryMethod specified.
 
         Args:
-        method (DeliveryMethod): The method to use for delivering the OTP verification code, for example phone or email
+        method (DeliveryMethod): The method to use for delivering the OTP verification code, for example Email, SMS, Voice call, or WhatsApp
         login_id (str): The Login ID of the user being validated
 
         Raise:
         AuthException: raised if either the sign_up or sign_in operation fails
         """
         if not login_id:
             raise AuthException(
@@ -126,15 +126,15 @@
 
     def verify_code(self, method: DeliveryMethod, login_id: str, code: str) -> dict:
         """
         Verify the validity of an OTP code entered by an end user during sign_in or sign_up.
         (This function is not needed if you are using the sign_up_or_in function.
 
         Args:
-        method (DeliveryMethod): The method to use for delivering the OTP verification code, for example phone or email
+        method (DeliveryMethod): The method to use for delivering the OTP verification code, for example Email, SMS, Voice call, or WhatsApp
         login_id (str): The Login ID of the user being validated
         code (str): The authorization code enter by the end user during signup/signin
 
         Return value (dict):
         Return dict in the format
              {"jwts": [], "user": "", "firstSeen": "", "error": ""}
         Includes all the jwts tokens (session token, refresh token), token claims, and user information
@@ -202,15 +202,15 @@
         on_merge_use_existing: bool = False,
         template_options: dict | None = None,
     ) -> str:
         """
         Update the phone number of an existing end user, after verifying the authenticity of the end user using OTP.
 
         Args:
-        method (DeliveryMethod): The method to use for delivering the OTP verification code, for example phone or email
+        method (DeliveryMethod): The method to use for delivering the OTP verification code, for example Email, SMS, Voice call, or WhatsApp
         login_id (str): The login ID of the user whose information is being updated
         phone (str): The new phone number. If a phone number already exists for this end user, it will be overwritten
         refresh_token (str): The session's refresh token (used for OTP verification)
         add_to_login_ids (bool): Defaults to false, determine whether to add this email to the login ids of hte user or not
         on_merge_use_existing (bool): Defaults to false, In case add_to_login_ids and there is such a user already
             determine whether keep the existing user, or this new one
 
@@ -226,15 +226,15 @@
         Auth.validate_phone(method, phone)
 
         uri = OTP._compose_update_phone_url(method)
         body = OTP._compose_update_user_phone_body(
             login_id, phone, add_to_login_ids, on_merge_use_existing, template_options
         )
         response = self._auth.do_post(uri, body, None, refresh_token)
-        return Auth.extract_masked_address(response.json(), DeliveryMethod.SMS)
+        return Auth.extract_masked_address(response.json(), method)
 
     @staticmethod
     def _compose_signup_url(method: DeliveryMethod) -> str:
         return Auth.compose_url(EndpointsV1.sign_up_auth_otp_path, method)
 
     @staticmethod
     def _compose_signin_url(method: DeliveryMethod) -> str:
```

### Comparing `descope-1.6.4/descope/authmethod/password.py` & `descope-1.6.5/descope/authmethod/password.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/saml.py` & `descope-1.6.5/descope/authmethod/saml.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/sso.py` & `descope-1.6.5/descope/authmethod/sso.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/totp.py` & `descope-1.6.5/descope/authmethod/totp.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/authmethod/webauthn.py` & `descope-1.6.5/descope/authmethod/webauthn.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/common.py` & `descope-1.6.5/descope/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 
 class DeliveryMethod(Enum):
     WHATSAPP = 1
     SMS = 2
     EMAIL = 3
     EMBEDDED = 4
+    VOICE = 5
 
 
 class LoginOptions:
     def __init__(
         self,
         stepup: bool = False,
         mfa: bool = False,
```

### Comparing `descope-1.6.4/descope/descope_client.py` & `descope-1.6.5/descope/descope_client.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/exceptions.py` & `descope-1.6.5/descope/exceptions.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/flask/__init__.py` & `descope-1.6.5/descope/flask/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,17 +198,17 @@
             return response
 
         return decorated
 
     return decorator
 
 
-def descope_verify_code_by_phone(descope_client: DescopeClient):
+def descope_verify_code_by_phone_sms(descope_client: DescopeClient):
     """
-    Verify code by email decorator
+    Verify code by phone sms decorator
     """
 
     def decorator(f):
         @wraps(f)
         def decorated(*args, **kwargs):
             data = request.get_json(force=True)
             phone = data.get("phone", None)
@@ -241,17 +241,60 @@
             return response
 
         return decorated
 
     return decorator
 
 
-def descope_verify_code_by_whatsapp(descope_client: DescopeClient):
+def descope_verify_code_by_phone_voice_call(descope_client: DescopeClient):
     """
-    Verify code by whatsapp decorator
+    Verify code by phone voice call decorator
+    """
+
+    def decorator(f):
+        @wraps(f)
+        def decorated(*args, **kwargs):
+            data = request.get_json(force=True)
+            phone = data.get("phone", None)
+            code = data.get("code", None)
+            if not code or not phone:
+                return Response("Unauthorized", 401)
+
+            try:
+                jwt_response = descope_client.otp.verify_code(
+                    DeliveryMethod.VOICE, phone, code
+                )
+            except AuthException:
+                return Response("Unauthorized", 401)
+
+            # Save the claims on the context execute the original API
+            _request_ctx_stack.top.claims = jwt_response
+            response = f(*args, **kwargs)
+
+            set_cookie_on_response(
+                response,
+                jwt_response[SESSION_TOKEN_NAME],
+                jwt_response[COOKIE_DATA_NAME],
+            )
+            set_cookie_on_response(
+                response,
+                jwt_response[REFRESH_SESSION_TOKEN_NAME],
+                jwt_response[COOKIE_DATA_NAME],
+            )
+
+            return response
+
+        return decorated
+
+    return decorator
+
+
+def descope_verify_code_by_phone_whatsapp(descope_client: DescopeClient):
+    """
+    Verify code by phone whatsapp decorator
     """
 
     def decorator(f):
         @wraps(f)
         def decorated(*args, **kwargs):
             data = request.get_json(force=True)
             phone = data.get("phone", None)
```

### Comparing `descope-1.6.4/descope/management/access_key.py` & `descope-1.6.5/descope/management/access_key.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/audit.py` & `descope-1.6.5/descope/management/audit.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/authz.py` & `descope-1.6.5/descope/management/authz.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/common.py` & `descope-1.6.5/descope/management/common.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/flow.py` & `descope-1.6.5/descope/management/flow.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/group.py` & `descope-1.6.5/descope/management/group.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/jwt.py` & `descope-1.6.5/descope/management/jwt.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/permission.py` & `descope-1.6.5/descope/management/permission.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/project.py` & `descope-1.6.5/descope/management/project.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/role.py` & `descope-1.6.5/descope/management/role.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/sso_application.py` & `descope-1.6.5/descope/management/sso_application.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/sso_settings.py` & `descope-1.6.5/descope/management/sso_settings.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/tenant.py` & `descope-1.6.5/descope/management/tenant.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/management/user.py` & `descope-1.6.5/descope/management/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1306,22 +1306,22 @@
     ) -> dict:
         """
         Generate OTP for the given login ID of a test user.
         This is useful when running tests and don't want to use 3rd party messaging services.
 
         Args:
         method (DeliveryMethod): The method to use for "delivering" the OTP verification code to the user, for example
-            EMAIL, SMS, WHATSAPP or EMBEDDED
+            EMAIL, SMS, VOICE, WHATSAPP or EMBEDDED
         login_id (str): The login ID of the test user being validated.
         login_options (LoginOptions): optional, can be provided to set custom claims to the generated jwt.
 
         Return value (dict):
         Return dict in the format
              {"code": "", "loginId": ""}
-        Containing the code for the login (exactly as it sent via Email or SMS).
+        Containing the code for the login (exactly as it sent via Email or Phone messaging).
 
         Raise:
         AuthException: raised if the operation fails
         """
         response = self._auth.do_post(
             MgmtV1.user_generate_otp_for_test_path,
             {
@@ -1342,23 +1342,23 @@
     ) -> dict:
         """
         Generate Magic Link for the given login ID of a test user.
         This is useful when running tests and don't want to use 3rd party messaging services.
 
         Args:
         method (DeliveryMethod): The method to use for "delivering" the verification magic link to the user, for example
-            EMAIL, SMS, WHATSAPP or EMBEDDED
+            EMAIL, SMS, VOICE, WHATSAPP or EMBEDDED
         login_id (str): The login ID of the test user being validated.
         uri (str): Optional redirect uri which will be used instead of any global configuration.
         login_options (LoginOptions): optional, can be provided to set custom claims to the generated jwt.
 
         Return value (dict):
         Return dict in the format
              {"link": "", "loginId": ""}
-        Containing the magic link for the login (exactly as it sent via Email or SMS).
+        Containing the magic link for the login (exactly as it sent via Email or Phone messaging).
 
         Raise:
         AuthException: raised if the operation fails
         """
         response = self._auth.do_post(
             MgmtV1.user_generate_magic_link_for_test_path,
             {
@@ -1385,15 +1385,15 @@
         login_id (str): The login ID of the test user being validated.
         uri (str): Optional redirect uri which will be used instead of any global configuration.
         login_options (LoginOptions): optional, can be provided to set custom claims to the generated jwt.
 
         Return value (dict):
         Return dict in the format
              {"link": "", "loginId": "", "pendingRef": ""}
-        Containing the enchanted link for the login (exactly as it sent via Email or SMS) and pendingRef.
+        Containing the enchanted link for the login (exactly as it sent via Email or Phone messaging) and pendingRef.
 
         Raise:
         AuthException: raised if the operation fails
         """
         response = self._auth.do_post(
             MgmtV1.user_generate_enchanted_link_for_test_path,
             {
```

### Comparing `descope-1.6.4/descope/management/user_pwd.py` & `descope-1.6.5/descope/management/user_pwd.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/descope/mgmt.py` & `descope-1.6.5/descope/mgmt.py`

 * *Files identical despite different names*

### Comparing `descope-1.6.4/pyproject.toml` & `descope-1.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.6.4"
+version = "1.6.5"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
@@ -56,15 +56,15 @@
 flake8-bugbear = {version = "24.1.17", python = ">=3.8.1"}
 liccheck = "0.9.2"
 isort = {version = "5.13.2", python = ">=3.8"}
 pep8-naming = {version = "0.13.3", python = ">=3.8"}
 tox = {version = "4.12.1", python = ">=3.8"}
 
 [tool.poetry.group.format.dependencies]
-black = {version = "24.1.1", python = ">=3.8"}
+black = {version = "24.3.0", python = ">=3.8"}
 
 [tool.poetry.group.types.dependencies]
 mypy = {version = "1.8.0", python = ">=3.8"}
 types-requests = {version = "2.31.0.20240125", python = ">=3.8"}
 types-setuptools = {version = "69.0.0.20240125", python = ">=3.8"}
 
 [tool.poetry.group.tests.dependencies]
```

### Comparing `descope-1.6.4/PKG-INFO` & `descope-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.6.4
+Version: 1.6.5
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
 
 If you're performing end-to-end testing, check out the [Utils for your end to end (e2e) tests and integration tests](#utils-for-your-end-to-end-e2e-tests-and-integration-tests) section. You will need to use the `DescopeClient` object created under [Setup](#setup-1) guide.
 
 For rate limiting information, please confer to the [API Rate Limits](#api-rate-limits) section.
 
 ### OTP Authentication
 
-Send a user a one-time password (OTP) using your preferred delivery method (_email / SMS_). An email address or phone number must be provided accordingly.
+Send a user a one-time password (OTP) using your preferred delivery method (_email / SMS / Voice call / WhatsApp_). An email address or phone number must be provided accordingly.
 
 The user can either `sign up`, `sign in` or `sign up or in`
 
 ```python
 from descope import DeliveryMethod
 
 # Every user must have a login ID. All other user information is optional
@@ -139,15 +139,15 @@
 refresh_token = jwt_response[REFRESH_SESSION_TOKEN_NAME].get("jwt")
 ```
 
 The session and refresh JWTs should be returned to the caller, and passed with every request in the session. Read more on [session validation](#session-validation)
 
 ### Magic Link
 
-Send a user a Magic Link using your preferred delivery method (_email / SMS_).
+Send a user a Magic Link using your preferred delivery method (_email / SMS / Voice call / WhatsApp_).
 The Magic Link will redirect the user to page where the its token needs to be verified.
 This redirection can be configured in code, or generally in the [Descope Console](https://app.descope.com/settings/authentication/magiclink)
 
 The user can either `sign up`, `sign in` or `sign up or in`
 
 ```python
 from descope import DeliveryMethod
@@ -1360,15 +1360,15 @@
 apps = apps_resp["apps"]
     for app in apps:
         # Do something
 
 ### Utils for your end to end (e2e) tests and integration tests
 
 To ease your e2e tests, we exposed dedicated management methods,
-that way, you don't need to use 3rd party messaging services in order to receive sign-in/up Emails or SMS, and avoid the need of parsing the code and token from them.
+that way, you don't need to use 3rd party messaging services in order to receive sign-in/up Email, SMS, Voice call, WhatsApp, and avoid the need of parsing the code and token from them.
 
 ```Python
 # User for test can be created, this user will be able to generate code/link without
 # the need of 3rd party messaging services.
 # Test user must have a loginId, other fields are optional.
 # Roles should be set directly if no tenants exist, otherwise set
 # on a per-tenant basis.
```

