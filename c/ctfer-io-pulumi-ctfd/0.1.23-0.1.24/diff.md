# Comparing `tmp/ctfer-io_pulumi-ctfd-0.1.23.tar.gz` & `tmp/ctfer-io_pulumi-ctfd-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfer-io_pulumi-ctfd-0.1.23.tar", last modified: Wed Apr  3 07:03:11 2024, max compression
+gzip compressed data, was "ctfer-io_pulumi-ctfd-0.1.24.tar", last modified: Mon Apr  8 21:19:54 2024, max compression
```

## Comparing `ctfer-io_pulumi-ctfd-0.1.23.tar` & `ctfer-io_pulumi-ctfd-0.1.24.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:03:11.587759 ctfer-io_pulumi-ctfd-0.1.23/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 07:03:11.587759 ctfer-io_pulumi-ctfd-0.1.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:03:11.583759 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    45926 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/challenge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:03:11.583759 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/get_challenges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23775 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    24618 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:03:11.587759 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:03:11.587759 ctfer-io_pulumi-ctfd-0.1.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 07:03:11.000000 ctfer-io_pulumi-ctfd-0.1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:19:54.139088 ctfer-io_pulumi-ctfd-0.1.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-08 21:19:54.139088 ctfer-io_pulumi-ctfd-0.1.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:19:54.139088 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45584 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/challenge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:19:54.139088 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/get_challenges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24566 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24304 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:19:54.139088 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-08 21:19:54.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-08 21:19:54.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:19:54.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:19:54.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 21:19:54.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 21:19:54.000000 ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:19:54.139088 ctfer-io_pulumi-ctfd-0.1.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-08 21:19:53.000000 ctfer-io_pulumi-ctfd-0.1.24/setup.py
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/PKG-INFO` & `ctfer-io_pulumi-ctfd-0.1.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfer-io_pulumi-ctfd
-Version: 0.1.23
+Version: 0.1.24
 Summary: The CTFd provider for Pulumi, to manage its resources as code.
 Home-page: https://ctfer.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ctfer-io/pulumi-ctfd
 Keywords: pulumi ctfd category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctfer-io_pulumi-ctfd Version: 0.1.23 Summary: The
+Metadata-Version: 2.1 Name: ctfer-io_pulumi-ctfd Version: 0.1.24 Summary: The
 CTFd provider for Pulumi, to manage its resources as code. Home-page: https://
 ctfer.io License: Apache-2.0 Project-URL: Repository, https://github.com/ctfer-
 io/pulumi-ctfd Keywords: pulumi ctfd category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown
                ************ [[rreess//ccttffdd..ppnngg]]PPuulluummii CCTTFFdd PPrroovviiddeerr ************
                             LLeett''ss ccooddee yyoouurr CCTTFF((dd))
                              _[_r_e_f_e_r_e_n_c_e_][License]
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/README.md` & `ctfer-io_pulumi-ctfd-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/__init__.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/__init__.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/_inputs.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/_inputs.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/_utilities.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/_utilities.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/challenge.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,22 +627,14 @@
                  value: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         CTFd is built around the Challenge resource, which contains all the attributes to define a part of the Capture The Flag event.
 
         This provider builds a cleaner API on top of CTFd's one to improve its adoption and lifecycle management.
 
-        ## Import
-
-        Challenge can be imported by the CTFd ID (check URLs)
-
-        ```sh
-        $ pulumi import ctfd:index/challenge:Challenge http 1
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] category: Category of the challenge that CTFd groups by on the web UI.
         :param pulumi.Input[str] connection_info: Connection Information to connect to the challenge instance, useful for pwn, web and infrastructure pentests.
         :param pulumi.Input[int] decay: The decay defines from each number of solves does the decay function triggers until reaching minimum. This function is defined by CTFd and could be configured through `.function`.
         :param pulumi.Input[str] description: Description of the challenge, consider using multiline descriptions for better style.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ChallengeFileArgs']]]] files: List of files given to players to flag the challenge.
@@ -667,22 +659,14 @@
                  args: ChallengeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         CTFd is built around the Challenge resource, which contains all the attributes to define a part of the Capture The Flag event.
 
         This provider builds a cleaner API on top of CTFd's one to improve its adoption and lifecycle management.
 
-        ## Import
-
-        Challenge can be imported by the CTFd ID (check URLs)
-
-        ```sh
-        $ pulumi import ctfd:index/challenge:Challenge http 1
-        ```
-
         :param str resource_name: The name of the resource.
         :param ChallengeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ChallengeArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/config/vars.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/config/vars.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/get_challenges.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/get_challenges.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/get_teams.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/get_teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         """
         return pulumi.get(self, "banned")
 
     @property
     @pulumi.getter
     def captain(self) -> str:
         """
-        Member who is captain of the team. Must be part of the members too.
+        Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         """
         return pulumi.get(self, "captain")
 
     @property
     @pulumi.getter
     def country(self) -> str:
         """
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/get_users.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/get_users.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/outputs.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/outputs.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/provider.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/provider.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/team.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/team.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  banned: Optional[pulumi.Input[bool]] = None,
                  country: Optional[pulumi.Input[str]] = None,
                  hidden: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  website: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Team resource.
-        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too.
+        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         :param pulumi.Input[str] email: Email of the team.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of members (User), defined by their IDs.
         :param pulumi.Input[str] password: Password of the team. Notice that during a CTF you may not want to update those to avoid defaulting team accesses.
         :param pulumi.Input[str] affiliation: Affiliation to a company or agency.
         :param pulumi.Input[bool] banned: Is true if the team is banned from the CTF.
         :param pulumi.Input[str] country: Country the team represent or is hail from.
         :param pulumi.Input[bool] hidden: Is true if the team is hidden to the participants.
@@ -54,15 +54,15 @@
         if website is not None:
             pulumi.set(__self__, "website", website)
 
     @property
     @pulumi.getter
     def captain(self) -> pulumi.Input[str]:
         """
-        Member who is captain of the team. Must be part of the members too.
+        Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         """
         return pulumi.get(self, "captain")
 
     @captain.setter
     def captain(self, value: pulumi.Input[str]):
         pulumi.set(self, "captain", value)
 
@@ -188,15 +188,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  website: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Team resources.
         :param pulumi.Input[str] affiliation: Affiliation to a company or agency.
         :param pulumi.Input[bool] banned: Is true if the team is banned from the CTF.
-        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too.
+        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         :param pulumi.Input[str] country: Country the team represent or is hail from.
         :param pulumi.Input[str] email: Email of the team.
         :param pulumi.Input[bool] hidden: Is true if the team is hidden to the participants.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of members (User), defined by their IDs.
         :param pulumi.Input[str] name: Name of the team.
         :param pulumi.Input[str] password: Password of the team. Notice that during a CTF you may not want to update those to avoid defaulting team accesses.
         :param pulumi.Input[str] website: Website, blog, or anything similar (displayed to other participants).
@@ -246,15 +246,15 @@
     def banned(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "banned", value)
 
     @property
     @pulumi.getter
     def captain(self) -> Optional[pulumi.Input[str]]:
         """
-        Member who is captain of the team. Must be part of the members too.
+        Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         """
         return pulumi.get(self, "captain")
 
     @captain.setter
     def captain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "captain", value)
 
@@ -376,27 +376,19 @@
             email="lucastesson@protonmail.com",
             password="password",
             members=[ctfer.id],
             captain=ctfer.id)
         ```
         <!--End PulumiCodeChooser -->
 
-        ## Import
-
-        User can be imported by the CTFd ID (check URLs)
-
-        ```sh
-        $ pulumi import ctfd:index/team:Team cybercombattants 1
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] affiliation: Affiliation to a company or agency.
         :param pulumi.Input[bool] banned: Is true if the team is banned from the CTF.
-        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too.
+        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         :param pulumi.Input[str] country: Country the team represent or is hail from.
         :param pulumi.Input[str] email: Email of the team.
         :param pulumi.Input[bool] hidden: Is true if the team is hidden to the participants.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of members (User), defined by their IDs.
         :param pulumi.Input[str] name: Name of the team.
         :param pulumi.Input[str] password: Password of the team. Notice that during a CTF you may not want to update those to avoid defaulting team accesses.
         :param pulumi.Input[str] website: Website, blog, or anything similar (displayed to other participants).
@@ -424,22 +416,14 @@
             email="lucastesson@protonmail.com",
             password="password",
             members=[ctfer.id],
             captain=ctfer.id)
         ```
         <!--End PulumiCodeChooser -->
 
-        ## Import
-
-        User can be imported by the CTFd ID (check URLs)
-
-        ```sh
-        $ pulumi import ctfd:index/team:Team cybercombattants 1
-        ```
-
         :param str resource_name: The name of the resource.
         :param TeamArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TeamArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -513,15 +497,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] affiliation: Affiliation to a company or agency.
         :param pulumi.Input[bool] banned: Is true if the team is banned from the CTF.
-        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too.
+        :param pulumi.Input[str] captain: Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         :param pulumi.Input[str] country: Country the team represent or is hail from.
         :param pulumi.Input[str] email: Email of the team.
         :param pulumi.Input[bool] hidden: Is true if the team is hidden to the participants.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of members (User), defined by their IDs.
         :param pulumi.Input[str] name: Name of the team.
         :param pulumi.Input[str] password: Password of the team. Notice that during a CTF you may not want to update those to avoid defaulting team accesses.
         :param pulumi.Input[str] website: Website, blog, or anything similar (displayed to other participants).
@@ -558,15 +542,15 @@
         """
         return pulumi.get(self, "banned")
 
     @property
     @pulumi.getter
     def captain(self) -> pulumi.Output[str]:
         """
-        Member who is captain of the team. Must be part of the members too.
+        Member who is captain of the team. Must be part of the members too. Note it could cause a fatal error in case of resource import with an inconsistent CTFd configuration i.e. if a team has no captain yet (should not be possible).
         """
         return pulumi.get(self, "captain")
 
     @property
     @pulumi.getter
     def country(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer-io_pulumi-ctfd/user.py` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer-io_pulumi-ctfd/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,22 +393,14 @@
                  type: Optional[pulumi.Input[str]] = None,
                  verified: Optional[pulumi.Input[bool]] = None,
                  website: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         CTFd defines a User as someone who will either play or administrate the Capture The Flag event.
 
-        ## Import
-
-        User can be imported by the CTFd ID (check URLs)
-
-        ```sh
-        $ pulumi import ctfd:index/user:User ctfer 1
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] affiliation: Affiliation to a team, company or agency.
         :param pulumi.Input[bool] banned: Is true if the user is banned from the CTF.
         :param pulumi.Input[str] country: Country the user represent or is native from.
         :param pulumi.Input[str] email: Email of the user, may be used to verify the account.
         :param pulumi.Input[bool] hidden: Is true if the user is hidden to the participants.
@@ -424,22 +416,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         CTFd defines a User as someone who will either play or administrate the Capture The Flag event.
 
-        ## Import
-
-        User can be imported by the CTFd ID (check URLs)
-
-        ```sh
-        $ pulumi import ctfd:index/user:User ctfer 1
-        ```
-
         :param str resource_name: The name of the resource.
         :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfer-io-pulumi-ctfd
-Version: 0.1.23
+Version: 0.1.24
 Summary: The CTFd provider for Pulumi, to manage its resources as code.
 Home-page: https://ctfer.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ctfer-io/pulumi-ctfd
 Keywords: pulumi ctfd category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctfer-io-pulumi-ctfd Version: 0.1.23 Summary: The
+Metadata-Version: 2.1 Name: ctfer-io-pulumi-ctfd Version: 0.1.24 Summary: The
 CTFd provider for Pulumi, to manage its resources as code. Home-page: https://
 ctfer.io License: Apache-2.0 Project-URL: Repository, https://github.com/ctfer-
 io/pulumi-ctfd Keywords: pulumi ctfd category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown
                ************ [[rreess//ccttffdd..ppnngg]]PPuulluummii CCTTFFdd PPrroovviiddeerr ************
                             LLeett''ss ccooddee yyoouurr CCTTFF((dd))
                              _[_r_e_f_e_r_e_n_c_e_][License]
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt` & `ctfer-io_pulumi-ctfd-0.1.24/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.23/setup.py` & `ctfer-io_pulumi-ctfd-0.1.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.23"
+VERSION = "0.1.24"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ctfd Pulumi Package - Development Version"
```

