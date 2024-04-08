# Comparing `tmp/gn2pg_client-1.6.1.tar.gz` & `tmp/gn2pg_client-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gn2pg_client-1.6.1.tar", max compression
+gzip compressed data, was "gn2pg_client-1.6.2.tar", max compression
```

## Comparing `gn2pg_client-1.6.1.tar` & `gn2pg_client-1.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-01-23 09:06:00.451002 gn2pg_client-1.6.1/LICENSE
--rw-r--r--   0        0        0     7798 2024-01-23 09:06:00.451002 gn2pg_client-1.6.1/README.rst
--rw-r--r--   0        0        0     1059 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/__init__.py
--rw-r--r--   0        0        0     7244 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/api.py
--rw-r--r--   0        0        0        0 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/__init__.py
--rw-r--r--   0        0        0     1041 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/admin_views.py
--rw-r--r--   0        0        0     1391 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/app.py
--rw-r--r--   0        0        0     1942 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/config.py
--rw-r--r--   0        0        0      456 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/database.py
--rw-r--r--   0        0        0      240 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/env.py
--rw-r--r--   0        0        0      202 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/index.py
--rw-r--r--   0        0        0     1953 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/models.py
--rw-r--r--   0        0        0      216 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/static/css/custom_flaks_admin.css
--rw-r--r--   0        0        0    30240 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/static/img/src_gn2pg.png
--rw-r--r--   0        0        0      185 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/templates/admin/master.html
--rw-r--r--   0        0        0      353 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/templates/index.html
--rw-r--r--   0        0        0        0 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/utils/__init__.py
--rw-r--r--   0        0        0      582 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/app/utils/admin_views.py
--rw-r--r--   0        0        0    11145 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/check_conf.py
--rw-r--r--   0        0        0     1835 2024-01-23 09:06:00.455002 gn2pg_client-1.6.1/gn2pg/data/gn2pgconfig.toml
--rw-r--r--   0        0        0    46508 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/data/to_gnsynthese.sql
--rw-r--r--   0        0        0     8839 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/download.py
--rw-r--r--   0        0        0      241 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/env.py
--rw-r--r--   0        0        0     3968 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/helpers.py
--rw-r--r--   0        0        0     4100 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
--rw-r--r--   0        0        0    10575 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
--rw-r--r--   0        0        0    10307 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
--rwxr-xr-x   0        0        0     6063 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/main.py
--rw-r--r--   0        0        0      765 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/metadata.py
--rw-r--r--   0        0        0    20834 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/store_postgresql.py
--rw-r--r--   0        0        0     1387 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/gn2pg/utils.py
--rw-r--r--   0        0        0     3169 2024-01-23 09:06:00.459002 gn2pg_client-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     9925 1970-01-01 00:00:00.000000 gn2pg_client-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-08 16:17:10.063278 gn2pg_client-1.6.2/LICENSE
+-rw-r--r--   0        0        0     6629 2024-04-08 16:17:10.063278 gn2pg_client-1.6.2/README.md
+-rw-r--r--   0        0        0     1059 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/__init__.py
+-rw-r--r--   0        0        0     7244 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/api.py
+-rw-r--r--   0        0        0        0 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/admin_views.py
+-rw-r--r--   0        0        0     1391 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/app.py
+-rw-r--r--   0        0        0     1942 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/config.py
+-rw-r--r--   0        0        0      456 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/database.py
+-rw-r--r--   0        0        0      240 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/env.py
+-rw-r--r--   0        0        0      202 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/index.py
+-rw-r--r--   0        0        0     1953 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/models.py
+-rw-r--r--   0        0        0      216 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/static/css/custom_flaks_admin.css
+-rw-r--r--   0        0        0    30240 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/static/img/src_gn2pg.png
+-rw-r--r--   0        0        0      185 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/templates/admin/master.html
+-rw-r--r--   0        0        0      353 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/templates/index.html
+-rw-r--r--   0        0        0        0 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/utils/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/app/utils/admin_views.py
+-rw-r--r--   0        0        0    11145 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/check_conf.py
+-rw-r--r--   0        0        0     1835 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/data/gn2pgconfig.toml
+-rw-r--r--   0        0        0    46535 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/data/to_gnsynthese.sql
+-rw-r--r--   0        0        0     8839 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/download.py
+-rw-r--r--   0        0        0      241 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/env.py
+-rw-r--r--   0        0        0     3968 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/helpers.py
+-rw-r--r--   0        0        0     4100 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
+-rw-r--r--   0        0        0    10575 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
+-rw-r--r--   0        0        0    10307 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
+-rwxr-xr-x   0        0        0     6063 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/main.py
+-rw-r--r--   0        0        0      765 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/metadata.py
+-rw-r--r--   0        0        0    20834 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/store_postgresql.py
+-rw-r--r--   0        0        0     1387 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/gn2pg/utils.py
+-rw-r--r--   0        0        0     3146 2024-04-08 16:17:10.071278 gn2pg_client-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     8661 1970-01-01 00:00:00.000000 gn2pg_client-1.6.2/PKG-INFO
```

### Comparing `gn2pg_client-1.6.1/LICENSE` & `gn2pg_client-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/__init__.py` & `gn2pg_client-1.6.2/gn2pg/__init__.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/api.py` & `gn2pg_client-1.6.2/gn2pg/api.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/app/admin_views.py` & `gn2pg_client-1.6.2/gn2pg/app/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/app/app.py` & `gn2pg_client-1.6.2/gn2pg/app/app.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/app/config.py` & `gn2pg_client-1.6.2/gn2pg/app/config.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/app/models.py` & `gn2pg_client-1.6.2/gn2pg/app/models.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/app/static/img/src_gn2pg.png` & `gn2pg_client-1.6.2/gn2pg/app/static/img/src_gn2pg.png`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/app/utils/admin_views.py` & `gn2pg_client-1.6.2/gn2pg/app/utils/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/check_conf.py` & `gn2pg_client-1.6.2/gn2pg/check_conf.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/data/gn2pgconfig.toml` & `gn2pg_client-1.6.2/gn2pg/data/gn2pgconfig.toml`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/data/to_gnsynthese.sql` & `gn2pg_client-1.6.2/gn2pg/data/to_gnsynthese.sql`

 * *Files 1% similar despite different names*

```diff
@@ -697,15 +697,15 @@
                ELSE ref_nomenclatures.get_id_nomenclature('TYPE', new.item #>> '{label}')
                END AS id_nomenclature_determination_method
     INTO the_id_nomenclature_determination_method;
     SELECT new.item #>> '{comment_releve}'
     INTO the_comment_context;
     SELECT new.item #>> '{comment_occurence}'
     INTO the_comment_description;
-    SELECT NULL
+    SELECT new.item #> '{additional_data}'
     INTO the_additional_data;
     SELECT NULL
     INTO the_meta_validation_date;
 
     /* Proceed to upsert */
     INSERT INTO gn_synthese.synthese ( unique_id_sinp
                                      , unique_id_sinp_grp
```

### Comparing `gn2pg_client-1.6.1/gn2pg/download.py` & `gn2pg_client-1.6.2/gn2pg/download.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/helpers.py` & `gn2pg_client-1.6.2/gn2pg/helpers.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po` & `gn2pg_client-1.6.2/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po` & `gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~` & `gn2pg_client-1.6.2/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/main.py` & `gn2pg_client-1.6.2/gn2pg/main.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/metadata.py` & `gn2pg_client-1.6.2/gn2pg/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Information describing the project.
 """
 
 # The package name, which is also the "UNIX name" for the project.
 PACKAGE = "gn2pg_client"
 PROJECT = "GeoNature 2 PostgreSQL Client application"
 PROJECT_NO_SPACES = PROJECT.replace(" ", "")
-VERSION = "1.6.1"
+VERSION = "1.6.2"
 DESCRIPTION = "Import tool from GeoNature to a PostgreSQL database through Export module API"
 AUTHORS = [
     "@lpofredc (LPOAuRA)",
     "@ophdlv (@NaturalSolutions)",
     "@mvergez (@NaturalSolutions)",
     "@Adrien-Pajot (@NaturalSolutions)",
     "@camillemonchicourt (@PnEcrins)",
```

### Comparing `gn2pg_client-1.6.1/gn2pg/store_postgresql.py` & `gn2pg_client-1.6.2/gn2pg/store_postgresql.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/gn2pg/utils.py` & `gn2pg_client-1.6.2/gn2pg/utils.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.1/pyproject.toml` & `gn2pg_client-1.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "gn2pg_client"
 packages = [{ include = "gn2pg" }]
-version = "1.6.1"
+version = "1.6.2"
 description = "Import tool from GeoNature to a PostgreSQL database through Export module API (client side)"
 authors = ["lpofredc <frederic.cloitre@lpo.fr>"]
 maintainers = ["lpofredc <frederic.cloitre@lpo.fr>"]
 license = "AGPL-3.0-or-later"
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/lpoaura/gn2gn_client/"
 keywords = ["GeoNature", "Export", "SINP", "opendata", "biodiversity"]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Affero General Public License v3",
@@ -26,26 +26,26 @@
 
 [tool.poetry.scripts]
 gn2pg_cli = "gn2pg.main:run"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-requests = "^2.28.2"
-psycopg2-binary = "^2.9.5"
-coloredlogs = "^15.0.1"
-schema = "^0.7.5"
-toml = "^0.10.2"
-sqlalchemy = "^1.4.46"
-flask = { version = "^2.2.3", optional = true }
-flask-sqlalchemy = { version = "^3.0.3", optional = true }
-flask-admin = { version = "^1.6.1", optional = true }
-gunicorn = { version = "^20.1.0", optional = true }
-python-decouple = { version = "^3.8", optional = true }
-python-dotenv = { version = "^1.0.0", optional = true }
+requests = "^2"
+psycopg2-binary = "^2"
+coloredlogs = ">=0.0.0"
+schema = "^0"
+toml = "^0"
+sqlalchemy = "^1"
+flask = { version = "^2", optional = true }
+flask-sqlalchemy = { version = "^3", optional = true }
+flask-admin = { version = "^1", optional = true }
+gunicorn = { version = ">=0.0.0", optional = true }
+python-decouple = { version = "^3", optional = true }
+python-dotenv = { version = "^1", optional = true }
 
 [tool.poetry.extras]
 dashboard = [
     'flask',
     'flask-sqlalchemy',
     'flask-admin',
     'gunicorn',
@@ -66,17 +66,18 @@
 types-setuptools = "^67.2.0.0"
 no-implicit-optional = "^1.3"
 types-toml = "^0.10.8.3"
 types-requests = "^2.28.11.12"
 
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1.3"
+sphinx = "^6"
 sphinx-rtd-theme = "^1.2.0"
 sphinxcontrib-napoleon = "^0.7"
+myst-parser = "^2.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 sqlalchemy-utils = "^0.39.0"
 pytest = "^7.2.1"
 
 [tool.isort]
```

