# Comparing `tmp/amazon-ads-api-connector-0.1.3.tar.gz` & `tmp/amazon-ads-api-connector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-ads-api-connector-0.1.3.tar", last modified: Sat Mar  9 23:00:44 2024, max compression
+gzip compressed data, was "amazon-ads-api-connector-0.1.4.tar", last modified: Mon Apr  8 11:52:03 2024, max compression
```

## Comparing `amazon-ads-api-connector-0.1.3.tar` & `amazon-ads-api-connector-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-03-09 23:00:44.722962 amazon-ads-api-connector-0.1.3/
--rw-r--r--   0 muw        (501) staff       (20)     1080 2023-10-16 20:58:50.000000 amazon-ads-api-connector-0.1.3/LICENSE.txt 
--rw-r--r--   0 muw        (501) staff       (20)     4609 2024-03-09 23:00:44.722712 amazon-ads-api-connector-0.1.3/PKG-INFO
--rw-r--r--   0 muw        (501) staff       (20)     4351 2024-03-07 21:45:38.000000 amazon-ads-api-connector-0.1.3/README.md
-drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-03-09 23:00:44.721281 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector/
--rw-r--r--   0 muw        (501) staff       (20)      225 2024-03-08 21:13:55.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector/__init__.py
--rw-r--r--   0 muw        (501) staff       (20)    32588 2024-03-09 22:58:57.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector/amazon_ads_api_connector.py
--rw-r--r--   0 muw        (501) staff       (20)    13422 2024-03-08 21:11:14.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector/report_types.py
-drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-03-09 23:00:44.722333 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/
--rw-r--r--   0 muw        (501) staff       (20)     4609 2024-03-09 23:00:44.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/PKG-INFO
--rw-r--r--   0 muw        (501) staff       (20)      401 2024-03-09 23:00:44.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/SOURCES.txt
--rw-r--r--   0 muw        (501) staff       (20)        1 2024-03-09 23:00:44.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/dependency_links.txt
--rw-r--r--   0 muw        (501) staff       (20)       24 2024-03-09 23:00:44.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/requires.txt
--rw-r--r--   0 muw        (501) staff       (20)       25 2024-03-09 23:00:44.000000 amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/top_level.txt
--rw-r--r--   0 muw        (501) staff       (20)       38 2024-03-09 23:00:44.723014 amazon-ads-api-connector-0.1.3/setup.cfg
--rw-r--r--   0 muw        (501) staff       (20)      448 2024-03-09 23:00:27.000000 amazon-ads-api-connector-0.1.3/setup.py
+drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-04-08 11:52:03.972426 amazon-ads-api-connector-0.1.4/
+-rw-r--r--   0 muw        (501) staff       (20)     1080 2024-03-09 23:03:48.000000 amazon-ads-api-connector-0.1.4/LICENSE.txt 
+-rw-r--r--   0 muw        (501) staff       (20)     5325 2024-04-08 11:52:03.972188 amazon-ads-api-connector-0.1.4/PKG-INFO
+-rw-r--r--   0 muw        (501) staff       (20)     5067 2024-04-08 11:18:54.000000 amazon-ads-api-connector-0.1.4/README.md
+drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-04-08 11:52:03.970371 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/
+-rw-r--r--   0 muw        (501) staff       (20)      225 2024-03-08 21:13:55.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/__init__.py
+-rw-r--r--   0 muw        (501) staff       (20)    32588 2024-03-11 20:49:48.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/amazon_ads_api_connector.py
+-rw-r--r--   0 muw        (501) staff       (20)    13422 2024-03-08 21:11:14.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/report_types.py
+drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-04-08 11:52:03.971725 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/
+-rw-r--r--   0 muw        (501) staff       (20)     5325 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/PKG-INFO
+-rw-r--r--   0 muw        (501) staff       (20)      401 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 muw        (501) staff       (20)        1 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 muw        (501) staff       (20)       24 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/requires.txt
+-rw-r--r--   0 muw        (501) staff       (20)       25 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/top_level.txt
+-rw-r--r--   0 muw        (501) staff       (20)       38 2024-04-08 11:52:03.972483 amazon-ads-api-connector-0.1.4/setup.cfg
+-rw-r--r--   0 muw        (501) staff       (20)      448 2024-04-08 11:51:49.000000 amazon-ads-api-connector-0.1.4/setup.py
```

### Comparing `amazon-ads-api-connector-0.1.3/LICENSE.txt ` & `amazon-ads-api-connector-0.1.4/LICENSE.txt `

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Markus U. Wahl
+Copyright (c) 2024 Markus U. Wahl
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `amazon-ads-api-connector-0.1.3/PKG-INFO` & `amazon-ads-api-connector-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: amazon-ads-api-connector
-Version: 0.1.3
-Summary: API wrapper for the Amazon Ads API
-Author: Markus U. Wahl
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt 
-Requires-Dist: requests
-Requires-Dist: types-requests
-
 # Amazon Ads API Connector
 
 A simple Python wrapper for the <a href="https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod">latest version of the Amazon Ads API for Sponsored Products campaign management</a>.
 
-This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product AISIN targeting. 
+This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product ASIN targeting and auto campaigns. 
 
 Please note that this module does not yet support Sponsored Brands and Sponsored Display campaigns.
 
 ## Installation
 
 Amazon Ads API Connector is available on PyPI:
 
@@ -28,17 +18,19 @@
 
 The primary class of the module is `AmazonAdsAPIConnector`. This class provides methods to create, list, update and delete 
 - campaigns, 
 - ad groups, 
 - product ads, 
 - keywords, 
 - negative keywords, and
-- targeting clauses (ASIN targeting). 
+- targeting clauses (ASIN targeting).
+
+It furthermore provides methods to get `keyword recommendations`, which include bid recommendations for keyword targets, as well as `bid recommendations for ad groups`, which include bid recommendations for auto campaigns.
 
-It furthermore provides methods to request and retrieve reports via the API.
+And lastly, it provides also methods to request and retrieve reports via the API.
 
 To create an instance of the `AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a dictionary. The dictionary must contain the following keys:
 
 - `refresh_token`
 - `client_id`
 - `client_secret`
 - `profile_id`
@@ -82,34 +74,40 @@
                 "budgetType": "DAILY",
                 "budget": 0,
             },
         },
     ]
 )
 ```
-Please note that all create and update methods expect a list of dictionaries as their only argument. This reflects the fact that the Amazon Ads API allows to create or update multiple objects at once. To ensure the greatest possible flexibility, the structure of the list and the dictionaries corresponds to the structure specified by the API and described in the API documentation.
+Please note that all create and update methods expect a list of dictionaries as their only argument. This reflects the fact that the Amazon Ads API allows to create or update multiple objects at once. To ensure the greatest possible flexibility, the structure of the list and the dictionaries corresponds to the structure specified by the API and described in the API documentation. For more information about the structure of the lists and dictionaries, as well for information on data limits per request, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod).
 
 ### Request and retrieve a report
 
-The module furthermore contains classes which represent basic configurations of the available report types:
+The module contains classes which represent basic configurations of the available report types:
 
 - `CampaignsReport`
 - `TargetingReport`
 - `SearchTermReport`
 - `AdvertisedProductReports`
 - `PurchasedProductReport`
 
-For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
+For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types).
+
+To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
 
 ```python
 from amazon_ads_api_connector import SearchTermReport
 
-report_configuration = SearchTermReport("2023-10-01", "2023-10-07")
+report_configuration = SearchTermReport("2023-10-01", ◊"2023-10-07")
 
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
 
-This module depends on the `requests` library, which is not included in the standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+This module depends on the `requests` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+
+## Disclaimer
+
+This module is not affiliated with Amazon in any way. It is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,58 +1,63 @@
-Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.3 Summary:
-API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
-Type: text/markdown License-File: LICENSE.txt Requires-Dist: requests Requires-
-Dist: types-requests # Amazon Ads API Connector A simple Python wrapper for the
-_l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n
-_m_a_n_a_g_e_m_e_n_t. This module covers the key endpoints for managing Sponsored
-Products campaigns. This includes methods for authentication, pagination and
-report generation. It features keyword and negative keyword targeting, as well
-as product AISIN targeting. Please note that this module does not yet support
+# Amazon Ads API Connector A simple Python wrapper for the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f
+_t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n_ _m_a_n_a_g_e_m_e_n_t. This module
+covers the key endpoints for managing Sponsored Products campaigns. This
+includes methods for authentication, pagination and report generation. It
+features keyword and negative keyword targeting, as well as product ASIN
+targeting and auto campaigns. Please note that this module does not yet support
 Sponsored Brands and Sponsored Display campaigns. ## Installation Amazon Ads
 API Connector is available on PyPI: ```bash pip install amazon-ads-api-
 connector ``` ## Getting started The primary class of the module is
 `AmazonAdsAPIConnector`. This class provides methods to create, list, update
 and delete - campaigns, - ad groups, - product ads, - keywords, - negative
 keywords, and - targeting clauses (ASIN targeting). It furthermore provides
-methods to request and retrieve reports via the API. To create an instance of
-the `AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials
-as a dictionary. The dictionary must contain the following keys: -
-`refresh_token` - `client_id` - `client_secret` - `profile_id` Upon
-initialization, the AmazonAdsAPIConnector object will create a new access
-token. This access token will be valid for 60 minutes, however, the object
-automatically requests a new access token in case it has expired when trying to
-make a new request. For more information about the Amazon Ads API, please visit
-the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-
-started/how-to-use-api). ## Examples ### Import the library ```python from
-amazon_ads_api_connector import AmazonAdsAPIConnector ``` ### Create an
-instance ```python api = AmazonAdsAPIConnector( { "refresh_token":
-"your_refresh_token", "client_id": "your_client_id", "client_secret":
-"your_client_secret", "profile_id": "your_profile_id", } ) ``` ### List
-campaigns ```python campaigns = api.list_campaigns() ``` ### Create campaigns
-```python api.create_campaign( campaigns=[ { "name": "My Campaign",
-"targetingType": "MANUAL", "state": "ENABLED", "dynamicBidding": { "strategy":
-"LEGACY_FOR_SALES", }, "bugdget": { "budgetType": "DAILY", "budget": 0, }, }, ]
-) ``` Please note that all create and update methods expect a list of
-dictionaries as their only argument. This reflects the fact that the Amazon Ads
-API allows to create or update multiple objects at once. To ensure the greatest
-possible flexibility, the structure of the list and the dictionaries
-corresponds to the structure specified by the API and described in the API
-documentation. ### Request and retrieve a report The module furthermore
-contains classes which represent basic configurations of the available report
-types: - `CampaignsReport` - `TargetingReport` - `SearchTermReport` -
-`AdvertisedProductReports` - `PurchasedProductReport` For more information
-about the report types, please visit the [official documentation](https://
-advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
-request a report you need to pass an instance of one of these classes to the
-`create_report` method of the `AmazonAdsAPIConnector` class. To customize the
-report, change the properties of the class instance before passing it to the
-`create_report` method. ```python from amazon_ads_api_connector import
-SearchTermReport report_configuration = SearchTermReport("2023-10-01", "2023-
-10-07") res = api.create_report(report_configuration) report = api.get_report
-(res) ``` Please note that report gerneration is asynchronous. The
-`create_report` method returns a dictionary containing the report ID. The
-`get_report` takes this dictionary as an argument and returns the report once
-it is completed and available. The completion of a report usually takes a few
-minutes and can take up to 3 hours. ## Dependencies This module depends on the
-`requests` library, which is not included in the standard library, but will be
-installed automatically when you install the `amazon-ads-api-connector`
-package.
+methods to get `keyword recommendations`, which include bid recommendations for
+keyword targets, as well as `bid recommendations for ad groups`, which include
+bid recommendations for auto campaigns. And lastly, it provides also methods to
+request and retrieve reports via the API. To create an instance of the
+`AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a
+dictionary. The dictionary must contain the following keys: - `refresh_token` -
+`client_id` - `client_secret` - `profile_id` Upon initialization, the
+AmazonAdsAPIConnector object will create a new access token. This access token
+will be valid for 60 minutes, however, the object automatically requests a new
+access token in case it has expired when trying to make a new request. For more
+information about the Amazon Ads API, please visit the [official documentation]
+(https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api). ##
+Examples ### Import the library ```python from amazon_ads_api_connector import
+AmazonAdsAPIConnector ``` ### Create an instance ```python api =
+AmazonAdsAPIConnector( { "refresh_token": "your_refresh_token", "client_id":
+"your_client_id", "client_secret": "your_client_secret", "profile_id":
+"your_profile_id", } ) ``` ### List campaigns ```python campaigns =
+api.list_campaigns() ``` ### Create campaigns ```python api.create_campaign
+( campaigns=[ { "name": "My Campaign", "targetingType": "MANUAL", "state":
+"ENABLED", "dynamicBidding": { "strategy": "LEGACY_FOR_SALES", }, "bugdget":
+{ "budgetType": "DAILY", "budget": 0, }, }, ] ) ``` Please note that all create
+and update methods expect a list of dictionaries as their only argument. This
+reflects the fact that the Amazon Ads API allows to create or update multiple
+objects at once. To ensure the greatest possible flexibility, the structure of
+the list and the dictionaries corresponds to the structure specified by the API
+and described in the API documentation. For more information about the
+structure of the lists and dictionaries, as well for information on data limits
+per request, please visit the [official documentation](https://
+advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod). ###
+Request and retrieve a report The module contains classes which represent basic
+configurations of the available report types: - `CampaignsReport` -
+`TargetingReport` - `SearchTermReport` - `AdvertisedProductReports` -
+`PurchasedProductReport` For more information about the report types, please
+visit the [official documentation](https://advertising.amazon.com/API/docs/en-
+us/guides/reporting/v3/report-types). To request a report you need to pass an
+instance of one of these classes to the `create_report` method of the
+`AmazonAdsAPIConnector` class. To customize the report, change the properties
+of the class instance before passing it to the `create_report` method.
+```python from amazon_ads_api_connector import SearchTermReport
+report_configuration = SearchTermReport("2023-10-01", â"2023-10-07") res =
+api.create_report(report_configuration) report = api.get_report(res) ``` Please
+note that report gerneration is asynchronous. The `create_report` method
+returns a dictionary containing the report ID. The `get_report` takes this
+dictionary as an argument and returns the report once it is completed and
+available. The completion of a report usually takes a few minutes and can take
+up to 3 hours. ## Dependencies This module depends on the `requests` library,
+which is not included in the Python standard library, but will be installed
+automatically when you install the `amazon-ads-api-connector` package. ##
+Disclaimer This module is not affiliated with Amazon in any way. It is an
+independent project that aims to provide a simple and easy-to-use interface to
+the Amazon Ads API for Sponsored Products campaign management.
```

### Comparing `amazon-ads-api-connector-0.1.3/README.md` & `amazon-ads-api-connector-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+Metadata-Version: 2.1
+Name: amazon-ads-api-connector
+Version: 0.1.4
+Summary: API wrapper for the Amazon Ads API
+Author: Markus U. Wahl
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt 
+Requires-Dist: requests
+Requires-Dist: types-requests
+
 # Amazon Ads API Connector
 
 A simple Python wrapper for the <a href="https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod">latest version of the Amazon Ads API for Sponsored Products campaign management</a>.
 
-This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product AISIN targeting. 
+This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product ASIN targeting and auto campaigns. 
 
 Please note that this module does not yet support Sponsored Brands and Sponsored Display campaigns.
 
 ## Installation
 
 Amazon Ads API Connector is available on PyPI:
 
@@ -18,17 +28,19 @@
 
 The primary class of the module is `AmazonAdsAPIConnector`. This class provides methods to create, list, update and delete 
 - campaigns, 
 - ad groups, 
 - product ads, 
 - keywords, 
 - negative keywords, and
-- targeting clauses (ASIN targeting). 
+- targeting clauses (ASIN targeting).
+
+It furthermore provides methods to get `keyword recommendations`, which include bid recommendations for keyword targets, as well as `bid recommendations for ad groups`, which include bid recommendations for auto campaigns.
 
-It furthermore provides methods to request and retrieve reports via the API.
+And lastly, it provides also methods to request and retrieve reports via the API.
 
 To create an instance of the `AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a dictionary. The dictionary must contain the following keys:
 
 - `refresh_token`
 - `client_id`
 - `client_secret`
 - `profile_id`
@@ -72,34 +84,40 @@
                 "budgetType": "DAILY",
                 "budget": 0,
             },
         },
     ]
 )
 ```
-Please note that all create and update methods expect a list of dictionaries as their only argument. This reflects the fact that the Amazon Ads API allows to create or update multiple objects at once. To ensure the greatest possible flexibility, the structure of the list and the dictionaries corresponds to the structure specified by the API and described in the API documentation.
+Please note that all create and update methods expect a list of dictionaries as their only argument. This reflects the fact that the Amazon Ads API allows to create or update multiple objects at once. To ensure the greatest possible flexibility, the structure of the list and the dictionaries corresponds to the structure specified by the API and described in the API documentation. For more information about the structure of the lists and dictionaries, as well for information on data limits per request, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod).
 
 ### Request and retrieve a report
 
-The module furthermore contains classes which represent basic configurations of the available report types:
+The module contains classes which represent basic configurations of the available report types:
 
 - `CampaignsReport`
 - `TargetingReport`
 - `SearchTermReport`
 - `AdvertisedProductReports`
 - `PurchasedProductReport`
 
-For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
+For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types).
+
+To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
 
 ```python
 from amazon_ads_api_connector import SearchTermReport
 
-report_configuration = SearchTermReport("2023-10-01", "2023-10-07")
+report_configuration = SearchTermReport("2023-10-01", ◊"2023-10-07")
 
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
 
-This module depends on the `requests` library, which is not included in the standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+This module depends on the `requests` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+
+## Disclaimer
+
+This module is not affiliated with Amazon in any way. It is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,54 +1,66 @@
-# Amazon Ads API Connector A simple Python wrapper for the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f
-_t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n_ _m_a_n_a_g_e_m_e_n_t. This module
-covers the key endpoints for managing Sponsored Products campaigns. This
-includes methods for authentication, pagination and report generation. It
-features keyword and negative keyword targeting, as well as product AISIN
-targeting. Please note that this module does not yet support Sponsored Brands
-and Sponsored Display campaigns. ## Installation Amazon Ads API Connector is
-available on PyPI: ```bash pip install amazon-ads-api-connector ``` ## Getting
-started The primary class of the module is `AmazonAdsAPIConnector`. This class
-provides methods to create, list, update and delete - campaigns, - ad groups, -
-product ads, - keywords, - negative keywords, and - targeting clauses (ASIN
-targeting). It furthermore provides methods to request and retrieve reports via
-the API. To create an instance of the `AmazonAdsAPIConnector`, you need to pass
-your Amazon Ads API credentials as a dictionary. The dictionary must contain
-the following keys: - `refresh_token` - `client_id` - `client_secret` -
-`profile_id` Upon initialization, the AmazonAdsAPIConnector object will create
-a new access token. This access token will be valid for 60 minutes, however,
-the object automatically requests a new access token in case it has expired
-when trying to make a new request. For more information about the Amazon Ads
-API, please visit the [official documentation](https://advertising.amazon.com/
-API/docs/en-us/get-started/how-to-use-api). ## Examples ### Import the library
-```python from amazon_ads_api_connector import AmazonAdsAPIConnector ``` ###
-Create an instance ```python api = AmazonAdsAPIConnector( { "refresh_token":
-"your_refresh_token", "client_id": "your_client_id", "client_secret":
-"your_client_secret", "profile_id": "your_profile_id", } ) ``` ### List
-campaigns ```python campaigns = api.list_campaigns() ``` ### Create campaigns
-```python api.create_campaign( campaigns=[ { "name": "My Campaign",
-"targetingType": "MANUAL", "state": "ENABLED", "dynamicBidding": { "strategy":
-"LEGACY_FOR_SALES", }, "bugdget": { "budgetType": "DAILY", "budget": 0, }, }, ]
-) ``` Please note that all create and update methods expect a list of
-dictionaries as their only argument. This reflects the fact that the Amazon Ads
-API allows to create or update multiple objects at once. To ensure the greatest
-possible flexibility, the structure of the list and the dictionaries
-corresponds to the structure specified by the API and described in the API
-documentation. ### Request and retrieve a report The module furthermore
-contains classes which represent basic configurations of the available report
-types: - `CampaignsReport` - `TargetingReport` - `SearchTermReport` -
-`AdvertisedProductReports` - `PurchasedProductReport` For more information
-about the report types, please visit the [official documentation](https://
-advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
-request a report you need to pass an instance of one of these classes to the
-`create_report` method of the `AmazonAdsAPIConnector` class. To customize the
-report, change the properties of the class instance before passing it to the
-`create_report` method. ```python from amazon_ads_api_connector import
-SearchTermReport report_configuration = SearchTermReport("2023-10-01", "2023-
-10-07") res = api.create_report(report_configuration) report = api.get_report
-(res) ``` Please note that report gerneration is asynchronous. The
-`create_report` method returns a dictionary containing the report ID. The
-`get_report` takes this dictionary as an argument and returns the report once
-it is completed and available. The completion of a report usually takes a few
-minutes and can take up to 3 hours. ## Dependencies This module depends on the
-`requests` library, which is not included in the standard library, but will be
-installed automatically when you install the `amazon-ads-api-connector`
-package.
+Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.4 Summary:
+API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
+Type: text/markdown License-File: LICENSE.txt Requires-Dist: requests Requires-
+Dist: types-requests # Amazon Ads API Connector A simple Python wrapper for the
+_l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n
+_m_a_n_a_g_e_m_e_n_t. This module covers the key endpoints for managing Sponsored
+Products campaigns. This includes methods for authentication, pagination and
+report generation. It features keyword and negative keyword targeting, as well
+as product ASIN targeting and auto campaigns. Please note that this module does
+not yet support Sponsored Brands and Sponsored Display campaigns. ##
+Installation Amazon Ads API Connector is available on PyPI: ```bash pip install
+amazon-ads-api-connector ``` ## Getting started The primary class of the module
+is `AmazonAdsAPIConnector`. This class provides methods to create, list, update
+and delete - campaigns, - ad groups, - product ads, - keywords, - negative
+keywords, and - targeting clauses (ASIN targeting). It furthermore provides
+methods to get `keyword recommendations`, which include bid recommendations for
+keyword targets, as well as `bid recommendations for ad groups`, which include
+bid recommendations for auto campaigns. And lastly, it provides also methods to
+request and retrieve reports via the API. To create an instance of the
+`AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a
+dictionary. The dictionary must contain the following keys: - `refresh_token` -
+`client_id` - `client_secret` - `profile_id` Upon initialization, the
+AmazonAdsAPIConnector object will create a new access token. This access token
+will be valid for 60 minutes, however, the object automatically requests a new
+access token in case it has expired when trying to make a new request. For more
+information about the Amazon Ads API, please visit the [official documentation]
+(https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api). ##
+Examples ### Import the library ```python from amazon_ads_api_connector import
+AmazonAdsAPIConnector ``` ### Create an instance ```python api =
+AmazonAdsAPIConnector( { "refresh_token": "your_refresh_token", "client_id":
+"your_client_id", "client_secret": "your_client_secret", "profile_id":
+"your_profile_id", } ) ``` ### List campaigns ```python campaigns =
+api.list_campaigns() ``` ### Create campaigns ```python api.create_campaign
+( campaigns=[ { "name": "My Campaign", "targetingType": "MANUAL", "state":
+"ENABLED", "dynamicBidding": { "strategy": "LEGACY_FOR_SALES", }, "bugdget":
+{ "budgetType": "DAILY", "budget": 0, }, }, ] ) ``` Please note that all create
+and update methods expect a list of dictionaries as their only argument. This
+reflects the fact that the Amazon Ads API allows to create or update multiple
+objects at once. To ensure the greatest possible flexibility, the structure of
+the list and the dictionaries corresponds to the structure specified by the API
+and described in the API documentation. For more information about the
+structure of the lists and dictionaries, as well for information on data limits
+per request, please visit the [official documentation](https://
+advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod). ###
+Request and retrieve a report The module contains classes which represent basic
+configurations of the available report types: - `CampaignsReport` -
+`TargetingReport` - `SearchTermReport` - `AdvertisedProductReports` -
+`PurchasedProductReport` For more information about the report types, please
+visit the [official documentation](https://advertising.amazon.com/API/docs/en-
+us/guides/reporting/v3/report-types). To request a report you need to pass an
+instance of one of these classes to the `create_report` method of the
+`AmazonAdsAPIConnector` class. To customize the report, change the properties
+of the class instance before passing it to the `create_report` method.
+```python from amazon_ads_api_connector import SearchTermReport
+report_configuration = SearchTermReport("2023-10-01", â"2023-10-07") res =
+api.create_report(report_configuration) report = api.get_report(res) ``` Please
+note that report gerneration is asynchronous. The `create_report` method
+returns a dictionary containing the report ID. The `get_report` takes this
+dictionary as an argument and returns the report once it is completed and
+available. The completion of a report usually takes a few minutes and can take
+up to 3 hours. ## Dependencies This module depends on the `requests` library,
+which is not included in the Python standard library, but will be installed
+automatically when you install the `amazon-ads-api-connector` package. ##
+Disclaimer This module is not affiliated with Amazon in any way. It is an
+independent project that aims to provide a simple and easy-to-use interface to
+the Amazon Ads API for Sponsored Products campaign management.
```

### Comparing `amazon-ads-api-connector-0.1.3/amazon_ads_api_connector/amazon_ads_api_connector.py` & `amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/amazon_ads_api_connector.py`

 * *Files identical despite different names*

### Comparing `amazon-ads-api-connector-0.1.3/amazon_ads_api_connector/report_types.py` & `amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/report_types.py`

 * *Files identical despite different names*

### Comparing `amazon-ads-api-connector-0.1.3/amazon_ads_api_connector.egg-info/PKG-INFO` & `amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: amazon-ads-api-connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: API wrapper for the Amazon Ads API
 Author: Markus U. Wahl
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt 
 Requires-Dist: requests
 Requires-Dist: types-requests
 
 # Amazon Ads API Connector
 
 A simple Python wrapper for the <a href="https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod">latest version of the Amazon Ads API for Sponsored Products campaign management</a>.
 
-This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product AISIN targeting. 
+This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product ASIN targeting and auto campaigns. 
 
 Please note that this module does not yet support Sponsored Brands and Sponsored Display campaigns.
 
 ## Installation
 
 Amazon Ads API Connector is available on PyPI:
 
@@ -28,17 +28,19 @@
 
 The primary class of the module is `AmazonAdsAPIConnector`. This class provides methods to create, list, update and delete 
 - campaigns, 
 - ad groups, 
 - product ads, 
 - keywords, 
 - negative keywords, and
-- targeting clauses (ASIN targeting). 
+- targeting clauses (ASIN targeting).
 
-It furthermore provides methods to request and retrieve reports via the API.
+It furthermore provides methods to get `keyword recommendations`, which include bid recommendations for keyword targets, as well as `bid recommendations for ad groups`, which include bid recommendations for auto campaigns.
+
+And lastly, it provides also methods to request and retrieve reports via the API.
 
 To create an instance of the `AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a dictionary. The dictionary must contain the following keys:
 
 - `refresh_token`
 - `client_id`
 - `client_secret`
 - `profile_id`
@@ -82,34 +84,40 @@
                 "budgetType": "DAILY",
                 "budget": 0,
             },
         },
     ]
 )
 ```
-Please note that all create and update methods expect a list of dictionaries as their only argument. This reflects the fact that the Amazon Ads API allows to create or update multiple objects at once. To ensure the greatest possible flexibility, the structure of the list and the dictionaries corresponds to the structure specified by the API and described in the API documentation.
+Please note that all create and update methods expect a list of dictionaries as their only argument. This reflects the fact that the Amazon Ads API allows to create or update multiple objects at once. To ensure the greatest possible flexibility, the structure of the list and the dictionaries corresponds to the structure specified by the API and described in the API documentation. For more information about the structure of the lists and dictionaries, as well for information on data limits per request, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod).
 
 ### Request and retrieve a report
 
-The module furthermore contains classes which represent basic configurations of the available report types:
+The module contains classes which represent basic configurations of the available report types:
 
 - `CampaignsReport`
 - `TargetingReport`
 - `SearchTermReport`
 - `AdvertisedProductReports`
 - `PurchasedProductReport`
 
-For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
+For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types).
+
+To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
 
 ```python
 from amazon_ads_api_connector import SearchTermReport
 
-report_configuration = SearchTermReport("2023-10-01", "2023-10-07")
+report_configuration = SearchTermReport("2023-10-01", ◊"2023-10-07")
 
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
 
-This module depends on the `requests` library, which is not included in the standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+This module depends on the `requests` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+
+## Disclaimer
+
+This module is not affiliated with Amazon in any way. It is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,58 +1,66 @@
-Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.4 Summary:
 API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
 Type: text/markdown License-File: LICENSE.txt Requires-Dist: requests Requires-
 Dist: types-requests # Amazon Ads API Connector A simple Python wrapper for the
 _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n
 _m_a_n_a_g_e_m_e_n_t. This module covers the key endpoints for managing Sponsored
 Products campaigns. This includes methods for authentication, pagination and
 report generation. It features keyword and negative keyword targeting, as well
-as product AISIN targeting. Please note that this module does not yet support
-Sponsored Brands and Sponsored Display campaigns. ## Installation Amazon Ads
-API Connector is available on PyPI: ```bash pip install amazon-ads-api-
-connector ``` ## Getting started The primary class of the module is
-`AmazonAdsAPIConnector`. This class provides methods to create, list, update
+as product ASIN targeting and auto campaigns. Please note that this module does
+not yet support Sponsored Brands and Sponsored Display campaigns. ##
+Installation Amazon Ads API Connector is available on PyPI: ```bash pip install
+amazon-ads-api-connector ``` ## Getting started The primary class of the module
+is `AmazonAdsAPIConnector`. This class provides methods to create, list, update
 and delete - campaigns, - ad groups, - product ads, - keywords, - negative
 keywords, and - targeting clauses (ASIN targeting). It furthermore provides
-methods to request and retrieve reports via the API. To create an instance of
-the `AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials
-as a dictionary. The dictionary must contain the following keys: -
-`refresh_token` - `client_id` - `client_secret` - `profile_id` Upon
-initialization, the AmazonAdsAPIConnector object will create a new access
-token. This access token will be valid for 60 minutes, however, the object
-automatically requests a new access token in case it has expired when trying to
-make a new request. For more information about the Amazon Ads API, please visit
-the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-
-started/how-to-use-api). ## Examples ### Import the library ```python from
-amazon_ads_api_connector import AmazonAdsAPIConnector ``` ### Create an
-instance ```python api = AmazonAdsAPIConnector( { "refresh_token":
-"your_refresh_token", "client_id": "your_client_id", "client_secret":
-"your_client_secret", "profile_id": "your_profile_id", } ) ``` ### List
-campaigns ```python campaigns = api.list_campaigns() ``` ### Create campaigns
-```python api.create_campaign( campaigns=[ { "name": "My Campaign",
-"targetingType": "MANUAL", "state": "ENABLED", "dynamicBidding": { "strategy":
-"LEGACY_FOR_SALES", }, "bugdget": { "budgetType": "DAILY", "budget": 0, }, }, ]
-) ``` Please note that all create and update methods expect a list of
-dictionaries as their only argument. This reflects the fact that the Amazon Ads
-API allows to create or update multiple objects at once. To ensure the greatest
-possible flexibility, the structure of the list and the dictionaries
-corresponds to the structure specified by the API and described in the API
-documentation. ### Request and retrieve a report The module furthermore
-contains classes which represent basic configurations of the available report
-types: - `CampaignsReport` - `TargetingReport` - `SearchTermReport` -
-`AdvertisedProductReports` - `PurchasedProductReport` For more information
-about the report types, please visit the [official documentation](https://
-advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
-request a report you need to pass an instance of one of these classes to the
-`create_report` method of the `AmazonAdsAPIConnector` class. To customize the
-report, change the properties of the class instance before passing it to the
-`create_report` method. ```python from amazon_ads_api_connector import
-SearchTermReport report_configuration = SearchTermReport("2023-10-01", "2023-
-10-07") res = api.create_report(report_configuration) report = api.get_report
-(res) ``` Please note that report gerneration is asynchronous. The
-`create_report` method returns a dictionary containing the report ID. The
-`get_report` takes this dictionary as an argument and returns the report once
-it is completed and available. The completion of a report usually takes a few
-minutes and can take up to 3 hours. ## Dependencies This module depends on the
-`requests` library, which is not included in the standard library, but will be
-installed automatically when you install the `amazon-ads-api-connector`
-package.
+methods to get `keyword recommendations`, which include bid recommendations for
+keyword targets, as well as `bid recommendations for ad groups`, which include
+bid recommendations for auto campaigns. And lastly, it provides also methods to
+request and retrieve reports via the API. To create an instance of the
+`AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a
+dictionary. The dictionary must contain the following keys: - `refresh_token` -
+`client_id` - `client_secret` - `profile_id` Upon initialization, the
+AmazonAdsAPIConnector object will create a new access token. This access token
+will be valid for 60 minutes, however, the object automatically requests a new
+access token in case it has expired when trying to make a new request. For more
+information about the Amazon Ads API, please visit the [official documentation]
+(https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api). ##
+Examples ### Import the library ```python from amazon_ads_api_connector import
+AmazonAdsAPIConnector ``` ### Create an instance ```python api =
+AmazonAdsAPIConnector( { "refresh_token": "your_refresh_token", "client_id":
+"your_client_id", "client_secret": "your_client_secret", "profile_id":
+"your_profile_id", } ) ``` ### List campaigns ```python campaigns =
+api.list_campaigns() ``` ### Create campaigns ```python api.create_campaign
+( campaigns=[ { "name": "My Campaign", "targetingType": "MANUAL", "state":
+"ENABLED", "dynamicBidding": { "strategy": "LEGACY_FOR_SALES", }, "bugdget":
+{ "budgetType": "DAILY", "budget": 0, }, }, ] ) ``` Please note that all create
+and update methods expect a list of dictionaries as their only argument. This
+reflects the fact that the Amazon Ads API allows to create or update multiple
+objects at once. To ensure the greatest possible flexibility, the structure of
+the list and the dictionaries corresponds to the structure specified by the API
+and described in the API documentation. For more information about the
+structure of the lists and dictionaries, as well for information on data limits
+per request, please visit the [official documentation](https://
+advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod). ###
+Request and retrieve a report The module contains classes which represent basic
+configurations of the available report types: - `CampaignsReport` -
+`TargetingReport` - `SearchTermReport` - `AdvertisedProductReports` -
+`PurchasedProductReport` For more information about the report types, please
+visit the [official documentation](https://advertising.amazon.com/API/docs/en-
+us/guides/reporting/v3/report-types). To request a report you need to pass an
+instance of one of these classes to the `create_report` method of the
+`AmazonAdsAPIConnector` class. To customize the report, change the properties
+of the class instance before passing it to the `create_report` method.
+```python from amazon_ads_api_connector import SearchTermReport
+report_configuration = SearchTermReport("2023-10-01", â"2023-10-07") res =
+api.create_report(report_configuration) report = api.get_report(res) ``` Please
+note that report gerneration is asynchronous. The `create_report` method
+returns a dictionary containing the report ID. The `get_report` takes this
+dictionary as an argument and returns the report once it is completed and
+available. The completion of a report usually takes a few minutes and can take
+up to 3 hours. ## Dependencies This module depends on the `requests` library,
+which is not included in the Python standard library, but will be installed
+automatically when you install the `amazon-ads-api-connector` package. ##
+Disclaimer This module is not affiliated with Amazon in any way. It is an
+independent project that aims to provide a simple and easy-to-use interface to
+the Amazon Ads API for Sponsored Products campaign management.
```

