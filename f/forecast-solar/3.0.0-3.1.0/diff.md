# Comparing `tmp/forecast_solar-3.0.0.tar.gz` & `tmp/forecast_solar-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecast_solar-3.0.0.tar", last modified: Sun Apr 23 18:06:29 2023, max compression
+gzip compressed data, was "forecast_solar-3.1.0.tar", last modified: Mon Apr  8 11:11:58 2024, max compression
```

## Comparing `forecast_solar-3.0.0.tar` & `forecast_solar-3.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:06:29.882314 forecast_solar-3.0.0/forecast_solar/
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/forecast_solar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/forecast_solar/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/forecast_solar/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/forecast_solar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:58.444060 forecast_solar-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-04-08 11:11:58.444060 forecast_solar-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:58.440060 forecast_solar-3.1.0/forecast_solar/
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/forecast_solar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/forecast_solar/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/forecast_solar/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:58.444060 forecast_solar-3.1.0/forecast_solar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-04-08 11:11:58.000000 forecast_solar-3.1.0/forecast_solar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-08 11:11:58.000000 forecast_solar-3.1.0/forecast_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:11:58.000000 forecast_solar-3.1.0/forecast_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:11:58.000000 forecast_solar-3.1.0/forecast_solar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 11:11:58.000000 forecast_solar-3.1.0/forecast_solar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 11:11:58.000000 forecast_solar-3.1.0/forecast_solar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 11:11:58.444060 forecast_solar-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:58.440060 forecast_solar-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-08 11:11:49.000000 forecast_solar-3.1.0/tests/test_models.py
```

### Comparing `forecast_solar-3.0.0/LICENSE` & `forecast_solar-3.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2021-2023 Klaas Schoute
+Copyright (c) 2021-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `forecast_solar-3.0.0/PKG-INFO` & `forecast_solar-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecast_solar
-Version: 3.0.0
+Version: 3.1.0
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/klaasnicolaas/forecast_solar
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 License: MIT license
 Keywords: forecast,solar,power,energy,api,async,client
 Classifier: Framework :: AsyncIO
@@ -13,14 +13,17 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.0.0
+Requires-Dist: aiodns>=3.0.0
+Requires-Dist: backports.zoneinfo; python_version < "3.9"
 
 <!--
 *** To avoid retyping too much info. Do a search and replace for the following:
 *** github_username, repo_name
 -->
 
 ## Python API fetching Solarpanels forecast information.
@@ -70,14 +73,19 @@
 ### API Info
 
 - Timezone
 - Rate limit
 - Account type
 - Rate remaining
 
+### Validation
+
+- API key (bool)
+- Plane (bool)
+
 ## Example
 
 ```python
 import asyncio
 
 from forecast_solar import ForecastSolar
 
@@ -122,15 +130,15 @@
 
 Thank you for being involved! :heart_eyes:
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2023 Klaas Schoute
+Copyright (c) 2021-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -147,15 +155,15 @@
 SOFTWARE.
 
 <!-- LINKS -->
 [forecast-horizon]: https://doc.forecast.solar/doku.php?id=api#horizon
 [forecast-damping]: https://doc.forecast.solar/doku.php?id=damping
 
 <!-- MARKDOWN LINKS & IMAGES -->
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg?style=for-the-badge
 [contributors-shield]: https://img.shields.io/github/contributors/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [contributors-url]: https://github.com/home-assistant-libs/forecast_solar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [forks-url]: https://github.com/home-assistant-libs/forecast_solar/network/members
 [stars-shield]: https://img.shields.io/github/stars/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [stars-url]: https://github.com/home-assistant-libs/forecast_solar/stargazers
 [issues-shield]: https://img.shields.io/github/issues/home-assistant-libs/forecast_solar.svg?style=for-the-badge
```

### Comparing `forecast_solar-3.0.0/README.md` & `forecast_solar-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 ### API Info
 
 - Timezone
 - Rate limit
 - Account type
 - Rate remaining
 
+### Validation
+
+- API key (bool)
+- Plane (bool)
+
 ## Example
 
 ```python
 import asyncio
 
 from forecast_solar import ForecastSolar
 
@@ -102,15 +107,15 @@
 
 Thank you for being involved! :heart_eyes:
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2023 Klaas Schoute
+Copyright (c) 2021-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -127,15 +132,15 @@
 SOFTWARE.
 
 <!-- LINKS -->
 [forecast-horizon]: https://doc.forecast.solar/doku.php?id=api#horizon
 [forecast-damping]: https://doc.forecast.solar/doku.php?id=damping
 
 <!-- MARKDOWN LINKS & IMAGES -->
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg?style=for-the-badge
 [contributors-shield]: https://img.shields.io/github/contributors/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [contributors-url]: https://github.com/home-assistant-libs/forecast_solar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [forks-url]: https://github.com/home-assistant-libs/forecast_solar/network/members
 [stars-shield]: https://img.shields.io/github/stars/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [stars-url]: https://github.com/home-assistant-libs/forecast_solar/stargazers
 [issues-shield]: https://img.shields.io/github/issues/home-assistant-libs/forecast_solar.svg?style=for-the-badge
```

### Comparing `forecast_solar-3.0.0/forecast_solar/__init__.py` & `forecast_solar-3.1.0/forecast_solar/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from aiodns import DNSResolver
 from aiodns.error import DNSError
 from aiohttp import ClientSession
 from yarl import URL
 
 from .exceptions import (
     ForecastSolarAuthenticationError,
+    ForecastSolarConfigError,
     ForecastSolarConnectionError,
     ForecastSolarError,
-    ForecastSolarRequestError,
     ForecastSolarRatelimit,
+    ForecastSolarRequestError,
 )
 from .models import Estimate, Ratelimit
 
 
 @dataclass
 class ForecastSolar:
     """Main class for handling connections with the Forecast.Solar API."""
@@ -40,23 +41,29 @@
     ratelimit: Ratelimit | None = None
     inverter: float | None = None
 
     async def _request(
         self,
         uri: str,
         *,
+        rate_limit=True,
+        authenticate=True,
         params: Mapping[str, str] | None = None,
     ) -> dict[str, Any]:
         """Handle a request to the Forecast.Solar API.
 
         A generic method for sending/handling HTTP requests done against
         the Forecast.Solar API.
 
         Args:
             uri: Request URI, for example, 'estimate'
+            rate_limit: Parse rate limit from response. Set to False for
+                endpoints that are missing rate limiting headers in response.
+            authenticate: Prefix request with api_key. Set to False for
+                endpoints that do not provide authentication.
 
         Returns:
             A Python dictionary (JSON decoded) with the response from
             the Forecast.Solar API.
 
         Raises:
             ForecastSolarAuthenticationError: If the API key is invalid.
@@ -86,15 +93,15 @@
                 "Could not resolve Forecast.Solar API address"
             )
 
         # Connect as normal
         url = URL.build(scheme="https", host=result[0].host)
 
         # Add API key if one is provided
-        if self.api_key is not None:
+        if authenticate and self.api_key is not None:
             url = url.with_path(f"{self.api_key}/")
 
         url = url.join(URL(uri))
 
         if self.session is None:
             self.session = ClientSession()
             self.close_session = True
@@ -103,46 +110,77 @@
             "GET",
             url,
             params=params,
             headers={"Host": "api.forecast.solar"},
             ssl=False,
         )
 
-        if response.status == 502:
+        if response.status in (502, 503):
             raise ForecastSolarConnectionError(
                 "The Forecast.Solar API is unreachable, "
             )
 
         if response.status == 400:
             data = await response.json()
             raise ForecastSolarRequestError(data["message"])
 
         if response.status in (401, 403):
             data = await response.json()
             raise ForecastSolarAuthenticationError(data["message"])
 
+        if response.status == 422:
+            data = await response.json()
+            raise ForecastSolarConfigError(data["message"])
+
         if response.status == 429:
             data = await response.json()
             raise ForecastSolarRatelimit(data["message"])
 
-        if response.status < 500:
+        if rate_limit and response.status < 500:
             self.ratelimit = Ratelimit.from_response(response)
 
         response.raise_for_status()
 
         content_type = response.headers.get("Content-Type", "")
         if "application/json" not in content_type:
             text = await response.text()
             raise ForecastSolarError(
                 "Unexpected response from the Forecast.Solar API",
                 {"Content-Type": content_type, "response": text},
             )
 
         return await response.json()
 
+    async def validate_plane(self) -> bool:
+        """Validate plane by calling the Forecast.Solar API
+
+        Returns:
+            True, if plane is valid.
+        """
+
+        await self._request(
+            f"check/{self.latitude}/{self.longitude}"
+            f"/{self.declination}/{self.azimuth}/{self.kwp}",
+            rate_limit=False,
+            authenticate=False,
+        )
+
+        return True
+
+    async def validate_api_key(self) -> bool:
+        """Validate api key by calling the Forecast.Solar API
+
+        Returns:
+            True, if api key is valid
+        """
+
+        await self._request("info", rate_limit=False)
+
+        return True
+
     async def estimate(self) -> Estimate:
         """Get solar production estimations from the Forecast.Solar API.
 
         Returns:
             A Estimate object, with a estimated production forecast.
         """
         params = {"time": "iso8601", "damping": str(self.damping)}
```

### Comparing `forecast_solar-3.0.0/forecast_solar/exceptions.py` & `forecast_solar-3.1.0/forecast_solar/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,34 @@
     """Generic Forecast.Solar exception."""
 
 
 class ForecastSolarConnectionError(ForecastSolarError):
     """Forecast.Solar API connection exception."""
 
 
+class ForecastSolarConfigError(ForecastSolarError):
+    """Forecast.Solar API configuration exception."""
+
+    def __init__(self, data: str) -> None:
+        """Init a solar config error."""
+        super().__init__(f'{data["text"]} (error 422)')
+
+
 class ForecastSolarAuthenticationError(ForecastSolarError):
     """Forecast.Solar API authentication exception."""
 
     def __init__(self, data: dict) -> None:
         """Init a solar auth error.
 
         https://doc.forecast.solar/doku.php?id=api#invalid_request
         """
-        super().__init__(f'{data["text"]} (error {data["code"]})')
-        self.code = data["code"]
+        # seems that code is missing in response in some endpoints (i.e /info)
+        code = data.get("code")
+        super().__init__(f'{data["text"]} (error {code})')
+        self.code = code
 
 
 class ForecastSolarRequestError(ForecastSolarError):
     """Forecast.Solar wrong request input variables."""
 
     def __init__(self, data: dict) -> None:
         """Init a solar request error.
```

### Comparing `forecast_solar-3.0.0/forecast_solar/models.py` & `forecast_solar-3.1.0/forecast_solar/models.py`

 * *Files identical despite different names*

### Comparing `forecast_solar-3.0.0/forecast_solar.egg-info/PKG-INFO` & `forecast_solar-3.1.0/forecast_solar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: forecast-solar
-Version: 3.0.0
+Name: forecast_solar
+Version: 3.1.0
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/klaasnicolaas/forecast_solar
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 License: MIT license
 Keywords: forecast,solar,power,energy,api,async,client
 Classifier: Framework :: AsyncIO
@@ -13,14 +13,17 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.0.0
+Requires-Dist: aiodns>=3.0.0
+Requires-Dist: backports.zoneinfo; python_version < "3.9"
 
 <!--
 *** To avoid retyping too much info. Do a search and replace for the following:
 *** github_username, repo_name
 -->
 
 ## Python API fetching Solarpanels forecast information.
@@ -70,14 +73,19 @@
 ### API Info
 
 - Timezone
 - Rate limit
 - Account type
 - Rate remaining
 
+### Validation
+
+- API key (bool)
+- Plane (bool)
+
 ## Example
 
 ```python
 import asyncio
 
 from forecast_solar import ForecastSolar
 
@@ -122,15 +130,15 @@
 
 Thank you for being involved! :heart_eyes:
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2023 Klaas Schoute
+Copyright (c) 2021-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -147,15 +155,15 @@
 SOFTWARE.
 
 <!-- LINKS -->
 [forecast-horizon]: https://doc.forecast.solar/doku.php?id=api#horizon
 [forecast-damping]: https://doc.forecast.solar/doku.php?id=damping
 
 <!-- MARKDOWN LINKS & IMAGES -->
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg?style=for-the-badge
 [contributors-shield]: https://img.shields.io/github/contributors/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [contributors-url]: https://github.com/home-assistant-libs/forecast_solar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [forks-url]: https://github.com/home-assistant-libs/forecast_solar/network/members
 [stars-shield]: https://img.shields.io/github/stars/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [stars-url]: https://github.com/home-assistant-libs/forecast_solar/stargazers
 [issues-shield]: https://img.shields.io/github/issues/home-assistant-libs/forecast_solar.svg?style=for-the-badge
```

### Comparing `forecast_solar-3.0.0/setup.py` & `forecast_solar-3.1.0/setup.py`

 * *Files identical despite different names*

