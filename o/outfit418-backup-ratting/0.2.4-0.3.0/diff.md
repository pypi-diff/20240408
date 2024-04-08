# Comparing `tmp/outfit418_backup_ratting-0.2.4.tar.gz` & `tmp/outfit418_backup_ratting-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outfit418_backup_ratting-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "outfit418_backup_ratting-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `outfit418_backup_ratting-0.2.4.tar` & `outfit418_backup_ratting-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rwxr-xr-x   0        0        0     1539 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/LICENSE
--rwxr-xr-x   0        0        0      536 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/README.md
--rwxr-xr-x   0        0        0      143 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/__init__.py
--rwxr-xr-x   0        0        0      178 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/apps.py
--rwxr-xr-x   0        0        0     1206 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/auth_hooks.py
--rwxr-xr-x   0        0        0      108 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/forms.py
--rwxr-xr-x   0        0        0     1409 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/migrations/0001_initial.py
--rw-r--r--   0        0        0      660 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/migrations/0002_general.py
--rwxr-xr-x   0        0        0        0 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/migrations/__init__.py
--rwxr-xr-x   0        0        0      782 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/models.py
--rwxr-xr-x   0        0        0     3877 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/tasks.py
--rw-r--r--   0        0        0     1326 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html
--rwxr-xr-x   0        0        0      438 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/templates/outfit418_backup_ratting/index.html
--rwxr-xr-x   0        0        0      247 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/urls.py
--rwxr-xr-x   0        0        0      851 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/utils.py
--rwxr-xr-x   0        0        0     2459 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/views.py
--rwxr-xr-x   0        0        0      877 2024-03-17 11:47:02.391647 outfit418_backup_ratting-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 outfit418_backup_ratting-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1539 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0      536 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/README.md
+-rwxr-xr-x   0        0        0      143 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/__init__.py
+-rwxr-xr-x   0        0        0      178 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/apps.py
+-rwxr-xr-x   0        0        0     1206 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/auth_hooks.py
+-rwxr-xr-x   0        0        0      108 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/forms.py
+-rwxr-xr-x   0        0        0     1409 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0001_initial.py
+-rw-r--r--   0        0        0      660 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0002_general.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/__init__.py
+-rwxr-xr-x   0        0        0      782 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/models.py
+-rwxr-xr-x   0        0        0     3877 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/tasks.py
+-rw-r--r--   0        0        0     1434 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html
+-rwxr-xr-x   0        0        0      486 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/index.html
+-rw-r--r--   0        0        0        0 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templatetags/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templatetags/outfit_tags.py
+-rwxr-xr-x   0        0        0      247 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/urls.py
+-rwxr-xr-x   0        0        0      851 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/utils.py
+-rwxr-xr-x   0        0        0     2363 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/views.py
+-rwxr-xr-x   0        0        0      868 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 outfit418_backup_ratting-0.3.0/PKG-INFO
```

### Comparing `outfit418_backup_ratting-0.2.4/LICENSE` & `outfit418_backup_ratting-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/README.md` & `outfit418_backup_ratting-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/auth_hooks.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/migrations/0001_initial.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/migrations/0002_general.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0002_general.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/models.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/models.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/tasks.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/tasks.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-{% extends 'allianceauth/base.html' %}
+{% extends 'allianceauth/base-bs5.html' %}
+{% load outfit_tags %}
 
 {% block page_title %}418 Audit{% endblock page_title %}
 
 {% block extra_css %}
-    {% include "bundles/datatables-css.html" %}
+    {% include "bundles/datatables-css-bs5.html" %}
 {% endblock %}
 
 {% block content %}
     <div class="col-lg-12" style="padding: 10px 10px 10px 10px">
         <table class="table table-aa">
             <thead>
                 <tr>
@@ -17,26 +18,26 @@
             </thead>
             <tbody>
                 {% for main in mains %}
                     <tr>
                         <td>{{ main.character.character_name }}</td>
                         <td>
                             {% for char in main.character.character_ownership.user.chars %}
-                                <span class="label label-primary">{{ char.character.character_name }}</span>
+                                <span class="badge {% if char.character|ct_is_active %}text-bg-primary{% else %}text-bg-danger{% endif %}">{{ char.character.character_name }}</span>
                             {% endfor %}
                         </td>
                     </tr>
                 {% endfor %}
             </tbody>
         </table>
     </div>
 {% endblock content %}
 
 {% block extra_javascript %}
-    {% include "bundles/datatables-js.html" %}
+    {% include "bundles/datatables-js-bs5.html" %}
 {% endblock extra_javascript %}
 
 {% block extra_script %}
     $(document).ready(function() {
         $('.table').DataTable({
             "pageLength": 50
         });
```

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/utils.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/utils.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.2.4/outfit418_backup_ratting/views.py` & `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,16 @@
     return render(request, 'outfit418_backup_ratting/index.html', context=context)
 
 
 @login_required
 @permission_required('outfit418_backup_ratting.audit_corp')
 def audit(request):
     corp_id = request.user.profile.main_character.corporation_id
-    ownership_qs = (
-        CharacterOwnership.objects
-        .filter(Exists(CharacterAudit.objects.filter(character=OuterRef('character'))))
-        .select_related('character')
-    )
+    ownership_qs = CharacterOwnership.objects.select_related('character__characteraudit')
+
     mains = (
         CharacterAudit.objects
         .filter(
             character__character_ownership__user__profile__main_character=F('character'),
             character__corporation_id=corp_id,
         )
         .select_related('character__character_ownership__user')
```

### Comparing `outfit418_backup_ratting-0.2.4/pyproject.toml` & `outfit418_backup_ratting-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "allianceauth",
 	"allianceauth_pve",
 	"outfit418",
 	"eveonline",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "allianceauth>=3.0.0,<5.0.0",
+    "allianceauth~=4.0",
 	"allianceauth_pve~=1.10",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Maestro-Zacht/outfit418-backup-ratting"
 Source = "https://github.com/Maestro-Zacht/outfit418-backup-ratting"
 Tracker = "https://github.com/Maestro-Zacht/outfit418-backup-ratting/issues"
```

### Comparing `outfit418_backup_ratting-0.2.4/PKG-INFO` & `outfit418_backup_ratting-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: outfit418_backup_ratting
-Version: 0.2.4
+Version: 0.3.0
 Summary: Backup for Outfit418 data
 Keywords: allianceauth,allianceauth_pve,outfit418,eveonline
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: allianceauth>=3.0.0,<5.0.0
+Requires-Dist: allianceauth~=4.0
 Requires-Dist: allianceauth_pve~=1.10
 Project-URL: Changelog, https://github.com/Maestro-Zacht/outfit418-backup-ratting/releases
 Project-URL: Homepage, https://github.com/Maestro-Zacht/outfit418-backup-ratting
 Project-URL: Source, https://github.com/Maestro-Zacht/outfit418-backup-ratting
 Project-URL: Tracker, https://github.com/Maestro-Zacht/outfit418-backup-ratting/issues
 
 # Outfit418 Backup Ratting
```

