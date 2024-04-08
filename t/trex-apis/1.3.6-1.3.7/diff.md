# Comparing `tmp/trex-apis-1.3.6.tar.gz` & `tmp/trex-apis-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.3.6.tar", last modified: Thu Apr  4 11:19:36 2024, max compression
+gzip compressed data, was "trex-apis-1.3.7.tar", last modified: Mon Apr  8 01:21:06 2024, max compression
```

## Comparing `trex-apis-1.3.6.tar` & `trex-apis-1.3.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.933993 trex-apis-1.3.6/
--rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-04 11:19:36.933871 trex-apis-1.3.6/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.3.6/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-04 11:19:36.934613 trex-apis-1.3.6/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2024-04-04 11:19:22.000000 trex-apis-1.3.6/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.933346 trex-apis-1.3.6/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1628 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.897688 trex-apis-1.3.6/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.3.6/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1269 2024-04-03 14:24:11.000000 trex-apis-1.3.6/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.920644 trex-apis-1.3.6/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.3.6/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.3.6/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7080 2023-12-04 14:21:25.000000 trex-apis-1.3.6/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    44555 2023-12-13 09:05:54.000000 trex-apis-1.3.6/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.3.6/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.3.6/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14912 2024-01-26 08:21:50.000000 trex-apis-1.3.6/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14268 2024-02-05 07:27:46.000000 trex-apis-1.3.6/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22414 2024-02-07 06:33:19.000000 trex-apis-1.3.6/trexapi/controllers/merchant_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7436 2024-01-30 09:36:58.000000 trex-apis-1.3.6/trexapi/controllers/message_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.3.6/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.3.6/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.3.6/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.3.6/trexapi/controllers/prepaid_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.3.6/trexapi/controllers/rating_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10501 2024-02-05 02:35:34.000000 trex-apis-1.3.6/trexapi/controllers/redemption_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27474 2024-01-29 10:13:52.000000 trex-apis-1.3.6/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-01-25 03:26:42.000000 trex-apis-1.3.6/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.3.6/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    84469 2024-04-04 07:59:04.000000 trex-apis-1.3.6/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.3.6/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16728 2024-01-19 03:44:19.000000 trex-apis-1.3.6/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.922490 trex-apis-1.3.6/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.3.6/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.3.6/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.925890 trex-apis-1.3.6/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.3.6/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7539 2023-12-13 05:36:24.000000 trex-apis-1.3.6/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.3.6/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.3.6/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.3.6/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.927009 trex-apis-1.3.6/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.3.6/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.3.6/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.931432 trex-apis-1.3.6/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.3.6/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2983 2024-01-03 03:38:30.000000 trex-apis-1.3.6/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.3.6/trexapi/utils/push_notification_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9242 2024-03-14 09:07:57.000000 trex-apis-1.3.6/trexapi/utils/redemption_catalogue_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)    79248 2024-01-29 13:58:07.000000 trex-apis-1.3.6/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.930520 trex-apis-1.3.7/
+-rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-08 01:21:06.930145 trex-apis-1.3.7/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.3.7/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-08 01:21:06.931379 trex-apis-1.3.7/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2024-04-08 01:20:51.000000 trex-apis-1.3.7/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.929495 trex-apis-1.3.7/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-08 01:21:06.000000 trex-apis-1.3.7/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1628 2024-04-08 01:21:06.000000 trex-apis-1.3.7/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-08 01:21:06.000000 trex-apis-1.3.7/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2024-04-08 01:21:06.000000 trex-apis-1.3.7/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-04-08 01:21:06.000000 trex-apis-1.3.7/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.892934 trex-apis-1.3.7/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.3.7/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1372 2024-04-05 03:13:41.000000 trex-apis-1.3.7/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.916463 trex-apis-1.3.7/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.3.7/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.3.7/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7080 2023-12-04 14:21:25.000000 trex-apis-1.3.7/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    44555 2023-12-13 09:05:54.000000 trex-apis-1.3.7/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.3.7/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.3.7/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14912 2024-01-26 08:21:50.000000 trex-apis-1.3.7/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14268 2024-02-05 07:27:46.000000 trex-apis-1.3.7/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22414 2024-02-07 06:33:19.000000 trex-apis-1.3.7/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7436 2024-01-30 09:36:58.000000 trex-apis-1.3.7/trexapi/controllers/message_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.3.7/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.3.7/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.3.7/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.3.7/trexapi/controllers/prepaid_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.3.7/trexapi/controllers/rating_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10501 2024-02-05 02:35:34.000000 trex-apis-1.3.7/trexapi/controllers/redemption_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27474 2024-01-29 10:13:52.000000 trex-apis-1.3.7/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-01-25 03:26:42.000000 trex-apis-1.3.7/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.3.7/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    87318 2024-04-05 05:35:22.000000 trex-apis-1.3.7/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.3.7/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16728 2024-01-19 03:44:19.000000 trex-apis-1.3.7/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.918079 trex-apis-1.3.7/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.3.7/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.3.7/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.921896 trex-apis-1.3.7/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.3.7/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7539 2023-12-13 05:36:24.000000 trex-apis-1.3.7/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.3.7/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.3.7/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.3.7/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.923098 trex-apis-1.3.7/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.3.7/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.3.7/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 01:21:06.927396 trex-apis-1.3.7/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.3.7/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2983 2024-01-03 03:38:30.000000 trex-apis-1.3.7/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.3.7/trexapi/utils/push_notification_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9242 2024-03-14 09:07:57.000000 trex-apis-1.3.7/trexapi/utils/redemption_catalogue_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    79248 2024-01-29 13:58:07.000000 trex-apis-1.3.7/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.3.6/setup.py` & `trex-apis-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.3.6',
+     version='1.3.7',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.3.6/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.3.7/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/conf.py` & `trex-apis-1.3.7/trexapi/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,7 +18,9 @@
 EARN_INSTANT_REWARD_URL                                         = os.environ.get('EARN_INSTANT_REWARD_URL')
 
 LUCKY_DRAW_URL                                                  = os.environ.get('LUCKY_DRAW_URL')
 
 FIREBASE_SERVICE_ACCOUNT_KEY_PATH                               = os.environ.get('FIREBASE_SERVICE_ACCOUNT_KEY_PATH')
 
 USE_VERIFICATION_REQUEST_ID                                     = os.environ.get('USE_VERIFICATION_REQUEST_ID')
+
+SEND_REAL_MESSAGE                                               = os.environ.get('SEND_REAL_MESSAGE')
```

### Comparing `trex-apis-1.3.6/trexapi/controllers/api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/app_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/merchant_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/merchant_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/message_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/message_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/prepaid_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/prepaid_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/rating_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/rating_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/redemption_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/redemption_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/user_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/user_api_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from trexmodel.models.datastore.user_models import User
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from werkzeug.datastructures import ImmutableMultiDict
 from trexapi.forms.user_api_forms import UserRegistrationForm, UserUpdateForm,\
     OutletReviewsForm
 from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL, MOBILE_APP_NAME,\
-    USE_VERIFICATION_REQUEST_ID
+    USE_VERIFICATION_REQUEST_ID, SEND_REAL_MESSAGE
 from trexmail.email_helper import trigger_send_email
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher,\
     CustomerPointReward, CustomerEntitledTierRewardSummary
 from trexapi.utils.api_helpers import generate_user_auth_token
 from trexapi.decorators.api_decorators import user_auth_token_required,\
@@ -36,14 +36,15 @@
 import os
 from trexlib.utils.sms_util import send_sms
 from trexmodel.models.datastore.message_models import Message
 from time import strftime
 from trexlib.utils.common.date_util import from_utc_datetime_to_local_datetime
 from trexmodel.conf import USER_STATUS_REGISTERED, GENDER_UNKNOWN_CODE
 from trexmodel.models.datastore.model_decorators import model_transactional
+from trexlib.libs.facebook.util.whatsapp_util import send_whatsapp_verification_message
 
 user_api_bp = Blueprint('user_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/users')
 
 logger = logging.getLogger('api')
@@ -1185,15 +1186,14 @@
 
     logger.debug('mobile_phone=%s', mobile_phone)
     logger.debug('send_method=%s', send_method)
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(mobile_phone):
         db_client                           = create_db_client(caller_info="reset_mobile_phone_verification_code")
-        user_acct                           = None
         
         with db_client.context():
             user_by_mobile_phone    = User.get_by_mobile_phone(mobile_phone)
         
             logger.debug('user_by_mobile_phone=%s', user_by_mobile_phone)
         
         if user_by_mobile_phone is not None:
@@ -1209,21 +1209,28 @@
                 logger.debug('reset_mobile_phone_verification_code: USE_VERIFICATION_REQUEST_ID=%s', USE_VERIFICATION_REQUEST_ID)   
                 
                 if boolify(USE_VERIFICATION_REQUEST_ID):
                     mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
                 else:
                     mobile_phone_vc_prefix = ''
                 
-                send_mobile_phone_verification_code_sms(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix)
-                
-                return create_rest_message(status_code=StatusCode.OK, 
-                                           expiry_datetime      = user_by_mobile_phone.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
-                                           code                 = user_by_mobile_phone.mobile_phone_vc,
-                                           prefix               = mobile_phone_vc_prefix,
-                                           )
+                try:
+                    send_mobile_phone_verification_code(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix, send_method=send_method)
+                    
+                    return create_rest_message(status_code=StatusCode.OK, 
+                                               expiry_datetime      = user_by_mobile_phone.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                               code                 = user_by_mobile_phone.mobile_phone_vc,
+                                               prefix               = mobile_phone_vc_prefix,
+                                               )
+                except:
+                    return create_rest_message(
+                                                'Could not send verification code at the moment',
+                                                status_code=StatusCode.BAD_REQUEST,
+                                               
+                                               )
             else:
                 return create_rest_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
         else:
             with db_client.context():
                 user_acct    = User.get_by_reference_code(reference_code)
             
             if user_acct is not None:
@@ -1235,22 +1242,30 @@
                 else:
                     mobile_phone_vc_prefix = ''
                 
                 logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', user_acct.mobile_phone_vc_expiry_datetime)
                 logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_acct.mobile_phone_vc)    
                 logger.debug('reset_mobile_phone_verification_code: USE_VERIFICATION_REQUEST_ID=%s', USE_VERIFICATION_REQUEST_ID)
                 
-                send_mobile_phone_verification_code_sms(mobile_phone, user_acct.mobile_phone_vc, mobile_phone_vc_prefix)
-                
-                return create_rest_message(status_code=StatusCode.OK, 
-                                           expiry_datetime      = user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
-                                           code                 = user_acct.mobile_phone_vc,
-                                           prefix               = mobile_phone_vc_prefix,
-                                           
-                                           )
+                try:
+                    send_mobile_phone_verification_code(mobile_phone, user_acct.mobile_phone_vc, mobile_phone_vc_prefix, send_method=send_method)
+                    
+                    return create_rest_message(status_code=StatusCode.OK, 
+                                               expiry_datetime      = user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                               code                 = user_acct.mobile_phone_vc,
+                                               prefix               = mobile_phone_vc_prefix,
+                                               
+                                               )
+                except:
+                    return create_rest_message(
+                                                'Could not send verification code at the moment',
+                                                status_code=StatusCode.BAD_REQUEST,
+                                               
+                                               )
+                    
             else:
                 return create_rest_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
                 
                 
     else:
         logger.warn('reset_mobile_phone_verification_code: mobile phone is invalid')
         return create_rest_message(gettext('Missing mobile phone'), status_code=StatusCode.BAD_REQUEST)  
@@ -1390,15 +1405,22 @@
             logger.debug('request_reset_password_via_mobile_phone_post debug: verification code=%s', user_by_mobile_phone.mobile_phone_vc)   
             
             if boolify(USE_VERIFICATION_REQUEST_ID):
                 mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
             else:
                 mobile_phone_vc_prefix = ''
             
-            send_mobile_phone_verification_code_sms(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix)
+            try:
+                send_mobile_phone_verification_code(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix, send_method=send_method)
+            except:
+                    return create_rest_message(
+                                                'Could not send verification code at the moment',
+                                                status_code=StatusCode.BAD_REQUEST,
+                                               
+                                               )
             
             with db_client.context():
                 reset_password_token = '%s-%s' % (mobile_phone_vc_prefix, user_by_mobile_phone.mobile_phone_vc)
                 logger.debug('request_reset_password_via_mobile_phone_post debug: reset_password_token=%s', reset_password_token)
                 user_by_mobile_phone.set_reset_password_token(reset_password_token)
             
             return create_rest_message(status_code=StatusCode.OK, 
@@ -1509,20 +1531,49 @@
     
     subject      = 'Email Verification from {mobile_app_name}'.format(mobile_app_name=MOBILE_APP_NAME)
     
     logger.info('DEPLOYMENT_MODE=%s', DEPLOYMENT_MODE)
     
     logger.info(message)
     
-    if DEPLOYMENT_MODE==PRODUCTION_MODE:
+    if boolify(SEND_REAL_MESSAGE):
         trigger_send_email(recipient_address = email, subject=subject, message=message)
     else:
         logger.debug('not send email for development or local mode')
         
+
+def send_mobile_phone_verification_code(mobile_phone, verification_code, request_id, send_method='sms'):
+    logger.info('SEND_REAL_MESSAGE=%s', SEND_REAL_MESSAGE)
+    
+    if send_method=='sms':
+        if is_not_empty(request_id):
+            message = '{mobile_app_name} {request_id}-{verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
+                           request_id = request_id, 
+                           expiry_in_minute=os.environ.get('MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE'))
+        else:
+            message = '{mobile_app_name} {verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
+                           expiry_in_minute=os.environ.get('MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE'))
+        
+        logger.info('sms message: %s', message)
+        
+        if boolify(SEND_REAL_MESSAGE):
+            logger.info('Going to send sms to %s', mobile_phone)
+            send_sms(to_number=mobile_phone, body=message)
+        
+            
+    elif send_method == 'whatsapp':
+        
+        logger.info('whatsapp verification_code: %s', verification_code)
+        
+        if boolify(SEND_REAL_MESSAGE):
+            logger.info('Going to send whatsapp to %s', mobile_phone)
+            send_whatsapp_verification_message(mobile_phone, verification_code)
         
+        
+'''        
 def send_mobile_phone_verification_code_sms(mobile_phone, verification_code, request_id):
     if is_not_empty(request_id):
         message = '{mobile_app_name} {request_id}-{verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
                        request_id = request_id, 
                        expiry_in_minute=os.environ.get('MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE'))
     else:
         message = '{mobile_app_name} {verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
@@ -1533,15 +1584,15 @@
     logger.info('sms message: %s', message)
     
     if DEPLOYMENT_MODE in (PRODUCTION_MODE, DEMO_MODE):
         logger.info('Going to send sms to %s', mobile_phone)
         send_sms(to_number=mobile_phone, body=message)
     else:
         logger.debug('not send sms for development or local mode')
-
+'''
     
 def send_reset_password_request_email(user_acct):
     reset_password_link = '{base_url}/user/reset-password-request/{request_reset_password_token}'.format(base_url=APPLICATION_BASE_URL, request_reset_password_token=user_acct.request_reset_password_token)
     
     message = '''
                 Dear {name},
```

### Comparing `trex-apis-1.3.6/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.3.7/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/decorators/api_decorators.py` & `trex-apis-1.3.7/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/forms/customer_api_forms.py` & `trex-apis-1.3.7/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/forms/reward_api_forms.py` & `trex-apis-1.3.7/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/forms/sales_api_forms.py` & `trex-apis-1.3.7/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/forms/user_api_forms.py` & `trex-apis-1.3.7/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.3.7/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/utils/api_helpers.py` & `trex-apis-1.3.7/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/utils/redemption_catalogue_helper.py` & `trex-apis-1.3.7/trexapi/utils/redemption_catalogue_helper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.6/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.3.7/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

