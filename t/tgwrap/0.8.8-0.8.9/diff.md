# Comparing `tmp/tgwrap-0.8.8.tar.gz` & `tmp/tgwrap-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.8.8.tar", max compression
+gzip compressed data, was "tgwrap-0.8.9.tar", max compression
```

## Comparing `tgwrap-0.8.8.tar` & `tgwrap-0.8.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.8.8/LICENSE
--rw-r--r--   0        0        0    10353 2023-11-21 08:08:14.362959 tgwrap-0.8.8/README.md
--rw-r--r--   0        0        0      922 2024-01-10 10:45:19.768956 tgwrap-0.8.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.8.8/tgwrap/__init__.py
--rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.8.8/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    29060 2023-11-27 12:41:28.897080 tgwrap-0.8.8/tgwrap/cli.py
--rw-r--r--   0        0        0     9560 2023-11-15 14:30:12.754835 tgwrap-0.8.8/tgwrap/deploy.py
--rwxr-xr-x   0        0        0    74195 2024-01-10 10:34:44.827661 tgwrap-0.8.8/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.8.8/tgwrap/printer.py
--rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 tgwrap-0.8.8/setup.py
--rw-r--r--   0        0        0    11477 1970-01-01 00:00:00.000000 tgwrap-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.8.9/LICENSE
+-rw-r--r--   0        0        0    10353 2023-11-21 08:08:14.362959 tgwrap-0.8.9/README.md
+-rw-r--r--   0        0        0      922 2024-02-01 11:00:32.533856 tgwrap-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.8.9/tgwrap/__init__.py
+-rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.8.9/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    29060 2023-11-27 12:41:28.897080 tgwrap-0.8.9/tgwrap/cli.py
+-rw-r--r--   0        0        0     9577 2024-02-01 10:59:51.328863 tgwrap-0.8.9/tgwrap/deploy.py
+-rwxr-xr-x   0        0        0    74105 2024-01-31 12:13:03.117600 tgwrap-0.8.9/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.8.9/tgwrap/printer.py
+-rw-r--r--   0        0        0    11528 1970-01-01 00:00:00.000000 tgwrap-0.8.9/PKG-INFO
```

### Comparing `tgwrap-0.8.8/LICENSE` & `tgwrap-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.8/README.md` & `tgwrap-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.8/pyproject.toml` & `tgwrap-0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.8.8"
+version = "0.8.9"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.8.8/tgwrap/analyze.py` & `tgwrap-0.8.9/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.8/tgwrap/cli.py` & `tgwrap-0.8.9/tgwrap/cli.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.8/tgwrap/deploy.py` & `tgwrap-0.8.9/tgwrap/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         # a directory, which is not always what you want!!!!!
         #
         if os.path.isdir(target_path):
             include_statements = \
                 f"--include='{terragrunt_file}' {lock_file_stmt} {env_file_stmt} {excludes_stmt} " + \
                 "--exclude='.terragrunt-cache/' --exclude='.terraform/' " + \
                 "--exclude='terragrunt-debug.tfvars.json' --exclude=planfile " + \
-                "--exclude='.DS_Store' "
+                "--exclude='.DS_Store' --exclude='*.log'"
 
         cmd = f"rsync -aim {dry_run_stmt} {clean_stmt} " + \
             include_statements + \
             f"{source_path} {target_path}"
 
         cmd = re.sub(' +', ' ', cmd)
```

### Comparing `tgwrap-0.8.8/tgwrap/main.py` & `tgwrap-0.8.9/tgwrap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         """ Constructs the command """
 
         commands = {
             'generic': '{base_command} {command} --terragrunt-non-interactive {no_auto_approve} {update} {upgrade} {parallelism} {common}',
             'info': '{base_command} terragrunt-info --terragrunt-non-interactive {update} {upgrade} {common}',
             'plan': '{base_command} {command} --terragrunt-non-interactive  -out={planfile_name} {lock_level} {update} {parallelism} {common}',
             'apply': '{base_command} {command} {non_interactive} {no_auto_approve} {update} {parallelism} {common} {planfile}',
-            'show': '{base_command} {command} --terragrunt-non-interactive {ignore_deps} {planfile_name} {common}',
+            'show': '{base_command} {command} --terragrunt-non-interactive {planfile_name} {common}',
             'destroy': '{base_command} {command} {non_interactive} {no_auto_approve} {parallelism} {common} {planfile}',
         }
 
         lock_stmt = ''
         if no_lock and command in ['init', 'validate', 'validate-inputs', 'plan', 'info', 'output', 'show', 'state']:
             lock_stmt = '-lock=false'
             self.printer.warning('Terraform state will NOT be locked')
@@ -533,16 +533,14 @@
                 working_dir = module
             
             if add_to_workdir:
                 working_dir = os.path.join(working_dir, add_to_workdir)
 
             self.printer.verbose(f'Execute command: {command} in working dir: {working_dir}')
 
-            self.printer.verbose(f'Executing in directory: {working_dir}')
-
             self.printer.header(
                 f'\n\nStart processing module: {module} ({progress})\n\n',
                 print_line_before=True,
                 )
 
             if dry_run:
                 self.printer.warning(
```

### Comparing `tgwrap-0.8.8/tgwrap/printer.py` & `tgwrap-0.8.9/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.8/setup.py` & `tgwrap-0.8.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,278 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tgwrap
+Version: 0.8.9
+Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
+Home-page: https://gitlab.com/lunadata/tgwrap
+License: MIT
+Keywords: terraform,terragrunt,terrasafe,python
+Author: Gerco Grandia
+Author-email: gerco.grandia@4synergy.nl
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.0)
+Requires-Dist: inquirer (>=3.1.4,<4.0.0)
+Requires-Dist: networkx (>=2.8.8,<3.0.0)
+Requires-Dist: outdated (>=0.2.2)
+Requires-Dist: pydot (>=1.4.2,<2.0.0)
+Requires-Dist: pyhcl (>=0.4.4,<0.5.0)
+Requires-Dist: python-hcl2 (>=4.3.2,<5.0.0)
+Requires-Dist: pyyaml (>=6.0)
+Requires-Dist: terrasafe (>=0.5.1,<0.6.0)
+Project-URL: Documentation, https://gitlab.com/lunadata/tgwrap/
+Project-URL: Repository, https://gitlab.com/lunadata/tgwrap
+Description-Content-Type: text/markdown
 
-packages = \
-['tgwrap']
+# tg-wrap
 
-package_data = \
-{'': ['*']}
+This app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).
 
-install_requires = \
-['click>=8.0',
- 'inquirer>=3.1.4,<4.0.0',
- 'networkx>=2.8.8,<3.0.0',
- 'outdated>=0.2.2',
- 'pydot>=1.4.2,<2.0.0',
- 'pyhcl>=0.4.4,<0.5.0',
- 'python-hcl2>=4.3.2,<5.0.0',
- 'pyyaml>=6.0',
- 'terrasafe>=0.5.1,<0.6.0']
-
-entry_points = \
-{'console_scripts': ['tgwrap = tgwrap.cli:main']}
-
-setup_kwargs = {
-    'name': 'tgwrap',
-    'version': '0.8.8',
-    'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
-    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd when you can run it step by step, you can make the process also re-startable, which is also pretty handy!\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.\n\nIt needs a config file as follows:\n\n```yaml\n---\n#\n# Critically of resources as interpreted by \'tgwrap analyze\'.\n# It uses it for a \'terrasafe\' like validation if resources can safely be deleted.\n# On top of that it tries to analyze and quantify the drift impact of the changes,\n# so that this can be monitored.\n#\nlow:\n  # defaults:\n  #   terrasafe_level: ignore_deletions\n  #   drift_impact:\n  #     default: minor\n  #     delete: medium\n  azuread_application.: {} # if we you want to use the defaults\n  azuread_app_role_assignment: # or if you want to override these\n    drift_impact:\n      delete: minor\n  # and so on, and so forth\nmedium:\n  # defaults:\n  #   terrasafe_level: ignore_deletion_if_recreation\n  #   drift_impact:\n  #     default: medium\n  #     delete: major\n  azurerm_data_factory_linked_service_key_vault.: {}\n  # and so on, and so forth\nhigh:\n  # defaults:\n  #   terrasafe_level: unauthorized_deletion\n  #   drift_impact:\n  #     default: major\n  #     update: medium\n  azuread_group.:\n    drift_impact:\n      create: minor\n      update: minor\n  azurerm_application_insights.: {}\n  # and so on, and so forth\n```\n\n### Speeding up the performance of analyze\n\nThis `analyze` function turned out to be pretty slow, where most of the time went into the `terragrunt show` function that is executed for each individual module. \n\nThis was a bit surprising as the plan file is already available on the file system, but it turns out that terragrunt is taking quite a bit of time for managing the depdencies. Even when you\'re excluding the external dependencies and are located in a particular module.\n\nSo, if you add the following to your root `terragrunt.hcl`:\n\n```hcl\nterraform {\n  after_hook "link_to_current_module" {\n    commands = ["init", "plan", "apply", "validate", "destroy"]\n    execute  = ["bash", "-c", "ln -sf $(pwd) ${get_terragrunt_dir()}/.terragrunt-cache/current"]\n  }\n}\n```\n\nThe directory where the plan file is stored (including the other resources that terraform needs) becomes predictable and it becomes possible to run a native `terraform show` (instead `terragrunt show`) which dramatically speed up things.\n\nJust set the proper value as an environment variable:\n\n```console\nexport TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"\n```\n\nOr pass it along with the `--planfile-dir|-P` option and it will use that.\n\n## More than a wrapper\n\nOver time, tgwrap became more than a wrapper, blantly violating [#1 of the unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy#:~:text=The%20Unix%20philosophy%20is%20documented,%2C%20as%20yet%20unknown%2C%20program.): \'Make each program do one thing well\'.\n\nFor instance, the \'analyze\' functionality is already an example, but more features such as deploying a landing zone has crept into the application. It makes sense for how we\'re using it, but we\'re fully aware this makes it less generically applicable.\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# run-all with excluding a particular directory\ntgwrap run-all plan -E \'excluded-dir/*\'\n# or a directory somewhere further down in the path\ntgwrap run-all plan -E \'**/excluded-dir/**\'\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform # path where the terragrunt modules are stored \nconfig_path: terragrunt/config/platform-dev # path (relative to base path) where the config files are stored\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    source_dir: platform # optional, if the source modules are not directly in the stage dir, but in <stage>/<source_dir> directory\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    config_dir: ../../../config # this is relative to where you run the deploy\n    configs:\n      - my-config.hcl\n      - ../my-ss-config-dir\n    # skip_all_modules: True # could be handy if you only want to deploy substacks and no regular modules\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n    configs:\n      - my-ss-config.hcl\n      - ../my-ss-config-dir\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Generating change logs\n\ntgwrap can generate a change log by running:\n\n```console\ntgwrap change-log [--changelog-file ./CHANGELOG.md]\n```\n\nThe (optional) change log file will be, if passed along. tgwrap then checks the file for the existance of a start and end markers, in the following format:\n\n```python\n  start_marker = \'<!-- BEGINNING OF OF TGWRAP CHANGELOG SECTION -->\'\n  end_marker = \'<!-- END OF TGWRAP CHANGELOG SECTION -->\'\n```\n\nIf they exist, everything between these lines will be replaced by the new change log.\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
-    'author': 'Gerco Grandia',
-    'author_email': 'gerco.grandia@4synergy.nl',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/lunadata/tgwrap',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+Wait, why on earth do we need a wrapper for a wrapper (for a wrapper)?
+
+Well, first of all it is pretty opinionated so what works for us, doesn't necessarily work for you.
+
+But our reasoning for creating this is as follows:
+
+## 1. Less typing
+
+terraform is great, and in combination with terragrunt even greater! But let's face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don't like typing!
+
+## 2. Testing modules locally
+
+However, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.
+
+The thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.
+
+Which leads to (even) more typing, and worse: a higher chance for errors.
+
+Luckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.
+
+Nothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can't solve though!
+
+## 3. But the original reason was: Errors when using run-all are challenging
+
+One of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.
+
+terragrunt's error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.
+
+And if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.
+
+So we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.
+
+And when you can run it step by step, you can make the process also re-startable, which is also pretty handy!
+
+And this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we're at it, replacing the aliases with this was then pretty straightforward next step as well.
+
+## 4. Analyzing plan files
+
+When using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.
+
+It needs a config file as follows:
+
+```yaml
+---
+#
+# Critically of resources as interpreted by 'tgwrap analyze'.
+# It uses it for a 'terrasafe' like validation if resources can safely be deleted.
+# On top of that it tries to analyze and quantify the drift impact of the changes,
+# so that this can be monitored.
+#
+low:
+  # defaults:
+  #   terrasafe_level: ignore_deletions
+  #   drift_impact:
+  #     default: minor
+  #     delete: medium
+  azuread_application.: {} # if we you want to use the defaults
+  azuread_app_role_assignment: # or if you want to override these
+    drift_impact:
+      delete: minor
+  # and so on, and so forth
+medium:
+  # defaults:
+  #   terrasafe_level: ignore_deletion_if_recreation
+  #   drift_impact:
+  #     default: medium
+  #     delete: major
+  azurerm_data_factory_linked_service_key_vault.: {}
+  # and so on, and so forth
+high:
+  # defaults:
+  #   terrasafe_level: unauthorized_deletion
+  #   drift_impact:
+  #     default: major
+  #     update: medium
+  azuread_group.:
+    drift_impact:
+      create: minor
+      update: minor
+  azurerm_application_insights.: {}
+  # and so on, and so forth
+```
+
+### Speeding up the performance of analyze
+
+This `analyze` function turned out to be pretty slow, where most of the time went into the `terragrunt show` function that is executed for each individual module. 
+
+This was a bit surprising as the plan file is already available on the file system, but it turns out that terragrunt is taking quite a bit of time for managing the depdencies. Even when you're excluding the external dependencies and are located in a particular module.
+
+So, if you add the following to your root `terragrunt.hcl`:
+
+```hcl
+terraform {
+  after_hook "link_to_current_module" {
+    commands = ["init", "plan", "apply", "validate", "destroy"]
+    execute  = ["bash", "-c", "ln -sf $(pwd) ${get_terragrunt_dir()}/.terragrunt-cache/current"]
+  }
 }
+```
+
+The directory where the plan file is stored (including the other resources that terraform needs) becomes predictable and it becomes possible to run a native `terraform show` (instead `terragrunt show`) which dramatically speed up things.
+
+Just set the proper value as an environment variable:
+
+```console
+export TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"
+```
+
+Or pass it along with the `--planfile-dir|-P` option and it will use that.
+
+## More than a wrapper
+
+Over time, tgwrap became more than a wrapper, blantly violating [#1 of the unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy#:~:text=The%20Unix%20philosophy%20is%20documented,%2C%20as%20yet%20unknown%2C%20program.): 'Make each program do one thing well'.
+
+For instance, the 'analyze' functionality is already an example, but more features such as deploying a landing zone has crept into the application. It makes sense for how we're using it, but we're fully aware this makes it less generically applicable.
+
+## Usage
+
+```console
+# general help
+tgwrap --help
+
+tgwrap run -h
+tgwrap run-all -h
+
+# run a plan
+tgwrap plan # which is the same as tgwrap run plan
+
+# run-all a plan
+tgwrap run-all plan
+
+# run-all with excluding a particular directory
+tgwrap run-all plan -E 'excluded-dir/*'
+# or a directory somewhere further down in the path
+tgwrap run-all plan -E '**/excluded-dir/**'
+
+# or do the same in step-by-step mode
+tgwrap run-all plan -s
+
+# or excluding (aka ignoring) external dependencies
+tgwrap run-all plan -sx
+
+# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)
+tgwrap output -- -json
+```
+
+> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:
+
+`tgwrap state mv 'azuread_group.this[\"viewers\"]' 'azuread_group.this[\"readers\"]'`
+
+## A word about escaping inputs
+
+Your shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.
+
+For example:
+
+```console
+# to exclude certain modules from an action (such as analyze):
+tgwrap analyze -E 'integrations/\*/\*'
+
+# to import a resource that has a " in its address:
+tgwrap import -a 'azuread_group.this[\"my_group\"]' -i ${GROUP_ID}
+```
+
+## Deploy manifests
+
+In order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:
+
+```yaml
+---
+git_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git
+base_path: terragrunt/my-platform # path where the terragrunt modules are stored 
+config_path: terragrunt/config/platform-dev # path (relative to base path) where the config files are stored
+
+deploy: # which modules do you want to deploy
+  dtap:
+    applies_to_stages:
+      - dev
+      - tst
+      - acc
+      - prd
+    source_stage: dev
+    source_dir: platform # optional, if the source modules are not directly in the stage dir, but in <stage>/<source_dir> directory
+    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks
+    config_dir: ../../../config # this is relative to where you run the deploy
+    configs:
+      - my-config.hcl
+      - ../my-ss-config-dir
+    # skip_all_modules: True # could be handy if you only want to deploy substacks and no regular modules
+    exclude_modules: # these modules will always be excluded, can be omitted
+      - my-specific-module
+    include_modules: {} # omit or use an empty dict for all of them
+      # or specify your modules as follows
+      # base: {} # just a simple include
+      # networking-connected: # or a bit more complicated
+      #  - source: networking
+      #  - target: networking-connected
+
+sub_stacks:
+  is01:
+    source: shared-integration/intsvc01
+    target: integration/is01
+    exclude_modules:  # a list of modules that will always be excluded, can be omitted
+      - my-specific-module
+    configs:
+      - my-ss-config.hcl
+      - ../my-ss-config-dir
+  is02:
+    source: shared-integration/intsvc01
+    target: integration/is02
+
+# global configuration files that are deployed as well
+# note that these files are typically applicable to all landing zones and stages!
+# this might lead to unexpected behaviour
+# note that you can exclude syncing these files with a command line switch
+global_config_files:
+  root-terragrunt:
+    source: ../../terragrunt.hcl # relative to base_path
+    target: ../../terragrunt.hcl # can be omitted, then it is same as source path
+  terrasafe-config:
+    source: ../../terrasafe-config.json
+```
+
+## Generating change logs
+
+tgwrap can generate a change log by running:
+
+```console
+tgwrap change-log [--changelog-file ./CHANGELOG.md]
+```
+
+The (optional) change log file will be, if passed along. tgwrap then checks the file for the existance of a start and end markers, in the following format:
+
+```python
+  start_marker = '<!-- BEGINNING OF OF TGWRAP CHANGELOG SECTION -->'
+  end_marker = '<!-- END OF TGWRAP CHANGELOG SECTION -->'
+```
+
+If they exist, everything between these lines will be replaced by the new change log.
+
+## Development
 
+In order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.
 
-setup(**setup_kwargs)
```

