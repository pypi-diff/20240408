# Comparing `tmp/instagram-location-search-1.4.2.tar.gz` & `tmp/instagram-location-search-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-location-search-1.4.2.tar", last modified: Wed Apr  3 13:25:53 2024, max compression
+gzip compressed data, was "instagram-location-search-1.5.1.tar", last modified: Mon Apr  8 09:44:38 2024, max compression
```

## Comparing `instagram-location-search-1.4.2.tar` & `instagram-location-search-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/instagram_location_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 13:25:53.000000 instagram-location-search-1.4.2/instagram_location_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/instagram_locations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/instagram_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/instagram_locations/instagram_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/instagram_locations/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:25:53.515728 instagram-location-search-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 13:25:19.000000 instagram-location-search-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:44:38.952869 instagram-location-search-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 09:43:58.000000 instagram-location-search-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-08 09:44:38.952869 instagram-location-search-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-08 09:43:58.000000 instagram-location-search-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:44:38.952869 instagram-location-search-1.5.1/instagram_location_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-08 09:44:38.000000 instagram-location-search-1.5.1/instagram_location_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 09:44:38.000000 instagram-location-search-1.5.1/instagram_location_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:44:38.000000 instagram-location-search-1.5.1/instagram_location_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 09:44:38.000000 instagram-location-search-1.5.1/instagram_location_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 09:44:38.000000 instagram-location-search-1.5.1/instagram_location_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 09:44:38.000000 instagram-location-search-1.5.1/instagram_location_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:44:38.952869 instagram-location-search-1.5.1/instagram_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:43:58.000000 instagram-location-search-1.5.1/instagram_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-08 09:43:58.000000 instagram-location-search-1.5.1/instagram_locations/instagram_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 09:43:58.000000 instagram-location-search-1.5.1/instagram_locations/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:44:38.952869 instagram-location-search-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 09:43:58.000000 instagram-location-search-1.5.1/setup.py
```

### Comparing `instagram-location-search-1.4.2/LICENSE` & `instagram-location-search-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-location-search-1.4.2/PKG-INFO` & `instagram-location-search-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-location-search
-Version: 1.4.2
+Version: 1.5.1
 Summary: Finds Instagram location IDs near a specified latitude and longitude.
 Home-page: https://www.bellingcat.com
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT License
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `instagram-location-search-1.4.2/README.md` & `instagram-location-search-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `instagram-location-search-1.4.2/instagram_location_search.egg-info/PKG-INFO` & `instagram-location-search-1.5.1/instagram_location_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-location-search
-Version: 1.4.2
+Version: 1.5.1
 Summary: Finds Instagram location IDs near a specified latitude and longitude.
 Home-page: https://www.bellingcat.com
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT License
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `instagram-location-search-1.4.2/instagram_locations/instagram_locations.py` & `instagram-location-search-1.5.1/instagram_locations/instagram_locations.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,21 +47,20 @@
     locs = requests.get("https://www.instagram.com/web/search/topsearch/?context=place&query=" + query).json()
 
     return [v["place"]["location"] for v in locs["places"]]
 
 
 # queries the instagram location API for several points around a central lat/lng
 # in order to return additional results
-def get_fuzzy_locations(lat, lng, cookie, sigma=2):
+def get_fuzzy_locations(lat, lng, cookie, sigma=0):
     locs = get_instagram_locations(lat, lng, cookie)
-    print(locs)
     loc_ids = {v["external_id"] for v in locs if "external_id" in v}
 
-    std_lat = pstdev([v["lat"] for v in locs if "lat" in v])
-    std_lng = pstdev([v["lng"] for v in locs if "lng" in v])
+    std_lat = pstdev([v["lat"] for v in locs if "lat" in v]) / 8.0
+    std_lng = pstdev([v["lng"] for v in locs if "lng" in v]) / 8.0
 
     # filter to avoid calling with both lat and lng deltas equal zero (which would duplicate the call
     # to obtain the initial loc)
     deltas = (
         (lat + delta_lat * std_lat, lng + delta_lng * std_lng)
         for delta_lat, delta_lng in filter(lambda x: any(x), product(range(-sigma, sigma + 1), repeat=2))
     )
@@ -209,27 +208,33 @@
     parser.add_argument("--geojson", action="store", dest="geojson")
     parser.add_argument("--map", action="store", dest="map")
     parser.add_argument("--csv", action="store", dest="csv")
     parser.add_argument("--lat", action="store", dest="lat")
     parser.add_argument("--lng", action="store", dest="lng")
     parser.add_argument("--date", action="store", dest="date")
     parser.add_argument("--ids", action="store", dest="dump_ids")
+    parser.add_argument("--more", action="store_true", dest="more")
 
     args = parser.parse_args()
 
+    sigma = 2 if args.more else 0
+
     cookie = args.cookie
     # If user run command without cookie we are trying to perform automated flow to acquire the cookie
     if not cookie:
         cookie = get_insta_cookies()
 
     date_var = ""
     if args.date is not None:
         date_var = "?max_id=" + encode_date(args.date)
 
-    locations = get_fuzzy_locations(float(args.lat), float(args.lng), cookie)
+    locations = get_fuzzy_locations(float(args.lat), float(args.lng), cookie, sigma=sigma)
+
+    for i in locations:
+        i["url"] = f"https://www.instagram.com/explore/locations/{i['external_id']}{date_var}"
 
     if args.output:
         json.dump(locations, open(args.output, "w"))
 
     if args.geojson:
         json.dump(make_geojson(locations), open(args.geojson, "w"))
 
@@ -238,28 +243,28 @@
         viz = s.substitute(lat=args.lat, lng=args.lng, locs=json.dumps(make_geojson(locations)), date_var=date_var)
 
         f = open(args.map, "w")
         f.write(viz)
         f.close()
 
     if args.csv:
-        for i in locations:
-            i["url"] = f"https://www.instagram.com/explore/locations/{i['external_id']}{date_var}"
-
         # leading empty string for 'id' column is for backward compatibility since that's the pandas behavior.
         fieldnames = ["", "name", "external_id", "external_id_source", "lat", "lng", "address", "minimum_age", "url"]
 
         with open(args.csv, "w") as f:
             writer = csv.DictWriter(f, fieldnames=fieldnames)
             writer.writeheader()
             for idx, row in enumerate(locations):
                 row[""] = idx
                 writer.writerow(row)
 
     if args.dump_ids:
         ids = map(lambda loc: str(loc["external_id"]), locations)
         with open(args.dump_ids, "w") as f:
             f.write("\n".join(ids))
+
+    if not args.dump_ids and not args.csv and not args.map and not args.geojson and not args.output:
+        print('\n'.join([f"{loc['name']} ({loc['url']})" for loc in locations]))
             
 
 if __name__ == "__main__":
     main()
```

### Comparing `instagram-location-search-1.4.2/setup.py` & `instagram-location-search-1.5.1/setup.py`

 * *Files identical despite different names*

