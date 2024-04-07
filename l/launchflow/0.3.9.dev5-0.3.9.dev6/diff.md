# Comparing `tmp/launchflow-0.3.9.dev5.tar.gz` & `tmp/launchflow-0.3.9.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchflow-0.3.9.dev5.tar", last modified: Fri Apr  5 02:56:58 2024, max compression
+gzip compressed data, was "launchflow-0.3.9.dev6.tar", last modified: Sun Apr  7 23:54:42 2024, max compression
```

## Comparing `launchflow-0.3.9.dev5.tar` & `launchflow-0.3.9.dev6.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.263659 launchflow-0.3.9.dev5/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      118 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/MANIFEST.in
--rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-05 02:56:58.263659 launchflow-0.3.9.dev5/PKG-INFO
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1996 2024-03-13 23:12:43.000000 launchflow-0.3.9.dev5/README.md
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.227658 launchflow-0.3.9.dev5/launchflow/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      528 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.231658 launchflow-0.3.9.dev5/launchflow/aws/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       67 2024-03-20 15:00:34.000000 launchflow-0.3.9.dev5/launchflow/aws/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4480 2024-04-04 22:30:13.000000 launchflow-0.3.9.dev5/launchflow/aws/rds.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3512 2024-04-02 20:56:37.000000 launchflow-0.3.9.dev5/launchflow/aws/s3.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.231658 launchflow-0.3.9.dev5/launchflow/cache/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       95 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev5/launchflow/cache/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4980 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cache/launchflow_tmp.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-25 20:38:50.000000 launchflow-0.3.9.dev5/launchflow/cli/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/accounts/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev5/launchflow/cli/accounts/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1250 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/accounts/account_commands.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/config/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev5/launchflow/cli/config/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1026 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/config/config_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      566 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/constants.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/environments/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev5/launchflow/cli/environments/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2535 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/environments/environment_commands.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/gen/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2692 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.235658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      209 2024-04-02 23:44:00.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.239658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.239658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      216 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    15518 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.239658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:53:05.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      162 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.239658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      100 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.243658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      748 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      151 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      487 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      264 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2021 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.243658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.243658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:52:02.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.243658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      164 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      326 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.243658 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    14570 2024-04-05 00:17:09.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/django_template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.247659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.247659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      217 2024-04-02 23:47:30.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17805 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.247659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.247659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      576 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.247659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.247659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      573 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    18560 2024-04-05 00:17:11.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/fastapi_template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.251659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.251659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      215 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17114 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.251659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.251659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      297 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.255659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:33.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.255659 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      324 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17509 2024-04-05 00:17:00.000000 launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/flask_template.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    19278 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/main.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.255659 launchflow-0.3.9.dev5/launchflow/cli/project/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-30 20:01:40.000000 launchflow-0.3.9.dev5/launchflow/cli/project/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1702 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/cli/project/project_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3067 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/project_gen.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.255659 launchflow-0.3.9.dev5/launchflow/cli/resources/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev5/launchflow/cli/resources/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4436 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/resources/resource_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5382 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/cli/resources_ast.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.255659 launchflow-0.3.9.dev5/launchflow/cli/services/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/cli/services/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4413 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/cli/services/service_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3501 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev5/launchflow/cli/utils.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      482 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/cli/utyper.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.255659 launchflow-0.3.9.dev5/launchflow/clients/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      296 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/clients/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1155 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/clients/accounts_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1137 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev5/launchflow/clients/client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1832 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/clients/connect_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4806 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/clients/environments_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1911 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/clients/operations_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1820 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/clients/projects_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5117 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/clients/resources_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3767 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/clients/response_schemas.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3477 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/clients/services_client.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.259659 launchflow-0.3.9.dev5/launchflow/config/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev5/launchflow/config/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4412 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev5/launchflow/config/launchflow_config.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1361 2024-04-03 22:09:55.000000 launchflow-0.3.9.dev5/launchflow/config/launchflow_env.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5144 2024-03-14 16:50:08.000000 launchflow-0.3.9.dev5/launchflow/config/launchflow_yaml.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.259659 launchflow-0.3.9.dev5/launchflow/context/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-03-13 17:41:44.000000 launchflow-0.3.9.dev5/launchflow/context/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    16535 2024-04-03 22:10:20.000000 launchflow-0.3.9.dev5/launchflow/context/launchflow_ctx.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/exceptions.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5180 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev5/launchflow/fastapi.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       52 2024-03-27 23:08:23.000000 launchflow-0.3.9.dev5/launchflow/flask.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.259659 launchflow-0.3.9.dev5/launchflow/flows/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      129 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev5/launchflow/flows/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1236 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/flows/account_id.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3746 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/flows/auth.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    27918 2024-04-05 00:59:31.000000 launchflow-0.3.9.dev5/launchflow/flows/cloud_provider.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     7171 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev5/launchflow/flows/environments_flows.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev5/launchflow/flows/project_flows.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    18602 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev5/launchflow/flows/resource_flows.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.263659 launchflow-0.3.9.dev5/launchflow/gcp/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      219 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/gcp/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     7762 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/gcp/cloudsql.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2978 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/gcp/compute_engine.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3523 2024-04-02 20:56:22.000000 launchflow-0.3.9.dev5/launchflow/gcp/gcs.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2755 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev5/launchflow/gcp/memorystore.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2575 2024-04-03 23:45:13.000000 launchflow-0.3.9.dev5/launchflow/gcp/utils.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2059 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev5/launchflow/operations.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2288 2024-04-02 21:12:53.000000 launchflow-0.3.9.dev5/launchflow/resource.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       50 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev5/launchflow/service.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      789 2024-03-28 23:07:50.000000 launchflow-0.3.9.dev5/launchflow/utils.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-05 02:56:58.263659 launchflow-0.3.9.dev5/launchflow.egg-info/
--rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-05 02:56:58.000000 launchflow-0.3.9.dev5/launchflow.egg-info/PKG-INFO
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     8331 2024-04-05 02:56:58.000000 launchflow-0.3.9.dev5/launchflow.egg-info/SOURCES.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        1 2024-04-05 02:56:58.000000 launchflow-0.3.9.dev5/launchflow.egg-info/dependency_links.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       84 2024-04-05 02:56:58.000000 launchflow-0.3.9.dev5/launchflow.egg-info/entry_points.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      309 2024-04-05 02:56:58.000000 launchflow-0.3.9.dev5/launchflow.egg-info/requires.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       11 2024-04-05 02:56:58.000000 launchflow-0.3.9.dev5/launchflow.egg-info/top_level.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1421 2024-04-05 02:56:52.000000 launchflow-0.3.9.dev5/pyproject.toml
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       38 2024-04-05 02:56:58.263659 launchflow-0.3.9.dev5/setup.cfg
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.242891 launchflow-0.3.9.dev6/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      118 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/MANIFEST.in
+-rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-07 23:54:42.242891 launchflow-0.3.9.dev6/PKG-INFO
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1996 2024-03-13 23:12:43.000000 launchflow-0.3.9.dev6/README.md
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.214890 launchflow-0.3.9.dev6/launchflow/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      528 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.214890 launchflow-0.3.9.dev6/launchflow/aws/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       67 2024-03-20 15:00:34.000000 launchflow-0.3.9.dev6/launchflow/aws/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4480 2024-04-04 22:30:13.000000 launchflow-0.3.9.dev6/launchflow/aws/rds.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3512 2024-04-02 20:56:37.000000 launchflow-0.3.9.dev6/launchflow/aws/s3.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.214890 launchflow-0.3.9.dev6/launchflow/cache/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       95 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/cache/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4980 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cache/launchflow_tmp.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-25 20:38:50.000000 launchflow-0.3.9.dev6/launchflow/cli/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/accounts/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/accounts/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1250 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/accounts/account_commands.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/config/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/config/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1026 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/config/config_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      566 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/constants.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/environments/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/environments/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2535 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/environments/environment_commands.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2692 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      209 2024-04-02 23:44:00.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      216 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    15518 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:53:05.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      162 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      100 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      748 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      151 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      487 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      264 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2021 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:52:02.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      164 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      326 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    14570 2024-04-05 00:17:09.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/django_template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      217 2024-04-02 23:47:30.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17805 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      576 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      573 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    18560 2024-04-05 00:17:11.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/fastapi_template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      215 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17114 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      297 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:33.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      324 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17509 2024-04-05 00:17:00.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/flask_template.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    19278 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/main.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/project/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-30 20:01:40.000000 launchflow-0.3.9.dev6/launchflow/cli/project/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1702 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/cli/project/project_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3067 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/project_gen.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/resources/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/resources/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4436 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/resources/resource_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5382 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/resources_ast.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/services/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/cli/services/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4413 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/services/service_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3501 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/cli/utils.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      482 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/cli/utyper.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/clients/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      296 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1155 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/accounts_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1137 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/clients/client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1832 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/connect_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4806 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/clients/environments_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1911 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/operations_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1820 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/projects_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5117 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/resources_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3767 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/response_schemas.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3477 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/services_client.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/config/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/config/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4412 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/config/launchflow_config.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1361 2024-04-03 22:09:55.000000 launchflow-0.3.9.dev6/launchflow/config/launchflow_env.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5144 2024-03-14 16:50:08.000000 launchflow-0.3.9.dev6/launchflow/config/launchflow_yaml.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/context/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-03-13 17:41:44.000000 launchflow-0.3.9.dev6/launchflow/context/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    16535 2024-04-03 22:10:20.000000 launchflow-0.3.9.dev6/launchflow/context/launchflow_ctx.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/exceptions.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5180 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev6/launchflow/fastapi.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       52 2024-03-27 23:08:23.000000 launchflow-0.3.9.dev6/launchflow/flask.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/flows/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      129 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/flows/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1236 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/flows/account_id.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3746 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/flows/auth.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    27648 2024-04-06 20:06:09.000000 launchflow-0.3.9.dev6/launchflow/flows/cloud_provider.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     7171 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev6/launchflow/flows/environments_flows.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev6/launchflow/flows/project_flows.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    18602 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/flows/resource_flows.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/gcp/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      219 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     7762 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/cloudsql.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2978 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/compute_engine.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3523 2024-04-02 20:56:22.000000 launchflow-0.3.9.dev6/launchflow/gcp/gcs.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2755 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/memorystore.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2578 2024-04-05 21:08:46.000000 launchflow-0.3.9.dev6/launchflow/gcp/utils.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2059 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/operations.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2288 2024-04-02 21:12:53.000000 launchflow-0.3.9.dev6/launchflow/resource.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       50 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/service.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      789 2024-03-28 23:07:50.000000 launchflow-0.3.9.dev6/launchflow/utils.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow.egg-info/
+-rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/PKG-INFO
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     8331 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        1 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       84 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/entry_points.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      309 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/requires.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       11 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/top_level.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1421 2024-04-07 23:54:33.000000 launchflow-0.3.9.dev6/pyproject.toml
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       38 2024-04-07 23:54:42.242891 launchflow-0.3.9.dev6/setup.cfg
```

### Comparing `launchflow-0.3.9.dev5/PKG-INFO` & `launchflow-0.3.9.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchflow
-Version: 0.3.9.dev5
+Version: 0.3.9.dev6
 Summary: Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic.
 Author-email: CalebTVanDyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: beaupy
 Requires-Dist: rich
```

### Comparing `launchflow-0.3.9.dev5/README.md` & `launchflow-0.3.9.dev6/README.md`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/__init__.py` & `launchflow-0.3.9.dev6/launchflow/__init__.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/aws/rds.py` & `launchflow-0.3.9.dev6/launchflow/aws/rds.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/aws/s3.py` & `launchflow-0.3.9.dev6/launchflow/aws/s3.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cache/launchflow_tmp.py` & `launchflow-0.3.9.dev6/launchflow/cache/launchflow_tmp.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/accounts/account_commands.py` & `launchflow-0.3.9.dev6/launchflow/cli/accounts/account_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/config/config_commands.py` & `launchflow-0.3.9.dev6/launchflow/cli/config/config_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/constants.py` & `launchflow-0.3.9.dev6/launchflow/cli/constants.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/environments/environment_commands.py` & `launchflow-0.3.9.dev6/launchflow/cli/environments/environment_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/template.py` & `launchflow-0.3.9.dev6/launchflow/cli/gen/template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/django/django_template.py` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/django_template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/fastapi/fastapi_template.py` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/fastapi_template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/gen/templates/flask/flask_template.py` & `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/flask_template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/main.py` & `launchflow-0.3.9.dev6/launchflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/project/project_commands.py` & `launchflow-0.3.9.dev6/launchflow/cli/project/project_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/project_gen.py` & `launchflow-0.3.9.dev6/launchflow/cli/project_gen.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/resources/resource_commands.py` & `launchflow-0.3.9.dev6/launchflow/cli/resources/resource_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/resources_ast.py` & `launchflow-0.3.9.dev6/launchflow/cli/resources_ast.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/services/service_commands.py` & `launchflow-0.3.9.dev6/launchflow/cli/services/service_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/cli/utils.py` & `launchflow-0.3.9.dev6/launchflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/accounts_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/accounts_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/client.py` & `launchflow-0.3.9.dev6/launchflow/clients/client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/connect_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/connect_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/environments_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/environments_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/operations_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/operations_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/projects_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/projects_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/resources_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/resources_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/response_schemas.py` & `launchflow-0.3.9.dev6/launchflow/clients/response_schemas.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/clients/services_client.py` & `launchflow-0.3.9.dev6/launchflow/clients/services_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/config/launchflow_config.py` & `launchflow-0.3.9.dev6/launchflow/config/launchflow_config.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/config/launchflow_env.py` & `launchflow-0.3.9.dev6/launchflow/config/launchflow_env.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/config/launchflow_yaml.py` & `launchflow-0.3.9.dev6/launchflow/config/launchflow_yaml.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/context/launchflow_ctx.py` & `launchflow-0.3.9.dev6/launchflow/context/launchflow_ctx.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/exceptions.py` & `launchflow-0.3.9.dev6/launchflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/fastapi.py` & `launchflow-0.3.9.dev6/launchflow/fastapi.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/flows/account_id.py` & `launchflow-0.3.9.dev6/launchflow/flows/account_id.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/flows/auth.py` & `launchflow-0.3.9.dev6/launchflow/flows/auth.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/flows/cloud_provider.py` & `launchflow-0.3.9.dev6/launchflow/flows/cloud_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     (CloudProvider.GCP, "Google Cloud Platform"),
     (CloudProvider.AWS, "Amazon Web Services"),
     # (CloudProvider.AZURE, "Microsoft Azure"),
 ]
 
 
 def select_cloud_provider() -> CloudProvider:
-    options = [f"{f[0].value} - {f[1]}" for f in CLOUD_PROVIDER_CHOICES]
+    options = [f"{f[0].value.upper()} - {f[1]}" for f in CLOUD_PROVIDER_CHOICES]
     answer = beaupy.select(options=options, return_index=True)
     rich.print(f"[pink1]>[/pink1] {options[answer]}")
     return CLOUD_PROVIDER_CHOICES[answer][0]
 
 
 async def connect(
     client: LaunchFlowAsyncClient,
@@ -53,26 +53,40 @@
         )
         provider = select_cloud_provider()
 
     setup_status = await client.connect.status(
         account_id=account_id, include_aws_template_url=True
     )
     if provider == CloudProvider.GCP:
-        await _connect_gcp(
-            client,
-            account_id,
-            setup_status.gcp_connection_info.admin_service_account_email,
-        )
+        if setup_status.gcp_connection_info.verified_at:
+            rich.print(
+                "[green][bold]GCP is already connected[/bold][/green] 🚀\n"
+                "You can now create environments and deploy resources to your GCP account using LaunchFlow.\n"
+            )
+            _setup_local_gcp_env()
+        else:
+            await _connect_gcp(
+                client,
+                account_id,
+                setup_status.gcp_connection_info.admin_service_account_email,
+            )
     elif provider == CloudProvider.AWS:
-        await _connect_aws(
-            client,
-            account_id,
-            setup_status.aws_connection_info.external_role_id,
-            setup_status.aws_connection_info.cloud_foundation_template_url,
-        )
+        if setup_status.aws_connection_info.verified_at:
+            rich.print(
+                "[green][bold]AWS is already connected[/bold][/green] 🚀\n"
+                "You can now create environments and deploy resources to your AWS account using LaunchFlow.\n"
+            )
+            _setup_local_aws_env()
+        else:
+            await _connect_aws(
+                client,
+                account_id,
+                setup_status.aws_connection_info.external_role_id,
+                setup_status.aws_connection_info.cloud_foundation_template_url,
+            )
     else:
         raise ValueError(f"LaunchFlow currently does not support `{provider.value}`")
 
 
 AWS_REGIONS = [
     "us-east-1",
     "us-east-2",
@@ -115,15 +129,15 @@
     if ask:
         answer = beaupy.confirm(
             "Would you like us to verify your local AWS setup?", default_is_yes=True
         )
     if answer:
         process = subprocess.run("aws --version", shell=True, capture_output=True)
         if process.returncode == 127:
-            rich.print("[red]Error: `aws` was not installed[/red].")
+            rich.print("[red]Error: `aws` CLI is not installed on your machine[/red].")
             install = beaupy.confirm(
                 "Would you like to install it? (we will follow the steps outlined on https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)",
                 default_is_yes=True,
             )
             if not install:
                 return
             install_dir = beaupy.prompt(
@@ -196,164 +210,129 @@
                     f.write(response.raw.read())
                 progress.remove_task(download_task)
                 progress.console.print(
                     f"[green]✓[/green] Downloaded aws for {system} {proc_type}."
                 )
             with zipfile.ZipFile(zip_file, "r") as zip_ref:
                 zip_ref.extractall(install_dir)
-            install_sh = subprocess.run("./aws/install", shell=True, cwd=install_dir)
+            os.chmod(os.path.join(install_dir, "aws", "install"), 0o755)
+            os.chmod(os.path.join(install_dir, "aws", "dist", "aws"), 0o744)
+            bin_dir = os.path.join(install_dir, "bin")
+            install_sh = subprocess.run(
+                f"./aws/install --install-dir {install_dir} --bin-dir {bin_dir}",
+                shell=True,
+                cwd=install_dir,
+            )
+            add_to_path = beaupy.confirm(
+                "Would you like to add the `aws` binary to your PATH?",
+                default_is_yes=True,
+            )
+            if add_to_path:
+                if os.path.exists(os.path.expanduser("~/.bashrc")):
+                    with open(os.path.expanduser("~/.bashrc"), "a") as f:
+                        f.write(f'export PATH="$PATH:{bin_dir}"\n')
+                if os.path.exists(os.path.expanduser("~/.zshrc")):
+                    with open(os.path.expanduser("~/.zshrc"), "a") as f:
+                        f.write(f'export PATH="$PATH:{bin_dir}"\n')
             if install_sh.returncode != 0:
                 rich.print(
-                    f"[red]Error: failed to install aws, please run `./aws/install` in {install_dir}.[/red]."
+                    f"[red]Error: failed to install aws, please run `./aws/install --bin-dir {bin_dir}` in {install_dir}.[/red]."
                 )
                 return
             rich.print(
-                "[green]`aws` successfully installed. You will need to reload your terminal to use it.[/green]"
+                "[green]`aws` CLI successfully installed. You will need to reload your terminal to use it.[/green]"
             )
         else:
-            rich.print("[green]`aws` is installed[/green]")
+            rich.print("[green]`aws` CLI is installed[/green]")
         process = subprocess.run(
             "aws sts get-caller-identity", shell=True, capture_output=True
         )
         if process.returncode != 0:
             rich.print("[red]Error: No default `aws` credentials found.[/red]")
             set_up_auth = beaupy.confirm(
                 "Would you like us to authenticate for you?", default_is_yes=True
             )
             if set_up_auth:
+                profile_name = beaupy.prompt(
+                    "What profile name would you like to use (defaults to `LocalProfile`)?",
+                    initial_value="LocalProfile",
+                )
                 use_sso = beaupy.confirm(
-                    "Does your AWS account use AWS SSO? Hint: you would have a URL like `https://<account_id>.awsapps.com/start`",
-                    default_is_no=False,
+                    "Does your AWS account use AWS SSO? Hint: you would have a login URL like `https://<org_name>.awsapps.com/start`",
+                    default_is_yes=False,
                 )
                 if use_sso:
                     rich.print(
-                        "Running:\n\n\t$ aws sso login\n\nYou will need to have your AWS SSO URL ready. Visit https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sso.html for more information.\n"
+                        f"Running:\n\n\t$ aws configure sso --profile {profile_name}\n\nYou will need to have your AWS SSO URL ready. Visit https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sso.html for more information.\n"
+                    )
+                    process = subprocess.run(
+                        f"aws configure sso --profile {profile_name}", shell=True
                     )
-                    process = subprocess.run("aws sso login", shell=True)
                 else:
                     rich.print(
-                        "Running:\n\n\t$ aws configure\n\nYou will need to have your AWS access key ID and secret access key ready. Visit https://console.aws.amazon.com/iam/home#/security_credentials to create them.\nVisit https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html for more information.\n"
+                        f"Running:\n\n\t$ aws configure --profile {profile_name}\n\nYou will need to have your AWS access key ID and secret access key ready. Visit https://console.aws.amazon.com/iam/home#/security_credentials to create them.\nVisit https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html for more information.\n"
+                    )
+                    process = subprocess.run(
+                        f"aws configure --profile {profile_name}", shell=True
+                    )
+                set_default_profile = beaupy.confirm(
+                    f"Would you like to set `{profile_name}` as your default AWS profile? (Recommended)",
+                    default_is_yes=True,
+                )
+                if set_default_profile:
+                    print(
+                        f"Running:\n\n\t$ aws configure set default.profile {profile_name}\n"
+                    )
+                    process = subprocess.run(
+                        f"aws configure set default.profile {profile_name}", shell=True
                     )
-                    process = subprocess.run("aws configure", shell=True)
+                # TODO: Make sure this doesnt run on cntl+c
+                rich.print(
+                    f"[green]`aws` successfully authenticated with profile `{profile_name}`[/green]"
+                )
         else:
             rich.print("[green]`aws` is authenticated[/green]")
 
-
-def _add_aws_permissions():
-    try:
-        import boto3
-    except ImportError:
-        rich.print(
-            "[red]Error: Ensure AWS dependencies are installed by running `pip install launchflow\[aws]` to setup aws.[/red]"
-        )
-        raise typer.Exit(1)
-    with Progress(
-        SpinnerColumn(),
-        TextColumn("[progress.description]{task.description}"),
-    ) as progress:
-        try:
-            task = progress.add_task("Looking up AWS account IDs...", total=None)
-            client = boto3.client("organizations")
-            accounts = client.list_accounts()
-        except Exception as e:
-            progress.remove_task(task)
-            rich.print(f"[red]Error: {e}[/red]")
-            raise typer.Exit(1)
-        account_ids = []
-        prompts = []
-        for account in accounts["Accounts"]:
-            account_ids.append(account["Id"])
-            prompts.append(f"{account['Name']} ({account['Id']})")
-        progress.remove_task(task)
-    if not account_ids:
-        rich.print("[red]Error: no accounts found.[/red]")
-        raise typer.Exit(1)
-    rich.print("Select the account you would like to connect LaunchFlow to:")
-    answer = beaupy.select(prompts, return_index=True, strict=True)
-    rich.print(f"[pink1]>[/pink1] {prompts[answer]}\n")
-    account_id = account_ids[answer]
-    with Progress(
-        SpinnerColumn(),
-        TextColumn("[progress.description]{task.description}"),
-    ) as progress:
-        task = progress.add_task(
-            f"Running AWS CloudFormation stack for `{account_id}`...", total=None
-        )
-        try:
-            client = boto3.client("cloudformation")
-            response = client.create_stack(
-                StackName="LaunchFlowRole",
-                TemplateURL="https://launchflow-public-assets.s3.amazonaws.com/launchflow-role.yaml",
-                Parameters=[
-                    {
-                        "ParameterKey": "LaunchFlowExternalID",
-                        "ParameterValue": "launchflow",
-                    }
-                ],
-                Capabilities=["CAPABILITY_NAMED_IAM"],
-            )
-            stack_id = response["StackId"]
-            waiter = client.get_waiter("stack_create_complete")
-            waiter.wait(StackName=stack_id)
-        except Exception as e:
-            progress.remove_task(task)
-            rich.print(f"[red]Error: {e}[/red]")
-            raise typer.Exit(1)
-    progress.console.print(
-        f"[green]✓[/green] CloudFormation stack created for `{account_id}`."
+    rich.print(
+        "\n[i]Your local machine is setup to interact with AWS resources using LaunchFlow's Python SDK or the `aws` CLI.[/i]"
     )
+    rich.print("Happy launching! 🚀\n")
 
 
 async def _connect_aws(
     client: LaunchFlowAsyncClient,
     account_id: str,
     external_role_id: str,
     template_url: str,
 ):
+    aws_account_id = Prompt.ask(
+        "\nEnter your AWS account ID (can be found in the top right corner of https://console.aws.amazon.com/)."
+    )
+
+    print("\nSelect the AWS region you would like to setup LaunchFlow in:")
+    region = beaupy.select(AWS_REGIONS, pagination=True)
+    rich.print(f"[pink1]>[/pink1] {region}\n")
+
+    url = _AWS_URL.format(
+        region=region, external_id=external_role_id, template_url=template_url
+    )
+    webbrowser.open(url)
+    rich.print(" - Visit the AWS Console to create a CloudFormation stack")
+    rich.print(' - Scroll to the bottom and check the "I acknowledge..." box ')
     rich.print(
-        f"\n`[cyan]{external_role_id}[/cyan]` needs the following role on your AWS account:"
+        ' - Click on "Create Stack". It may take a few minutes for the fole to be fully created.\n'
     )
-    rich.print("- LaunchFlowRole ([i]LaunchFlowExternalID=launchflow[/i])\n")
+
     rich.print(
         "[i]This role will be used to provision AWS resources and deployments in your AWS account.[/i]\n"
     )
 
-    rich.print("How would you like to add this role?")
-    options = [
-        "Have LaunchFlow add it using my local credentials",
-        "Manually add this role via the AWS console",
-    ]
-    answer = beaupy.select(options, strict=True, return_index=True)
-    rich.print(f"[pink1]>[/pink1] {options[answer]}")
-    if answer == 0:
-        rich.print("Verifying local AWS setup...")
-        _setup_local_aws_env(ask=False)
-        _add_aws_permissions()
-    else:
-        aws_account_id = Prompt.ask(
-            "\nEnter your AWS account ID (can be found in the top right corner of https://console.aws.amazon.com/). You will then be prompted to login to your AWS account"
-        )
-        webbrowser.open("https://console.aws.amazon.com/")
-
-        print("\nSelect the AWS region you would like to setup LaunchFlow in:")
-        region = beaupy.select(AWS_REGIONS, pagination=True)
-        rich.print(f"[pink1]>[/pink1] {region}\n")
-
-        url = _AWS_URL.format(
-            region=region, external_id=external_role_id, template_url=template_url
-        )
-        webbrowser.open(url)
-        rich.print(" - Visit the AWS Console to create a CloudFormation stack")
-        rich.print(' - Scroll to the bottom and check the "I acknowledge..." box ')
-        rich.print(
-            ' - Click on "Create Stack". It may take a few minutes for the fole to be fully created.\n'
-        )
-        _ = Prompt.ask(
-            "Once the role is fully created hit enter to have us verify the setup"
-        )
+    _ = Prompt.ask(
+        "Once the role is fully created hit enter to have us verify the setup"
+    )
 
     # polls for a successful connection for up to 60 seconds
     start_time = time.time()
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
     ) as progress:
@@ -373,19 +352,15 @@
                     )
             await asyncio.sleep(3)
 
         progress.remove_task(task)
 
     rich.print("\n[bold]AWS successfully connected[/bold] 🚀")
 
-    if answer == 1:
-        _setup_local_aws_env()
-    rich.print(
-        "[i]You can now create environments and deploy resources to your AWS account using LaunchFlow.[/i]"
-    )
+    _setup_local_aws_env()
 
 
 def _setup_local_gcp_env(ask: bool = True):
     answer = True
     if ask:
         answer = beaupy.confirm(
             "Would you like us to verify your local GCP setup?", default_is_yes=True
@@ -514,14 +489,19 @@
                 )
                 process = subprocess.run(
                     "gcloud auth login --update-adc", shell=True, start_new_session=True
                 )
         else:
             rich.print("[green]`gcloud` is authenticated[/green]")
 
+    rich.print(
+        "\n[i]Your local machine is setup to interact with GCP resources using LaunchFlow's Python SDK or the `gcloud` CLI.[/i]"
+    )
+    rich.print("Happy launching! 🚀\n")
+
 
 async def _add_gcp_permissions(service_account: str):
     try:
         import googleapiclient.discovery
         from google.auth import exceptions
         from google.cloud import resourcemanager_v3
         from googleapiclient.errors import HttpError
```

### Comparing `launchflow-0.3.9.dev5/launchflow/flows/environments_flows.py` & `launchflow-0.3.9.dev6/launchflow/flows/environments_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/flows/project_flows.py` & `launchflow-0.3.9.dev6/launchflow/flows/project_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/flows/resource_flows.py` & `launchflow-0.3.9.dev6/launchflow/flows/resource_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/gcp/cloudsql.py` & `launchflow-0.3.9.dev6/launchflow/gcp/cloudsql.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/gcp/compute_engine.py` & `launchflow-0.3.9.dev6/launchflow/gcp/compute_engine.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/gcp/gcs.py` & `launchflow-0.3.9.dev6/launchflow/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/gcp/memorystore.py` & `launchflow-0.3.9.dev6/launchflow/gcp/memorystore.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/gcp/utils.py` & `launchflow-0.3.9.dev6/launchflow/gcp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import os
 from typing import Optional
 
 import requests
 from google.auth import default, impersonated_credentials
-
 from launchflow.context import ctx
 
 _ProjectIdMetadataKey = "project/project-id"
 _ProjectNumberMetadataKey = "project/numeric-project-id"
 _RegionMetadataKey = "instance/region"
 _InstanceIdMetadataKey = "instance/id"
 _ServiceAccountEmailMetadataKey = "instance/service-accounts/default/email"
 _ServiceAccountTokenMetadataKey = "instance/service-accounts/default/token"
 
 
 # Cloud Run automatically sets the K_SERVICE environment variable
 # Docs: https://cloud.google.com/run/docs/container-contract#env-vars
-def is_running_on_cloud_run():
+def _is_running_on_cloud_run():
     """Check if running on Google Cloud Run."""
     return "K_SERVICE" in os.environ
 
 
 # Cloud Run instances expose a metadata server to fetch info at runtime
 # Docs: https://cloud.google.com/run/docs/reference/container-contract#metadata-server
-def get_cloud_run_metadata(metadata_key: str):
+def _get_cloud_run_metadata(metadata_key: str):
     """
     Get the metadata value from the Cloud Run instance metadata server.
     """
     metadata_server_url = "http://metadata.google.internal/computeMetadata/v1/"
     metadata_server_url += metadata_key
 
     headers = {"Metadata-Flavor": "Google"}
@@ -41,17 +40,17 @@
     project_name: Optional[str] = None,
     environment_name: Optional[str] = None,
 ) -> str:
     """
     Get the GCP service account credentials for the specified project and environment.
     """
 
-    if is_running_on_cloud_run():
+    if _is_running_on_cloud_run():
         # If running on Cloud Run, fetch the service account from the metadata server
-        gcp_service_account_email = get_cloud_run_metadata(
+        gcp_service_account_email = _get_cloud_run_metadata(
             _ServiceAccountEmailMetadataKey
         )
     else:
         # If not on Cloud Run, fetch the GCP service account email from LaunchFlow
         gcp_service_account_email = ctx.get_gcp_service_account_email(
             project_name, environment_name
         )
```

### Comparing `launchflow-0.3.9.dev5/launchflow/operations.py` & `launchflow-0.3.9.dev6/launchflow/operations.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/resource.py` & `launchflow-0.3.9.dev6/launchflow/resource.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow/utils.py` & `launchflow-0.3.9.dev6/launchflow/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/launchflow.egg-info/PKG-INFO` & `launchflow-0.3.9.dev6/launchflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchflow
-Version: 0.3.9.dev5
+Version: 0.3.9.dev6
 Summary: Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic.
 Author-email: CalebTVanDyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: beaupy
 Requires-Dist: rich
```

### Comparing `launchflow-0.3.9.dev5/launchflow.egg-info/SOURCES.txt` & `launchflow-0.3.9.dev6/launchflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev5/pyproject.toml` & `launchflow-0.3.9.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launchflow"
-version = "0.3.9.dev5"
+version = "0.3.9.dev6"
 description = "Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic."
 authors = [
     { name = "CalebTVanDyke", email = "caleb@launchflow.com" },
     { name = "Josh Tanke", email = "josh@launchflow.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
```

