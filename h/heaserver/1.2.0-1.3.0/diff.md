# Comparing `tmp/heaserver-1.2.0.tar.gz` & `tmp/heaserver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.2.0.tar", last modified: Fri Apr  5 18:39:00 2024, max compression
+gzip compressed data, was "heaserver-1.3.0.tar", last modified: Mon Apr  8 18:03:45 2024, max compression
```

## Comparing `heaserver-1.2.0.tar` & `heaserver-1.3.0.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.101987 heaserver-1.2.0/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.2.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.2.0/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6567 2024-04-05 18:39:00.100986 heaserver-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4572 2024-04-05 18:37:34.000000 heaserver-1.2.0/README.md
--rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.2.0/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.695224 heaserver-1.2.0/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.696226 heaserver-1.2.0/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.726193 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19321 2024-03-26 22:51:02.000000 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.727192 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.697194 heaserver-1.2.0/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.697194 heaserver-1.2.0/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.730191 heaserver-1.2.0/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.737192 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.2.0/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.699192 heaserver-1.2.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.699192 heaserver-1.2.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.761191 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.788193 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5792 2023-12-16 23:04:09.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5553 2024-04-05 04:20:14.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5222 2024-04-05 04:20:06.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4656 2024-04-05 04:24:57.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.790192 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.2.0/pytest.ini
--rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.2.0/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 18:39:00.101987 heaserver-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2870 2024-04-05 18:38:17.000000 heaserver-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.701192 heaserver-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.701192 heaserver-1.2.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.842197 heaserver-1.2.0/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.2.0/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.2.0/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    23214 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.854193 heaserver-1.2.0/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.2.0/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    25526 2024-04-05 16:50:29.000000 heaserver-1.2.0/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.2.0/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    30855 2024-04-04 23:45:07.000000 heaserver-1.2.0/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.2.0/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4515 2024-04-05 04:18:06.000000 heaserver-1.2.0/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.2.0/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.2.0/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.862195 heaserver-1.2.0/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.2.0/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.2.0/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.874196 heaserver-1.2.0/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    25695 2024-04-01 23:40:09.000000 heaserver-1.2.0/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.2.0/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.2.0/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.2.0/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.2.0/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.899475 heaserver-1.2.0/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    40278 2024-04-01 23:40:09.000000 heaserver-1.2.0/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.2.0/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.2.0/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    18431 2024-04-05 04:45:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.2.0/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.2.0/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.2.0/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.099985 heaserver-1.2.0/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     6567 2024-04-05 18:38:59.000000 heaserver-1.2.0/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17473 2024-04-05 18:38:59.000000 heaserver-1.2.0/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:38:59.000000 heaserver-1.2.0/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2024-04-05 18:38:59.000000 heaserver-1.2.0/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 18:38:59.000000 heaserver-1.2.0/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.705192 heaserver-1.2.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.705192 heaserver-1.2.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:38:59.965474 heaserver-1.2.0/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.003474 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.005473 heaserver-1.2.0/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    16505 2024-04-01 23:40:09.000000 heaserver-1.2.0/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.008473 heaserver-1.2.0/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.017473 heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5351 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5675 2024-04-05 04:15:03.000000 heaserver-1.2.0/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.037473 heaserver-1.2.0/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.096986 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.2.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7012 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5322 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:39:00.097986 heaserver-1.2.0/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.2.0/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.516742 heaserver-1.3.0/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.3.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.3.0/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6762 2024-04-08 18:03:45.514742 heaserver-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4767 2024-04-08 18:02:09.000000 heaserver-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.3.0/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.060134 heaserver-1.3.0/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.060134 heaserver-1.3.0/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.095857 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19401 2024-04-08 16:43:14.000000 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.097926 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.061708 heaserver-1.3.0/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.061721 heaserver-1.3.0/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.100509 heaserver-1.3.0/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.109185 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.3.0/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.062714 heaserver-1.3.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.062714 heaserver-1.3.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.138392 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.173146 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5792 2023-12-16 23:04:09.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5553 2024-04-05 18:40:52.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5222 2024-04-05 18:40:52.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4656 2024-04-05 18:40:52.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.174146 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.3.0/pytest.ini
+-rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.3.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:03:45.516742 heaserver-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2870 2024-04-08 18:02:55.000000 heaserver-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.066716 heaserver-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.066716 heaserver-1.3.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.229212 heaserver-1.3.0/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.3.0/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.3.0/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    23214 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.241213 heaserver-1.3.0/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.3.0/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    26792 2024-04-08 17:34:02.000000 heaserver-1.3.0/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.3.0/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    31543 2024-04-08 17:42:07.000000 heaserver-1.3.0/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.3.0/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.3.0/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.3.0/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.3.0/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.247213 heaserver-1.3.0/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.3.0/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.3.0/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.258212 heaserver-1.3.0/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    25695 2024-04-01 23:40:09.000000 heaserver-1.3.0/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.3.0/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.3.0/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.3.0/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.3.0/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.295213 heaserver-1.3.0/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    40278 2024-04-01 23:40:09.000000 heaserver-1.3.0/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.3.0/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.3.0/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    18431 2024-04-05 18:40:52.000000 heaserver-1.3.0/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.3.0/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.3.0/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.3.0/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.513742 heaserver-1.3.0/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     6762 2024-04-08 18:03:44.000000 heaserver-1.3.0/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17473 2024-04-08 18:03:45.000000 heaserver-1.3.0/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:03:44.000000 heaserver-1.3.0/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      455 2024-04-08 18:03:44.000000 heaserver-1.3.0/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 18:03:44.000000 heaserver-1.3.0/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.069714 heaserver-1.3.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.070715 heaserver-1.3.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.366748 heaserver-1.3.0/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.411744 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.413743 heaserver-1.3.0/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    16505 2024-04-01 23:40:09.000000 heaserver-1.3.0/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.417742 heaserver-1.3.0/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.426743 heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5351 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5675 2024-04-05 18:40:52.000000 heaserver-1.3.0/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.448741 heaserver-1.3.0/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.510742 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.3.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7012 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5322 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:03:45.512741 heaserver-1.3.0/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.3.0/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.2.0/LICENSE` & `heaserver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/PKG-INFO` & `heaserver-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.2.0
+Version: 1.3.0
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,19 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.3.0
+* Performance improvement getting accounts.
+* heaserver.service.db.database.DatabaseContextManagers now allow initializing with either a volume id or a Credentials
+object.
+
 ## Version 1.2.0
 * get_volumes() in the database module and Database class can now filter by account ids.
 * New heaobject dependency: new heaobject.root.AbstractAssociation base class and heaobject.account.AccountAssociation
 implementation, and heaobject.organization.Organization class now has an accounts attribute using AccountAssociation.
 
 ## Version 1.1.3
 * Fixed permissions setting in mongoservicelib.aggregate().
```

### Comparing `heaserver-1.2.0/README.md` & `heaserver-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.3.0
+* Performance improvement getting accounts.
+* heaserver.service.db.database.DatabaseContextManagers now allow initializing with either a volume id or a Credentials
+object.
+
 ## Version 1.2.0
 * get_volumes() in the database module and Database class can now filter by account ids.
 * New heaobject dependency: new heaobject.root.AbstractAssociation base class and heaobject.account.AccountAssociation
 implementation, and heaobject.organization.Organization class now has an accounts attribute using AccountAssociation.
 
 ## Version 1.1.3
 * Fixed permissions setting in mongoservicelib.aggregate().
```

### Comparing `heaserver-1.2.0/RELEASING.md` & `heaserver-1.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 
 class TestAWSServiceLib(AWSS3FolderTestCase):
 
     def setUp(self):
         super().setUp()
         self.s3 = boto3.client('s3')
 
+    def tearDown(self):
+        super().tearDown()
+        self.s3.close()
+
     async def test_list_bucket_not_found(self):
         with self.assertRaises(ClientError):
             l = [o async for o in awsservicelib.list_objects(self.s3, 'blah')]
 
     async def test_list_bucket(self):
         expected = [{'Key': 'TestFolder/', 'LastModified': FakeDatetime(2022, 5, 17, 0, 0, tzinfo=tzutc()),
                      'ETag': '"d41d8cd98f00b204e9800998ecf8427e"', 'Size': 0, 'StorageClass': 'STANDARD'},
```

### Comparing `heaserver-1.2.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.3.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.3.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.3.0/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.3.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/setup.py` & `heaserver-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.2.0',
+      version='1.3.0',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
```

### Comparing `heaserver-1.2.0/src/heaserver/service/__init__.py` & `heaserver-1.3.0/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/activity.py` & `heaserver-1.3.0/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/aiohttp.py` & `heaserver-1.3.0/src/heaserver/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/appfactory.py` & `heaserver-1.3.0/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/appproperty.py` & `heaserver-1.3.0/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/backgroundtasks.py` & `heaserver-1.3.0/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/caching.py` & `heaserver-1.3.0/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/client.py` & `heaserver-1.3.0/src/heaserver/service/client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/config.py` & `heaserver-1.3.0/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/db/aws.py` & `heaserver-1.3.0/src/heaserver/service/db/aws.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,32 +82,35 @@
         :param app: the aiohttp app.
         :param name: the property's name.
         :return: a Property instance or None (if not found).
         """
         return await client.get_property(app=app, name=name)
 
     @overload
-    async def get_client(self, request: Request, service_name: Literal['s3'], volume_id: str) -> S3Client:
+    async def get_client(self, request: Request, service_name: Literal['s3'], volume_id: str | None = None,
+                         credentials: AWSCredentials | None = None) -> S3Client:
         ...
 
     @overload
-    async def get_client(self, request: Request, service_name: Literal['sts'], volume_id: str) -> STSClient:
+    async def get_client(self, request: Request, service_name: Literal['sts'], volume_id: str | None = None,
+                         credentials: AWSCredentials | None = None) -> STSClient:
         ...
 
     @overload
-    async def get_client(self, request: Request, service_name: Literal['account'], volume_id: str) -> AccountClient:
+    async def get_client(self, request: Request, service_name: Literal['account'], volume_id: str | None = None,
+                         credentials: AWSCredentials | None = None) -> AccountClient:
         ...
 
     @overload
-    async def get_client(self, request: Request, service_name: Literal['organizations'],
-                         volume_id: str) -> OrganizationsClient:
+    async def get_client(self, request: Request, service_name: Literal['organizations'], volume_id: str | None = None,
+                         credentials: AWSCredentials | None = None) -> OrganizationsClient:
         ...
 
-    async def get_client(self, request: Request, service_name: str,
-                         volume_id: str) -> S3Client | STSClient | AccountClient | OrganizationsClient:
+    async def get_client(self, request: Request, service_name: str, volume_id: str | None = None,
+                         credentials: AWSCredentials | None = None) -> S3Client | STSClient | AccountClient | OrganizationsClient:
         """
         Gets an AWS service client.  If the volume has no credentials, it uses the boto3 library to try and find them.
         This method is not designed to be overridden.
 
         :param request: the HTTP request (required).
         :param service_name: AWS service name (required).
         :param volume_id: the id string of a volume (required).
@@ -116,17 +119,20 @@
         application-level property.
         :raise ValueError: if there is no volume with the provided volume id, the volume's file system does not exist,
         the volume's credentials were not found, or a necessary service is not registered.
 
         TODO: need a separate exception thrown for when a service is not registered (so that the server can respond with a 500 error).
         TODO: need to lock around client creation because it's not threadsafe, manifested by sporadic KeyError: 'endpoint_resolver'.
         """
-        return await self.__get_resource_or_client(request, service_name, volume_id, create_client)
+        if credentials is None:
+            credentials = await self.get_credentials_from_volume(request, volume_id)
+        return await self.__get_resource_or_client(request, service_name, create_client, credentials)
 
-    async def get_resource(self, request: Request, service_name: str, volume_id: str) -> S3ServiceResource:
+    async def get_resource(self, request: Request, service_name: str, volume_id: str | None = None,
+                           credentials: AWSCredentials | None = None) -> S3ServiceResource:
         """
         Gets an AWS resource. If the volume has no credentials, it uses the boto3 library to try and find them. This
         method is not designed to be overridden.
 
         :param request: the HTTP request (required).
         :param service_name: AWS service name (required).
         :param volume_id: the id string of a volume (required).
@@ -134,15 +140,17 @@
         was provided, the return value will be the "default" Mongo client for the microservice found in the HEA_DB
         application-level property.
         :raise ValueError: if there is no volume with the provided volume id, the volume's file system does not exist,
         the volume's credentials were not found, or a necessary service is not registered.
 
         TODO: need to lock around resource creation because it's not threadsafe, manifested by sporadic KeyError: 'endpoint_resolver'.
         """
-        return await self.__get_resource_or_client(request, service_name, volume_id, create_resource)
+        if credentials is None:
+            credentials = await self.get_credentials_from_volume(request, volume_id)
+        return await self.__get_resource_or_client(request, service_name, create_resource, credentials)
 
     async def has_account(self, request: Request, volume_id: str) -> bool:
         """
         Return whether the current user can access the AWS accounts associated with the provided volume_id.
 
         :param request: the HTTP request object (required).
         :param volume_id: the volume id (required).
@@ -154,16 +162,15 @@
         """
         Gets the current user's AWS account associated with the provided volume_id.
 
         :param request: the HTTP request object (required).
         :param volume_id: the volume id (required).
         :return: the AWS account, or None if not found.
         """
-        async with STSClientContext(request, volume_id) as sts_client:
-            return await S3._get_account(request, volume_id)
+        return await self._get_account(request, volume_id)
 
     async def get_accounts(self, request: Request, volume_ids: Sequence[str]) -> AsyncGenerator[
         tuple[AWSAccount, str], None]:
         """
         Gets the AWS accounts associated with the provided volume ids.
 
         :param request: the HTTP request object (required).
@@ -224,83 +231,86 @@
         account.name = aid
         account.display_name = aid
         account.owner = AWS_USER
         account.source = AWS_SOURCE
         account.source_detail = AWS_SOURCE
         return account
 
-    @staticmethod
-    async def _get_account(request: Request, volume_id: str) -> AWSAccount:
+    async def _get_account(self, request: Request, volume_id: str) -> AWSAccount:
         logger = logging.getLogger(__name__)
         loop = asyncio.get_running_loop()
-        async with STSClientContext(request, volume_id) as sts_client:
+        credentials = await self.get_credentials_from_volume(request, volume_id)
+        logger.debug('Got credentials %s for volume %s', credentials, volume_id)
+
+        async with STSClientContext(request, credentials=credentials) as sts_client:
             account = await S3._get_basic_account_info(sts_client)
             aid = account.id
 
-        try:
-            async with AccountClientContext(request, volume_id) as account_client:
-                contact_info = await loop.run_in_executor(None, partial(account_client.get_contact_information, AccountId=aid))
-                account.full_name = contact_info.get('FullName')
-                account.phone_number = contact_info.get('PhoneNumber')
-        except ClientError as e:
-            code = e.response['Error']['Code']
-            if code != 'AccessDeniedException':
-                logger.exception('Client error %s', code)
-                raise e
-            logger.debug('Account %s is not authorized to access contact information', aid, exc_info=True)
-
-        try:
-            async with OrganizationsClientContext(request, volume_id) as org_client:
-                account_info = await loop.run_in_executor(None, partial(org_client.describe_account, AccountId=aid))
-                account_info_ = account_info['Account']
-                account.name = account_info_.get('Name')
-                account.email_address = account_info_.get('Email')
-        except ParamValidationError:
-            logger.debug('Account %s is not part of an organization', aid, exc_info=True)
-        except ClientError as e:
-            code = e.response['Error']['Code']
-            if code != 'AccessDeniedException':
-                logger.exception('Client error %s', code)
-                raise e
-            logger.debug('Account %s is not authorized to access organization-level account information',
-                        aid, exc_info=True)
+        async def populate_contact_info():
+            try:
+                async with AccountClientContext(request, credentials=credentials) as account_client:
+                    contact_info = await loop.run_in_executor(None, partial(account_client.get_contact_information, AccountId=aid))
+                    account.full_name = contact_info.get('FullName')
+                    account.phone_number = contact_info.get('PhoneNumber')
+            except ClientError as e:
+                code = e.response['Error']['Code']
+                if code != 'AccessDeniedException':
+                    logger.exception('Client error %s', code)
+                    raise e
+                logger.debug('Account %s is not authorized to access contact information', aid, exc_info=True)
+
+        async def populate_organization_info():
+            try:
+                async with OrganizationsClientContext(request, credentials=credentials) as org_client:
+                    account_info = await loop.run_in_executor(None, partial(org_client.describe_account, AccountId=aid))
+                    account_info_ = account_info['Account']
+                    account.name = account_info_.get('Name')
+                    account.email_address = account_info_.get('Email')
+            except ParamValidationError:
+                logger.debug('Account %s is not part of an organization', aid, exc_info=True)
+            except ClientError as e:
+                code = e.response['Error']['Code']
+                if code != 'AccessDeniedException':
+                    logger.exception('Client error %s', code)
+                    raise e
+                logger.debug('Account %s is not authorized to access organization-level account information',
+                            aid, exc_info=True)
+
+        await asyncio.gather(populate_contact_info(), populate_organization_info())
 
         # account.created = user['CreateDate']
         # FIXME this info coming from Alternate Contact(below) gets 'permission denied' with IAMUser even with admin level access
         # not sure if only root account user can access. This is useful info need to investigate different strategy
         # alt_contact_resp = account_client.get_alternate_contact(AccountId=account.id, AlternateContactType='BILLING' )
         # alt_contact =  alt_contact_resp.get("AlternateContact ", None)
         # if alt_contact:
         # account.full_name = alt_contact.get("Name", None)
 
         return account
 
-    async def __get_resource_or_client(self, request: Request, service_name: str, volume_id: str,
+    async def __get_resource_or_client(self, request: Request, service_name: str,
                                        creator: Callable[[str, str | None, str | None, str | None,
-                                                          str | None], _S3Service]) -> _S3Service:
+                                                          str | None], _S3Service],
+                                       credentials: AWSCredentials | None) -> _S3Service:
         logger = logging.getLogger(__name__)
-        if volume_id is not None:
-            credentials = await self.get_credentials_from_volume(request, volume_id)
-            logger.debug("credentials retrieved from database checking if expired: %r", credentials)
-            loop = asyncio.get_running_loop()
-            if not credentials:  # delegate to boto3 to find the credentials
-                return await loop.run_in_executor(None, creator, service_name)
-            elif credentials.temporary:
-                return await self.__get_temporary_credentials(request=request,
-                                                              credentials=credentials,
-                                                              creator=creator,
-                                                              service_name=service_name)
-            else:  # for permanent credentials
-                return await loop.run_in_executor(None, partial(creator, service_name,
-                                                                region_name=credentials.where,
-                                                                aws_access_key_id=credentials.account,
-                                                                aws_secret_access_key=credentials.password))
+        logger.debug("credentials retrieved from database checking if expired: %r", credentials)
+        loop = asyncio.get_running_loop()
+        if not credentials:  # delegate to boto3 to find the credentials
+            return await loop.run_in_executor(None, creator, service_name)
+        elif credentials.temporary:
+            return await self.__get_temporary_credentials(request=request,
+                                                            credentials=credentials,
+                                                            creator=creator,
+                                                            service_name=service_name)
+        else:  # for permanent credentials
+            return await loop.run_in_executor(None, partial(creator, service_name,
+                                                            region_name=credentials.where,
+                                                            aws_access_key_id=credentials.account,
+                                                            aws_secret_access_key=credentials.password))
 
-        else:
-            raise ValueError('volume_id is required')
 
     async def __get_temporary_credentials(self, request: web.Request, credentials: AWSCredentials,
                                           creator: Callable[
                                               [str, str | None, str | None, str | None, str | None], _S3Service],
                                           service_name: str) -> Any:
         """
             Gets temporary credentials and returns the authorized client. In order to do that it
@@ -364,55 +374,55 @@
 
 
 class S3ClientContext(DatabaseContextManager[S3Client]):  # Go into db package?
     """
     Provides an S3 client.
     """
 
-    def __init__(self, request: web.Request, volume_id: str):
-        super().__init__(request, volume_id)
+    def __init__(self, request: web.Request, volume_id: str | None = None, credentials: AWSCredentials | None = None):
+        super().__init__(request, volume_id, credentials)
 
     async def connection(self) -> S3Client:
-        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 's3', self.volume_id)
+        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 's3', self.volume_id, self.credentials)
 
 
 class STSClientContext(DatabaseContextManager[STSClient]):  # Go into db package?
     """
     Provides an STS client.
     """
 
-    def __init__(self, request: web.Request, volume_id: str):
-        super().__init__(request, volume_id)
+    def __init__(self, request: web.Request, volume_id: str | None = None, credentials: AWSCredentials | None = None):
+        super().__init__(request, volume_id, credentials)
 
     async def connection(self) -> STSClient:
-        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 'sts', self.volume_id)
+        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 'sts', self.volume_id, self.credentials)
 
 
 class AccountClientContext(DatabaseContextManager[AccountClient]):
     """
     Provides an Account client.
     """
 
-    def __init__(self, request: web.Request, volume_id: str):
-        super().__init__(request, volume_id)
+    def __init__(self, request: web.Request, volume_id: str | None = None, credentials: AWSCredentials | None = None):
+        super().__init__(request, volume_id, credentials)
 
     async def connection(self) -> AccountClient:
-        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 'account', self.volume_id)
+        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 'account', self.volume_id, self.credentials)
 
 
 class OrganizationsClientContext(DatabaseContextManager[OrganizationsClient]):
     """
     Provides an Organizations client.
     """
 
-    def __init__(self, request: web.Request, volume_id: str):
-        super().__init__(request, volume_id)
+    def __init__(self, request: web.Request, volume_id: str | None = None, credentials: AWSCredentials | None = None):
+        super().__init__(request, volume_id, credentials)
 
     async def connection(self) -> OrganizationsClient:
-        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 'organizations', self.volume_id)
+        return await cast(S3, self.request.app[HEA_DB]).get_client(self.request, 'organizations', self.volume_id, self.credentials)
 
 
 @overload
 def create_client(service_name: Literal['s3'],
                   region_name: str | None = None,
                   aws_access_key_id: str | None = None,
                   aws_secret_access_key: str | None = None,
```

### Comparing `heaserver-1.2.0/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.3.0/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/db/database.py` & `heaserver-1.3.0/src/heaserver/service/db/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -637,21 +637,33 @@
             self.delete_desktop_objects()
         finally:
             self.delete_content()
 
 DatabaseClient = TypeVar('DatabaseClient')
 
 class DatabaseContextManager(AbstractAsyncContextManager[DatabaseClient], ABC):
-    def __init__(self, request: Request, volume_id: str | None = None) -> None:
+    """
+    Abstract base class for creating context managers for HEA database connections.
+    """
+
+    def __init__(self, request: Request, volume_id: str | None = None, credentials: CredentialTypeVar | None = None) -> None:
+        """
+        Create the context manager.
+
+        :param request: the HTTP request (required).
+        :param volume_id: optional volume id. You must either provide a volume id or a credentials object.
+        :param credentials: optional credentials object. You must either provide a volume id or a credentials object.
+        """
         if request is None:
             raise ValueError('Request cannot be None')
         if not isinstance(request, Request):
             raise ValueError(f'request {request} must be a Request')
         self.__request = request
         self.__volume_id = str(volume_id) if volume_id is not None else None
+        self.__credentials = deepcopy(credentials) if credentials is not None else None;
 
     async def __aenter__(self) -> DatabaseClient:
         return await self.connection()
 
     async def __aexit__(self, exc_type: type[BaseException] | None,
                         exc_value: BaseException | None,
                         traceback: TracebackType | None) -> Any:
@@ -666,14 +678,18 @@
     def request(self) -> Request:
         return self.__request
 
     @property
     def volume_id(self) -> str:
         return self.__volume_id
 
+    @property
+    def credentials(self) -> CredentialTypeVar:
+        return self.__credentials
+
 
 class NoDatabaseManager(MicroserviceDatabaseManager):
     def get_database(self) -> Database:
         return NoDatabase()
 
     @classmethod
     def database_types(self) -> list[str]:
```

### Comparing `heaserver-1.2.0/src/heaserver/service/db/dbapi2.py` & `heaserver-1.3.0/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/db/mongo.py` & `heaserver-1.3.0/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.3.0/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.3.0/src/heaserver/service/db/mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/expression.py` & `heaserver-1.3.0/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/functional.py` & `heaserver-1.3.0/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.3.0/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/jsonschema.py` & `heaserver-1.3.0/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.3.0/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.3.0/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.3.0/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.3.0/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.3.0/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/messagebroker.py` & `heaserver-1.3.0/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/mimetypes.py` & `heaserver-1.3.0/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.3.0/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/openapi.py` & `heaserver-1.3.0/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/__init__.py` & `heaserver-1.3.0/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/cj.py` & `heaserver-1.3.0/src/heaserver/service/representor/cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/factory.py` & `heaserver-1.3.0/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.3.0/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/representor.py` & `heaserver-1.3.0/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/wstljson.py` & `heaserver-1.3.0/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.3.0/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/response.py` & `heaserver-1.3.0/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/runner.py` & `heaserver-1.3.0/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.3.0/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.3.0/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.3.0/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/collection.py` & `heaserver-1.3.0/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/docker.py` & `heaserver-1.3.0/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.3.0/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.3.0/src/heaserver/service/testcase/expectedvalues.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.3.0/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/mixin.py` & `heaserver-1.3.0/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.3.0/src/heaserver/service/testcase/mockaws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.3.0/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.3.0/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.3.0/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.3.0/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/testenv.py` & `heaserver-1.3.0/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/testcase/util.py` & `heaserver-1.3.0/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/uritemplate.py` & `heaserver-1.3.0/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/util.py` & `heaserver-1.3.0/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver/service/wstl.py` & `heaserver-1.3.0/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.3.0/src/heaserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.2.0
+Version: 1.3.0
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,19 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.3.0
+* Performance improvement getting accounts.
+* heaserver.service.db.database.DatabaseContextManagers now allow initializing with either a volume id or a Credentials
+object.
+
 ## Version 1.2.0
 * get_volumes() in the database module and Database class can now filter by account ids.
 * New heaobject dependency: new heaobject.root.AbstractAssociation base class and heaobject.account.AccountAssociation
 implementation, and heaobject.organization.Organization class now has an accounts attribute using AccountAssociation.
 
 ## Version 1.1.3
 * Fixed permissions setting in mongoservicelib.aggregate().
```

### Comparing `heaserver-1.2.0/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.3.0/src/heaserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.3.0/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.3.0/tests/heaserver/servicetest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.3.0/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.3.0/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.3.0/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.3.0/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.3.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/service.py` & `heaserver-1.3.0/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_client.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_response.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_util.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.3.0/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.2.0/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.3.0/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

