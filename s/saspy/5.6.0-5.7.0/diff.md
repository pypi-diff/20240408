# Comparing `tmp/saspy-5.6.0.tar.gz` & `tmp/saspy-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.6.0.tar", last modified: Mon Feb  5 19:02:47 2024, max compression
+gzip compressed data, was "saspy-5.7.0.tar", last modified: Tue Mar 19 14:58:34 2024, max compression
```

## Comparing `saspy-5.6.0.tar` & `saspy-5.7.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.534331 saspy-5.6.0/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2024-02-05 19:02:27.000000 saspy-5.6.0/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2024-02-05 19:02:27.000000 saspy-5.6.0/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-02-05 19:02:47.533331 saspy-5.6.0/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2024-02-05 19:02:27.000000 saspy-5.6.0/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2024-02-05 19:02:27.000000 saspy-5.6.0/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.495329 saspy-5.6.0/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.497329 saspy-5.6.0/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.513330 saspy-5.6.0/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.519330 saspy-5.6.0/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.531331 saspy-5.6.0/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   136264 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10965 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     3905 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    35993 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87598 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    88106 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   101414 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.531331 saspy-5.6.0/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2024-02-05 19:02:27.000000 saspy-5.6.0/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-02-05 19:02:47.532331 saspy-5.6.0/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-02-05 19:02:47.000000 saspy-5.6.0/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2024-02-05 19:02:47.000000 saspy-5.6.0/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2024-02-05 19:02:47.000000 saspy-5.6.0/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2024-02-05 19:02:47.000000 saspy-5.6.0/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2024-02-05 19:02:47.000000 saspy-5.6.0/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2024-02-05 19:02:47.534331 saspy-5.6.0/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2024-02-05 19:02:27.000000 saspy-5.6.0/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.058898 saspy-5.7.0/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2024-03-19 14:58:21.000000 saspy-5.7.0/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2024-03-19 14:58:21.000000 saspy-5.7.0/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-03-19 14:58:34.057898 saspy-5.7.0/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2024-03-19 14:58:21.000000 saspy-5.7.0/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2024-03-19 14:58:21.000000 saspy-5.7.0/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.033897 saspy-5.7.0/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.035897 saspy-5.7.0/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.045898 saspy-5.7.0/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.050898 saspy-5.7.0/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1095 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/cancel.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1332 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/cancel.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18884 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    34685 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    15824 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.056898 saspy-5.7.0/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   136277 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10965 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3905 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    35993 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    88492 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    89012 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   101414 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.056898 saspy-5.7.0/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.056898 saspy-5.7.0/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1451 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2024-03-19 14:58:34.058898 saspy-5.7.0/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2024-03-19 14:58:21.000000 saspy-5.7.0/setup.py
```

### Comparing `saspy-5.6.0/LICENSE.md` & `saspy-5.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/PKG-INFO` & `saspy-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.6.0
+Version: 5.7.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.6.0/README.md` & `saspy-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/SASLogLexer.py` & `saspy-5.7.0/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/__init__.py` & `saspy-5.7.0/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/autocfg.py` & `saspy-5.7.0/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.7.0/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.7.0/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.7.0/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.7.0/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/sas.core.jar` & `saspy-5.7.0/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.7.0/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.7.0/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/pyiom/saspy2j.java` & `saspy-5.7.0/saspy/java/pyiom/saspy2j.java`

 * *Files 4% similar despite different names*

```diff
@@ -89,33 +89,35 @@
    static IDataService        datasvc = null;
    static IBinaryStream       bstr    = null;
    static BridgeServer        server  = null;
 
    static Socket   sin      = null;
    static Socket   sout     = null;
    static Socket   serr     = null;
+   static Socket   scan     = null;
    static String   appName  = "";
    static String   iomhost  = "";
    static int      iomport  = 0;
    static String   omruser  = "";
    static String   omrpw    = "";
    static String   ad       = "";
    static String   physname = "";
    static int      hosts    = 0;
    static String[] iomhosts;
    static int      lrecl    = 32767;
    static int      logsz    = 32767;
-
+   static Thread   t1; 
 
    public static void main(String[] args) throws
                        InterruptedException, IOException, ConnectionFactoryException, GenericError
       {
       int inport  = 0;
       int outport = 0;
       int errport = 0;
+      int canport = 0;
       int len     = 0;
       int blen    = 0;
       int slen    = 0;
       int idx     = 0;
       int nargs   = args.length;
       long flen   = 0;
 
@@ -131,24 +133,28 @@
       boolean ods    = false;
       boolean undo   = false;
 
       OctetSeqHolder odsdata = new OctetSeqHolder();
       char[]         in      = new char[4097];
       byte[]         out     = new byte[32768];
 
+      Runnable cancel = new cancel(scan, lang);
+      
       for (int x = 0; x < nargs; x++)
          {
          if (args[x].equalsIgnoreCase("-host"))
             addr = args[x + 1];
          else if (args[x].equalsIgnoreCase("-stdinport"))
             inport = Integer.parseInt(args[x + 1]);
          else if (args[x].equalsIgnoreCase("-stdoutport"))
             outport = Integer.parseInt(args[x + 1]);
          else if (args[x].equalsIgnoreCase("-stderrport"))
             errport = Integer.parseInt(args[x + 1]);
+         else if (args[x].equalsIgnoreCase("-cancelport"))
+            canport = Integer.parseInt(args[x + 1]);
          else if (args[x].equalsIgnoreCase("-iomhost"))
             iomhost = args[x + 1];
          else if (args[x].equalsIgnoreCase("-iomport"))
             iomport = Integer.parseInt(args[x + 1]);
          else if (args[x].equalsIgnoreCase("-timeout"))
             timeout = Integer.parseInt(args[x + 1]) * 1000;
          else if (args[x].equalsIgnoreCase("-user"))
@@ -171,14 +177,15 @@
       hosts    = iomhosts.length;
 
       try
          {
          sin  = new Socket(addr, inport);
          sout = new Socket(addr, outport);
          serr = new Socket(addr, errport);
+         scan = new Socket(addr, canport);
          }
       catch (IOException e)
          {
          e.printStackTrace();
          }
 
       OutputStream odsout = sout.getOutputStream();
@@ -218,14 +225,19 @@
       else
          {
          if (! spn && uriStr == null)
             omrpw = inp.readLine();
          connect(false, false, false);
          }
 
+      cancel = new cancel(scan, lang);
+      t1 = new Thread(cancel);
+      t1.setName("cancel");
+      t1.start();
+      
       while (true)
          {
          try
             {
             pgm = new String();
             while (true)
                {
@@ -270,14 +282,19 @@
                                  }
                               }
                            catch (Exception e)
                               {
                               String msg = "We failed in Submit\n"+e.getMessage();
                               errp.write(msg);
                               errp.flush();
+                              sin.close();
+                              sout.close();
+                              serr.close();
+                              scan.close();
+                              t1.join();
                               System.out.print(msg);
                               e.printStackTrace();
                               throw new IOException();
                               }
                            }
                         bstr.Close();
                         }
@@ -323,14 +340,19 @@
                                  }
                               }
                            catch (Exception e)
                               {
                               String msg = "We failed in Submit\n"+e.getMessage();
                               errp.write(msg);
                               errp.flush();
+                              sin.close();
+                              sout.close();
+                              serr.close();
+                              scan.close();
+                              t1.join();
                               System.out.print(msg);
                               e.printStackTrace();
                               throw new IOException();
                               }
                            }
                         bstr.Close();
                         }
@@ -359,14 +381,19 @@
                            pgm = pgm.substring(idx + 13 + 33);
                            }
                         else
                            {
                            String msg = "We failed in Submit\n"+e.getMessage();
                            errp.write(msg);
                            errp.flush();
+                           sin.close();
+                           sout.close();
+                           serr.close();
+                           scan.close();
+                           t1.join();
                            System.out.print(msg);
                            e.printStackTrace();
                            throw new IOException();
                            }
                         }
                      pgm = pgm.substring(idx + 13 + 33);
                      }
@@ -428,31 +455,38 @@
                               }
                            catch(ConnectionFactoryException e2)
                               {
                               String msg = "We failed reconnecting in ENDSAS. WUWT?\n"+e2.getMessage();
                               System.out.print(msg+"\n");
                               errp.write(msg+"\n");
                               errp.flush();
+                              sin.close();
+                              sout.close();
+                              serr.close();
+                              scan.close();
+                              t1.join();
                               e2.printStackTrace();
                               }
                            }
                         }
 
                      cx.close();
                      sin.close();
                      sout.close();
                      serr.close();
+                     scan.close();
+                     t1.join();
                      return;
                      }
                   else if (eol.contains("PRINTTO"))
                      {
                      undo = true;
                      pgm  = pgm.substring(idx + 13 + 33);
                      }
-                  else
+                  else  /* SUBMIT */
                      {
                      pgm = pgm.substring(0, idx);
                      try
                         {
                         lang.Submit(pgm);
                         if (undo)
                            lang.Submit("\nproc printto;run;\n%put "+eol.substring(1)+";\n");
@@ -464,15 +498,14 @@
                      catch (org.omg.CORBA.DATA_CONVERSION e)
                         {
                         String msg = "We failed in Submit\n"+e.getMessage();
                         errp.write(msg);
                         errp.flush();
                         System.out.print(msg);
                         e.printStackTrace();
-                        //throw new IOException();
                         }
                      catch(org.omg.CORBA.COMM_FAILURE e)
                         {
                         if (reconnect)
                            {
                            connect(true, false, false);
                            lang.Submit(pgm);
@@ -484,19 +517,38 @@
                            break;
                            }
                         else
                            {
                            String msg = "We failed in Submit\n"+e.getMessage();
                            errp.write(msg);
                            errp.flush();
+                           sin.close();
+                           sout.close();
+                           serr.close();
+                           scan.close();
+                           t1.join();
                            System.out.print(msg);
                            e.printStackTrace();
                            throw new IOException();
                            }
                         }
+                     catch(org.omg.CORBA.OBJECT_NOT_EXIST e)
+                        {
+                        String msg = "We failed in Submit\n"+e.getMessage();
+                        errp.write(msg);
+                        errp.flush();
+                        sin.close();
+                        sout.close();
+                        serr.close();
+                        scan.close();
+                        t1.join();
+                        System.out.print(msg);
+                        e.printStackTrace();
+                        throw new IOException();
+                        }
                      }
                   }
                else
                   {
                   len = inp.read(in, 0, 4096);
                   if (len > 0)
                      pgm += String.valueOf(Arrays.copyOfRange(in, 0, len));
@@ -546,14 +598,19 @@
                         bstr.Read(blen, odsdata);
                         }
                      else
                         {
                         String msg = "We failed in Submit\n"+e.getMessage();
                         errp.write(msg);
                         errp.flush();
+                        sin.close();
+                        sout.close();
+                        serr.close();
+                        scan.close();
+                        t1.join();
                         System.out.print(msg);
                         e.printStackTrace();
                         throw new IOException();
                         }
                      }
                   }
                bstr.Close();
@@ -590,113 +647,129 @@
                      if (reconnect)
                         connect(true, false, false);
                      else
                         {
                         String msg = "We failed in reading the List\n"+e.getMessage();
                         errp.write(msg);
                         errp.flush();
+                        sin.close();
+                        sout.close();
+                        serr.close();
+                        scan.close();
+                        t1.join();
                         System.out.print(msg);
                         e.printStackTrace();
                         throw new IOException();
                         }
                      }
                   catch (IOException e)
                      {
                      String msg = "We failed in reading the List\n"+e.getMessage();
                      errp.write(msg);
                      errp.flush();
                      System.out.print(msg);
                      sin.close();
                      sout.close();
                      serr.close();
+                     scan.close();
+                     t1.join();
                      e.printStackTrace();
                      break;
                      }
                   }
 
-                  if (fndeol)
-                     break;
+               if (fndeol)
+                  break;
 
-                  slen = 1;
-                  while (slen > 0)
+               slen = 1;
+               while (slen > 0)
+                  {
+                  try
                      {
-                     try
+                     log  = lang.FlushLog(logsz);
+                     slen = log.length();
+                     if (slen > 0)
                         {
-                        log  = lang.FlushLog(logsz);
-                        slen = log.length();
-                        if (slen > 0)
-                           {
-                           errp.write(log);
-                           errp.flush();
+                        errp.write(log);
+                        errp.flush();
 
-                           if ((plog+log).contains(eol))
+                        if ((plog+log).contains(eol))
+                           {
+                           outp.write(eol);
+                           if (ods)
                               {
-                              outp.write(eol);
-                              if (ods)
-                                 {
-                                 outp.write(fn);
-                                 ods = false;
-                                 }
-                              outp.flush();
-                              fndeol = true;
+                              outp.write(fn);
+                              ods = false;
                               }
-                           plog = log;
-                           }
-                        }
-                     catch (org.omg.CORBA.COMM_FAILURE e)
-                        {
-                        if (reconnect)
-                           connect(true, false, false);
-                        else
-                           {
-                           String msg = "We failed in reading the Log\n"+e.getMessage();
-                           errp.write(msg);
-                           errp.flush();
-                           System.out.print(msg);
-                           e.printStackTrace();
-                           throw new IOException();
+                           outp.flush();
+                           fndeol = true;
                            }
+                        plog = log;
                         }
-                     catch (IOException e)
+                     }
+                  catch (org.omg.CORBA.COMM_FAILURE e)
+                     {
+                     if (reconnect)
+                        connect(true, false, false);
+                     else
                         {
                         String msg = "We failed in reading the Log\n"+e.getMessage();
                         errp.write(msg);
                         errp.flush();
-                        System.out.print(msg);
                         sin.close();
                         sout.close();
                         serr.close();
+                        scan.close();
+                        t1.join();
+                        System.out.print(msg);
                         e.printStackTrace();
-                        break;
-                        }
-                     catch (org.omg.CORBA.DATA_CONVERSION e)
-                        {
-                        String msg = "We failed in reading the Log\n"+e.getMessage();
-                        errp.write(msg);
-                        errp.flush();
-                        lang.Submit("%put "+eol.substring(1)+";\n");
-                        slen = 1;
-                        continue;
+                        throw new IOException();
                         }
                      }
+                  catch (IOException e)
+                     {
+                     String msg = "We failed in reading the Log\n"+e.getMessage();
+                     errp.write(msg);
+                     errp.flush();
+                     System.out.print(msg);
+                     sin.close();
+                     sout.close();
+                     serr.close();
+                     scan.close();
+                     t1.join();
+                     e.printStackTrace();
+                     break;
+                     }
+                  catch (org.omg.CORBA.DATA_CONVERSION e)
+                     {
+                     String msg = "We failed in reading the Log\n"+e.getMessage();
+                     errp.write(msg);
+                     errp.flush();
+                     lang.Submit("%put "+eol.substring(1)+";\n");
+                     slen = 1;
+                     continue;
+                     }
                   }
                }
-          catch (GenericError e)
-             {
-             String msg = "We failed in outer loop\n"+e.getMessage();
-             errp.write(msg);
-             errp.flush();
-             System.out.print(msg);
-             sin.close();
-             sout.close();
-             serr.close();
-             e.printStackTrace();
-             break;
-             }
-          }
+            }
+         catch (GenericError e)
+            {
+            String msg = "We failed in outer loop\n"+e.getMessage();
+            errp.write(msg);
+            errp.flush();
+            System.out.print(msg);
+            sin.close();
+            sout.close();
+            serr.close();
+            scan.close();
+            t1.join();
+            e.printStackTrace();
+            break;
+            }
+         }
       }
 
 private static void connect(boolean recon, boolean ods, boolean zero) throws IOException, ConnectionFactoryException, GenericError
    {
     boolean                       failed             = false;
     boolean[]                     fieldInclusionMask = new boolean[0];
     StringHolder                  retname            = new StringHolder();
```

### Comparing `saspy-5.6.0/saspy/java/thirdparty/NOTICE.md` & `saspy-5.7.0/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.7.0/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.7.0/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/libname_gen.sas` & `saspy-5.7.0/saspy/libname_gen.sas`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasViyaML.py` & `saspy-5.7.0/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sas_magic.py` & `saspy-5.7.0/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasbase.py` & `saspy-5.7.0/saspy/sasbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -932,15 +932,15 @@
 
         if results == '':
             if self.results.upper() == 'PANDAS':
                 results = 'HTML'
             else:
                 results = self.results
 
-        ll = self._io.submit(code, results, prompt, undo=printto, **kwargs)
+        ll = self._io.submit(code, results, prompt, undo=printto, cancel=True, **kwargs)
 
         if self.sascfg.colorLOG:
            clog = highlight(ll['LOG'], SASLogLexer(), HtmlFormatter(full=True, style=SASLogStyle, lineseparator="<br>"))
            ll['LOG'] = clog
 
         return ll
```

### Comparing `saspy-5.6.0/saspy/sascfg.py` & `saspy-5.7.0/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasdata.py` & `saspy-5.7.0/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasdecorator.py` & `saspy-5.7.0/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasets.py` & `saspy-5.7.0/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasexceptions.py` & `saspy-5.7.0/saspy/sasexceptions.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasiocom.py` & `saspy-5.7.0/saspy/sasiocom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasiohttp.py` & `saspy-5.7.0/saspy/sasiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,14 +1071,15 @@
       NOTE: to view HTML results in the ipykernel, issue: from IPython.display import HTML  and use HTML() instead of print()
       i.e,: results = sas.submit("data a; x=1; run; proc print;run')
             print(results['LOG'])
             HTML(results['LST'])
       '''
       prompt  = prompt if prompt is not None else {}
       printto = kwargs.pop('undo', False)
+      cancel  = kwargs.pop('cancel', False)
 
       odsopen  = json.dumps("ods listing close;ods "+self.sascfg.output+" (id=saspy_internal) options(bitmap_mode='inline') device=svg style="+self._sb.HTML_Style+"; ods graphics on / outputfmt=png;\n")
       odsclose = json.dumps("ods "+self.sascfg.output+" (id=saspy_internal) close;ods listing;\n")
       ods      = True;
 
       if self._session == None:
          #return dict(LOG="No SAS process attached. SAS process has terminated unexpectedly.", LST='')
@@ -1131,19 +1132,26 @@
          jobid = json.loads(resp.decode(self.sascfg.encoding))
       except:
          raise SASHTTPsubmissionError(msg="Problem parsing response from Compute Service.\n   Status="+str(status)+"\n   Response="+str(resp))
 
       if not jobid or status > 299:
          raise SASHTTPsubmissionError(msg="Problem submitting job to Compute Service.\n   Status code="+str(jobid.get('httpStatusCode'))+"\n   Message="+jobid.get('message'))
 
+      uri = None
+      can = None
       for ld in jobid.get('links'):
          if ld.get('method') == 'GET' and ld.get('rel') == 'state':
             uri = ld.get('uri')
+         if ld.get('method') == 'PUT' and ld.get('rel') == 'cancel':
+            can = ld.get('uri')
+         if uri and can:
             break
 
+      Etag = req.getheader("Etag")
+
       conn    = self.sascfg.HTTPConn;
       headers = {"Accept":"text/plain", "Authorization":"Bearer "+self.sascfg._token}
       done    = False
 
       delay   = kwargs.get('GETstatusDelay'  , 0)
       excpcnt = kwargs.get('GETstatusFailcnt', 5)
 
@@ -1151,31 +1159,47 @@
          try:
             while True:
                # GET Status for JOB
                conn.connect()
                conn.request('GET', uri, headers=headers)
                req = conn.getresponse()
                resp = req.read()
+               Etag = req.getheader("Etag")
                conn.close()
                if resp not in [b'running', b'pending']:
                   done = True
                   break
                sleep(delay)
 
          except (KeyboardInterrupt, SystemExit):
             conn.close()
             print('Exception caught!')
-            response = self.sascfg._prompt(
-                      "SAS attention handling not yet supported over HTTP. Please enter (Q) to Quit waiting for results or (C) to continue waiting.")
+            if cancel:
+               msg = "Please enter (C) to Cancel submitted code or (Q) to Quit waiting for results or (W) continue to Wait."
+            else:
+               msg = "CANCEL is only supported for the submit*() methods. Please enter (Q) to Quit waiting for results or (W) to continue to Wait."
+
+            response = self.sascfg._prompt(msg)
+
             while True:
+               if cancel and response is None or response.upper() == 'C':
+                  # GET Status for JOB
+                  canheaders = {"Accept":"text/plain", "Authorization":"Bearer "+self.sascfg._token, "If-Match":Etag}
+                  conn.connect()
+                  conn.request('PUT', can, headers=canheaders)
+                  req = conn.getresponse()
+                  resp = req.read()
+                  conn.close()
+                  print('Canceled submitted statements\n')
+                  break
                if response is None or response.upper() == 'Q':
-                  return dict(LOG='', LST='', BC=True)
-               if response.upper() == 'C':
+                  return dict(LOG='', LST='')
+               if response.upper() == 'W':
                   break
-               response = self.sascfg._prompt("Please enter (Q) to Quit waiting for results or (C) to continue waiting.")
+               response = self.sascfg._prompt(msg)
 
          except hc.RemoteDisconnected as Dis:
             conn.close()
             print('RemoteDisconnected Exception caught!\n'+str(Dis))
             excpcnt -= 1
             if excpcnt < 0:
                raise
```

### Comparing `saspy-5.6.0/saspy/sasioiom.py` & `saspy-5.7.0/saspy/sasioiom.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,20 +332,26 @@
          self.sockout = socks.socket()
          self.sockout.bind(("127.0.0.1",port))
          #self.sockout.bind(("",32702))
 
          self.sockerr = socks.socket()
          self.sockerr.bind(("127.0.0.1",port))
          #self.sockerr.bind(("",32703))
+
+         self.sockcan = socks.socket()
+         self.sockcan.bind(("127.0.0.1",port))
+         #self.sockcan.bind(("",32704))
+
       except OSError:
          logger.fatal('Error try to open a socket in the _startsas method. Call failed.')
          return None
       self.sockin.listen(1)
       self.sockout.listen(1)
       self.sockerr.listen(1)
+      self.sockcan.listen(1)
 
       if not zero:
          if self.sascfg.output.lower() == 'html':
             logger.warning("""HTML4 is only valid in 'local' mode (SAS_output_options in sascfg_personal.py).
 Please see SAS_config_names templates 'default' (STDIO) or 'winlocal' (IOM) in the sample sascfg.py.
 Will use HTML5 for this SASsession.""")
             self.sascfg.output = 'html5'
@@ -393,14 +399,15 @@
          parms += self.sascfg.javaparms
       parms += ["-classpath",  self.sascfg.classpath, "pyiom.saspy2j", "-host", "localhost"]
       #parms += ["-classpath", self.sascfg.classpath+":/u/sastpw/tkpy2j", "pyiom.saspy2j_sleep", "-host", "tomspc"]
       #parms += ["-classpath", self.sascfg.classpath+";U:\\tkpy2j", "pyiom.saspy2j_sleep", "-host", "tomspc"]
       parms += ["-stdinport",  str(self.sockin.getsockname()[1])]
       parms += ["-stdoutport", str(self.sockout.getsockname()[1])]
       parms += ["-stderrport", str(self.sockerr.getsockname()[1])]
+      parms += ["-cancelport", str(self.sockcan.getsockname()[1])]
       if self.sascfg.timeout is not None:
          parms += ["-timeout", str(self.sascfg.timeout)]
       if self.sascfg.appserver:
          parms += ["-appname", "'"+self.sascfg.appserver+"'"]
       if not zero:
          parms += ["-iomhost", self.sascfg.iomhost, "-iomport", str(self.sascfg.iomport)]
          if not self.sascfg.sspi:
@@ -546,14 +553,16 @@
                   else:
                      os.kill(self.pid, signal.SIGKILL)
                   self.pid = None
                   raise RuntimeError("No SAS OMR User password provided.")
             pw += '\n'
             self.stdin[0].send(pw.encode())
 
+      self.stdcan = self.sockcan.accept()
+
       enc = self.sascfg.encoding #validating encoding is done next, so handle it not being set for this one call
       if enc == '':
          self.sascfg.encoding = 'utf-8'
       ll = self.submit("options svgtitle='svgtitle'; options validvarname=any validmemname=extend pagesize=max nosyntaxcheck; ods graphics on;", "text")
       self.sascfg.encoding = enc
 
       if self.pid is None:
@@ -575,14 +584,22 @@
       rc = 0
       if self.pid:
          if os.name == 'nt':
             pid = self.pid.pid
          else:
             pid = self.pid
 
+         try: # Mac OS Python has bugs with this call
+            self.stdcan[0].send(b'C')
+            self.stdcan[0].shutdown(socks.SHUT_RDWR)
+         except:
+            pass
+         self.stdcan[0].close()
+         self.sockcan.close()
+
          try: # More Mac OS Python issues that don't work like everywhere else
             self.stdin[0].send(b'\ntom says EOL=ENDSAS                          \n')
             if os.name == 'nt':
                self._javalog  = self.pid.stderr.read(4096).decode()+'\n'
                self._javalog += self.pid.stdout.read(4096).decode()
                self.pid.stdin.close()
                self.pid.stdout.close()
@@ -790,14 +807,15 @@
       # what it generates. If the two are not of the same type (html, text) it could be problematic, beyond not being what was
       # expected in the first place. __flushlst__() used to be used, but was never needed. Adding this note and removing the
       # unnecessary read in submit as this can't happen in the current code.
 
       odsopen  = b"ods listing close;ods "+self.sascfg.output.encode()+ \
                  b" (id=saspy_internal) file="+self._tomods1+b" options(bitmap_mode='inline') device=svg style="+self._sb.HTML_Style.encode()+ \
                  b"; ods graphics on / outputfmt=png;\n"
+
       odsclose = b"ods "+self.sascfg.output.encode()+b" (id=saspy_internal) close;ods listing;\n"
       ods      = True
       pgm      = b""
 
       if results.upper() != "HTML":
          ods = False
 
@@ -836,14 +854,15 @@
       NOTE: to view HTML results in the ipykernel, issue: from IPython.display import HTML  and use HTML() instead of print()
       i.e,: results = sas.submit("data a; x=1; run; proc print;run')
             print(results['LOG'])
             HTML(results['LST'])
       '''
       prompt  = prompt if prompt is not None else {}
       printto = kwargs.pop('undo', False)
+      cancel  = kwargs.pop('cancel', False)
 
       #odsopen  = b"ods listing close;ods html5 (id=saspy_internal) file=STDOUT options(bitmap_mode='inline') device=svg; ods graphics on / outputfmt=png;\n"
       odsopen  = b"ods listing close;ods "+self.sascfg.output.encode()+ \
                  b" (id=saspy_internal) file="+self._tomods1+b" options(bitmap_mode='inline') device=svg style="+self._sb.HTML_Style.encode()+ \
                  b"; ods graphics on / outputfmt=png;\n"
       odsclose = b"ods "+self.sascfg.output.encode()+b" (id=saspy_internal) close;ods listing;\n"
       ods      = True;
@@ -1008,30 +1027,29 @@
              log =logf.partition(logcodeo)[0]+b'\nConnection Reset: SAS process has terminated unexpectedly. Pid State= '+str(rc).encode()
              #return dict(LOG=log.decode(errors='replace'), LST='')
              logger.fatal(log.decode(errors='replace'))
              raise SASIOConnectionTerminated(Exception)
 
          except (KeyboardInterrupt, SystemExit):
              print('Exception caught!')
-             ll = self._breakprompt(logcodeo)
+             ll = self._breakprompt(logcodeo, cancel)
 
              if ll.get('ABORT', False):
                 return ll
 
              logf += ll['LOG']
              lstf += ll['LST']
              bc    = ll['BC']
 
              if not bc:
-                print('Exception handled :)\n')
+                print('Canceled submitted statements\n')
+                self.stdin[0].send(odsclose+logcodei.encode()+b'tom says EOL='+logcodeo+b'\n')
              else:
                 print('Exception ignored, continuing to process...\n')
 
-             #self.stdin[0].send(odsclose+logcodei.encode()+b'tom says EOL='+logcodeo+b'\n')
-
       try:
          lstf = lstf.decode()
       except UnicodeDecodeError:
          try:
             lstf = lstf.decode(self.sascfg.encoding)
          except UnicodeDecodeError:
             lstf = lstf.decode(errors='replace')
@@ -1055,47 +1073,56 @@
       if logd.count('\nERROR:') > 0:
          warnings.warn("Noticed 'ERROR:' in LOG, you ought to take a look and see if there was a problem")
          self._sb.check_error_log = True
 
       self._sb._lastlog = logd
       return dict(LOG=logd, LST=lstd)
 
-   def _breakprompt(self, eos):
+   def _breakprompt(self, eos, cancel):
         found = False
         logf  = b''
         lstf  = b''
         bc    = False
 
         if self.pid is None:
             self._sb.SASpid = None
             return dict(LOG=b"No SAS process attached. SAS process has terminated unexpectedly.", LST=b'', ABORT=True)
 
         if True:
-           response = self.sascfg._prompt(
-                     "SAS attention handling is not yet supported over IOM. Please enter (T) to terminate SAS or (C) to continue.")
+           if cancel:
+              msg = "Please enter (T) to Terminate SAS or (C) to Cancel submitted code or (W) continue to Wait."
+           else:
+              msg = "CANCEL is only supported for the submit*() methods. Please enter (T) to Terminate SAS or (W) to continue to Wait."
+
+           response = self.sascfg._prompt(msg)
            while True:
-              if response is None or response.upper() == 'C':
+              if cancel and response is None or response.upper() == 'C':
+                 self.stdcan[0].send(b'C')
+                 return dict(LOG=b'', LST=b'', BC=False)
+              if response is None or response.upper() == 'W':
                  return dict(LOG=b'', LST=b'', BC=True)
               if response.upper() == 'T':
                  break
-              response = self.sascfg._prompt("Please enter (T) to terminate SAS or (C) to continue.")
+              response = self.sascfg._prompt(msg)
 
+        self._endsas()
+
+        '''
         if os.name == 'nt':
            self.pid.kill()
         else:
            interrupt = signal.SIGINT
            os.kill(self.pid, interrupt)
            sleep(.25)
 
         self.pid = None
         self._sb.SASpid = None
-        return dict(LOG=b"SAS process terminated", LST=b'', ABORT=True)
-
-
+        '''
 
+        return dict(LOG="SAS process terminated", LST='', ABORT=True)
 
         """
         while True:
             rc = os.waitid(os.P_PID, self.pid, os.WEXITED | os.WNOHANG)
             if rc is not None:
                 self.pid = None
                 self._sb.SASpid = None
```

### Comparing `saspy-5.6.0/saspy/sasiostdio.py` & `saspy-5.7.0/saspy/sasiostdio.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasml.py` & `saspy-5.7.0/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasproccommons.py` & `saspy-5.7.0/saspy/sasproccommons.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasqc.py` & `saspy-5.7.0/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasresults.py` & `saspy-5.7.0/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasstat.py` & `saspy-5.7.0/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sastabulate.py` & `saspy-5.7.0/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/sasutil.py` & `saspy-5.7.0/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy/scripts/run_sas.py` & `saspy-5.7.0/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.6.0/saspy.egg-info/PKG-INFO` & `saspy-5.7.0/saspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.6.0
+Version: 5.7.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.6.0/saspy.egg-info/SOURCES.txt` & `saspy-5.7.0/saspy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 saspy/java/iomclient/log4j-api-2.12.4.jar
 saspy/java/iomclient/log4j-api-2.17.1.jar
 saspy/java/iomclient/log4j-core-2.12.4.jar
 saspy/java/iomclient/log4j-core-2.17.1.jar
 saspy/java/iomclient/sas.core.jar
 saspy/java/iomclient/sas.security.sspi.jar
 saspy/java/iomclient/sas.svc.connection.jar
+saspy/java/pyiom/cancel.class
+saspy/java/pyiom/cancel.java
 saspy/java/pyiom/saspy2j.class
 saspy/java/pyiom/saspy2j.java
 saspy/java/thirdparty/NOTICE.md
 saspy/java/thirdparty/glassfish-corba-internal-api.jar
 saspy/java/thirdparty/glassfish-corba-omgapi.jar
 saspy/java/thirdparty/glassfish-corba-orb.jar
 saspy/java/thirdparty/pfl-basic.jar
```

### Comparing `saspy-5.6.0/setup.py` & `saspy-5.7.0/setup.py`

 * *Files identical despite different names*

