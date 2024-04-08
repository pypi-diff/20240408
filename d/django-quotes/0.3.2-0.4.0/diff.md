# Comparing `tmp/django_quotes-0.3.2.tar.gz` & `tmp/django_quotes-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_quotes-0.3.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django_quotes-0.3.2.tar` & `django_quotes-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,62 @@
--rw-r--r--   0        0        0     1493 2022-03-02 14:59:26.568004 django_quotes-0.3.2/LICENSE
--rw-r--r--   0        0        0     2120 2022-05-26 18:13:06.980209 django_quotes-0.3.2/README.md
--rw-r--r--   0        0        0        0 2022-04-22 15:18:45.308888 django_quotes-0.3.2/django_quotes/__init__.py
--rw-r--r--   0        0        0     1046 2022-03-24 18:23:16.119360 django_quotes-0.3.2/django_quotes/admin.py
--rw-r--r--   0        0        0        0 2022-03-02 15:47:13.379557 django_quotes-0.3.2/django_quotes/api/__init__.py
--rw-r--r--   0        0        0      718 2022-04-22 15:18:45.309394 django_quotes-0.3.2/django_quotes/api/serializers.py
--rw-r--r--   0        0        0     5191 2022-03-24 18:23:16.222620 django_quotes-0.3.2/django_quotes/api/views.py
--rw-r--r--   0        0        0      392 2022-03-02 15:50:11.592031 django_quotes-0.3.2/django_quotes/apps.py
--rw-r--r--   0        0        0        0 2022-03-02 15:47:33.486391 django_quotes-0.3.2/django_quotes/management/__init__.py
--rw-r--r--   0        0        0        0 2022-03-02 15:48:40.806119 django_quotes-0.3.2/django_quotes/management/commands/__init__.py
--rw-r--r--   0        0        0     1389 2022-03-03 14:09:27.700284 django_quotes-0.3.2/django_quotes/management/commands/makemarkov.py
--rw-r--r--   0        0        0      464 2022-03-21 15:46:40.511157 django_quotes-0.3.2/django_quotes/markov_utils.py
--rw-r--r--   0        0        0    10478 2022-03-24 18:27:39.830556 django_quotes-0.3.2/django_quotes/migrations/0001_initial.py
--rw-r--r--   0        0        0      513 2022-03-24 18:27:39.830829 django_quotes-0.3.2/django_quotes/migrations/0002_alter_sourcegroup_name.py
--rw-r--r--   0        0        0      779 2022-03-24 18:27:39.831069 django_quotes-0.3.2/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py
--rw-r--r--   0        0        0      565 2022-10-11 18:20:56.872765 django_quotes-0.3.2/django_quotes/migrations/0004_quote_pub_date.py
--rw-r--r--   0        0        0        0 2022-03-02 19:16:35.101240 django_quotes-0.3.2/django_quotes/migrations/__init__.py
--rw-r--r--   0        0        0    21750 2023-01-06 15:09:18.946973 django_quotes-0.3.2/django_quotes/models.py
--rw-r--r--   0        0        0        0 2022-03-23 18:29:46.875341 django_quotes-0.3.2/django_quotes/py.typed
--rw-r--r--   0        0        0     4370 2022-03-24 18:23:16.191416 django_quotes-0.3.2/django_quotes/receivers.py
--rw-r--r--   0        0        0      539 2022-03-02 16:00:48.225464 django_quotes-0.3.2/django_quotes/rules.py
--rw-r--r--   0        0        0      128 2022-03-02 16:00:48.231252 django_quotes-0.3.2/django_quotes/signals.py
--rw-r--r--   0        0        0        0 2022-03-02 16:28:54.879305 django_quotes-0.3.2/django_quotes/static/.gitkeep
--rw-r--r--   0        0        0      150 2022-03-02 17:32:10.444576 django_quotes-0.3.2/django_quotes/templates/base.html
--rw-r--r--   0        0        0        0 2022-03-02 16:48:01.441440 django_quotes-0.3.2/django_quotes/templates/quotes/base.html
--rw-r--r--   0        0        0      731 2022-03-03 14:09:27.701805 django_quotes-0.3.2/django_quotes/templates/quotes/group_create.html
--rw-r--r--   0        0        0      936 2022-03-03 14:09:27.701994 django_quotes-0.3.2/django_quotes/templates/quotes/group_delete.html
--rw-r--r--   0        0        0     3224 2022-03-03 14:09:27.702169 django_quotes-0.3.2/django_quotes/templates/quotes/group_detail.html
--rw-r--r--   0        0        0     2147 2022-05-19 15:28:06.979725 django_quotes-0.3.2/django_quotes/templates/quotes/group_list.html
--rw-r--r--   0        0        0      880 2022-03-03 14:09:27.702653 django_quotes-0.3.2/django_quotes/templates/quotes/group_update.html
--rw-r--r--   0        0        0     1422 2022-03-03 14:09:27.702888 django_quotes-0.3.2/django_quotes/templates/quotes/quote_create.html
--rw-r--r--   0        0        0     1622 2022-03-03 14:09:27.703108 django_quotes-0.3.2/django_quotes/templates/quotes/quote_delete.html
--rw-r--r--   0        0        0     2418 2022-10-11 18:20:56.953827 django_quotes-0.3.2/django_quotes/templates/quotes/quote_detail.html
--rw-r--r--   0        0        0     3320 2022-05-19 15:28:06.955997 django_quotes-0.3.2/django_quotes/templates/quotes/quote_list.html
--rw-r--r--   0        0        0     1659 2022-03-03 14:09:27.704048 django_quotes-0.3.2/django_quotes/templates/quotes/quote_update.html
--rw-r--r--   0        0        0     1196 2022-03-03 14:09:27.704325 django_quotes-0.3.2/django_quotes/templates/quotes/source_create.html
--rw-r--r--   0        0        0     1229 2022-03-03 14:09:27.704633 django_quotes-0.3.2/django_quotes/templates/quotes/source_delete.html
--rw-r--r--   0        0        0     3734 2022-03-03 14:09:27.704931 django_quotes-0.3.2/django_quotes/templates/quotes/source_detail.html
--rw-r--r--   0        0        0     2606 2022-05-19 15:26:25.961306 django_quotes-0.3.2/django_quotes/templates/quotes/source_list.html
--rw-r--r--   0        0        0     1239 2022-03-03 14:09:27.705510 django_quotes-0.3.2/django_quotes/templates/quotes/source_update.html
--rw-r--r--   0        0        0     2186 2022-03-24 18:23:16.174586 django_quotes-0.3.2/django_quotes/urls.py
--rw-r--r--   0        0        0     1943 2022-03-21 15:46:40.512004 django_quotes-0.3.2/django_quotes/utils.py
--rw-r--r--   0        0        0    11775 2023-01-06 15:14:23.203234 django_quotes-0.3.2/django_quotes/views.py
--rw-r--r--   0        0        0     4647 2023-01-06 15:17:02.964811 django_quotes-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3540 1970-01-01 00:00:00.000000 django_quotes-0.3.2/setup.py
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 django_quotes-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/__init__.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/admin.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/apps.py
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/py.typed
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/receivers.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/rules.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/signals.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/urls.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/utils.py
+-rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/api/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/api/serializers.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/api/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/management/commands/__init__.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/management/commands/makemarkov.py
+-rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0006_alter_source_description_rendered.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0008_auto_20240404_1952.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/static/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/base.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/base.html
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/group_create.html
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/group_delete.html
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/group_detail.html
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/group_list.html
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/group_update.html
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_create.html
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_delete.html
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_detail.html
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_list.html
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_update.html
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/source_create.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/source_delete.html
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/source_detail.html
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/source_list.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 django_quotes-0.4.0/src/django_quotes/templates/quotes/source_update.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/api_router.py
+-rw-r--r--   0        0        0    10144 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/django_settings.py
+-rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_api.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_docs.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_management.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_models.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_signals.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0    18070 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/test_views.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/factories/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 django_quotes-0.4.0/tests/factories/users.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 django_quotes-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 django_quotes-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 django_quotes-0.4.0/README.md
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 django_quotes-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 django_quotes-0.4.0/PKG-INFO
```

### Comparing `django_quotes-0.3.2/LICENSE` & `django_quotes-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_quotes-0.3.2/README.md` & `django_quotes-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 A simple reusable [Django](https://www.djangoproject.com) app that allows you to collect quotes from arbitrary groups of characters, and then serve random quotes or Markov-chain generated sentences based upon them. Includes a Bootstrap compatible set of templates an optional REST API.
 
 ![PyPI](https://img.shields.io/pypi/v/django-quotes)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/andrlik/django-quotes/blob/main/.pre-commit-config.yaml)
 [![License](https://img.shields.io/github/license/andrlik/django-quotes)](https://github.com/andrlik/django-quotes/blob/main/LICENSE)
+[![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/andrlik/django-quotes/releases)
 ![Test results](https://github.com/andrlik/django-quotes/actions/workflows/ci.yml/badge.svg)
-![Codestyle check results](https://github.com/andrlik/django-quotes/actions/workflows/codestyle.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/andrlik/django-quotes/badge.svg?branch=main)](https://coveralls.io/github/andrlik/django-quotes?branch=main)
 [![Documentation](https://img.shields.io/badge/docs-mkdocs-blue)](https://andrlik.github.io/django-quotes/)
 
 ## Features
 
 - Documentation and a full test suite.
 - Support for abstract grouping of quote sources.
```

### Comparing `django_quotes-0.3.2/django_quotes/api/views.py` & `django_quotes-0.4.0/src/django_quotes/api/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from rest_framework.decorators import action
 from rest_framework.fields import CharField
 from rest_framework.mixins import ListModelMixin, RetrieveModelMixin
 from rest_framework.response import Response
 from rest_framework.viewsets import GenericViewSet
 from rules.contrib.rest_framework import AutoPermissionViewSetMixin
 
-from ..models import Source, SourceGroup
-from .serializers import QuoteSerializer, SourceGroupSerializer, SourceSerializer
+from django_quotes.api.serializers import (
+    QuoteSerializer,
+    SourceGroupSerializer,
+    SourceSerializer,
+)
+from django_quotes.models import Source, SourceGroup
 
 
-class SourceGroupViewSet(
-    AutoPermissionViewSetMixin, RetrieveModelMixin, ListModelMixin, GenericViewSet
-):
+class SourceGroupViewSet(AutoPermissionViewSetMixin, RetrieveModelMixin, ListModelMixin, GenericViewSet):
     """
     A generic viewset for listing and retrieving details on sourceGroup groups.
     """
 
     serializer_class = SourceGroupSerializer
     lookup_field = "slug"
     lookup_url_kwarg = "group"
@@ -30,59 +32,47 @@
         "retrieve": "read",
         "update": "change",
         "get_random_quote": "read",
         "generate_sentence": "read",
     }
 
     def get_queryset(self, *args, **kwargs):
-        return SourceGroup.objects.filter(
-            owner=self.request.user  # type: ignore
-        ) | SourceGroup.objects.filter(public=True)
+        return SourceGroup.objects.filter(owner=self.request.user) | SourceGroup.objects.filter(  # type: ignore
+            public=True
+        )
 
     @extend_schema(responses={200: QuoteSerializer})
     @action(detail=True, methods=["get"])
     def get_random_quote(self, request, group=None):
         g = self.get_object()
         quote = g.get_random_quote()
         if quote is not None:
             qs = QuoteSerializer(quote)
             return Response(status=status.HTTP_200_OK, data=qs.data)
-        return Response(
-            status=status.HTTP_404_NOT_FOUND, data={"error": "No quotes found."}
-        )
+        return Response(status=status.HTTP_404_NOT_FOUND, data={"error": "No quotes found."})
 
-    @extend_schema(
-        responses={
-            200: inline_serializer(
-                name="generated_sentence", fields={"sentence": CharField()}
-            )
-        }
-    )
+    @extend_schema(responses={200: inline_serializer(name="generated_sentence", fields={"sentence": CharField()})})
     @action(detail=True, methods=["get"])
     def generate_sentence(self, request, group=None):
         g = self.get_object()
         if g.markov_sources == 0:
             return Response(
                 status=status.HTTP_403_FORBIDDEN,
-                data={
-                    "error": "This group does not currently allow sentence generation."
-                },
+                data={"error": "This group does not currently allow sentence generation."},
             )
         sentence = g.generate_markov_sentence()
         if sentence is not None:
             return Response(status=status.HTTP_200_OK, data={"sentence": sentence})
         return Response(
             status=status.HTTP_204_NO_CONTENT,
             data={"error": "Insufficent data to generate sentence."},
         )
 
 
-class SourceViewSet(
-    AutoPermissionViewSetMixin, RetrieveModelMixin, ListModelMixin, GenericViewSet
-):
+class SourceViewSet(AutoPermissionViewSetMixin, RetrieveModelMixin, ListModelMixin, GenericViewSet):
     """
     Retrieve and list views for sources.
     """
 
     serializer_class = SourceSerializer
     lookup_field = "slug"
     lookup_url_kwarg = "source"
@@ -94,18 +84,16 @@
         "retrieve": "read",
         "update": "change",
         "get_random_quote": "read",
         "generate_sentence": "read",
     }
 
     def get_queryset(self, *args, **kwargs):
-        group_slug = self.request.query_params.get("group")
-        queryset = Source.objects.filter(
-            owner=self.request.user  # type: ignore
-        ) | Source.objects.filter(public=True)
+        group_slug = self.request.query_params.get("group")  # type: ignore
+        queryset = Source.objects.filter(owner=self.request.user) | Source.objects.filter(public=True)  # type: ignore
         if group_slug:
             try:
                 group = SourceGroup.objects.get(slug=group_slug)
             except ObjectDoesNotExist:
                 return SourceGroup.objects.none()
             queryset = queryset.filter(group=group)
         return queryset
@@ -114,35 +102,25 @@
     @action(detail=True, methods=["get"])
     def get_random_quote(self, request, source=None):
         source = self.get_object()
         quote = source.get_random_quote()
         if quote is not None:
             qs = QuoteSerializer(quote)
             return Response(status=status.HTTP_200_OK, data=qs.data)
-        return Response(
-            status=status.HTTP_404_NOT_FOUND, data={"error": "No quotes found."}
-        )
+        return Response(status=status.HTTP_404_NOT_FOUND, data={"error": "No quotes found."})
 
-    @extend_schema(
-        responses={
-            200: inline_serializer(
-                name="generated_sentence", fields={"sentence": CharField()}
-            )
-        }
-    )
+    @extend_schema(responses={200: inline_serializer(name="generated_sentence", fields={"sentence": CharField()})})
     @action(detail=True, methods=["get"])
     def generate_sentence(self, request, source=None):
         source = self.get_object()
         if not source.allow_markov:
             return Response(
                 status=status.HTTP_403_FORBIDDEN,
                 data={"error": "This source does not permit sentence generation."},
             )
         sentence = source.get_markov_sentence()
         if sentence is not None:
             return Response(status=status.HTTP_200_OK, data={"sentence": sentence})
         return Response(
             status=status.HTTP_204_NO_CONTENT,
-            data={
-                "error": "Unable to generate markov sentence. This source may not have enough quotes yet."
-            },
+            data={"error": "Unable to generate markov sentence. This source may not have enough quotes yet."},
         )
```

### Comparing `django_quotes-0.3.2/django_quotes/management/commands/makemarkov.py` & `django_quotes-0.4.0/src/django_quotes/management/commands/makemarkov.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+"""Checks if markov models are out of date, and if so regenerates them."""
+
 from django.core.management.base import BaseCommand
 
-from ...models import GroupMarkovModel, SourceGroup, SourceMarkovModel
+from django_quotes.models import SourceGroup
 
 
 class Command(BaseCommand):
     help = "Checks if markov models are out of date, and if so regenerates them."
 
     def handle(self, *args, **kwargs):
         groups = SourceGroup.objects.all()
         groups_updated = 0
         characters_updated = 0
         for group in groups:
-            gmm = GroupMarkovModel.objects.get(group=group)
+            gmm = group.text_model
             update_group = False
             for character in group.source_set.filter(allow_markov=True):
                 if character.markov_ready:
                     quote_to_test = character.quote_set.all().order_by("-modified")[0]
-                    cmm = SourceMarkovModel.objects.get(source=character)
+                    cmm = character.text_model
                     if cmm.modified > gmm.modified:
                         update_group = True
                     if quote_to_test.modified > cmm.modified:
-                        cmm.generate_model_from_corpus()
+                        character.update_markov_model()
                         characters_updated += 1
                         update_group = True
             if update_group:
-                gmm.generate_model_from_corpus()
+                group.update_markov_model()
                 groups_updated += 1
         self.stdout.write(
             self.style.SUCCESS(
-                f"Updated models for {groups_updated} Character Groups and {characters_updated} Characters!"
+                f"Updated models for {groups_updated} Character Groups " f"and {characters_updated} Characters!"
             )
         )
```

### Comparing `django_quotes-0.3.2/django_quotes/models.py` & `django_quotes-0.4.0/src/django_quotes/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
-from typing import Any, Optional
-
 import random
+from typing import TYPE_CHECKING, Any
 
 import rules
+from asgiref.sync import async_to_sync
+
+if TYPE_CHECKING:
+    from django.db.models.manager import RelatedManager
 from django.conf import settings
 from django.db import models
 from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from loguru import logger
-from model_utils.models import TimeStampedModel
 from rules.contrib.models import RulesModelBase, RulesModelMixin
 
-from .markov_utils import MarkovPOSText
-from .rules import (  # is_character_owner,; is_group_owner_and_authenticated,
+from django_markov.models import MarkovTextModel
+from django_quotes.rules import (  # is_character_owner,; is_group_owner_and_authenticated,
     is_owner,
     is_owner_or_public,
 )
-from .signals import markov_sentence_generated, quote_random_retrieved
-from .utils import generate_unique_slug_for_model
+from django_quotes.signals import quote_random_retrieved
+from django_quotes.utils import generate_unique_slug_for_model
 
 MAX_QUOTES_FOR_RANDOM_SET = 50
 MAX_QUOTES_FOR_RANDOM_GROUP_SET = 50
 
 if hasattr(settings, "MAX_QUOTES_FOR_RANDOM_SET"):  # pragma: nocover
     MAX_QUOTES_FOR_RANDOM_SET = settings.MAX_QUOTES_FOR_RANDOM_SET
 
@@ -43,27 +45,33 @@
         owner (User): The user that created this object.
     """
 
     public = models.BooleanField(
         default=False,
         help_text=_("Is this a public source available for any user to view?"),
     )
-    allow_submissions = models.BooleanField(
-        default=False, help_text=_("Allow submissions from other users?")
-    )
+    allow_submissions = models.BooleanField(default=False, help_text=_("Allow submissions from other users?"))
     owner = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
 
     class Meta:
         abstract = True
 
 
+class TimeStampedModel(models.Model):
+    """Automatically adds a created and modified field."""
+
+    created = models.DateTimeField(auto_now_add=True, help_text=_("Created timestamp"))
+    modified = models.DateTimeField(auto_now=True, help_text=_("Last modified time"))
+
+    class Meta:
+        abstract = True
+
+
 # Create your models here.
-class SourceGroup(
-    AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase
-):
+class SourceGroup(AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase):
     """
     An abstract group or source for a given set of quotes. Multiple sources, or Source objects, can belong to
     the same group. For example, a novel or series if you plan to quote the characters within individually.
 
     Attributes:
         id (int): Database primary key for the object.
         name (str): Human readable string to name the group. This will be converted to a slug prefix.
@@ -74,20 +82,21 @@
         allow_submissions (bool): Allow other users to submit characters to this. Not yet implemented.
         slug (str): A unique slug to represent this group. Generated automatically from name.
         created (datetime): When this object was first created. Auto-generated.
         modified (datetime): Last time this object was modified. Auto-generated.
 
     """
 
+    if TYPE_CHECKING:
+        source_set: RelatedManager[Source]
+
     name = models.CharField(
         _("Source Name"),
         max_length=50,
-        help_text=_(
-            "A source for individuals making the quotes. Use as an abstract grouping."
-        ),
+        help_text=_("A source for individuals making the quotes. Use as an abstract grouping."),
         db_index=True,
     )
     description = models.TextField(
         help_text=_("Description for the source. You can style using Markdown."),
         null=True,
         blank=True,
     )
@@ -97,133 +106,146 @@
     slug = models.SlugField(
         unique=True,
         max_length=70,
         editable=False,
         blank=True,
         help_text=_("Unique slug for this group."),
     )
+    text_model = models.OneToOneField(
+        MarkovTextModel,
+        on_delete=models.CASCADE,
+        null=True,
+        blank=True,
+        help_text=_("The markov model for this group."),
+    )
+
+    class Meta:
+        rules_permissions = {
+            "add": rules.is_authenticated,
+            "read": is_owner_or_public,
+            "edit": is_owner,
+            "delete": is_owner,
+        }
+        ordering = ["name"]
+
+    def __str__(self):  # pragma: nocover
+        return self.name
+
+    def save(self, *args, **kwargs):
+        """Save and create slug if missing."""
+        if not self.slug:  # Once this slug is set, it does not change except through devil pacts
+            logger.debug("Group is being saved and a slug was provided.")
+            self.slug = generate_unique_slug_for_model(model_class=type(self), text=self.name)
+        super().save(*args, **kwargs)
+
+    def refresh_from_db(self, *args, **kwargs):
+        """
+        Also reset cached properties.
+        """
+        super().refresh_from_db(*args, **kwargs)
+        cached_properties = ["total_sources", "markov_sources", "total_quotes"]
+        for prop in cached_properties:
+            try:
+                del self.__dict__[prop]
+            except KeyError:  # pragma: nocover
+                pass
 
     @cached_property
     def total_sources(self) -> int:
+        """Total number of sources for the group."""
         return Source.objects.filter(group=self).count()
 
     @cached_property
     def markov_sources(self) -> int:
+        """Total number of Markov sources for the group."""
         return Source.objects.filter(group=self, allow_markov=True).count()
 
     @cached_property
     def total_quotes(self) -> int:
-        return Quote.objects.filter(
-            source__in=Source.objects.filter(group=self)
-        ).count()
+        """Total quotes for the group."""
+        return Quote.objects.filter(source__in=Source.objects.filter(group=self)).count()
 
     @cached_property
     def markov_ready(self) -> bool:
+        """Checks to see if there are Markov enabled sources and sufficient quotes."""
         if (
             self.markov_sources > 0
-            and Quote.objects.filter(
-                source__in=self.source_set.filter(allow_markov=True)
-            ).count()
-            > 10
+            and Quote.objects.filter(source__in=self.source_set.filter(allow_markov=True)).count() > 10  # noqa:PLR2004
         ):
             return True
         return False
 
-    def generate_markov_sentence(
-        self, max_characters: Optional[int] = 280
-    ) -> str | None:
+    async def aupdate_markov_model(self) -> None:
+        """Updates the related MarkovTextModel."""
+        markov_sources = self.source_set.filter(allow_markov=True)
+        if await markov_sources.aexists():
+            quotes = Quote.objects.filter(source__in=markov_sources)
+            await self.text_model.aupdate_model_from_corpus(corpus_entries=[quote.quote async for quote in quotes])
+
+    def update_markov_model(self) -> None:
+        """Updates the related MarkovTextModel."""
+        async_to_sync(self.aupdate_markov_model)()
+
+    def generate_markov_sentence(self, max_characters: int = 280, tries: int = 20) -> str | None:
         """
         Generate a markov sentence based on quotes from markov enabled characters for the group.
 
-        :return: str or None
+        Args:
+            max_characters (int): Maximum characters allowed in the resulting sentence.
+            tries (int): Maximum number of tries django_markov should use to create the sentence.
+
+        Returns:
+            (str | None): The generated sentence or None if no sentence was possible for the number
+                of tries.
         """
         if self.markov_ready:
             logger.debug("Group is ready for markov sentences. Checking model...")
-            mmodel = GroupMarkovModel.objects.get(group=self)
-            if mmodel.data is None:
-                logger.debug(
-                    "Markov model for group is not generated yet! Generating..."
-                )
-                mmodel.generate_model_from_corpus()
-            logger.debug("Loading text model...")
-            text_model = MarkovPOSText.from_json(mmodel.data)
+            mmodel = self.text_model
+            if not mmodel.is_ready:
+                logger.debug("Markov model for group is not generated yet! Generating...")
+                self.update_markov_model()
+                mmodel.refresh_from_db()
             logger.debug("Generating sentence...")
-            sentence: str | None = text_model.make_short_sentence(
-                max_chars=max_characters
-            )
+            sentence: str | None = mmodel.generate_sentence(char_limit=max_characters, tries=tries)
             if sentence is not None:
                 logger.debug(f"Returning generated sentence: '{sentence}'")
                 return sentence
         logger.debug("Group is not ready for markov requests yet!")
         return None
 
-    def get_random_quote(
-        self, max_quotes_to_process: Optional[int] = MAX_QUOTES_FOR_RANDOM_GROUP_SET
-    ) -> Any:
+    def get_random_quote(self, max_quotes_to_process: int | None = MAX_QUOTES_FOR_RANDOM_GROUP_SET) -> Any:
         """
         Get a random quote object from any of the characters defined within the group.
         Prioritizes quotes that have been returned less often.
 
-        :return: ``Quote`` object or None if no quotes are defined.
+        Args:
+            max_quotes_to_process (int | None): Maximum number of quotes to retrieve before
+                selecting a random one.
+
+        Returns:
+             (Quote | None) Quote object or None if no quotes are found.
         """
         # TODO: Create Q object to filter for null datetimes or less than now.
         quotes = (
             Quote.objects.filter(source__in=self.source_set.all())
-            .filter(
-                models.Q(pub_date__isnull=True) | models.Q(pub_date__lte=timezone.now())
-            )
+            .filter(models.Q(pub_date__isnull=True) | models.Q(pub_date__lte=timezone.now()))
             .select_related("stats")
             .order_by("stats__times_used")[:max_quotes_to_process]
         )
         if quotes.exists():
-            quote = random.choice(list(quotes))
-            quote_random_retrieved.send(
-                type(quote.source), instance=quote.source, quote_retrieved=quote
-            )
+            quote = random.choice(list(quotes))  # noqa: S311
+            quote_random_retrieved.send(type(quote.source), instance=quote.source, quote_retrieved=quote)
             return quote
         return None
 
-    def refresh_from_db(self, *args, **kwargs):
-        super().refresh_from_db(*args, **kwargs)
-        cached_properties = ["total_sources", "markov_sources", "total_quotes"]
-        for prop in cached_properties:
-            try:
-                del self.__dict__[prop]
-            except KeyError:  # pragma: nocover
-                pass
-
-    def save(self, *args, **kwargs):
-        if (
-            not self.slug
-        ):  # Once this slug is set, it does not change except through devil pacts
-            logger.debug("Group is being saved and a slug was provided.")
-            self.slug = generate_unique_slug_for_model(
-                model_class=type(self), text=self.name
-            )
-        super().save(*args, **kwargs)
-
-    def __str__(self):  # pragma: nocover
-        return self.name
-
-    class Meta:
-        rules_permissions = {
-            "add": rules.is_authenticated,
-            "read": is_owner_or_public,
-            "edit": is_owner,
-            "delete": is_owner,
-        }
-        ordering = ["name"]
-
 
-class Source(
-    AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase
-):
+class Source(AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase):
     """
     An individual source to attribute the quote to in the system, such as a character from a podcast/book, or a specific
-    author.
+    author. A user must be the owner of the related SourceGroup to add or delete a source.
 
     Attributes:
         id (int): Database primary key for the object.
         name (str): Unique name of a character within a ``CharacterGroup`` for this entity.
         group (SourceGroup): The parent ``SourceGroup``.
         slug (str): Slug made up of a generated version of the character name and the group slug prefix.
         description (str): Description for the character. Markdown can be used for styling.
@@ -233,143 +255,175 @@
         public (bool): Is the character public to other users? Defaults to False.
         allow_submissions (bool): Allow other users to submit quotes for this character? Defaults to False.
         created (datetime): When this object was first created. Auto-generated.
         modified (datetime): Last time this object was modified. Auto-generated.
 
     """
 
+    if TYPE_CHECKING:
+        quote_set: RelatedManager[Quote]
+
     name = models.CharField(max_length=100, help_text=_("Name of the character"))
     slug = models.SlugField(
         max_length=250,
-        help_text=_(
-            "Global slug of the character, will be auto generated from name and group if not overridden."
-        ),
+        help_text=_("Global slug of the character, will be auto generated from name and group if not overridden."),
         blank=True,
         editable=False,
         unique=True,
         db_index=True,
     )
     description = models.TextField(
         null=True,
         blank=True,
         help_text=_("Description of this character. You can style this with Markdown."),
     )
     description_rendered = models.TextField(
-        null=True, blank=True, help_text=_("Automatically generated from description.")
-    )
-    allow_markov = models.BooleanField(
-        default=False, help_text=_("Allow to be used in markov chains?")
+        null=True, blank=True, help_text=_("Automatically generated from description on save.")
     )
+    allow_markov = models.BooleanField(default=False, help_text=_("Allow to be used in markov chains?"))
     group = models.ForeignKey(
         SourceGroup,
         on_delete=models.CASCADE,
         help_text=_("The group this character belongs to."),
     )
+    text_model = models.OneToOneField(
+        MarkovTextModel,
+        on_delete=models.CASCADE,
+        null=True,
+        blank=True,
+        help_text=_("The text model for this character."),
+    )
+
+    class Meta:
+        rules_permissions = {
+            "add": rules.is_authenticated,
+            "read": is_owner_or_public,
+            "edit": is_owner,
+            "delete": is_owner,
+        }
+
+    def __str__(self):  # pragma: nocover
+        return self.name
+
+    def save(self, *args, **kwargs):
+        """Save and create slug, if missing."""
+        if not self.slug:
+            self.slug = generate_unique_slug_for_model(type(self), text=f"{self.group.slug} {self.name}")
+        super().save(*args, **kwargs)
 
     @property
     def markov_ready(self) -> bool:
         """
         Conducts sanity checks to see if requesting a markov chain is feasible. Markov must be enabled for a character
         and there must be a sufficient corpus to generate a sentence from. Currently set at a minimum of 10 quotes.
 
-        :return: bool
+        Returns:
+            (bool): If ready for markov requests.
+        """
+        if self.allow_markov and Quote.objects.filter(source=self).count() > 10:  # noqa:PLR2004
+            return True
+        return False
+
+    async def _amarkov_ready(self) -> bool:
+        """Async version of markov ready.
+
+        Returns:
+            (bool): If ready for markov
         """
-        if self.allow_markov and Quote.objects.filter(source=self).count() > 10:
+        if self.allow_markov and await Quote.objects.filter(source=self).acount() > 10:  # noqa: PLR2004
             return True
         return False
 
-    def get_markov_sentence(self, max_characters: Optional[int] = 280) -> Optional[str]:
+    async def aupdate_markov_model(self) -> None:
+        """
+        Process all quotes into the associated model.
+        """
+        if self.allow_markov:
+            await self.text_model.aupdate_model_from_corpus(
+                corpus_entries=[quote.quote async for quote in self.quote_set.all()], char_limit=0, store_compiled=False
+            )
+
+    def update_markov_model(self) -> None:
+        """
+        Sync wrapper around `aupdate_markov_model`.
+        """
+        async_to_sync(self.aupdate_markov_model)()
+
+    def get_markov_sentence(self, max_characters: int | None = 280, tries: int = 20) -> str | None:
         """
         If valid, generate a markov sentence. If not, return None.
 
-        :param max_characters: Optional maximum limit of characters in the return set. Default: 280
-        :return: str or None
+        Args:
+            max_characters (int | None): Maximum number of characters allowed in
+                resulting sentence.
+            tries (int): Number of times django_markov may try to generate sentence.
+
+        Returns:
+            (str | None): The resulting sentence or None if a sentence could not be formed.
         """
         logger.debug("Checking to see if character is markov ready...")
         if self.markov_ready:
             logger.debug("It IS ready. Fetching markov model.")
-            markov_model = SourceMarkovModel.objects.get(source=self)
-            if not markov_model.data:
+            markov_model = self.text_model
+            if not markov_model.is_ready:
                 logger.debug("No model defined yet, generating...")
-                markov_model.generate_model_from_corpus()
-            text_model = MarkovPOSText.from_json(markov_model.data)
+                self.update_markov_model()
             logger.debug("Markov text model loaded. Generating sentence.")
-            sentence: str | None = text_model.make_short_sentence(
-                max_chars=max_characters
-            )
+            sentence: str | None = markov_model.generate_sentence(char_limit=max_characters, tries=tries)
             if sentence is not None:
-                markov_sentence_generated.send(type(self), instance=self)
                 return sentence
         return None
 
-    def get_random_quote(
-        self, max_quotes_to_process: Optional[int] = MAX_QUOTES_FOR_RANDOM_SET
-    ) -> Optional[Any]:
+    def get_random_quote(self, max_quotes_to_process: int | None = MAX_QUOTES_FOR_RANDOM_SET) -> Any | None:
         """
         This actually not all that random. It's going to grab the quotes
         ordered ordered by how infrequently they've been returned, and then grab a random one
         in the set. But for our purposes, it's fine. If there aren't any quotes, it will return None.
 
-        :return: ``Quote`` object or None
+        Args:
+            max_quotes_to_process (int | None): Maximum number of quotes to retrive before
+                selecting at random.
+
+        Returns:
+            (Quote | None): The quote object or None if no quotes found.
         """
         quotes_to_pick = (
             Quote.objects.filter(source=self)
-            .filter(
-                models.Q(pub_date__isnull=True) | models.Q(pub_date__lte=timezone.now())
-            )
+            .filter(models.Q(pub_date__isnull=True) | models.Q(pub_date__lte=timezone.now()))
             .select_related("stats")
             .order_by("stats__times_used")[:max_quotes_to_process]
         )
         if quotes_to_pick.exists():
             # Select a random index in the result set.
-            quote_to_return = random.choice(list(quotes_to_pick))
-            quote_random_retrieved.send(
-                type(self), instance=self, quote_retrieved=quote_to_return
-            )
+            quote_to_return = random.choice(list(quotes_to_pick))  # noqa: S311
+            quote_random_retrieved.send(type(self), instance=self, quote_retrieved=quote_to_return)
             return quote_to_return
         return None
 
-    def __str__(self):  # pragma: nocover
-        return self.name
-
-    def save(self, *args, **kwargs):
-        if not self.slug:
-            self.slug = generate_unique_slug_for_model(
-                type(self), text=f"{self.group.slug} {self.name}"
-            )
-        super().save(*args, **kwargs)
 
-    class Meta:
-        rules_permissions = {
-            "add": rules.is_authenticated,
-            "read": is_owner_or_public,
-            "edit": is_owner,
-            "delete": is_owner,
-        }
-
-
-class Quote(
-    AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase
-):
+class Quote(AbstractOwnerModel, RulesModelMixin, TimeStampedModel, metaclass=RulesModelBase):
     """
-    A quote from a given source.
+    A quote from a given source. A user must own the related source to add or delete a quote.
 
     Attributes:
         id (int): Database primary key for the object.
         quote (str): The quote text to use. You can use Markdown for styling. Must be <= 280 characters for tweets
         quote_rendered (str): HTML rendered version of the quote field. Automatically generated.
         citation (str): Optional description of quote source, e.g. episode number or book title.
         citation_url (str): Optional accompanying URL for the citation.
         character (Source): The source of this quote.
         owner (User): The user that created and owns this quote.
         created (datetime): When this object was first created. Auto-generated.
         modified (datetime): Last time this object was modified. Auto-generated.
 
     """
 
+    if TYPE_CHECKING:
+        id: int
+
     quote = models.CharField(
         max_length=280,  # Keep the base limit to 280 so that quotes are 'tweetable'
         help_text="Plain text representation of quote. You can use Markdown here.",
     )
     quote_rendered = models.TextField(
         null=True,
         blank=True,
@@ -382,122 +436,31 @@
     )
     citation = models.CharField(
         max_length=250,
         blank=True,
         null=True,
         help_text=_("Where is this quote from? Episode #, book?"),
     )
-    citation_url = models.URLField(
-        null=True, blank=True, help_text=_("URL for citation, if applicable.")
-    )
+    citation_url = models.URLField(null=True, blank=True, help_text=_("URL for citation, if applicable."))
     pub_date = models.DateTimeField(
         null=True,
         blank=True,
         help_text=_("When is the earliest time this should appear in random results?"),
     )
 
-    def __str__(self):  # pragma: nocover
-        return f"{self.source.name}: {self.quote}"
-
     class Meta:
         rules_permissions = {
             # "add": is_character_owner,
             "read": is_owner_or_public,
             "edit": is_owner,
             "delete": is_owner,
         }
 
-
-class SourceMarkovModel(TimeStampedModel):
-    """
-    The cached markov model for a given source. The database object for this is automatically created
-    whenever a new character object is saved.
-
-    Attributes:
-        id (int): Database primary key for the object.
-        source (Source): The character who the model is sourced from.
-        data (json): The JSON representation of the Markov model created by ``markovify``.
-        created (datetime): When this object was first created. Auto-generated.
-        modified (datetime): Last time this object was modified. Auto-generated.
-
-    """
-
-    source = models.OneToOneField(Source, on_delete=models.CASCADE)
-    data = models.JSONField(null=True, blank=True)
-
-    def generate_model_from_corpus(self):
-        """
-        Collect all quotes attributed to the related character. Then
-        create, compile, and save the model.
-        """
-        logger.debug("Generating text model. Fetching quotes.")
-        quotes = Quote.objects.filter(source=self.source)
-        # Don't bother generating model if there isn't data.
-        if not quotes.exists():  # pragma: nocover
-            logger.debug("There are no quotes. Returning None.")
-            return
-        logger.debug("Quotes retrieved! Forming into corpus.")
-        corpus = " ".join(quote.quote for quote in quotes)
-        logger.debug("Building text model.")
-        text_model = MarkovPOSText(corpus)
-        logger.debug("Compiling text model.")
-        text_model.compile(inplace=True)
-        logger.debug("Saving model as JSON.")
-        self.data = text_model.to_json()
-        self.save()
-        logger.debug("Markov model populated to database.")
-
     def __str__(self):  # pragma: nocover
-        return self.source.name
-
-
-class GroupMarkovModel(TimeStampedModel):
-    """
-    The cached markov model for the entire group. It is made up of every quote from every markov enabled
-    character within the group.
-
-    Attributes:
-        id (int): The database id of this object.
-        group (SourceGroup): The OneToOne relationship to ``SourceGroup``
-        data (json): The cached markov model.
-        created (datetime): When the object was created.
-        modified (datetime): When the object was last modified.
-    """
-
-    group = models.OneToOneField(
-        SourceGroup,
-        on_delete=models.CASCADE,
-        help_text=_("The character group this model belongs to."),
-    )
-    data = models.JSONField(
-        null=True, blank=True, help_text=_("The cached markov model as JSON.")
-    )
-
-    def generate_model_from_corpus(self):
-        """
-        Collect all quotes from markov enabled characters in this group and then compile the model and save it.
-        """
-        logger.debug(f"Gathering corpus for character group: {self.group.name}")
-        quotes = Quote.objects.filter(
-            source__in=Source.objects.filter(group=self.group, allow_markov=True)
-        )
-        if quotes.exists():
-            if quotes.count() >= 10:
-                logger.debug("Found sufficient quotes for a model!")
-                corpus = " ".join(quote.quote for quote in quotes)
-                logger.debug("Forming text model...")
-                text_model = MarkovPOSText(corpus)
-                logger.debug("Compiling text model...")
-                text_model.compile(inplace=True)
-                logger.debug("Saving compiled model to JSON...")
-                self.data = text_model.to_json()
-                self.save()
-                logger.debug(
-                    f"Finished building and saving group markov model for {self.group.name}!"
-                )
+        return f"{self.source.name}: {self.quote}"
 
 
 class QuoteStats(TimeStampedModel):
     """
     A simple object used to track how often an individual quote is used.
 
     Attributes:
@@ -510,17 +473,15 @@
 
     quote = models.OneToOneField(
         Quote,
         on_delete=models.CASCADE,
         related_name="stats",
         help_text=_("The Quote the stats related to."),
     )
-    times_used = models.PositiveIntegerField(
-        default=0, help_text=_("Times used for random quotes, etc.")
-    )
+    times_used = models.PositiveIntegerField(default=0, help_text=_("Times used for random quotes, etc."))
 
     def __str__(self):  # pragma: nocover
         return f"Stats for Quote {self.quote.id}"
 
 
 class GroupStats(TimeStampedModel):
     """
@@ -528,39 +489,41 @@
 
     Attributes:
         group (SourceGroup): The group this is collecting stats for.
         quotes_requested (int): The number of times a quote from this object or its children has been requested.
         quotes_generated (int): The number of times a markov quote has been generated for this or it's children.
     """
 
-    group = models.OneToOneField(
-        SourceGroup, related_name="stats", on_delete=models.CASCADE
-    )
+    group = models.OneToOneField(SourceGroup, related_name="stats", on_delete=models.CASCADE)
     quotes_requested = models.PositiveIntegerField(
         default=0, help_text=_("Number of time child quotes have been requested.")
     )
     quotes_generated = models.PositiveIntegerField(
         default=0,
         help_text=_("Number of times markov generated quotes have been requested."),
     )
 
+    def __str__(self):  # pragma: nocover
+        return f"Stats for Group {self.group.name}"
+
 
 class SourceStats(TimeStampedModel):
     """
     An object for using to track usage stats for ``Character``.
 
     Attributes:
         source (Source): The source this is collecting stats for.
         quotes_requested (int): The number of times a quote from this object or its children has been requested.
         quotes_generated (int): The number of times a markov quote has been generated for this or it's children.
     """
 
-    source = models.OneToOneField(
-        Source, related_name="stats", on_delete=models.CASCADE
-    )
+    source = models.OneToOneField(Source, related_name="stats", on_delete=models.CASCADE)
     quotes_requested = models.PositiveIntegerField(
         default=0, help_text=_("Number of time child quotes have been requested.")
     )
     quotes_generated = models.PositiveIntegerField(
         default=0,
         help_text=_("Number of times markov generated quotes have been requested."),
     )
+
+    def __str__(self):  # pragma: nocover
+        return f"Stats for Source {self.source.name}"
```

### Comparing `django_quotes-0.3.2/django_quotes/receivers.py` & `django_quotes-0.4.0/src/django_quotes/receivers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+from django.core.exceptions import ObjectDoesNotExist
 from django.db import transaction
 from django.db.models import F
 from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 from markdown import markdown
 
-from .models import (
-    GroupMarkovModel,
+from django_markov.models import MarkovTextModel, sentence_generated
+from django_quotes.models import (
     GroupStats,
     Quote,
     QuoteStats,
     Source,
     SourceGroup,
-    SourceMarkovModel,
     SourceStats,
 )
-from .signals import markov_sentence_generated, quote_random_retrieved
+from django_quotes.signals import quote_random_retrieved
 
 
 @receiver(pre_save, sender=SourceGroup)
 @receiver(pre_save, sender=Source)
 def render_description(sender, instance, *args, **kwargs):
     """
     Automatically renders the description from markdown.
@@ -33,30 +33,30 @@
 def render_quote(sender, instance, *args, **kwargs):
     """
     Render the quote via markdown and save the results.
     """
     instance.quote_rendered = markdown(instance.quote)
 
 
-@receiver(post_save, sender=SourceGroup)
-def initialize_group_markov_object(sender, instance, created, *args, **kwargs):
+@receiver(pre_save, sender=SourceGroup)
+def initialize_group_markov_object(sender, instance, *args, **kwargs):
     """
     Creates the one-to-one object for the group markov model.
     """
-    if created:
-        GroupMarkovModel.objects.create(group=instance)
+    if not instance.text_model:
+        instance.text_model = MarkovTextModel.objects.create()
 
 
-@receiver(post_save, sender=Source)
-def initialize_markov_object(sender, instance, created, *args, **kwargs):
+@receiver(pre_save, sender=Source)
+def initialize_markov_object(sender, instance, *args, **kwargs):
     """
     Creates the one-to-one object to accompany the source object.
     """
-    if created:
-        SourceMarkovModel.objects.create(source=instance)
+    if not instance.text_model:
+        instance.text_model = MarkovTextModel.objects.create()
 
 
 @receiver(post_save, sender=SourceGroup)
 @receiver(post_save, sender=Source)
 @receiver(post_save, sender=Quote)
 def initialize_grouping_stat_object(sender, instance, created, *args, **kwargs):
     """
@@ -68,17 +68,15 @@
         elif sender == Source:
             SourceStats.objects.create(source=instance)
         elif sender == Quote:
             QuoteStats.objects.create(quote=instance)
 
 
 @receiver(quote_random_retrieved, sender=Source)
-def update_stats_for_quote_character(
-    sender, instance, quote_retrieved, *args, **kwargs
-):
+def update_stats_for_quote_character(sender, instance, quote_retrieved, *args, **kwargs):
     """
     Update the stats for the source, source group, and quote for a random retrieval.
     :param sender: Usually a source or sourcegroup class.
     :param instance: The source this was generated for.
     :param quote_retrieved: The quote that was returned.
     :return: None
     """
@@ -90,42 +88,48 @@
         group_stats.save()
         character_stats.quotes_requested = F("quotes_requested") + 1
         character_stats.save()
         quote_stats.times_used = F("times_used") + 1
         quote_stats.save()
 
 
-@receiver(markov_sentence_generated, sender=Source)
-def update_stats_for_markov(sender, instance, *args, **kwargs):
+@receiver(sentence_generated, sender=MarkovTextModel)
+def update_stats_for_markov(sender, instance, char_limit, sentence, *args, **kwargs):
     """
     For a given source, update the stats on the Source and SourceGroup for markov requests.
     :param sender: The requesting class, usually Source.
     :param instance: The specific source requested.
+    :param char_limit: The character limit used when generating the sentence.
+    :param sentence: The sentence that was generated.
     :return: None
     """
-    group_stats = instance.group.stats
-    source_stats = instance.stats
+    try:
+        source = Source.objects.get(text_model__pk=instance.pk)
+        group = source.group
+    except ObjectDoesNotExist:
+        # this is a group model
+        source = None
+        group = SourceGroup.objects.get(text_model__pk=instance.pk)
+    group_stats = group.stats
+    source_stats = source.stats if source else None
     with transaction.atomic():
         group_stats.quotes_generated = F("quotes_generated") + 1
         group_stats.save()
-        source_stats.quotes_generated = F("quotes_generated") + 1
-        source_stats.save()
+        if source_stats is not None:
+            source_stats.quotes_generated = F("quotes_generated") + 1
+            source_stats.save()
 
 
 # @receiver(post_save, sender=Quote)
 # def update_markov_model_on_quote_change(sender, instance, created, *args, **kwargs):
 #     if instance.character.allow_markov:
 #         cmm = CharacterMarkovModel.objects.get(character=instance.character)
 #         cmm.generate_model_from_corpus()
 
 
 @receiver(pre_save, sender=Source)
-def update_markov_model_for_character_enabling_markov(
-    sender, instance, *args, **kwargs
-):
+def update_markov_model_for_character_enabling_markov(sender, instance, *args, **kwargs):
     if instance.id and instance.allow_markov:
         old_version = Source.objects.get(id=instance.id)
         if not old_version.allow_markov:
-            cmm = SourceMarkovModel.objects.get(source=instance)
-            gmm = GroupMarkovModel.objects.get(group=instance.group)
-            cmm.generate_model_from_corpus()
-            gmm.generate_model_from_corpus()
+            instance.update_markov_model()
+            instance.group.update_markov_model()
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/group_create.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/group_create.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_filters %}
 {% block extratitle %}{% trans "Create new group" %} - {% endblock %}
 {% block content %}
    <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item active" aria-current="page">{% translate "Add Group" %}</li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n crispy_forms_filters %} {% block
+{% extends "../base.html" %} {% load i18n crispy_forms_filters %} {% block
 extratitle %}{% trans "Create new group" %} - {% endblock %} {% block content
 %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. {% translate "Add Group" %}
 ************ {{%% ttrraannss ""AAdddd nneeww ggrroouupp"" %%}} ************
 {% csrf_token %} {{ form|crispy }} {% trans "Create" %} _{_%_ _t_r_a_n_s_ _"_B_a_c_k_ _t_o_ _l_i_s_t_"
 _%_}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/group_delete.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/group_delete.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_tags %}
 {% block extratitle %}{% trans "Deleting" %} {{ group.name }} - {% endblock %}
 {% block content %}
         <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=group.slug %}">{{ group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% extends "base.html" %} {% load i18n crispy_forms_tags %} {% block extratitle
-%}{% trans "Deleting" %} {{ group.name }} - {% endblock %} {% block content %}
+{% extends "../base.html" %} {% load i18n crispy_forms_tags %} {% block
+extratitle %}{% trans "Deleting" %} {{ group.name }} - {% endblock %} {% block
+content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _g_r_o_u_p_._n_a_m_e_ _}_}
    3. {% translate "Delete" %}
 ************ {{%% ttrraannss ""DDeelleettiinngg"" %%}} {{{{ ggrroouupp..nnaammee }}}} ************
 {{%% ttrraannss ""AArree yyoouu ssuurree yyoouu wwaanntt ttoo ddeelleettee::"" %%}} {{ group.name }}?
 {% csrf_token %} {% trans "Delete" %} _{_%_ _t_r_a_n_s_ _"_G_o_ _b_a_c_k_"_ _%_}
 {% endblock %}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/group_detail.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/group_detail.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{{ group.name }} - {% endblock %}
 {% block content %}
     <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item active" aria-current="page">{{ group.name }}</li>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{{ group.name
-}} - {% endblock %} {% block content %}
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{
+{ group.name }} - {% endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. {{ group.name }}
 ************ {{%% ttrraannssllaattee ""GGrroouupp DDeettaaiill"" %%}}:: {{{{ ggrroouupp..nnaammee }}}} ************
 ********** {{{{ ggrroouupp..nnaammee }}}} **********
 {{ group.description_rendered|safe }}
 {% translate "Created at" %} {{ group.created }} {% translate "Last modified"
 %} {{ group.modified }}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/group_list.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/group_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_tags %}
 {% block extratitle %}{% trans "Source Groups" %} - {% endblock %}
 {% block content %}
   <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item active" aria-current="page">{% translate "Groups" %}</li>
   </ol>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends "base.html" %} {% load i18n crispy_forms_tags %} {% block extratitle
-%}{% trans "Source Groups" %} - {% endblock %} {% block content %}
+{% extends "../base.html" %} {% load i18n crispy_forms_tags %} {% block
+extratitle %}{% trans "Source Groups" %} - {% endblock %} {% block content %}
    1. {% translate "Groups" %}
 ************ {{%% ttrraannss ""YYoouurr SSoouurrccee GGrroouuppss"" %%}} ************
              {{%% ttrraannssllaattee ""SShhoowwiinngg"" %%}} {{{{ ppaaggee__oobbjj||lleennggtthh }}}} {{%% ttrraannssllaattee ""ooff"" %%}} {{
                            {{ ppaaggee__oobbjj..ppaaggiinnaattoorr..oobbjjeecctt__lliisstt..ccoouunntt }}}}
 {{%%                                                        {{%% ttrraannssllaattee ""##     {{%% ttrraannssllaattee ""##
 ttrraannssllaattee  {{%% ttrraannssllaattee ""SSuummmmaarryy"" %%}}                      SSoouurrcceess"" %%}}         QQuuootteess"" %%}}
 ""GGrroouupp"" %%}}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/group_update.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/group_update.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_filters %}
 {% block extratitle %}{% trans "Edit" %} {{ group.name }} - {% endblock %}
 {% block content %}
       <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=group.slug %}">{{ group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n crispy_forms_filters %} {% block
+{% extends "../base.html" %} {% load i18n crispy_forms_filters %} {% block
 extratitle %}{% trans "Edit" %} {{ group.name }} - {% endblock %} {% block
 content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _g_r_o_u_p_._n_a_m_e_ _}_}
    3. {% translate "Edit" %}
 ************ {{%% ttrraannss ""EEddiittiinngg"" %%}} {{{{ ggrroouupp..nnaammee }}}} ************
 {% csrf_token %} {{ form|crispy }} {% trans "Update" %} _{_%_ _t_r_a_n_s_ _"_C_a_n_c_e_l_ _E_d_i_t_"
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/quote_create.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_create.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_filters %}
 {% block extratitle %}{% blocktranslate %}Add quote for{% endblocktranslate %} {{ source.name }} - {% endblock %}
 {% block content %}
    <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=source.group.slug %}">{{ source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n crispy_forms_filters %} {% block
+{% extends "../base.html" %} {% load i18n crispy_forms_filters %} {% block
 extratitle %}{% blocktranslate %}Add quote for{% endblocktranslate %} {
 { source.name }} - {% endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _s_o_u_r_c_e_._n_a_m_e_ _}_}
    5. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_Q_u_o_t_e_s_"_ _%_}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/quote_delete.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_delete.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{% blocktranslate %}Delete quote{% endblocktranslate %} - {% endblock %}
 {% block content %}
           <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=object.source.group.slug %}">{{ object.source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{%
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{%
 blocktranslate %}Delete quote{% endblocktranslate %} - {% endblock %} {% block
 content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _o_b_j_e_c_t_._s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _o_b_j_e_c_t_._s_o_u_r_c_e_._n_a_m_e_ _}_}
    5. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_Q_u_o_t_e_s_"_ _%_}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/quote_detail.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{% blocktranslate %}Quote from{% endblocktranslate %} {{ quote.source.name }}- {% endblock %}
 {% block content %}
       <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=quote.source.group.slug %}">{{ quote.source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{%
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{%
 blocktranslate %}Quote from{% endblocktranslate %} {{ quote.source.name }}- {%
 endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _q_u_o_t_e_._s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _q_u_o_t_e_._s_o_u_r_c_e_._n_a_m_e_ _}_}
    5. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_Q_u_o_t_e_s_"_ _%_}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/quote_list.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{% blocktranslate %}Quotes from{% endblocktranslate %} {{ source.name }} - {% endblock %}
 {% block content %}
     <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=source.group.slug %}">{{ source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{%
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{%
 blocktranslate %}Quotes from{% endblocktranslate %} {{ source.name }} - {%
 endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _s_o_u_r_c_e_._n_a_m_e_ _}_}
    5. {% translate "Quotes" %}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/quote_update.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/quote_update.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_filters %}
 {% block extratitle %}{% blocktranslate %}Edit quote{% endblocktranslate %} - {% endblock %}
 {% block content %}
         <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=quote.source.group.slug %}">{{ quote.source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n crispy_forms_filters %} {% block
+{% extends "../base.html" %} {% load i18n crispy_forms_filters %} {% block
 extratitle %}{% blocktranslate %}Edit quote{% endblocktranslate %} - {%
 endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _q_u_o_t_e_._s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _q_u_o_t_e_._s_o_u_r_c_e_._n_a_m_e_ _}_}
    5. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_Q_u_o_t_e_s_"_ _%_}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/source_create.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/source_create.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_filters %}
 {% block extratitle %}{% trans "Add new source to" %} {{ group.name }} - {% endblock %}
 {% block content %}
    <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=group.slug %}">{{ group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n crispy_forms_filters %} {% block
+{% extends "../base.html" %} {% load i18n crispy_forms_filters %} {% block
 extratitle %}{% trans "Add new source to" %} {{ group.name }} - {% endblock %}
 {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. {% translate "Add source" %}
 ************ {{%% ttrraannssllaattee ""AAdddd ssoouurrccee ttoo"" %%}} {{{{ ggrroouupp..nnaammee }}}} ************
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/source_delete.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/source_delete.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{% trans "Deleting" %} {{ object.name }} - {% endblock %}
 {% block content %}
           <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=object.group.slug %}">{{ object.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{% trans
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{% trans
 "Deleting" %} {{ object.name }} - {% endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _o_b_j_e_c_t_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _o_b_j_e_c_t_._n_a_m_e_ _}_}
    5. {% translate "Delete" %}
 ************ {{%% ttrraannss ""DDeelleettiinngg::"" %%}} {{{{ oobbjjeecctt..nnaammee }}}} ************
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/source_detail.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/source_detail.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{{ source.name }} - {% endblock %}
 {% block content %}
       <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=source.group.slug %}">{{ source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{{ source.name
-}} - {% endblock %} {% block content %}
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{
+{ source.name }} - {% endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_o_u_r_c_e_s_"_ _%_}
    4. {{ source.name }}
 ************ {{%% ttrraannssllaattee ""SSoouurrccee DDeettaaiillss"" %%}}:: {{{{ ssoouurrccee..nnaammee }}}} ************
 ********** {{{{ ssoouurrccee..nnaammee }}}} **********
 {{ source.description_rendered|safe }}
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/source_list.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/source_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n %}
 {% block extratitle %}{% blocktranslate %}Sources in{% endblocktranslate %} {{ group.name }} - {% endblock %}
 {% block content %}
         <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=group.slug %}">{{ group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n %} {% block extratitle %}{%
+{% extends "../base.html" %} {% load i18n %} {% block extratitle %}{%
 blocktranslate %}Sources in{% endblocktranslate %} {{ group.name }} - {%
 endblock %} {% block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _g_r_o_u_p_._n_a_m_e_ _}_}
    3. {% translate "Sources" %}
 ************ {{%% bblloocckkttrraannssllaattee %%}}SSoouurrcceess iinn{{%% eennddbblloocckkttrraannssllaattee %%}} {{{{ ggrroouupp..nnaammee }}}}
 ************
```

### Comparing `django_quotes-0.3.2/django_quotes/templates/quotes/source_update.html` & `django_quotes-0.4.0/src/django_quotes/templates/quotes/source_update.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %}
+{% extends "../base.html" %}
 {% load i18n crispy_forms_filters %}
 {% block extratitle %}{% translate "Editing" %} {{ source.name }} - {% endblock %}
 {% block content %}
         <nav aria-label="breadcrumb">
   <ol class="breadcrumb">
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_list' %}">{% translate "Groups" %}</a></li>
     <li class="breadcrumb-item"><a href="{% url 'quotes:group_detail' group=source.group.slug %}">{{ source.group.name }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "base.html" %} {% load i18n crispy_forms_filters %} {% block
+{% extends "../base.html" %} {% load i18n crispy_forms_filters %} {% block
 extratitle %}{% translate "Editing" %} {{ source.name }} - {% endblock %} {%
 block content %}
    1. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_G_r_o_u_p_s_"_ _%_}
    2. _{_{_ _s_o_u_r_c_e_._g_r_o_u_p_._n_a_m_e_ _}_}
    3. _{_%_ _t_r_a_n_s_l_a_t_e_ _"_s_o_u_r_c_e_s_"_ _%_}
    4. _{_{_ _s_o_u_r_c_e_._n_a_m_e_ _}_}
    5. {% translate "Edit" %}
```

### Comparing `django_quotes-0.3.2/django_quotes/urls.py` & `django_quotes-0.4.0/src/django_quotes/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+"""Url patterns for application."""
+
 from django.urls import path
 
-from .views import (
+from django_quotes.views import (
     QuoteCreateView,
     QuoteDeleteView,
     QuoteDetailView,
     QuoteListView,
     QuoteUpdateView,
     SourceCreateView,
     SourceDeleteView,
@@ -69,16 +71,14 @@
     ),
     path(
         "sources/<slug:source>/quotes/add/",
         view=QuoteCreateView.as_view(),
         name="quote_create",
     ),
     path("quotes/<int:quote>/", view=QuoteDetailView.as_view(), name="quote_detail"),
-    path(
-        "quotes/<int:quote>/edit/", view=QuoteUpdateView.as_view(), name="quote_update"
-    ),
+    path("quotes/<int:quote>/edit/", view=QuoteUpdateView.as_view(), name="quote_update"),
     path(
         "quotes/<int:quote>/delete/",
         view=QuoteDeleteView.as_view(),
         name="quote_delete",
     ),
 ]
```

### Comparing `django_quotes-0.3.2/django_quotes/utils.py` & `django_quotes-0.4.0/src/django_quotes/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Optional, Type
-
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Model
 from loguru import logger
 from slugify import slugify
 
 
 def generate_unique_slug_for_model(
-    model_class: Type[Model],
+    model_class: type[Model],
     text: str,
-    slug_field: Optional[str] = "slug",
-    max_length_override: Optional[int] = None,
+    slug_field: str | None = "slug",
+    max_length_override: int | None = None,
 ) -> str:
     """
     Generate a unique slug for the given model.
 
-    :param model_class: A class based upon ``django.db.models.Model``
-    :param text: Text to convert to a slug.
-    :param slug_field: The name of the slug field of the model.
-    :param max_length_override: Maximum number of characters to use if not the same as what's defined in the slug field.
-    :return: The generated slug.
+    Args:
+        model_class (Model): A class based upon ``django.db.models.Model``
+        text (str): Text to convert to a slug.
+        slug_field (str | None): The name of the slug field of the model.
+        max_length_override (int | None): Maximum number of characters to use if not the same as what's defined in the slug field.
+    Returns:
+         (str): The generated slug.
     """
     unique_found: bool = False
     has_next: bool = False
     next_val: int = 0
     if not max_length_override:
         logger.debug("Setting max_length of slug from field definition.")
         max_length: int = model_class._meta.get_field(slug_field).max_length  # type: ignore
@@ -39,13 +39,13 @@
         except ObjectDoesNotExist:
             logger.debug("Slug is unique!")
             unique_found = True
         if not unique_found:
             logger.debug("Slug is not unique yet.")
             next_val += 1
             if has_next:
-                slug = slug[len(slug) - (len(str(next_val - 1)) - 1) :]  # noqa: E203
+                slug = slug[len(slug) - (len(str(next_val - 1)) - 1) :]
             if len(slug) >= max_length:
                 slug = slug[: max_length - (len(str(next_val)) + 1)]
             slug = slug + f"-{next_val}"
             has_next = True
     return slug
```

### Comparing `django_quotes-0.3.2/django_quotes/views.py` & `django_quotes-0.4.0/src/django_quotes/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+from typing import TYPE_CHECKING
+
 from django.contrib import messages
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.http import HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.urls import reverse_lazy
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import DetailView as GenericDetail
 from django.views.generic import ListView as GenericList
 from django.views.generic.edit import CreateView as GenericCreate
 from django.views.generic.edit import DeleteView as GenericDelete
 from django.views.generic.edit import UpdateView as GenericUpdate
 from rules.contrib.views import PermissionRequiredMixin
 
-from .models import Quote, Source, SourceGroup
+from django_quotes.models import Quote, Source, SourceGroup
 
 # Create your views here.
 
 
 # SOURCE GROUPS
 
 
 class SourceGroupListView(LoginRequiredMixin, GenericList):
     """
     Displays Source Groups owned by the user.
     TODO: For now, only user owned groups, we won't bother with public options.
+
+    Available at /groups/
     """
 
     model = SourceGroup
     context_object_name = "groups"
     template_name = "quotes/group_list.html"
     paginate_by = 15
     allow_empty = True
@@ -34,14 +38,16 @@
     def get_queryset(self):
         return SourceGroup.objects.filter(owner=self.request.user)  # type: ignore
 
 
 class SourceGroupDetailView(LoginRequiredMixin, PermissionRequiredMixin, GenericDetail):
     """
     Displays details for a source group.
+
+    Available at /groups/[group_slug]/
     """
 
     model = SourceGroup
     context_object_name = "group"
     template_name = "quotes/group_detail.html"
     permission_required = "django_quotes.read_sourcegroup"
     slug_url_kwarg = "group"
@@ -52,67 +58,74 @@
         context["source_sample"] = Source.objects.filter(group=context["group"])[:5]
         return context
 
 
 class SourceGroupUpdateView(LoginRequiredMixin, PermissionRequiredMixin, GenericUpdate):
     """
     Update an existing source group
+
+    Available at /groups/[group_slug]/edit/
     """
 
+    if TYPE_CHECKING:
+        object: SourceGroup
+
     model = SourceGroup
     context_object_name = "group"
     template_name = "quotes/group_update.html"
     permission_required = "django_quotes.edit_sourcegroup"
     fields = ["name", "description", "public"]
     slug_url_kwarg = "group"
 
     def get_success_url(self):
-        messages.success(
-            self.request, _(f"Successfully updated group {self.object.name}!")
-        )
+        messages.success(self.request, _(f"Successfully updated group {self.object.name}!"))
         return reverse_lazy("quotes:group_detail", kwargs={"group": self.object.slug})
 
 
 class SourceGroupDeleteView(LoginRequiredMixin, PermissionRequiredMixin, GenericDelete):  # type: ignore
     """
     Delete and existing source group.
+
+    Available at /groups/[group_slug]/delete/
     """
 
     model = SourceGroup
     context_object_name = "group"
     template_name = "quotes/group_delete.html"
     permission_required = "django_quotes.delete_sourcegroup"
     slug_url_kwarg = "group"
     success_url = reverse_lazy("quotes:group_list")
 
 
 class SourceGroupCreateView(LoginRequiredMixin, GenericCreate):
     """
     Create a new source group.
+
+    Available at /groups/create/
     """
 
     model = SourceGroup
     template_name = "quotes/group_create.html"
     fields = ["name", "description", "public"]
 
     def form_valid(self, form):
         form.instance.owner = self.request.user
         obj = form.save()
         messages.success(self.request, _(f"Successfully created group {obj.name}"))
-        return HttpResponseRedirect(
-            redirect_to=reverse_lazy("quotes:group_detail", kwargs={"group": obj.slug})
-        )
+        return HttpResponseRedirect(redirect_to=reverse_lazy("quotes:group_detail", kwargs={"group": obj.slug}))
 
 
 # SOURCES
 
 
 class SourceCreateView(LoginRequiredMixin, PermissionRequiredMixin, GenericCreate):
     """
     Create a new source and add them to a source group.
+
+    Available at /groups/[group_slug]/sources/add/
     """
 
     model = Source
     template_name = "quotes/source_create.html"
     fields = ["name", "description", "allow_markov", "public"]
     permission_required = "django_quotes.edit_sourcegroup"
     group = None
@@ -131,24 +144,22 @@
         return context
 
     def form_valid(self, form):
         form.instance.owner = self.request.user
         form.instance.group = self.group
         obj = form.save()
         messages.success(self.request, _(f"Successfully created source {obj.name}!"))
-        return HttpResponseRedirect(
-            redirect_to=reverse_lazy(
-                "quotes:source_detail", kwargs={"source": obj.slug}
-            )
-        )
+        return HttpResponseRedirect(redirect_to=reverse_lazy("quotes:source_detail", kwargs={"source": obj.slug}))
 
 
 class SourceDetailView(LoginRequiredMixin, PermissionRequiredMixin, GenericDetail):
     """
     Shows information about the specified source.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/
     """
 
     model = Source
     slug_url_kwarg = "source"
     slug_field = "slug"
     template_name = "quotes/source_detail.html"
     context_object_name = "source"
@@ -160,33 +171,35 @@
         context["samp_quotes"] = context["source"].quote_set.all()[:5]
         return context
 
 
 class SourceUpdateView(LoginRequiredMixin, PermissionRequiredMixin, GenericUpdate):
     """
     Allows editing and updating of a Source.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/edit/
     """
 
     model = Source
     slug_url_kwarg = "source"
     slug_field = "slug"
     template_name = "quotes/source_update.html"
     permission_required = "django_quotes.edit_source"
     fields = ["name", "description", "public", "allow_markov"]
 
     def get_success_url(self):
         messages.success(self.request, "Successfully updated source!")
-        return reverse_lazy(
-            "quotes:source_detail", kwargs={"source": self.kwargs["source"]}
-        )
+        return reverse_lazy("quotes:source_detail", kwargs={"source": self.kwargs["source"]})
 
 
 class SourceDeleteView(LoginRequiredMixin, PermissionRequiredMixin, GenericDelete):  # type: ignore
     """
     Used to delete a given Source
+
+    Available at /groups/[group_slug]/sources/[source_slug]/delete/
     """
 
     model = Source
     slug_field = "slug"
     slug_url_kwarg = "source"
     template_name = "quotes/source_delete.html"
     permission_required = "django_quotes.delete_source"
@@ -201,14 +214,16 @@
     def get_success_url(self):
         return reverse_lazy("quotes:source_list", kwargs={"group": self.group.slug})
 
 
 class SourceListView(LoginRequiredMixin, PermissionRequiredMixin, GenericList):
     """
     Display a list of sources for a given group.
+
+    Available at /groups/[group_slug]/sources/
     """
 
     model = Source
     template_name = "quotes/source_list.html"
     permission_required = "django_quotes.read_sourcegroup"
     context_object_name = "sources"
     paginate_by = 15
@@ -239,14 +254,16 @@
 
 # QUOTES
 
 
 class QuoteListView(LoginRequiredMixin, PermissionRequiredMixin, GenericList):
     """
     View for viewing quotes from a specific source.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/quotes/
     """
 
     model = Quote
     context_object_name = "quotes"
     template_name = "quotes/quote_list.html"
     permission_required = "django_quotes.read_source"
     paginate_by = 15
@@ -255,32 +272,30 @@
 
     def dispatch(self, request, *args, **kwargs):
         source_slug = kwargs.pop("source")
         self.source = get_object_or_404(Source, slug=source_slug)
         return super().dispatch(request, *args, **kwargs)
 
     def get_queryset(self):
-        return (
-            Quote.objects.filter(source=self.source)
-            .select_related("source", "source__group")
-            .order_by("-created")
-        )
+        return Quote.objects.filter(source=self.source).select_related("source", "source__group").order_by("-created")
 
     def get_permission_object(self):
         return self.source
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["source"] = self.source
         return context
 
 
 class QuoteCreateView(LoginRequiredMixin, PermissionRequiredMixin, GenericCreate):
     """
     View for adding a quote to a source.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/quotes/add/
     """
 
     model = Quote
     template_name = "quotes/quote_create.html"
     permission_required = "django_quotes.edit_source"
     fields = ["quote", "citation", "citation_url", "pub_date"]
 
@@ -305,64 +320,64 @@
                 _(f"This quote for source {self.source.name} already exists."),
             )
             return self.form_invalid(form)
         form.instance.source = self.source
         form.instance.owner = self.request.user
         form.save()
         messages.success(self.request, _("Successfully added quote!"))
-        return HttpResponseRedirect(
-            redirect_to=reverse_lazy(
-                "quotes:quote_list", kwargs={"source": self.source.slug}
-            )
-        )
+        return HttpResponseRedirect(redirect_to=reverse_lazy("quotes:quote_list", kwargs={"source": self.source.slug}))
 
 
 class QuoteUpdateView(LoginRequiredMixin, PermissionRequiredMixin, GenericUpdate):
     """
     View for updating a quote.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/quotes/[quote_id]/edit/
     """
 
     model = Quote
     permission_required = "django_quotes.edit_quote"
     template_name = "quotes/quote_update.html"
     fields = ["quote", "citation", "citation_url", "pub_date"]
     pk_url_kwarg = "quote"
 
     def form_valid(self, form):
         obj = form.save()
         messages.success(self.request, _("Successfully updated quote!"))
-        return HttpResponseRedirect(
-            redirect_to=reverse_lazy("quotes:quote_detail", kwargs={"quote": obj.id})
-        )
+        return HttpResponseRedirect(redirect_to=reverse_lazy("quotes:quote_detail", kwargs={"quote": obj.id}))
 
 
 class QuoteDetailView(LoginRequiredMixin, PermissionRequiredMixin, GenericDetail):
     """
     A quote detail view for use in things like previewing render or viewing statistics.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/quotes/[quote_id]/
     """
 
     model = Quote
     pk_url_kwarg = "quote"
     context_object_name = "quote"
     permission_required = "django_quotes.read_quote"
     template_name = "quotes/quote_detail.html"
     select_related = ["source", "source__group", "owner"]
 
 
 class QuoteDeleteView(LoginRequiredMixin, PermissionRequiredMixin, GenericDelete):  # type: ignore
     """
     View to delete a quote.
+
+    Available at /groups/[group_slug]/sources/[source_slug]/quotes/[quote_id]/delete/
     """
 
     model = Quote
     pk_url_kwarg = "quote"
     context_object_name = "quote"
     permission_required = "django_quotes.delete_quote"
     template_name = "quotes/quote_delete.html"
 
     def get_object(self, *args, **kwargs):
         object = super().get_object(*args, **kwargs)
-        self.source = object.source
+        self.source = object.source  # type: ignore
         return object
 
     def get_success_url(self):
         return reverse_lazy("quotes:quote_list", kwargs={"source": self.source.slug})
```

