# Comparing `tmp/pulumi_frontegg-0.2.35.tar.gz` & `tmp/pulumi_frontegg-0.2.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_frontegg-0.2.35.tar", last modified: Wed Apr  3 14:20:44 2024, max compression
+gzip compressed data, was "pulumi_frontegg-0.2.36.tar", last modified: Mon Apr  8 00:58:31 2024, max compression
```

## Comparing `pulumi_frontegg-0.2.35.tar` & `pulumi_frontegg-0.2.36.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/pulumi_frontegg/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104037 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/allowed_origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/pulumi_frontegg/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/get_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)   102460 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/permission_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/prehook.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)   126906 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:31.754062 pulumi_frontegg-0.2.36/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 00:58:31.754062 pulumi_frontegg-0.2.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:31.754062 pulumi_frontegg-0.2.36/pulumi_frontegg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104037 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/allowed_origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:31.754062 pulumi_frontegg-0.2.36/pulumi_frontegg/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/get_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102460 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/permission_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/prehook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126191 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/pulumi_frontegg/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:31.754062 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 00:58:31.000000 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 00:58:31.000000 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:58:31.000000 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:58:31.000000 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 00:58:31.000000 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 00:58:31.000000 pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:58:31.754062 pulumi_frontegg-0.2.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 00:58:30.000000 pulumi_frontegg-0.2.36/setup.py
```

### Comparing `pulumi_frontegg-0.2.35/PKG-INFO` & `pulumi_frontegg-0.2.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_frontegg
-Version: 0.2.35
+Version: 0.2.36
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/__init__.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/_inputs.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/_utilities.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,8 +284,8 @@
         await o._future,
         await o._is_known,
         await o._is_secret,
         await o._resources,
     )
 
 def get_plugin_download_url():
-	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.35/"
+	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.36/"
```

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/allowed_origin.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/allowed_origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/config/vars.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/get_permission.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/get_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/outputs.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/permission.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/permission_category.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/permission_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/prehook.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/prehook.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/provider.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/redirect_uri.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/role.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/tenant.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/user.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/webhook.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg/workspace.py` & `pulumi_frontegg-0.2.36/pulumi_frontegg/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                  mfa_policy: pulumi.Input['WorkspaceMfaPolicyArgs'],
                  open_saas_installed: pulumi.Input[bool],
                  password_policy: pulumi.Input['WorkspacePasswordPolicyArgs'],
                  bot_detection_email: Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']] = None,
                  brute_force_protection_email: Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs']] = None,
                  captcha_policy: Optional[pulumi.Input['WorkspaceCaptchaPolicyArgs']] = None,
-                 custom_domain: Optional[pulumi.Input[str]] = None,
+                 custom_domains: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  email_verification_email: Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']] = None,
                  facebook_social_login: Optional[pulumi.Input['WorkspaceFacebookSocialLoginArgs']] = None,
                  github_social_login: Optional[pulumi.Input['WorkspaceGithubSocialLoginArgs']] = None,
                  google_social_login: Optional[pulumi.Input['WorkspaceGoogleSocialLoginArgs']] = None,
                  hosted_login: Optional[pulumi.Input['WorkspaceHostedLoginArgs']] = None,
                  impossible_travel_email: Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']] = None,
                  lockout_policy: Optional[pulumi.Input['WorkspaceLockoutPolicyArgs']] = None,
@@ -76,17 +76,16 @@
         :param pulumi.Input['WorkspaceMfaPolicyArgs'] mfa_policy: Configures the multi-factor authentication (MFA) policy.
         :param pulumi.Input[bool] open_saas_installed: Whether the application associated with the workspace has OpenSaaS installed.
         :param pulumi.Input['WorkspacePasswordPolicyArgs'] password_policy: Configures the password policy.
         :param pulumi.Input['WorkspaceBotDetectionEmailArgs'] bot_detection_email: Configures the bot detection email.
         :param pulumi.Input['WorkspaceBruteForceProtectionEmailArgs'] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs'] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input['WorkspaceCaptchaPolicyArgs'] captcha_policy: Configures the CAPTCHA policy in the signup form.
-        :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-               points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-               that points to your client ID before setting this field.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_domains: List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+               get record values from the portal.
         :param pulumi.Input['WorkspaceEmailVerificationEmailArgs'] email_verification_email: Configures the verification email.
         :param pulumi.Input['WorkspaceFacebookSocialLoginArgs'] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input['WorkspaceGithubSocialLoginArgs'] github_social_login: Configures social login with GitHub.
         :param pulumi.Input['WorkspaceGoogleSocialLoginArgs'] google_social_login: Configures social login with Google.
         :param pulumi.Input['WorkspaceHostedLoginArgs'] hosted_login: Configures Frontegg-hosted OAuth login.
         :param pulumi.Input['WorkspaceImpossibleTravelEmailArgs'] impossible_travel_email: Configures the impossible travel email.
         :param pulumi.Input['WorkspaceLockoutPolicyArgs'] lockout_policy: Configures the user lockout policy.
@@ -129,16 +128,16 @@
             pulumi.set(__self__, "bot_detection_email", bot_detection_email)
         if brute_force_protection_email is not None:
             pulumi.set(__self__, "brute_force_protection_email", brute_force_protection_email)
         if bulk_tenants_invites_email is not None:
             pulumi.set(__self__, "bulk_tenants_invites_email", bulk_tenants_invites_email)
         if captcha_policy is not None:
             pulumi.set(__self__, "captcha_policy", captcha_policy)
-        if custom_domain is not None:
-            pulumi.set(__self__, "custom_domain", custom_domain)
+        if custom_domains is not None:
+            pulumi.set(__self__, "custom_domains", custom_domains)
         if email_verification_email is not None:
             pulumi.set(__self__, "email_verification_email", email_verification_email)
         if facebook_social_login is not None:
             pulumi.set(__self__, "facebook_social_login", facebook_social_login)
         if github_social_login is not None:
             pulumi.set(__self__, "github_social_login", github_social_login)
         if google_social_login is not None:
@@ -365,26 +364,25 @@
         return pulumi.get(self, "captcha_policy")
 
     @captcha_policy.setter
     def captcha_policy(self, value: Optional[pulumi.Input['WorkspaceCaptchaPolicyArgs']]):
         pulumi.set(self, "captcha_policy", value)
 
     @property
-    @pulumi.getter(name="customDomain")
-    def custom_domain(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="customDomains")
+    def custom_domains(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-        points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-        that points to your client ID before setting this field.
-        """
-        return pulumi.get(self, "custom_domain")
-
-    @custom_domain.setter
-    def custom_domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "custom_domain", value)
+        List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+        get record values from the portal.
+        """
+        return pulumi.get(self, "custom_domains")
+
+    @custom_domains.setter
+    def custom_domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "custom_domains", value)
 
     @property
     @pulumi.getter(name="emailVerificationEmail")
     def email_verification_email(self) -> Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']]:
         """
         Configures the verification email.
         """
@@ -763,15 +761,15 @@
                  auth_policy: Optional[pulumi.Input['WorkspaceAuthPolicyArgs']] = None,
                  backend_stack: Optional[pulumi.Input[str]] = None,
                  bot_detection_email: Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']] = None,
                  brute_force_protection_email: Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs']] = None,
                  captcha_policy: Optional[pulumi.Input['WorkspaceCaptchaPolicyArgs']] = None,
                  country: Optional[pulumi.Input[str]] = None,
-                 custom_domain: Optional[pulumi.Input[str]] = None,
+                 custom_domains: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  email_verification_email: Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']] = None,
                  facebook_social_login: Optional[pulumi.Input['WorkspaceFacebookSocialLoginArgs']] = None,
                  frontegg_domain: Optional[pulumi.Input[str]] = None,
                  frontend_stack: Optional[pulumi.Input[str]] = None,
                  github_social_login: Optional[pulumi.Input['WorkspaceGithubSocialLoginArgs']] = None,
                  google_social_login: Optional[pulumi.Input['WorkspaceGoogleSocialLoginArgs']] = None,
                  hosted_login: Optional[pulumi.Input['WorkspaceHostedLoginArgs']] = None,
@@ -812,17 +810,16 @@
         :param pulumi.Input['WorkspaceAuthPolicyArgs'] auth_policy: Configures the general authentication policy.
         :param pulumi.Input[str] backend_stack: The backend stack of the application associated with the workspace.
         :param pulumi.Input['WorkspaceBotDetectionEmailArgs'] bot_detection_email: Configures the bot detection email.
         :param pulumi.Input['WorkspaceBruteForceProtectionEmailArgs'] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs'] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input['WorkspaceCaptchaPolicyArgs'] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] country: The country associated with the workspace.
-        :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-               points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-               that points to your client ID before setting this field.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_domains: List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+               get record values from the portal.
         :param pulumi.Input['WorkspaceEmailVerificationEmailArgs'] email_verification_email: Configures the verification email.
         :param pulumi.Input['WorkspaceFacebookSocialLoginArgs'] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input['WorkspaceGithubSocialLoginArgs'] github_social_login: Configures social login with GitHub.
         :param pulumi.Input['WorkspaceGoogleSocialLoginArgs'] google_social_login: Configures social login with Google.
@@ -871,16 +868,16 @@
             pulumi.set(__self__, "brute_force_protection_email", brute_force_protection_email)
         if bulk_tenants_invites_email is not None:
             pulumi.set(__self__, "bulk_tenants_invites_email", bulk_tenants_invites_email)
         if captcha_policy is not None:
             pulumi.set(__self__, "captcha_policy", captcha_policy)
         if country is not None:
             pulumi.set(__self__, "country", country)
-        if custom_domain is not None:
-            pulumi.set(__self__, "custom_domain", custom_domain)
+        if custom_domains is not None:
+            pulumi.set(__self__, "custom_domains", custom_domains)
         if email_verification_email is not None:
             pulumi.set(__self__, "email_verification_email", email_verification_email)
         if facebook_social_login is not None:
             pulumi.set(__self__, "facebook_social_login", facebook_social_login)
         if frontegg_domain is not None:
             pulumi.set(__self__, "frontegg_domain", frontegg_domain)
         if frontend_stack is not None:
@@ -1056,26 +1053,25 @@
         return pulumi.get(self, "country")
 
     @country.setter
     def country(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "country", value)
 
     @property
-    @pulumi.getter(name="customDomain")
-    def custom_domain(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="customDomains")
+    def custom_domains(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-        points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-        that points to your client ID before setting this field.
-        """
-        return pulumi.get(self, "custom_domain")
-
-    @custom_domain.setter
-    def custom_domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "custom_domain", value)
+        List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+        get record values from the portal.
+        """
+        return pulumi.get(self, "custom_domains")
+
+    @custom_domains.setter
+    def custom_domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "custom_domains", value)
 
     @property
     @pulumi.getter(name="emailVerificationEmail")
     def email_verification_email(self) -> Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']]:
         """
         Configures the verification email.
         """
@@ -1517,15 +1513,15 @@
                  auth_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']]] = None,
                  backend_stack: Optional[pulumi.Input[str]] = None,
                  bot_detection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']]] = None,
                  brute_force_protection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']]] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']]] = None,
                  captcha_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']]] = None,
                  country: Optional[pulumi.Input[str]] = None,
-                 custom_domain: Optional[pulumi.Input[str]] = None,
+                 custom_domains: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  email_verification_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']]] = None,
                  facebook_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']]] = None,
                  frontegg_domain: Optional[pulumi.Input[str]] = None,
                  frontend_stack: Optional[pulumi.Input[str]] = None,
                  github_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']]] = None,
                  google_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']]] = None,
                  hosted_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']]] = None,
@@ -1569,17 +1565,16 @@
         :param pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']] auth_policy: Configures the general authentication policy.
         :param pulumi.Input[str] backend_stack: The backend stack of the application associated with the workspace.
         :param pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']] bot_detection_email: Configures the bot detection email.
         :param pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] country: The country associated with the workspace.
-        :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-               points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-               that points to your client ID before setting this field.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_domains: List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+               get record values from the portal.
         :param pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']] email_verification_email: Configures the verification email.
         :param pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']] github_social_login: Configures social login with GitHub.
         :param pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']] google_social_login: Configures social login with Google.
@@ -1642,15 +1637,15 @@
                  auth_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']]] = None,
                  backend_stack: Optional[pulumi.Input[str]] = None,
                  bot_detection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']]] = None,
                  brute_force_protection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']]] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']]] = None,
                  captcha_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']]] = None,
                  country: Optional[pulumi.Input[str]] = None,
-                 custom_domain: Optional[pulumi.Input[str]] = None,
+                 custom_domains: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  email_verification_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']]] = None,
                  facebook_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']]] = None,
                  frontegg_domain: Optional[pulumi.Input[str]] = None,
                  frontend_stack: Optional[pulumi.Input[str]] = None,
                  github_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']]] = None,
                  google_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']]] = None,
                  hosted_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']]] = None,
@@ -1707,15 +1702,15 @@
             __props__.__dict__["bot_detection_email"] = bot_detection_email
             __props__.__dict__["brute_force_protection_email"] = brute_force_protection_email
             __props__.__dict__["bulk_tenants_invites_email"] = bulk_tenants_invites_email
             __props__.__dict__["captcha_policy"] = captcha_policy
             if country is None and not opts.urn:
                 raise TypeError("Missing required property 'country'")
             __props__.__dict__["country"] = country
-            __props__.__dict__["custom_domain"] = custom_domain
+            __props__.__dict__["custom_domains"] = custom_domains
             __props__.__dict__["email_verification_email"] = email_verification_email
             __props__.__dict__["facebook_social_login"] = facebook_social_login
             if frontegg_domain is None and not opts.urn:
                 raise TypeError("Missing required property 'frontegg_domain'")
             __props__.__dict__["frontegg_domain"] = frontegg_domain
             if frontend_stack is None and not opts.urn:
                 raise TypeError("Missing required property 'frontend_stack'")
@@ -1773,15 +1768,15 @@
             auth_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']]] = None,
             backend_stack: Optional[pulumi.Input[str]] = None,
             bot_detection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']]] = None,
             brute_force_protection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']]] = None,
             bulk_tenants_invites_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']]] = None,
             captcha_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']]] = None,
             country: Optional[pulumi.Input[str]] = None,
-            custom_domain: Optional[pulumi.Input[str]] = None,
+            custom_domains: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             email_verification_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']]] = None,
             facebook_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']]] = None,
             frontegg_domain: Optional[pulumi.Input[str]] = None,
             frontend_stack: Optional[pulumi.Input[str]] = None,
             github_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']]] = None,
             google_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']]] = None,
             hosted_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']]] = None,
@@ -1827,17 +1822,16 @@
         :param pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']] auth_policy: Configures the general authentication policy.
         :param pulumi.Input[str] backend_stack: The backend stack of the application associated with the workspace.
         :param pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']] bot_detection_email: Configures the bot detection email.
         :param pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] country: The country associated with the workspace.
-        :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-               points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-               that points to your client ID before setting this field.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_domains: List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+               get record values from the portal.
         :param pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']] email_verification_email: Configures the verification email.
         :param pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']] github_social_login: Configures social login with GitHub.
         :param pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']] google_social_login: Configures social login with Google.
@@ -1881,15 +1875,15 @@
         __props__.__dict__["auth_policy"] = auth_policy
         __props__.__dict__["backend_stack"] = backend_stack
         __props__.__dict__["bot_detection_email"] = bot_detection_email
         __props__.__dict__["brute_force_protection_email"] = brute_force_protection_email
         __props__.__dict__["bulk_tenants_invites_email"] = bulk_tenants_invites_email
         __props__.__dict__["captcha_policy"] = captcha_policy
         __props__.__dict__["country"] = country
-        __props__.__dict__["custom_domain"] = custom_domain
+        __props__.__dict__["custom_domains"] = custom_domains
         __props__.__dict__["email_verification_email"] = email_verification_email
         __props__.__dict__["facebook_social_login"] = facebook_social_login
         __props__.__dict__["frontegg_domain"] = frontegg_domain
         __props__.__dict__["frontend_stack"] = frontend_stack
         __props__.__dict__["github_social_login"] = github_social_login
         __props__.__dict__["google_social_login"] = google_social_login
         __props__.__dict__["hosted_login"] = hosted_login
@@ -1994,22 +1988,21 @@
     def country(self) -> pulumi.Output[str]:
         """
         The country associated with the workspace.
         """
         return pulumi.get(self, "country")
 
     @property
-    @pulumi.getter(name="customDomain")
-    def custom_domain(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="customDomains")
+    def custom_domains(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
-        points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
-        that points to your client ID before setting this field.
+        List of custom domains at which Frontegg services will be reachable. You must configure CNAME for each domain, you can
+        get record values from the portal.
         """
-        return pulumi.get(self, "custom_domain")
+        return pulumi.get(self, "custom_domains")
 
     @property
     @pulumi.getter(name="emailVerificationEmail")
     def email_verification_email(self) -> pulumi.Output[Optional['outputs.WorkspaceEmailVerificationEmail']]:
         """
         Configures the verification email.
         """
```

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/PKG-INFO` & `pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-frontegg
-Version: 0.2.35
+Version: 0.2.36
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/SOURCES.txt` & `pulumi_frontegg-0.2.36/pulumi_frontegg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.35/setup.py` & `pulumi_frontegg-0.2.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = '0.2.35'
+VERSION = '0.2.36'
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "frontegg Pulumi Package - Development Version"
```

