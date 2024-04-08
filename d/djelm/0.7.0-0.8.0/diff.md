# Comparing `tmp/djelm-0.7.0.tar.gz` & `tmp/djelm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djelm-0.7.0.tar", max compression
+gzip compressed data, was "djelm-0.8.0.tar", max compression
```

## Comparing `djelm-0.7.0.tar` & `djelm-0.8.0.tar`

### file list

```diff
@@ -1,56 +1,67 @@
--rw-r--r--   0        0        0     1082 2024-04-03 07:20:59.898015 djelm-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0    23669 2024-04-03 07:20:59.898015 djelm-0.7.0/README_pypi.md
--rw-r--r--   0        0        0     1360 2024-04-03 07:20:59.898015 djelm-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      254 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/__init__.py
--rw-r--r--   0        0        0       83 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/apps.py
--rw-r--r--   0        0        0     1291 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/cookiecutter.py
--rw-r--r--   0        0        0      345 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/effect.py
--rw-r--r--   0        0        0     1659 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/elm.py
--rw-r--r--   0        0        0      179 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/__init__.py
--rw-r--r--   0        0        0      514 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/adapters.py
--rw-r--r--   0        0        0       65 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/__init__.py
--rw-r--r--   0        0        0      813 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/adapters.py
--rw-r--r--   0        0        0     2045 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/helpers.py
--rw-r--r--   0        0        0      444 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/primitives.py
--rw-r--r--   0        0        0      592 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/flags/form/serializer.py
--rw-r--r--   0        0        0    21933 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/flags/main.py
--rw-r--r--   0        0        0     1211 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/flags/primitives.py
--rw-r--r--   0        0        0       36 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/forms/widgets/main.py
--rw-r--r--   0        0        0    13914 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/generators.py
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/management/commands/__init__.py
--rw-r--r--   0        0        0     3376 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/management/commands/djelm.py
--rw-r--r--   0        0        0      105 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/model_template/cookiecutter.json
--rw-r--r--   0        0        0      432 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/model_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elmf
--rw-r--r--   0        0        0     1384 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/npm.py
--rw-r--r--   0        0        0      112 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/cookiecutter.json
--rw-r--r--   0        0        0     1464 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm
--rw-r--r--   0        0        0      791 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts
--rw-r--r--   0        0        0       99 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
--rw-r--r--   0        0        0      375 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.pyf
--rw-r--r--   0        0        0      603 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py
--rw-r--r--   0        0        0       75 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/cookiecutter.json
--rw-r--r--   0        0        0      430 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/hooks/post_gen_project.py
--rw-r--r--   0        0        0      167 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/apps.py
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/flags/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static/dist/.gitkeep
--rw-r--r--   0        0        0      446 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/.gitignore
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/djelm_src/.gitkeep
--rw-r--r--   0        0        0      475 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/elm.json
--rw-r--r--   0        0        0      384 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/package.json
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/src/Models/.gitkeep
--rw-r--r--   0        0        0       92 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/include.html
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/{{cookiecutter.app_name}}/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/templatetags/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}.djelm
--rw-r--r--   0        0        0    21257 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/strategy.py
--rw-r--r--   0        0        0     1010 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/subprocess.py
--rw-r--r--   0        0        0     3348 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/utils.py
--rw-r--r--   0        0        0    20835 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/validate.py
--rw-r--r--   0        0        0      112 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/cookiecutter.json
--rw-r--r--   0        0        0     3912 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw
--rw-r--r--   0        0        0      813 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts
--rw-r--r--   0        0        0      429 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField.pyf
--rw-r--r--   0        0        0      753 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py
--rw-r--r--   0        0        0      105 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
--rw-r--r--   0        0        0    24512 1970-01-01 00:00:00.000000 djelm-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-08 08:39:45.980995 djelm-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0    23839 2024-04-08 08:39:45.980995 djelm-0.8.0/README_pypi.md
+-rw-r--r--   0        0        0     1360 2024-04-08 08:39:45.984995 djelm-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      254 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/apps.py
+-rw-r--r--   0        0        0     2234 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/annotation.py
+-rw-r--r--   0        0        0     2332 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/compiler.py
+-rw-r--r--   0        0        0     2128 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/elm.py
+-rw-r--r--   0        0        0     5288 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/expression.py
+-rw-r--r--   0        0        0      202 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/format.py
+-rw-r--r--   0        0        0       98 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/module_name.py
+-rw-r--r--   0        0        0     1325 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/op.py
+-rw-r--r--   0        0        0      101 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/range.py
+-rw-r--r--   0        0        0       88 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/utils.py
+-rw-r--r--   0        0        0    11043 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/writer.py
+-rw-r--r--   0        0        0     1291 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/cookiecutter.py
+-rw-r--r--   0        0        0      345 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/effect.py
+-rw-r--r--   0        0        0     1659 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/elm.py
+-rw-r--r--   0        0        0     1739 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/README.md
+-rw-r--r--   0        0        0      199 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/adapters.py
+-rw-r--r--   0        0        0       65 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/__init__.py
+-rw-r--r--   0        0        0      813 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/adapters.py
+-rw-r--r--   0        0        0     2045 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/helpers.py
+-rw-r--r--   0        0        0      444 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/primitives.py
+-rw-r--r--   0        0        0      592 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/serializer.py
+-rw-r--r--   0        0        0    38411 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/main.py
+-rw-r--r--   0        0        0     1828 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/primitives.py
+-rw-r--r--   0        0        0       36 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/forms/widgets/main.py
+-rw-r--r--   0        0        0    13914 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/generators.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/management/commands/__init__.py
+-rw-r--r--   0        0        0     3376 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/management/commands/djelm.py
+-rw-r--r--   0        0        0      105 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/model_template/cookiecutter.json
+-rw-r--r--   0        0        0      385 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/model_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elmf
+-rw-r--r--   0        0        0     1384 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/npm.py
+-rw-r--r--   0        0        0      112 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/cookiecutter.json
+-rw-r--r--   0        0        0     1464 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm
+-rw-r--r--   0        0        0      791 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts
+-rw-r--r--   0        0        0       99 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
+-rw-r--r--   0        0        0      375 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.pyf
+-rw-r--r--   0        0        0      603 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py
+-rw-r--r--   0        0        0       75 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/cookiecutter.json
+-rw-r--r--   0        0        0      430 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      167 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/apps.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/flags/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static/dist/.gitkeep
+-rw-r--r--   0        0        0      446 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/djelm_src/.gitkeep
+-rw-r--r--   0        0        0      475 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/elm.json
+-rw-r--r--   0        0        0      384 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/package.json
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/src/Models/.gitkeep
+-rw-r--r--   0        0        0       92 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/include.html
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/{{cookiecutter.app_name}}/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/templatetags/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}.djelm
+-rw-r--r--   0        0        0    21257 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/strategy.py
+-rw-r--r--   0        0        0     1010 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/subprocess.py
+-rw-r--r--   0        0        0     3348 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/utils.py
+-rw-r--r--   0        0        0    20835 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/validate.py
+-rw-r--r--   0        0        0      112 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/cookiecutter.json
+-rw-r--r--   0        0        0     3912 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw
+-rw-r--r--   0        0        0      813 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts
+-rw-r--r--   0        0        0      429 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField.pyf
+-rw-r--r--   0        0        0      753 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py
+-rw-r--r--   0        0        0      105 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
+-rw-r--r--   0        0        0    24682 1970-01-01 00:00:00.000000 djelm-0.8.0/PKG-INFO
```

### Comparing `djelm-0.7.0/LICENSE.txt` & `djelm-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/README_pypi.md` & `djelm-0.8.0/README_pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -569,14 +569,16 @@
         Err _ -> -- Flag failed to decode to an Int, Error!
             ( Error, Cmd.none )
 ```
 
 To summarize, we get compile and runtime guarantees that our program will behave as we expect. This is what makes Elm programs
 incredibly robust and nearly impossible to produce a runtime exception with.
 
+You can check out all the python flags you can use to express your data shape [here](https://github.com/Confidenceman02/django-elm/blob/main/src/djelm/flags/README.md).
+
 ## `generatemodel` Command
 
 Our python flag classes have a little trick up their sleeve that makes keeping both our python and Elm flag contracts in
 sync for us.
 
 We can see that in the `elm_programs/static_src/src/Models/Main.elm` module we have the following comment:
```

### Comparing `djelm-0.7.0/pyproject.toml` & `djelm-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.mypy]
 plugins = [ "mypy_django_plugin.main" ]
 
 [tool.poetry]
 name = "djelm"
-version = "0.7.0"
+version = "0.8.0"
 description = "A framework for using Elm programs in a Django project"
 authors = ["Confidenceman02"]
 readme = "README_pypi.md"
 keywords = ["django", "elm"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `djelm-0.7.0/src/djelm/cookiecutter.py` & `djelm-0.8.0/src/djelm/cookiecutter.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/elm.py` & `djelm-0.8.0/src/djelm/elm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/flags/adapters.py` & `djelm-0.8.0/src/djelm/flags/adapters.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/flags/form/adapters.py` & `djelm-0.8.0/src/djelm/flags/form/adapters.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/flags/form/helpers.py` & `djelm-0.8.0/src/djelm/flags/form/helpers.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/flags/form/serializer.py` & `djelm-0.8.0/src/djelm/flags/form/serializer.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/flags/primitives.py` & `djelm-0.8.0/src/djelm/flags/primitives.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,40 @@
 @dataclass(slots=True)
 class ObjectFlag(Flag):
     """Flag for the Elm {} primitive"""
 
     obj: typing.Dict[str, Flag]
 
 
+@dataclass(slots=True)
+class CustomTypeFlag(Flag):
+    """
+    A Flag for an Elm custom type.
+
+    <https://guide.elm-lang.org/types/custom_types>
+
+    variants = A list of tuples that specify the a discriminator and flag.
+
+    i.e.
+            FlagModel = Flags(CustomTypeFlag(variants=[("Custom1",StringFLag()), ("Custom2",IntFlag())]))
+
+            Turns into the the Elm type:
+
+            type SomeCustomType
+                = Custom1 String
+                | Custom2 Int
+
+            Then we parse a valid data structure:
+
+            FlagModel.parse("Hi there")
+    """
+
+    variants: list[tuple[str, Flag]]
+
+
 FlagsObject = dict[str, "PrimitiveFlag"]
 FlagsList = list["PrimitiveFlag"]
 FlagsNullable = typing.Union[type[str], type[int], type[float], type[bool], type[None]]
 PrimitiveObjectFlagType = (
     type[str]
     | type[int]
     | type[float]
```

### Comparing `djelm-0.7.0/src/djelm/generators.py` & `djelm-0.8.0/src/djelm/generators.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/management/commands/djelm.py` & `djelm-0.8.0/src/djelm/management/commands/djelm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/npm.py` & `djelm-0.8.0/src/djelm/npm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm` & `djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts` & `djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py` & `djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/strategy.py` & `djelm-0.8.0/src/djelm/strategy.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/subprocess.py` & `djelm-0.8.0/src/djelm/subprocess.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/utils.py` & `djelm-0.8.0/src/djelm/utils.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/validate.py` & `djelm-0.8.0/src/djelm/validate.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw` & `djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts` & `djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py` & `djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py`

 * *Files identical despite different names*

### Comparing `djelm-0.7.0/PKG-INFO` & `djelm-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djelm
-Version: 0.7.0
+Version: 0.8.0
 Summary: A framework for using Elm programs in a Django project
 Keywords: django,elm
 Author: Confidenceman02
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -592,14 +592,16 @@
         Err _ -> -- Flag failed to decode to an Int, Error!
             ( Error, Cmd.none )
 ```
 
 To summarize, we get compile and runtime guarantees that our program will behave as we expect. This is what makes Elm programs
 incredibly robust and nearly impossible to produce a runtime exception with.
 
+You can check out all the python flags you can use to express your data shape [here](https://github.com/Confidenceman02/django-elm/blob/main/src/djelm/flags/README.md).
+
 ## `generatemodel` Command
 
 Our python flag classes have a little trick up their sleeve that makes keeping both our python and Elm flag contracts in
 sync for us.
 
 We can see that in the `elm_programs/static_src/src/Models/Main.elm` module we have the following comment:
```

