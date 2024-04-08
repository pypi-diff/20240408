# Comparing `tmp/NorenRestApi-0.0.27-py2.py3-none-any.whl.zip` & `tmp/NorenRestApi-0.0.28-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 22358 bytes, number of entries: 7
--rw-rw-r--  2.0 unx    34683 b- defN 23-Oct-09 10:25 NorenRestApiPy/NorenApi.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-20 11:12 NorenRestApiPy/__init__.py
--rw-rw-r--  2.0 unx      187 b- defN 23-Oct-09 10:45 NorenRestApi-0.0.27.dist-info/LICENSE
--rw-rw-r--  2.0 unx    70361 b- defN 23-Oct-09 10:45 NorenRestApi-0.0.27.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Oct-09 10:45 NorenRestApi-0.0.27.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Oct-09 10:45 NorenRestApi-0.0.27.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      581 b- defN 23-Oct-09 10:45 NorenRestApi-0.0.27.dist-info/RECORD
-7 files, 105937 bytes uncompressed, 21322 bytes compressed:  79.9%
+Zip file size: 22292 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx    34055 b- defN 24-Apr-08 05:16 NorenRestApiPy/NorenApi.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 05:14 NorenRestApiPy/__init__.py
+-rw-rw-r--  2.0 unx      187 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    70334 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/RECORD
+7 files, 105282 bytes uncompressed, 21256 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: NorenRestApiPy/NorenApi.py
 Comment: 
 
 Filename: NorenRestApiPy/__init__.py
 Comment: 
 
-Filename: NorenRestApi-0.0.27.dist-info/LICENSE
+Filename: NorenRestApi-0.0.28.dist-info/LICENSE
 Comment: 
 
-Filename: NorenRestApi-0.0.27.dist-info/METADATA
+Filename: NorenRestApi-0.0.28.dist-info/METADATA
 Comment: 
 
-Filename: NorenRestApi-0.0.27.dist-info/WHEEL
+Filename: NorenRestApi-0.0.28.dist-info/WHEEL
 Comment: 
 
-Filename: NorenRestApi-0.0.27.dist-info/top_level.txt
+Filename: NorenRestApi-0.0.28.dist-info/top_level.txt
 Comment: 
 
-Filename: NorenRestApi-0.0.27.dist-info/RECORD
+Filename: NorenRestApi-0.0.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NorenRestApiPy/NorenApi.py

```diff
@@ -85,16 +85,15 @@
           'holdings' : '/Holdings',
           'limits' : '/Limits',
           'positions': '/PositionBook',
           'scripinfo': '/GetSecurityInfo',
           'getquotes': '/GetQuotes',
           'span_calculator' :'/SpanCalc',
           'option_greek' :'/GetOptionGreek',
-          'get_daily_price_series' :'/EODChartData',  
-          'forgot_password_OTP':'/FgtPwdOTP',    
+          'get_daily_price_series' :'/EODChartData',      
       },
       'websocket_endpoint': 'wss://wsendpoint/',
       #'eoddata_endpoint' : 'http://eodhost/'
     }
 
     def __init__(self, host, websocket):
         self.__service_config['host'] = host
@@ -484,15 +483,15 @@
 
         return resDict
 
 
     def place_order(self, buy_or_sell, product_type,
                     exchange, tradingsymbol, quantity, discloseqty,
                     price_type, price=0.0, trigger_price=None,
-                    retention='DAY', amo='NO', remarks=None, bookloss_price = 0.0, bookprofit_price = 0.0, trail_price = 0.0):
+                    retention='DAY', amo=None, remarks=None, bookloss_price = 0.0, bookprofit_price = 0.0, trail_price = 0.0):
         config = NorenApi.__service_config
 
         #prepare the uri
         url = f"{config['host']}{config['routes']['placeorder']}" 
         reportmsg(url)
         #prepare the data
         values              = {'ordersource':'API'}
@@ -505,15 +504,17 @@
         values["qty"]       = str(quantity)
         values["dscqty"]    = str(discloseqty)        
         values["prctyp"]    = price_type
         values["prc"]       = str(price)
         values["trgprc"]    = str(trigger_price)
         values["ret"]       = retention
         values["remarks"]   = remarks
-        values["amo"]       = amo
+      
+        if amo is not None:
+           values["amo"]       = amo
         
         #if cover order or high leverage order
         if product_type == 'H':            
             values["blprc"]       = str(bookloss_price)
             #trailing price
             if trail_price != 0.0:
                 values["trailprc"] = str(trail_price)
@@ -1083,29 +1084,7 @@
 
         res = requests.post(url, data=payload)
         reportmsg(res.text)
 
         resDict = json.loads(res.text)        
 
         return resDict
-        
-    def forgot_password_OTP(self, userid, pan):
-        config = NorenApi.__service_config
-
-        #prepare the uri
-        url = f"{config['host']}{config['routes']['forgot_password_OTP']}" 
-        reportmsg(url)
-
-        #prepare the data
-        values              = { "source": "API" }
-        values["uid"]       = userid
-        values["pan"]       = pan
-
-        payload = 'jData=' + json.dumps(values)
-        reportmsg("Req:" + payload)
-        
-        res = requests.post(url, data=payload)
-        reportmsg(res.text)
-
-        resDict = json.loads(res.text)        
-
-        return resDict
```

## Comparing `NorenRestApi-0.0.27.dist-info/METADATA` & `NorenRestApi-0.0.28.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: NorenRestApi
-Version: 0.0.27
+Version: 0.0.28
 Summary: A package for NorenOMS
+Home-page: UNKNOWN
 Author: KumarAnand
 Author-email: kumar.anand@kambala.co.in
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests (==2.28.2)
-Requires-Dist: websocket-client (==1.5.1)
-Requires-Dist: pandas (==1.5.3)
-Requires-Dist: PyYAML (==6.0)
+Requires-Dist: PyYAML ==6.0
+Requires-Dist: pandas ==1.5.3
+Requires-Dist: requests ==2.28.2
+Requires-Dist: websocket-client ==1.5.1
 
 # NorenApi
 
 Api used to connect to NorenOMS
 ****
 
 ## Build
@@ -87,15 +89,15 @@
 Request Details :
 
 |Json Fields|Possible value|Description|
 | --- | --- | ---|
 |apkversion*||Application version.|
 |uid*||User Id of the login user|
 |pwd*||Sha256 of the user entered password.|
-|factor2*||DOB or PAN as entered by the user. (DOB should be in DD-MM-YYYY)|
+|factor2*||OTP or TOTP|
 |vc*||Vendor code provided by noren team, along with connection URLs|
 |appkey*||Sha256 of  uid|vendor_key|
 |imei*||Send mac if users logs in for desktop, imei is from mobile|
 |addldivinf||Optional field, Value must be in below format:|iOS - iosInfo.utsname.machine - iosInfo.systemVersion|Android - androidInfo.model - androidInfo.version|examples:|iOS - iPhone 8.0 - 9.0|Android - Moto G - 9 PKQ1.181203.01|
 |ipaddr||Optional field|
 |source|API||
 
@@ -2353,7 +2355,9 @@
 Copying of this file, via any medium is strictly prohibited.
 Proprietary and confidential.
 All file transfers are logged.
 
 ****
 
 
+
+
```

## Comparing `NorenRestApi-0.0.27.dist-info/RECORD` & `NorenRestApi-0.0.28.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-NorenRestApiPy/NorenApi.py,sha256=iS3ZlVMqcu4wSjJw8ycIJWl3xxA-DDnp8X-3_bCJXyc,34683
+NorenRestApiPy/NorenApi.py,sha256=fJ3EM-Iwy9inYusfTDxiPn_gAdD9g7_TxTGJ0MbsMjs,34055
 NorenRestApiPy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-NorenRestApi-0.0.27.dist-info/LICENSE,sha256=mqXdxwEe__d9rE8OthmQzKK9sCAPBfJvi_5VUdiazls,187
-NorenRestApi-0.0.27.dist-info/METADATA,sha256=3H4TG9vG2NzOZVLIe07-1GcfMiC0VsKcZIEwZi__0gM,70361
-NorenRestApi-0.0.27.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-NorenRestApi-0.0.27.dist-info/top_level.txt,sha256=T_X85fuNUvAPVEDBEZofFPOpbANpopXmBDcaFW8Q2W0,15
-NorenRestApi-0.0.27.dist-info/RECORD,,
+NorenRestApi-0.0.28.dist-info/LICENSE,sha256=mqXdxwEe__d9rE8OthmQzKK9sCAPBfJvi_5VUdiazls,187
+NorenRestApi-0.0.28.dist-info/METADATA,sha256=52lcfbgdk3Y5ate1z5Ja-iU0rkTKp24QP4Ut_29_nOI,70334
+NorenRestApi-0.0.28.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+NorenRestApi-0.0.28.dist-info/top_level.txt,sha256=T_X85fuNUvAPVEDBEZofFPOpbANpopXmBDcaFW8Q2W0,15
+NorenRestApi-0.0.28.dist-info/RECORD,,
```

