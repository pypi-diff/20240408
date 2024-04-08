# Comparing `tmp/convictquandary-0.0.5.tar.gz` & `tmp/convictquandary-0.0.6.tar.gz`

## Comparing `convictquandary-0.0.5.tar` & `convictquandary-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,35 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 convictquandary-0.0.5/.flake8
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 convictquandary-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 convictquandary-0.0.5/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convictquandary-0.0.5/tox.ini
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 convictquandary-0.0.5/.github/workflows/test-and-publish.yaml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/constants.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/game.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/player.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/player_logic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/utils.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/player_logics/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/player_logics/logic_always_cooperate_believe_truth.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 convictquandary-0.0.5/src/convictquandary/player_logics/logic_always_defect_believe_truth.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 convictquandary-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 convictquandary-0.0.5/tests/test_game.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 convictquandary-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 convictquandary-0.0.5/LICENSE
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 convictquandary-0.0.5/README.md
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 convictquandary-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 convictquandary-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 convictquandary-0.0.6/.flake8
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 convictquandary-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 convictquandary-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convictquandary-0.0.6/tox.ini
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 convictquandary-0.0.6/.github/workflows/test-and-publish.yaml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convictquandary-0.0.6/changelog.d/20240402_154951_prashantsinha94_dev.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 convictquandary-0.0.6/changelog.d/20240403_183118_prashantsinha94_dev.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 convictquandary-0.0.6/changelog.d/20240405_020805_prashantsinha94_dev.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/constants.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/game.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/player.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategy.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategy_filter.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/tournament.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/utils.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/alternator.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/cooperator.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/davis.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/defector.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/grofman.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/grudger.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/random.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/titfortat.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 convictquandary-0.0.6/src/convictquandary/strategies/tullock.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 convictquandary-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 convictquandary-0.0.6/tests/test_game.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 convictquandary-0.0.6/tests/test_player.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 convictquandary-0.0.6/tests/test_tournament.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 convictquandary-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 convictquandary-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 convictquandary-0.0.6/README.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 convictquandary-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 convictquandary-0.0.6/PKG-INFO
```

### Comparing `convictquandary-0.0.5/.pre-commit-config.yaml` & `convictquandary-0.0.6/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -86,7 +86,12 @@
         name: bandit-security-checks
         entry: bandit -r ./src/
         language: python
         types: [python]
         pass_filenames: false
         additional_dependencies: [bandit]
         verbose: true
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: master
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
```

### Comparing `convictquandary-0.0.5/requirements.txt` & `convictquandary-0.0.6/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 ﻿anyio==4.3.0
+argcomplete==3.2.3
+attrs==23.2.0
 bandit==1.7.7
 black==24.2.0
 build==1.0.3
 cachetools==5.3.3
 certifi==2024.2.2
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
+click-log==0.4.0
 colorama==0.4.6
+commitizen==3.21.3
 coverage==7.4.2
+decli==0.6.1
 distlib==0.3.8
 docutils==0.20.1
 editables==0.5
 filelock==3.13.1
 flake8==7.0.0
 h11==0.14.0
 hatch==1.9.4
@@ -23,16 +28,18 @@
 hyperlink==21.0.0
 identify==2.5.35
 idna==3.6
 importlib-metadata==7.0.1
 iniconfig==2.0.0
 isort==5.13.2
 jaraco.classes==3.3.1
+Jinja2==3.1.3
 keyring==24.3.1
 markdown-it-py==3.0.0
+MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
 mypy-extensions==1.0.0
 nh3==0.2.15
 nodeenv==1.8.0
 packaging==23.2
@@ -40,36 +47,41 @@
 pbr==6.0.0
 pep8-naming==0.13.3
 pexpect==4.9.0
 pkginfo==1.9.6
 platformdirs==4.2.0
 pluggy==1.4.0
 pre-commit==3.6.2
+prompt-toolkit==3.0.36
 ptyprocess==0.7.0
 pycodestyle==2.11.1
 pyflakes==3.2.0
 Pygments==2.17.2
 pyproject-api==1.6.1
 pyproject_hooks==1.0.0
 pytest==8.0.1
 pywin32-ctypes==0.2.2
 PyYAML==6.0.1
+questionary==2.0.1
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.0
+scriv==1.5.1
 setuptools==69.1.0
 shellingham==1.5.4
 sniffio==1.3.1
 stevedore==5.2.0
+termcolor==2.4.0
 tomli_w==1.0.0
 tomlkit==0.12.4
 tox==4.13.0
 tox-gh-actions==3.2.0
 trove-classifiers==2024.3.25
 twine==5.0.0
 urllib3==2.2.1
 userpath==1.9.2
 virtualenv==20.25.1
+wcwidth==0.2.13
 zipp==3.17.0
 zstandard==0.22.0
```

### Comparing `convictquandary-0.0.5/tox.ini` & `convictquandary-0.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.5/.github/workflows/test-and-publish.yaml` & `convictquandary-0.0.6/.github/workflows/test-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.5/src/convictquandary/player_logics/logic_always_cooperate_believe_truth.py` & `convictquandary-0.0.6/src/convictquandary/strategies/grudger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,19 @@
 from ..constants import Action, Belief, Persuasion
-from ..player_logic import PlayerLogic
+from ..strategy import Strategy
 
 
-class LogicAlwaysCooperateBelieveTruth(PlayerLogic):
+class Grudger(Strategy):
 
-    def get_persuasion(
-        self,
-        player_actions: list[Action],
-        player_persuasions: list[Persuasion],
-        player_beliefs: list[Belief],
-        opponent_actions: list[Action],
-        opponent_persuasions: list[Persuasion],
-    ) -> Persuasion:
-        return Persuasion.TRUTH
-
-    def get_belief(
-        self,
-        player_actions: list[Action],
-        player_persuasions: list[Persuasion],
-        player_beliefs: list[Belief],
-        opponent_actions: list[Action],
-        opponent_persuasions: list[Persuasion],
-    ) -> Belief:
-        return Belief.BELIEVE
+    meta = {"strategy_set": "axelrod1984"}
 
     def get_action(
         self,
         player_actions: list[Action],
         player_persuasions: list[Persuasion],
         player_beliefs: list[Belief],
         opponent_actions: list[Action],
         opponent_persuasions: list[Persuasion],
     ) -> Action:
+        if Action.DEFECT in opponent_actions:
+            return Action.DEFECT
         return Action.COOPERATE
```

### Comparing `convictquandary-0.0.5/.gitignore` & `convictquandary-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.5/LICENSE` & `convictquandary-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.5/README.md` & `convictquandary-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/prashant94/47b3dd14f7c852987394f631ada1ae1b/raw/covbadge.json)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/prashant94/convict_quandary/test-and-publish.yaml?style=flat&logo=github)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/convictquandary)
 ![PyPI - Status](https://img.shields.io/pypi/status/convictquandary)
+[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
```

### Comparing `convictquandary-0.0.5/pyproject.toml` & `convictquandary-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,8 +34,12 @@
 Homepage = "https://github.com/prashant94/convict_quandary"
 Issues = "https://github.com/prashant94/convict_quandary/issues"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [tool.hatch.version]
-source = "vcs"
+source = "vcs"
+
+[tool.scriv]
+version = "command: git describe --tags --abbrev=0"
+format = "md"
```

### Comparing `convictquandary-0.0.5/PKG-INFO` & `convictquandary-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: convictquandary
-Version: 0.0.5
+Version: 0.0.6
 Summary: A extension of the iterated prisoners dilemma tournaments by Axelrod
 Project-URL: Homepage, https://github.com/prashant94/convict_quandary
 Project-URL: Issues, https://github.com/prashant94/convict_quandary/issues
 Author-email: Prashant Sinha <prashantsinha94@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Prashant Sinha
@@ -51,8 +51,9 @@
 ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/prashant94/47b3dd14f7c852987394f631ada1ae1b/raw/covbadge.json)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/prashant94/convict_quandary/test-and-publish.yaml?style=flat&logo=github)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/convictquandary)
 ![PyPI - Status](https://img.shields.io/pypi/status/convictquandary)
+[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
```

