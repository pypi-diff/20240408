# Comparing `tmp/contact-energy-nz-0.1.7430397263.tar.gz` & `tmp/contact-energy-nz-0.1.8595366105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-energy-nz-0.1.7430397263.tar", last modified: Sat Jan  6 08:07:13 2024, max compression
+gzip compressed data, was "contact-energy-nz-0.1.8595366105.tar", last modified: Mon Apr  8 06:16:49 2024, max compression
```

## Comparing `contact-energy-nz-0.1.7430397263.tar` & `contact-energy-nz-0.1.8595366105.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:07:13.212448 contact-energy-nz-0.1.7430397263/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-01-06 08:07:13.212448 contact-energy-nz-0.1.7430397263/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:07:13.212448 contact-energy-nz-0.1.7430397263/contact_energy_nz/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz/contact_energy_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz/usage_datum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:07:13.212448 contact-energy-nz-0.1.7430397263/contact_energy_nz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-01-06 08:07:13.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-06 08:07:13.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 08:07:13.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-06 08:07:13.000000 contact-energy-nz-0.1.7430397263/contact_energy_nz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 08:07:13.212448 contact-energy-nz-0.1.7430397263/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:07:13.212448 contact-energy-nz-0.1.7430397263/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-06 08:07:00.000000 contact-energy-nz-0.1.7430397263/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:16:49.488741 contact-energy-nz-0.1.8595366105/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-08 06:16:49.488741 contact-energy-nz-0.1.8595366105/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:16:49.488741 contact-energy-nz-0.1.8595366105/contact_energy_nz/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz/contact_energy_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz/usage_datum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:16:49.488741 contact-energy-nz-0.1.8595366105/contact_energy_nz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-08 06:16:49.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 06:16:49.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:16:49.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 06:16:49.000000 contact-energy-nz-0.1.8595366105/contact_energy_nz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-08 06:16:36.000000 contact-energy-nz-0.1.8595366105/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:16:49.488741 contact-energy-nz-0.1.8595366105/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:16:49.488741 contact-energy-nz-0.1.8595366105/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 06:16:35.000000 contact-energy-nz-0.1.8595366105/tests/test_integration.py
```

### Comparing `contact-energy-nz-0.1.7430397263/LICENSE` & `contact-energy-nz-0.1.8595366105/LICENSE`

 * *Files identical despite different names*

### Comparing `contact-energy-nz-0.1.7430397263/PKG-INFO` & `contact-energy-nz-0.1.8595366105/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-energy-nz
-Version: 0.1.7430397263
+Version: 0.1.8595366105
 Summary: API Connector to fetch usage data from Contact Energy NZ utilities provider
 Author-email: Tkhadimullin <hello@wiseowls.co.nz>
 License: MIT
 Project-URL: Homepage, https://github.com/tkhadimullin/contact-energy-nz
 Project-URL: Bug Tracker, https://github.com/tkhadimullin/contact-energy-nz/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -301,14 +301,26 @@
         "unit": "kWh",
         "timeZone": "Pacific/Auckland",
         "percentage": 9.99
     }
 ]
 ```
 
+#### To get hourly data
+
+```python
+try:
+    async with async_timeout.timeout(TIMEOUT):
+        data = await connector.get_hourly_usage(date.fromisoformat("2024-04-08"))
+    except asyncio.TimeoutError as e:
+        pass # handle timeout
+```
+
+Call to `/usage/v2/{contract_id}?ba={account_id}&interval=hourly&from=YYY-MM-DD&to=YYYY-MM-DD` returns the same structure as above.
+
 ## Contributing
 Contributions are welcome and encouraged. If you want to add new features, please feel free to open PRs here.
 
 ## License
 This library is provided under the MIT License.
 
 ---
```

### Comparing `contact-energy-nz-0.1.7430397263/README.md` & `contact-energy-nz-0.1.8595366105/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -290,14 +290,26 @@
         "unit": "kWh",
         "timeZone": "Pacific/Auckland",
         "percentage": 9.99
     }
 ]
 ```
 
+#### To get hourly data
+
+```python
+try:
+    async with async_timeout.timeout(TIMEOUT):
+        data = await connector.get_hourly_usage(date.fromisoformat("2024-04-08"))
+    except asyncio.TimeoutError as e:
+        pass # handle timeout
+```
+
+Call to `/usage/v2/{contract_id}?ba={account_id}&interval=hourly&from=YYY-MM-DD&to=YYYY-MM-DD` returns the same structure as above.
+
 ## Contributing
 Contributions are welcome and encouraged. If you want to add new features, please feel free to open PRs here.
 
 ## License
 This library is provided under the MIT License.
 
 ---
```

### Comparing `contact-energy-nz-0.1.7430397263/contact_energy_nz/contact_energy_api.py` & `contact-energy-nz-0.1.8595366105/contact_energy_nz/contact_energy_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -126,7 +126,22 @@
         url = f"{API_BASE_URL}/usage/v2/{self.contract_id}?ba={self.account_id}&interval=monthly&from={formatted_start_date}&to={formatted_end_date}"
         monthly_stats = await self._try_fetch_data(url, "post")
         return sorted(
             [UsageDatum(item) for item in monthly_stats],
             key=lambda x: x.date,
             reverse=True,
         )
+
+    async def get_hourly_usage(self, date: datetime) -> list[UsageDatum]:
+        """Query hourly usage stats for a given day"""
+        formatted_date = date.strftime("%Y-%m-%d")
+
+        # `to` parameter may be unnecessary, the api only returns the data
+        # for the day specified in `from`, but the javascript on the website
+        # always puts the `to` parameter in anyway.
+        url = f"{API_BASE_URL}/usage/v2/{self.contract_id}?ba={self.account_id}&interval=hourly&from={formatted_date}&to={formatted_date}"
+        hourly_stats = await self._try_fetch_data(url, "post")
+        return sorted(
+            [UsageDatum(item) for item in hourly_stats],
+            key=lambda x: x.date,
+            reverse=False,  # We want the data to be in order from start of the day to the end of the day
+        )
```

### Comparing `contact-energy-nz-0.1.7430397263/contact_energy_nz/usage_datum.py` & `contact-energy-nz-0.1.8595366105/contact_energy_nz/usage_datum.py`

 * *Files identical despite different names*

### Comparing `contact-energy-nz-0.1.7430397263/contact_energy_nz.egg-info/PKG-INFO` & `contact-energy-nz-0.1.8595366105/contact_energy_nz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-energy-nz
-Version: 0.1.7430397263
+Version: 0.1.8595366105
 Summary: API Connector to fetch usage data from Contact Energy NZ utilities provider
 Author-email: Tkhadimullin <hello@wiseowls.co.nz>
 License: MIT
 Project-URL: Homepage, https://github.com/tkhadimullin/contact-energy-nz
 Project-URL: Bug Tracker, https://github.com/tkhadimullin/contact-energy-nz/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -301,14 +301,26 @@
         "unit": "kWh",
         "timeZone": "Pacific/Auckland",
         "percentage": 9.99
     }
 ]
 ```
 
+#### To get hourly data
+
+```python
+try:
+    async with async_timeout.timeout(TIMEOUT):
+        data = await connector.get_hourly_usage(date.fromisoformat("2024-04-08"))
+    except asyncio.TimeoutError as e:
+        pass # handle timeout
+```
+
+Call to `/usage/v2/{contract_id}?ba={account_id}&interval=hourly&from=YYY-MM-DD&to=YYYY-MM-DD` returns the same structure as above.
+
 ## Contributing
 Contributions are welcome and encouraged. If you want to add new features, please feel free to open PRs here.
 
 ## License
 This library is provided under the MIT License.
 
 ---
```

### Comparing `contact-energy-nz-0.1.7430397263/pyproject.toml` & `contact-energy-nz-0.1.8595366105/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "contact-energy-nz"
-version = "0.1.7430397263"
+version = "0.1.8595366105"
 description = "API Connector to fetch usage data from Contact Energy NZ utilities provider"
 authors = [
     {name = "Tkhadimullin", email = "hello@wiseowls.co.nz"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
```

### Comparing `contact-energy-nz-0.1.7430397263/tests/test_integration.py` & `contact-energy-nz-0.1.8595366105/tests/test_integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,8 +30,18 @@
 
 @pytest.mark.asyncio
 async def test_should_be_able_to_get_monthly_usage_for_current_month(api_client):
     current_month = datetime.date.today().month
     results = await api_client.get_latest_usage()
     
     assert results
-    assert results.date.month == current_month
+    assert results.date.month == current_month
+
+@pytest.mark.asyncio
+async def test_should_be_able_to_get_hourly_usage(api_client):
+    # Timedelta as hourly usage doesn't get updated for a few days
+    day_to_test = datetime.date.today() - datetime.timedelta(weeks=1)
+    results = await api_client.get_hourly_usage(day_to_test)
+
+    assert results
+    assert results[0].date.day == day_to_test.day
+    assert results[0].date.hour == 0
```

