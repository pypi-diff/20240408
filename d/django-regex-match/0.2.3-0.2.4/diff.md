# Comparing `tmp/django-regex-match-0.2.3.tar.gz` & `tmp/django-regex-match-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/vitorohe/Admetricks/django-regex-match/dist/tmpdizg8hd4/django-regex-match-0.2.3.tar", last modified: Thu Oct 20 17:45:44 2022, max compression
+gzip compressed data, was "django-regex-match-0.2.4.tar", last modified: Mon Apr  8 20:15:22 2024, max compression
```

## Comparing `django-regex-match-0.2.3.tar` & `django-regex-match-0.2.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.844226 django-regex-match-0.2.3/
--rw-r--r--   0 vitorohe   (501) staff       (20)      116 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/MANIFEST.in
--rw-r--r--   0 vitorohe   (501) staff       (20)      410 2022-10-20 17:45:44.842441 django-regex-match-0.2.3/PKG-INFO
--rw-r--r--   0 vitorohe   (501) staff       (20)     1597 2022-10-19 14:54:24.000000 django-regex-match-0.2.3/README.md
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.751588 django-regex-match-0.2.3/django_regex_match.egg-info/
--rw-r--r--   0 vitorohe   (501) staff       (20)      410 2022-10-20 17:45:44.000000 django-regex-match-0.2.3/django_regex_match.egg-info/PKG-INFO
--rw-r--r--   0 vitorohe   (501) staff       (20)     1246 2022-10-20 17:45:44.000000 django-regex-match-0.2.3/django_regex_match.egg-info/SOURCES.txt
--rw-r--r--   0 vitorohe   (501) staff       (20)        1 2022-10-20 17:45:44.000000 django-regex-match-0.2.3/django_regex_match.egg-info/dependency_links.txt
--rw-r--r--   0 vitorohe   (501) staff       (20)        1 2022-10-19 14:55:37.000000 django-regex-match-0.2.3/django_regex_match.egg-info/not-zip-safe
--rw-r--r--   0 vitorohe   (501) staff       (20)       79 2022-10-20 17:45:44.000000 django-regex-match-0.2.3/django_regex_match.egg-info/requires.txt
--rw-r--r--   0 vitorohe   (501) staff       (20)      102 2022-10-20 17:45:44.000000 django-regex-match-0.2.3/django_regex_match.egg-info/top_level.txt
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.753790 django-regex-match-0.2.3/regex_match/
--rw-r--r--   0 vitorohe   (501) staff       (20)      170 2022-10-20 17:45:16.000000 django-regex-match-0.2.3/regex_match/__init__.py
--rw-r--r--   0 vitorohe   (501) staff       (20)     1336 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/factory.py
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.789491 django-regex-match-0.2.3/regex_match/migrations/
--rw-r--r--   0 vitorohe   (501) staff       (20)     5250 2022-10-20 17:44:46.000000 django-regex-match-0.2.3/regex_match/migrations/0001_initial.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      405 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/0002_modelrule_priority.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      374 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/0003_auto_20151110_1315.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      408 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/0004_auto_20151112_1808.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      409 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/0005_auto_20151117_2133.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      703 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/0006_auto_20160916_1428.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      494 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/0007_auto_20200715_1610.py
--rw-r--r--   0 vitorohe   (501) staff       (20)        0 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/migrations/__init__.py
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.814258 django-regex-match-0.2.3/regex_match/models/
--rw-r--r--   0 vitorohe   (501) staff       (20)      879 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/models/__init__.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      255 2022-10-19 14:54:24.000000 django-regex-match-0.2.3/regex_match/models/exception_parser.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      848 2022-10-19 14:54:24.000000 django-regex-match-0.2.3/regex_match/models/matching_rule.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      572 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/models/model_exception.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      707 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/models/model_rule.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      862 2022-10-19 14:54:24.000000 django-regex-match-0.2.3/regex_match/models/parser.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      290 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/models/parser_method.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      683 2022-10-19 14:54:24.000000 django-regex-match-0.2.3/regex_match/models/regex_rule.py
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.829372 django-regex-match-0.2.3/regex_match/objects/
--rw-r--r--   0 vitorohe   (501) staff       (20)      880 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/__init__.py
--rw-r--r--   0 vitorohe   (501) staff       (20)      605 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/exception_parser.py
--rw-r--r--   0 vitorohe   (501) staff       (20)     2701 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/model_matcher.py
-drwxr-xr-x   0 vitorohe   (501) staff       (20)        0 2022-10-20 17:45:44.840366 django-regex-match-0.2.3/regex_match/objects/parsers/
--rw-r--r--   0 vitorohe   (501) staff       (20)      888 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/parsers/__init__.py
--rw-r--r--   0 vitorohe   (501) staff       (20)     6892 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/parsers/url.py
--rw-r--r--   0 vitorohe   (501) staff       (20)     2016 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/parsers/url_parser.py
--rw-r--r--   0 vitorohe   (501) staff       (20)     3095 2022-10-11 20:40:09.000000 django-regex-match-0.2.3/regex_match/objects/url_to_matching_rule.py
--rw-r--r--   0 vitorohe   (501) staff       (20)       38 2022-10-20 17:45:44.844534 django-regex-match-0.2.3/setup.cfg
--rw-r--r--   0 vitorohe   (501) staff       (20)     1611 2022-10-19 14:54:24.000000 django-regex-match-0.2.3/setup.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      116 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/MANIFEST.in
+-rw-r--r--   0 sebastiang  (1000) sebastiang  (1000)      564 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/PKG-INFO
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1597 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/README.md
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/django_regex_match.egg-info/
+-rw-r--r--   0 sebastiang  (1000) sebastiang  (1000)      564 2024-04-08 20:15:22.000000 django-regex-match-0.2.4/django_regex_match.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1246 2024-04-08 20:15:22.000000 django-regex-match-0.2.4/django_regex_match.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        1 2024-04-08 20:15:22.000000 django-regex-match-0.2.4/django_regex_match.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        1 2024-04-08 20:15:22.000000 django-regex-match-0.2.4/django_regex_match.egg-info/not-zip-safe
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)       79 2024-04-08 20:15:22.000000 django-regex-match-0.2.4/django_regex_match.egg-info/requires.txt
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      102 2024-04-08 20:15:22.000000 django-regex-match-0.2.4/django_regex_match.egg-info/top_level.txt
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/regex_match/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      170 2024-04-08 20:09:55.000000 django-regex-match-0.2.4/regex_match/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1336 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/factory.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/regex_match/migrations/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     5016 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0001_initial.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      405 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0002_modelrule_priority.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      374 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0003_auto_20151110_1315.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      408 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0004_auto_20151112_1808.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      409 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0005_auto_20151117_2133.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      703 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0006_auto_20160916_1428.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      494 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/0007_auto_20200715_1610.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        0 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/migrations/__init__.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/regex_match/models/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      879 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      255 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/exception_parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      848 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/matching_rule.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      572 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/model_exception.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      707 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/model_rule.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      862 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      290 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/parser_method.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      683 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/models/regex_rule.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/regex_match/objects/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      880 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/objects/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      605 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/objects/exception_parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     2701 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/objects/model_matcher.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/regex_match/objects/parsers/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      888 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/objects/parsers/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     6892 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/objects/parsers/url.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     2016 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/regex_match/objects/parsers/url_parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     3422 2024-04-08 20:04:53.000000 django-regex-match-0.2.4/regex_match/objects/url_to_matching_rule.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)       38 2024-04-08 20:15:22.190034 django-regex-match-0.2.4/setup.cfg
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1611 2024-03-15 16:30:04.000000 django-regex-match-0.2.4/setup.py
```

### Comparing `django-regex-match-0.2.3/README.md` & `django-regex-match-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/django_regex_match.egg-info/SOURCES.txt` & `django-regex-match-0.2.4/django_regex_match.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/factory.py` & `django-regex-match-0.2.4/regex_match/factory.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/migrations/0001_initial.py` & `django-regex-match-0.2.4/regex_match/migrations/0001_initial.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,73 +52,73 @@
                 ('type', models.CharField(max_length=50)),
                 ('name', models.CharField(max_length=50)),
             ],
         ),
         migrations.CreateModel(
             name='ExceptionParser',
             fields=[
-                ('parser_ptr', models.OneToOneField(primary_key=True, parent_link=True, to='regex_match.Parser', auto_created=True, serialize=False, on_delete=models.CASCADE)),
+                ('parser_ptr', models.OneToOneField(primary_key=True, parent_link=True, to='regex_match.Parser', auto_created=True, serialize=False)),
                 ('name', models.CharField(max_length=32)),
             ],
             options={
                 'abstract': False,
             },
             bases=('regex_match.parser',),
         ),
         migrations.CreateModel(
             name='ModelException',
             fields=[
-                ('modelrule_ptr', models.OneToOneField(primary_key=True, parent_link=True, to='regex_match.ModelRule', auto_created=True, serialize=False, on_delete=models.CASCADE)),
+                ('modelrule_ptr', models.OneToOneField(primary_key=True, parent_link=True, to='regex_match.ModelRule', auto_created=True, serialize=False)),
                 ('name', models.CharField(max_length=32)),
                 ('template', models.CharField(max_length=64)),
             ],
             options={
                 'abstract': False,
             },
             bases=('regex_match.modelrule',),
         ),
         migrations.CreateModel(
             name='RegexRule',
             fields=[
-                ('parser_ptr', models.OneToOneField(primary_key=True, parent_link=True, to='regex_match.Parser', auto_created=True, serialize=False, on_delete=models.CASCADE)),
+                ('parser_ptr', models.OneToOneField(primary_key=True, parent_link=True, to='regex_match.Parser', auto_created=True, serialize=False)),
                 ('regex', models.CharField(max_length=32)),
             ],
             options={
                 'abstract': False,
             },
             bases=('regex_match.parser',),
         ),
         migrations.AlterUniqueTogether(
             name='parsermethod',
             unique_together=set([('name', 'type')]),
         ),
         migrations.AddField(
             model_name='parser',
             name='parser_method',
-            field=models.ForeignKey(related_name='parsers', to='regex_match.ParserMethod', on_delete=models.CASCADE),
+            field=models.ForeignKey(related_name='parsers', to='regex_match.ParserMethod'),
         ),
         migrations.AddField(
             model_name='parser',
             name='polymorphic_ctype',
-            field=models.ForeignKey(related_name='polymorphic_regex_match.parser_set+', editable=False, to='contenttypes.ContentType', null=True, on_delete=models.CASCADE),
+            field=models.ForeignKey(related_name='polymorphic_regex_match.parser_set+', editable=False, to='contenttypes.ContentType', null=True),
         ),
         migrations.AddField(
             model_name='modelrule',
             name='polymorphic_ctype',
-            field=models.ForeignKey(related_name='polymorphic_regex_match.modelrule_set+', editable=False, to='contenttypes.ContentType', null=True, on_delete=models.CASCADE),
+            field=models.ForeignKey(related_name='polymorphic_regex_match.modelrule_set+', editable=False, to='contenttypes.ContentType', null=True),
         ),
         migrations.AddField(
             model_name='matchingrule',
             name='model_rule',
-            field=models.ForeignKey(related_name='matching_rules', to='regex_match.ModelRule', on_delete=models.CASCADE),
+            field=models.ForeignKey(related_name='matching_rules', to='regex_match.ModelRule'),
         ),
         migrations.AddField(
             model_name='regexrule',
             name='matching_rule',
-            field=models.ForeignKey(related_name='regex_rules', to='regex_match.MatchingRule', on_delete=models.CASCADE),
+            field=models.ForeignKey(related_name='regex_rules', to='regex_match.MatchingRule'),
         ),
         migrations.AddField(
             model_name='exceptionparser',
             name='model_exception',
-            field=models.ForeignKey(related_name='parsers', to='regex_match.ModelException', on_delete=models.CASCADE),
+            field=models.ForeignKey(related_name='parsers', to='regex_match.ModelException'),
         ),
     ]
```

### Comparing `django-regex-match-0.2.3/regex_match/migrations/0006_auto_20160916_1428.py` & `django-regex-match-0.2.4/regex_match/migrations/0006_auto_20160916_1428.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/models/__init__.py` & `django-regex-match-0.2.4/regex_match/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/models/matching_rule.py` & `django-regex-match-0.2.4/regex_match/models/matching_rule.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/models/model_exception.py` & `django-regex-match-0.2.4/regex_match/models/model_exception.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/models/model_rule.py` & `django-regex-match-0.2.4/regex_match/models/model_rule.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/models/parser.py` & `django-regex-match-0.2.4/regex_match/models/parser.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/models/regex_rule.py` & `django-regex-match-0.2.4/regex_match/models/regex_rule.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/__init__.py` & `django-regex-match-0.2.4/regex_match/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/exception_parser.py` & `django-regex-match-0.2.4/regex_match/objects/exception_parser.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/model_matcher.py` & `django-regex-match-0.2.4/regex_match/objects/model_matcher.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/parsers/__init__.py` & `django-regex-match-0.2.4/regex_match/objects/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/parsers/url.py` & `django-regex-match-0.2.4/regex_match/objects/parsers/url.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/parsers/url_parser.py` & `django-regex-match-0.2.4/regex_match/objects/parsers/url_parser.py`

 * *Files identical despite different names*

### Comparing `django-regex-match-0.2.3/regex_match/objects/url_to_matching_rule.py` & `django-regex-match-0.2.4/regex_match/objects/url_to_matching_rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,99 @@
 from funcy import keep
 
 from regex_match.models import MatchingRule, ParserMethod, RegexRule
 from regex_match.objects.parsers import UrlParser
 
 
 class UrlToMatchingRule(object):
-    default_regex_template_domain = '((^.*[.])|^){}$'
-    default_regex_template_path = '^{}(/.*|)$'
-    default_regex_template_query = '(^|.+&){}={}($|&.+)'
+    default_regex_template_domain = "((^.*[.])|^){}$"
+    default_regex_template_path = "^{}(/.*|)$"
+    default_regex_template_query = "(^|.+&){}={}($|&.+)"
 
     def __init__(
-            self, model_rule, urls, priority_func=None, description='',
-            regex_template_domain=None, regex_template_path=None,
-            regex_template_query=None):
-        self.regex_template_domain = regex_template_domain or self.default_regex_template_domain
-        self.regex_template_path = regex_template_path or self.default_regex_template_path
-        self.regex_template_query = regex_template_query or self.default_regex_template_query
+        self,
+        model_rule,
+        urls,
+        priority_func=None,
+        description="",
+        regex_template_domain=None,
+        regex_template_path=None,
+        regex_template_query=None,
+    ):
+        self.regex_template_domain = (
+            regex_template_domain or self.default_regex_template_domain
+        )
+        self.regex_template_path = (
+            regex_template_path or self.default_regex_template_path
+        )
+        self.regex_template_query = (
+            regex_template_query or self.default_regex_template_query
+        )
 
         self.model_rule = model_rule
         self.urls = urls
         self.priority_func = priority_func
         self.description = description
 
     def create(self):
         matching_rule_array = keep(self._create_matching_rule, self.urls)
         return list(matching_rule_array)
 
     def _create_matching_rule(self, url):
         obj = UrlParser(url)
 
-        matching_rule = MatchingRule(model_rule=self.model_rule, description=self.description)
+        matching_rule = MatchingRule(
+            model_rule=self.model_rule, description=self.description
+        )
         matching_rule.save()
 
         domain_rule = self._create_domain_matching_rule(matching_rule, obj)
 
-        path_rule = self._create_path_matching_rule(matching_rule, obj, bool(obj.url.query_params()))
+        path_rule = self._create_path_matching_rule(
+            matching_rule, obj, bool(obj.url.query_params())
+        )
 
         query_rules = self._create_query_matching_rule(matching_rule, obj)
 
         if self.priority_func is not None:
             self.priority = self.priority_func(domain_rule, path_rule, query_rules)
 
         return matching_rule
 
     def _create_domain_matching_rule(self, matching_rule, url):
-        if url.domain() != '':
+        if url.domain() != "":
 
-            parser_method = ParserMethod.objects.get(name='domain')
+            parser_method = ParserMethod.objects.get(name="domain")
             return RegexRule.objects.create(
                 matching_rule=matching_rule,
                 parser_method=parser_method,
-                regex=self.regex_template_domain.format(url.domain().replace('.', '[.]'))
+                regex=self.regex_template_domain.format(
+                    url.domain().replace(".", "[.]").replace("+", "[+]")
+                ),
             )
 
     def _create_path_matching_rule(self, matching_rule, url, has_params):
-        if url.path() != '':
+        if url.path() != "":
             regex_template = self.regex_template_path
-            parser_method = ParserMethod.objects.get(name='path')
+            parser_method = ParserMethod.objects.get(name="path")
             return RegexRule.objects.create(
                 matching_rule=matching_rule,
                 parser_method=parser_method,
-                regex=regex_template.format(url.path().replace('.', '[.]'))
+                regex=regex_template.format(
+                    url.path().replace(".", "[.]").replace("+", "[+]")
+                ),
             )
 
     def _create_query_matching_rule(self, matching_rule, url):
         result = list()
         query_params = url.url.query_params()
         for k in query_params:
-            parser_method = ParserMethod.objects.get(name='query')
+            parser_method = ParserMethod.objects.get(name="query")
             rule = RegexRule.objects.create(
                 matching_rule=matching_rule,
                 parser_method=parser_method,
-                regex=self.regex_template_query.format(k, url.query_param(k).replace('.', '[.]'))
+                regex=self.regex_template_query.format(
+                    k, url.query_param(k).replace(".", "[.]").replace("+", "[+]")
+                ),
             )
             result.append(rule)
         return result
```

### Comparing `django-regex-match-0.2.3/setup.py` & `django-regex-match-0.2.4/setup.py`

 * *Files identical despite different names*

