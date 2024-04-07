# Comparing `tmp/collective.listmonk-1.0.0a1.tar.gz` & `tmp/collective.listmonk-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.listmonk-1.0.0a1.tar", last modified: Sun Apr  7 15:51:14 2024, max compression
+gzip compressed data, was "collective.listmonk-1.0.0a2.tar", last modified: Sun Apr  7 23:17:10 2024, max compression
```

## Comparing `collective.listmonk-1.0.0a1.tar` & `collective.listmonk-1.0.0a2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.801306 collective.listmonk-1.0.0a1/
--rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/.editorconfig
--rw-r--r--   0 davisagli   (501) staff       (20)      413 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/CHANGES.md
--rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/CONTRIBUTORS.md
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/LICENSE.md
--rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/MANIFEST.in
--rw-r--r--   0 davisagli   (501) staff       (20)     6411 2024-04-07 15:51:14.801027 collective.listmonk-1.0.0a1/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/README.md
--rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/constraints.txt
--rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/docker-compose.yml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.792356 collective.listmonk-1.0.0a1/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/docs/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/docs/dlr.svg
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.793011 collective.listmonk-1.0.0a1/news/
--rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/news/.changelog_template.jinja
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/news/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-07 15:51:14.801353 collective.listmonk-1.0.0a1/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.788691 collective.listmonk-1.0.0a1/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.793173 collective.listmonk-1.0.0a1/src/collective/
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.795581 collective.listmonk-1.0.0a1/src/collective/listmonk/
--rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.795836 collective.listmonk-1.0.0a1/src/collective/listmonk/behaviors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/behaviors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/behaviors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.796100 collective.listmonk-1.0.0a1/src/collective/listmonk/content/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/content/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2818 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/content/newsletter.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.796371 collective.listmonk-1.0.0a1/src/collective/listmonk/controlpanel/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/controlpanel/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/controlpanel/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/dependencies.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/interfaces.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1247 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/listmonk.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.796770 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2249 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/collective.listmonk.pot
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.789279 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/de/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.796918 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/de/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     1926 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.789426 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/en/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.797075 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/en/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     1876 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
--rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/locales/update.py
--rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/permissions.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.789749 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.797681 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/rolemap.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.797824 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/types/
--rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/types/Newsletter.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.797972 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/uninstall/
--rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/profiles.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.798668 collective.listmonk-1.0.0a1/src/collective/listmonk/services/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/services/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/services/base.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1254 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/services/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/services/mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5246 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/services/subscriptions.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.798810 collective.listmonk-1.0.0a1/src/collective/listmonk/setuphandlers/
--rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/setuphandlers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3184 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/testing.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.799090 collective.listmonk-1.0.0a1/src/collective/listmonk/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/upgrades/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective/listmonk/upgrades/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.800369 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)     6411 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     2409 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/top_level.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.799307 collective.listmonk-1.0.0a1/tests/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.799642 collective.listmonk-1.0.0a1/tests/api/
--rw-r--r--   0 davisagli   (501) staff       (20)     5076 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/tests/api/test_mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4273 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/tests/api/test_subscriptions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2699 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/tests/conftest.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.799965 collective.listmonk-1.0.0a1/tests/setup/
--rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/tests/setup/test_setup_install.py
--rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 15:51:14.800138 collective.listmonk-1.0.0a1/tests/setup/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-07 15:51:14.000000 collective.listmonk-1.0.0a1/tests/setup/upgrades/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.940748 collective.listmonk-1.0.0a2/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/.editorconfig
+-rw-r--r--   0 davisagli   (501) staff       (20)      527 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/CHANGES.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/CONTRIBUTORS.md
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/LICENSE.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 davisagli   (501) staff       (20)     6525 2024-04-07 23:17:10.940500 collective.listmonk-1.0.0a2/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/README.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/constraints.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/docker-compose.yml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.932298 collective.listmonk-1.0.0a2/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/docs/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/docs/dlr.svg
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.932644 collective.listmonk-1.0.0a2/news/
+-rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/news/.changelog_template.jinja
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/news/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-07 23:17:10.940791 collective.listmonk-1.0.0a2/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.923169 collective.listmonk-1.0.0a2/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.932801 collective.listmonk-1.0.0a2/src/collective/
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.935102 collective.listmonk-1.0.0a2/src/collective/listmonk/
+-rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.935359 collective.listmonk-1.0.0a2/src/collective/listmonk/behaviors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/behaviors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/behaviors/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.935625 collective.listmonk-1.0.0a2/src/collective/listmonk/content/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/content/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2818 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/content/newsletter.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.935890 collective.listmonk-1.0.0a2/src/collective/listmonk/controlpanel/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/controlpanel/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/controlpanel/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/dependencies.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/interfaces.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1445 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/listmonk.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.936298 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2249 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/collective.listmonk.pot
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.923807 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/de/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.936445 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/de/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1926 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.923961 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/en/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.936597 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/en/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1876 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
+-rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/locales/update.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/permissions.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.924309 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.937194 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/rolemap.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.937359 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/types/Newsletter.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/types.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.937525 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/uninstall/
+-rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/profiles.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.938304 collective.listmonk-1.0.0a2/src/collective/listmonk/services/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/services/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/services/base.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1254 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/services/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/services/mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5246 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/services/subscriptions.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.938465 collective.listmonk-1.0.0a2/src/collective/listmonk/setuphandlers/
+-rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/setuphandlers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3184 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/testing.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.938749 collective.listmonk-1.0.0a2/src/collective/listmonk/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/upgrades/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective/listmonk/upgrades/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.939842 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)     6525 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     2409 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.938888 collective.listmonk-1.0.0a2/tests/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.939177 collective.listmonk-1.0.0a2/tests/api/
+-rw-r--r--   0 davisagli   (501) staff       (20)     5076 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/tests/api/test_mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4273 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/tests/api/test_subscriptions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2699 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/tests/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.939469 collective.listmonk-1.0.0a2/tests/setup/
+-rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/tests/setup/test_setup_install.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-07 23:17:10.939609 collective.listmonk-1.0.0a2/tests/setup/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-07 23:17:10.000000 collective.listmonk-1.0.0a2/tests/setup/upgrades/conftest.py
```

### Comparing `collective.listmonk-1.0.0a1/.editorconfig` & `collective.listmonk-1.0.0a2/.editorconfig`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/LICENSE.GPL` & `collective.listmonk-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/LICENSE.md` & `collective.listmonk-1.0.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/PKG-INFO` & `collective.listmonk-1.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2024-04-07)
+
+
+### Bug fixes:
+
+- Avoid runtime dependency on plone.app.robotframework. @davisagli #10
+
 ## 1.0.0a1 (2024-04-07)
 
 No significant changes.
 
 
 ## 1.0a1 (unreleased)
```

### Comparing `collective.listmonk-1.0.0a1/README.md` & `collective.listmonk-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/docker-compose.yml` & `collective.listmonk-1.0.0a2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/docs/dlr.svg` & `collective.listmonk-1.0.0a2/docs/dlr.svg`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/pyproject.toml` & `collective.listmonk-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/setup.py` & `collective.listmonk-1.0.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {Path("CONTRIBUTORS.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 
 setup(
     name="collective.listmonk",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="A Listmonk newsletter integration for Plone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/content/newsletter.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/content/newsletter.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/listmonk.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/listmonk.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-from plone.restapi.testing import RelativeSession
 from pydantic_settings import BaseSettings
 from pydantic_settings import SettingsConfigDict
+from requests.exceptions import ConnectionError
 from requests.exceptions import HTTPError
 from typing import Optional
 from zExceptions import BadRequest
 
+import requests
+import time
+
 
 class ListmonkSettings(BaseSettings):
     model_config = SettingsConfigDict(env_prefix="listmonk_")
 
     url: str = "http://localhost:9000/api"
     username: str = "admin"
     password: str = "admin"
 
 
 settings = ListmonkSettings()
-client = RelativeSession(settings.url)
-client.auth = (settings.username, settings.password)
 
 
 def call_listmonk(method, path, **kw):
-    func = getattr(client, method.lower())
-    response = func(path, **kw)
+    func = getattr(requests, method.lower())
+    url = settings.url.rstrip("/") + "/" + path.lstrip("/")
+    try:
+        response = func(url, auth=(settings.username, settings.password), **kw)
+    except ConnectionError:
+        time.sleep(2)
+        response = func(url, auth=(settings.username, settings.password), **kw)
     try:
         response.raise_for_status()
     except HTTPError as err:
         if err.response.status_code == 400:
             raise err.__class__(err.response.json()["message"])
+        raise
     return response.json()
 
 
 def get_subscriber(email: str) -> Optional[dict]:
     result = call_listmonk(
         "get",
         "/subscribers",
```

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/locales/collective.listmonk.pot` & `collective.listmonk-1.0.0a2/src/collective/listmonk/locales/collective.listmonk.pot`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a2/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a2/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/locales/update.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/rolemap.xml` & `collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/profiles/default/types/Newsletter.xml` & `collective.listmonk-1.0.0a2/src/collective/listmonk/profiles/default/types/Newsletter.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/profiles.zcml` & `collective.listmonk-1.0.0a2/src/collective/listmonk/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/services/base.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/services/base.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/services/configure.zcml` & `collective.listmonk-1.0.0a2/src/collective/listmonk/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/services/mailings.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/services/mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/services/subscriptions.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective/listmonk/testing.py` & `collective.listmonk-1.0.0a2/src/collective/listmonk/testing.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/PKG-INFO` & `collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2024-04-07)
+
+
+### Bug fixes:
+
+- Avoid runtime dependency on plone.app.robotframework. @davisagli #10
+
 ## 1.0.0a1 (2024-04-07)
 
 No significant changes.
 
 
 ## 1.0a1 (unreleased)
```

### Comparing `collective.listmonk-1.0.0a1/src/collective.listmonk.egg-info/SOURCES.txt` & `collective.listmonk-1.0.0a2/src/collective.listmonk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/tests/api/test_mailings.py` & `collective.listmonk-1.0.0a2/tests/api/test_mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/tests/api/test_subscriptions.py` & `collective.listmonk-1.0.0a2/tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/tests/conftest.py` & `collective.listmonk-1.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/tests/setup/test_setup_install.py` & `collective.listmonk-1.0.0a2/tests/setup/test_setup_install.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/tests/setup/test_setup_uninstall.py` & `collective.listmonk-1.0.0a2/tests/setup/test_setup_uninstall.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a1/tests/setup/upgrades/conftest.py` & `collective.listmonk-1.0.0a2/tests/setup/upgrades/conftest.py`

 * *Files identical despite different names*

