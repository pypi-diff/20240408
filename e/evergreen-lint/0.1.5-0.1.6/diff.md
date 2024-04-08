# Comparing `tmp/evergreen_lint-0.1.5.tar.gz` & `tmp/evergreen_lint-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evergreen_lint-0.1.5.tar", max compression
+gzip compressed data, was "evergreen_lint-0.1.6.tar", max compression
```

## Comparing `evergreen_lint-0.1.5.tar` & `evergreen_lint-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       93 2024-02-06 15:46:17.998967 evergreen_lint-0.1.5/evergreen_lint/__init__.py
--rw-r--r--   0        0        0     2814 2024-02-02 11:05:21.130327 evergreen_lint-0.1.5/evergreen_lint/__main__.py
--rw-r--r--   0        0        0     4929 2024-02-06 15:46:17.999955 evergreen_lint-0.1.5/evergreen_lint/config.py
--rw-r--r--   0        0        0      630 2024-02-02 11:05:21.130758 evergreen_lint-0.1.5/evergreen_lint/config_with_bad_yaml.yml
--rw-r--r--   0        0        0    11356 2024-02-06 15:46:18.001022 evergreen_lint-0.1.5/evergreen_lint/helpers.py
--rw-r--r--   0        0        0      584 2024-02-02 11:05:21.131176 evergreen_lint-0.1.5/evergreen_lint/model.py
--rw-r--r--   0        0        0     2751 2024-02-06 15:46:18.001853 evergreen_lint-0.1.5/evergreen_lint/rules/__init__.py
--rw-r--r--   0        0        0     5809 2024-02-02 11:05:21.131646 evergreen_lint-0.1.5/evergreen_lint/rules/commonsense.py
--rw-r--r--   0        0        0     1694 2024-02-02 11:05:21.131861 evergreen_lint-0.1.5/evergreen_lint/rules/dependency_for_func.py
--rw-r--r--   0        0        0     4692 2024-02-06 15:46:18.002526 evergreen_lint-0.1.5/evergreen_lint/rules/enforce_tags_for_tasks.py
--rw-r--r--   0        0        0     1388 2024-02-02 14:46:52.358352 evergreen_lint-0.1.5/evergreen_lint/rules/invalid_build_parameter.py
--rw-r--r--   0        0        0    11710 2024-02-02 11:05:21.132393 evergreen_lint-0.1.5/evergreen_lint/rules/required_expansions_write.py
--rw-r--r--   0        0        0     3210 2024-02-02 11:05:21.132563 evergreen_lint-0.1.5/evergreen_lint/rules/tasks_for_variants.py
--rw-r--r--   0        0        0      925 2024-02-06 15:46:18.003257 evergreen_lint-0.1.5/evergreen_lint/yamlhandler.py
--rw-r--r--   0        0        0     1266 2024-02-06 15:46:18.005202 evergreen_lint-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 evergreen_lint-0.1.5/setup.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 evergreen_lint-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       93 2024-04-08 16:46:32.759520 evergreen_lint-0.1.6/evergreen_lint/__init__.py
+-rw-r--r--   0        0        0     2814 2024-02-02 11:05:21.130327 evergreen_lint-0.1.6/evergreen_lint/__main__.py
+-rw-r--r--   0        0        0     5025 2024-04-08 16:46:32.760490 evergreen_lint-0.1.6/evergreen_lint/config.py
+-rw-r--r--   0        0        0      630 2024-02-02 11:05:21.130758 evergreen_lint-0.1.6/evergreen_lint/config_with_bad_yaml.yml
+-rw-r--r--   0        0        0    11356 2024-02-06 15:46:18.001022 evergreen_lint-0.1.6/evergreen_lint/helpers.py
+-rw-r--r--   0        0        0      584 2024-02-02 11:05:21.131176 evergreen_lint-0.1.6/evergreen_lint/model.py
+-rw-r--r--   0        0        0     2890 2024-04-08 16:46:32.761218 evergreen_lint-0.1.6/evergreen_lint/rules/__init__.py
+-rw-r--r--   0        0        0     5809 2024-02-02 11:05:21.131646 evergreen_lint-0.1.6/evergreen_lint/rules/commonsense.py
+-rw-r--r--   0        0        0     1694 2024-02-02 11:05:21.131861 evergreen_lint-0.1.6/evergreen_lint/rules/dependency_for_func.py
+-rw-r--r--   0        0        0     4696 2024-04-08 16:46:32.761955 evergreen_lint-0.1.6/evergreen_lint/rules/enforce_tags_for_tasks.py
+-rw-r--r--   0        0        0     4188 2024-04-08 16:46:32.762393 evergreen_lint-0.1.6/evergreen_lint/rules/enforce_tags_for_variants.py
+-rw-r--r--   0        0        0     1388 2024-02-02 14:46:52.358352 evergreen_lint-0.1.6/evergreen_lint/rules/invalid_build_parameter.py
+-rw-r--r--   0        0        0    11710 2024-02-02 11:05:21.132393 evergreen_lint-0.1.6/evergreen_lint/rules/required_expansions_write.py
+-rw-r--r--   0        0        0     3210 2024-02-02 11:05:21.132563 evergreen_lint-0.1.6/evergreen_lint/rules/tasks_for_variants.py
+-rw-r--r--   0        0        0      925 2024-02-06 15:46:18.003257 evergreen_lint-0.1.6/evergreen_lint/yamlhandler.py
+-rw-r--r--   0        0        0     1266 2024-04-08 16:46:32.763122 evergreen_lint-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 evergreen_lint-0.1.6/PKG-INFO
```

### Comparing `evergreen_lint-0.1.5/evergreen_lint/__main__.py` & `evergreen_lint-0.1.6/evergreen_lint/__main__.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/config.py` & `evergreen_lint-0.1.6/evergreen_lint/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,10 +127,14 @@
     # Enforce variants must run the specified list of tasks
     - rule: "tasks-for-variants"
       task-variant-mappings: {{}}
 
     # Enforce tasks must have tags
     - rule: "enforce-tags-for-tasks"
       tag_groups: {[]}
+
+    # Enforce variants must have tags
+    - rule: "enforce-tags-for-variants"
+      tags: {[]}
 """[
     1:-1
 ]  # <--- this strips the leading and trailing newlines from this HEREDOC
```

### Comparing `evergreen_lint-0.1.5/evergreen_lint/config_with_bad_yaml.yml` & `evergreen_lint-0.1.6/evergreen_lint/config_with_bad_yaml.yml`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/helpers.py` & `evergreen_lint-0.1.6/evergreen_lint/helpers.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/model.py` & `evergreen_lint-0.1.6/evergreen_lint/model.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/__init__.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     NoMultilineExpansionsUpdate,
     NoShellExec,
     NoWorkingDirOnShell,
     ShellExecExplicitShell,
 )
 from evergreen_lint.rules.dependency_for_func import DependencyForFunc
 from evergreen_lint.rules.enforce_tags_for_tasks import EnforceTagsForTasks
+from evergreen_lint.rules.enforce_tags_for_variants import EnforceTagsForVariants
 from evergreen_lint.rules.invalid_build_parameter import InvalidBuildParameter
 from evergreen_lint.rules.required_expansions_write import RequiredExpansionsWrite
 from evergreen_lint.rules.tasks_for_variants import TasksForVariants
 
 RULES: Dict[str, Type[Rule]] = {
     "limit-keyval-inc": LimitKeyvalInc,
     "shell-exec-explicit-shell": ShellExecExplicitShell,
@@ -24,14 +25,15 @@
     "no-shell-exec": NoShellExec,
     "no-multiline-expansions-update": NoMultilineExpansionsUpdate,
     "invalid-build-parameter": InvalidBuildParameter,
     "required-expansions-write": RequiredExpansionsWrite,
     "dependency-for-func": DependencyForFunc,
     "tasks-for-variants": TasksForVariants,
     "enforce-tags-for-tasks": EnforceTagsForTasks,
+    "enforce-tags-for-variants": EnforceTagsForVariants,
 }
 # Thoughts on Writing Rules
 # - see .helpers for reliable iteration helpers
 # - Do not assume a key exists, unless it's been mentioned here
 # - Do not allow exceptions to percolate outside of the rule function
 # - YAML anchors are not available. Unless you want to write your own yaml
 #   parser, or fork adrienverge/yamllint, abandon all hope on that idea you have.
```

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/commonsense.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/commonsense.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/dependency_for_func.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/dependency_for_func.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/enforce_tags_for_tasks.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/enforce_tags_for_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             " Please add/remove tag(s) of the tag group list to/from the task '{task_name}'"
             " to match the requirement."
         )
 
         failed_checks = []
         rule_config = EnforceTagsForTasksConfig.from_config_dict(config)
 
-        for task_def in cast(List, yaml.get("tasks")):
+        for task_def in cast(List, yaml.get("tasks", [])):
             actual_tags = task_def.get("tags")
             actual_tags_set = set()
             if actual_tags is not None:
                 actual_tags_set = set(actual_tags)
 
             for tag_group_config in rule_config.tag_groups:
                 matching_tag_regex_tags = actual_tags_set
```

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/invalid_build_parameter.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/invalid_build_parameter.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/required_expansions_write.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/required_expansions_write.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/rules/tasks_for_variants.py` & `evergreen_lint-0.1.6/evergreen_lint/rules/tasks_for_variants.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/evergreen_lint/yamlhandler.py` & `evergreen_lint-0.1.6/evergreen_lint/yamlhandler.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.5/pyproject.toml` & `evergreen_lint-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evergreen-lint"
-version = "0.1.5"  # Duplicated in the top-level __init__.py.
+version = "0.1.6"  # Duplicated in the top-level __init__.py.
 description = ""
 authors = [
     "DevProd Build Team <devprod-build-team@mongodb.com>",
     "DevProd Correctness Team <devprod-correctness-team@mongodb.com>",
 ]
 
 [tool.poetry.scripts]
```

