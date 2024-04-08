# Comparing `tmp/tap-linkedin-ads-2.1.0.tar.gz` & `tmp/tap-linkedin-ads-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-linkedin-ads-2.1.0.tar", last modified: Tue Apr 11 13:58:33 2023, max compression
+gzip compressed data, was "tap-linkedin-ads-2.2.0.tar", last modified: Mon Apr  8 17:48:54 2024, max compression
```

## Comparing `tap-linkedin-ads-2.1.0.tar` & `tap-linkedin-ads-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.141007 tap-linkedin-ads-2.1.0/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    34523 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/LICENSE
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      339 2023-04-11 13:58:33.141007 tap-linkedin-ads-2.1.0/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    16976 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/README.md
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       38 2023-04-11 13:58:33.141007 tap-linkedin-ads-2.1.0/setup.cfg
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      840 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/setup.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.137007 tap-linkedin-ads-2.1.0/tap_linkedin_ads/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1620 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    14809 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/client.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      612 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/discover.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2706 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schema.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.137007 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1696 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/account_users.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3471 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/accounts.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    13824 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    13791 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2989 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaign_groups.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12277 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaigns.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2192 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/creatives.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1989 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/video_ads.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    31980 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/streams.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     5605 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/sync.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12355 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/transform.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.137007 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      339 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      822 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        1 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       84 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/entry_points.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       73 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/requires.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       17 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-02-03 11:59:41.000000 tap-linkedin-ads-2.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16976 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2024-04-08 17:45:26.000000 tap-linkedin-ads-2.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.443050 tap-linkedin-ads-2.2.0/tap_linkedin_ads/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-04-08 17:01:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14809 2024-04-08 17:39:42.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      612 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-11-06 17:25:42.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/account_users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3471 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13824 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13791 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2989 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaign_groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12277 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/creatives.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/video_ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31980 2024-04-08 17:15:30.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5605 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12355 2023-02-03 11:59:41.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/transform.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.443050 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      822 2024-04-08 17:48:54.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/top_level.txt
```

### Comparing `tap-linkedin-ads-2.1.0/LICENSE` & `tap-linkedin-ads-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/README.md` & `tap-linkedin-ads-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/setup.py` & `tap-linkedin-ads-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-linkedin-ads',
-      version='2.1.0',
+      version='2.2.0',
       description='Singer.io tap for extracting data from the LinkedIn Marketing Ads API API 2.0',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_linkedin_ads'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/__init__.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/client.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from singer import metrics
 import singer
 
 LOGGER = singer.get_logger()
 BASE_URL = 'https://api.linkedin.com/rest'
 LINKEDIN_TOKEN_URI = 'https://www.linkedin.com/oauth/v2/accessToken'
 INTROSPECTION_URI = 'https://www.linkedin.com/oauth/v2/introspectToken'
-LINKEDIN_VERSION = '202302'
+LINKEDIN_VERSION = '202304'
 
 # set default timeout of 300 seconds
 REQUEST_TIMEOUT = 300
 
 class LinkedInError(Exception):
     pass
```

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/discover.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schema.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schema.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/account_users.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/accounts.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaign_groups.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaigns.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/creatives.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/video_ads.json` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/video_ads.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/streams.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/streams.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/sync.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/sync.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads/transform.py` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads/transform.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/SOURCES.txt` & `tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

