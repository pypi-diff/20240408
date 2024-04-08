# Comparing `tmp/qodex_cameras-2.1.7-py3-none-any.whl.zip` & `tmp/qodex_cameras-2.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 39881 bytes, number of entries: 18
+Zip file size: 39866 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 06:46 qodex_cameras/__init__.py
 -rw-rw-rw-  2.0 fat      166 b- defN 23-May-02 11:08 qodex_cameras/functions.py
--rw-rw-rw-  2.0 fat     2950 b- defN 24-Feb-26 14:00 qodex_cameras/main.py
--rw-rw-rw-  2.0 fat     3420 b- defN 24-Feb-26 13:21 qodex_cameras/mixins.py
+-rw-rw-rw-  2.0 fat     3092 b- defN 24-Apr-08 10:46 qodex_cameras/main.py
+-rw-rw-rw-  2.0 fat     3402 b- defN 24-Apr-08 11:06 qodex_cameras/mixins.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-12 08:58 qodex_cameras/settings.py
 -rw-rw-rw-  2.0 fat     2007 b- defN 24-Apr-01 15:03 qodex_cameras/video_saver.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 04:44 qodex_cameras/other/__init__.py
 -rw-rw-rw-  2.0 fat     6078 b- defN 23-May-02 04:46 qodex_cameras/other/pyhik_mode.py
 -rw-rw-rw-  2.0 fat     7365 b- defN 23-May-12 06:25 qodex_cameras/photos/Test.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 05:38 qodex_cameras/photos/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 12:07 qodex_cameras/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 24-Feb-21 14:19 qodex_cameras/tests/main_tests.py
 -rw-rw-rw-  2.0 fat    26529 b- defN 23-May-12 08:58 qodex_cameras/tests/test.png
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-01 15:03 qodex_cameras-2.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      304 b- defN 24-Apr-01 15:03 qodex_cameras-2.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 15:03 qodex_cameras-2.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-01 15:03 qodex_cameras-2.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1508 b- defN 24-Apr-01 15:03 qodex_cameras-2.1.7.dist-info/RECORD
-18 files, 53280 bytes uncompressed, 37383 bytes compressed:  29.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-08 11:08 qodex_cameras-2.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      304 b- defN 24-Apr-08 11:08 qodex_cameras-2.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 11:08 qodex_cameras-2.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-08 11:08 qodex_cameras-2.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1508 b- defN 24-Apr-08 11:08 qodex_cameras-2.1.8.dist-info/RECORD
+18 files, 53404 bytes uncompressed, 37368 bytes compressed:  30.0%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: qodex_cameras/tests/main_tests.py
 Comment: 
 
 Filename: qodex_cameras/tests/test.png
 Comment: 
 
-Filename: qodex_cameras-2.1.7.dist-info/LICENSE
+Filename: qodex_cameras-2.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: qodex_cameras-2.1.7.dist-info/METADATA
+Filename: qodex_cameras-2.1.8.dist-info/METADATA
 Comment: 
 
-Filename: qodex_cameras-2.1.7.dist-info/WHEEL
+Filename: qodex_cameras-2.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_cameras-2.1.7.dist-info/top_level.txt
+Filename: qodex_cameras-2.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_cameras-2.1.7.dist-info/RECORD
+Filename: qodex_cameras-2.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qodex_cameras/main.py

```diff
@@ -31,26 +31,30 @@
         self.stop_record_thumb = None
 
     def get_photo_rest(self):
         return self.get_http_photo()
 
     def start_record(self, rtsp_stream_link=None, output="output.avi"):
         self.output = output
-        self.start_record_thumb = self.make_pic()
+        pic_res = self.make_pic()
+        if not pic_res["error"]:
+            self.start_record_thumb = pic_res
         rtsp_stream_link = f"rtsp://{self.cam_login}:{self.cam_pass}@{self.ip}:{self.rtsp_port}/Streaming/Channels/101"
         super(HikCamera, self).start_record(
             rtsp_stream_link=rtsp_stream_link, output=output)
 
     def stop_record(self):
         threading.Thread(target=self.make_stop_record_thumb).start()
         super(HikCamera, self).stop_record()
         return self.output
 
     def make_stop_record_thumb(self):
-        self.stop_record_thumb = self.make_pic()
+        pic_res = self.make_pic()
+        if not pic_res["error"]:
+            self.start_record_thumb = pic_res
 
 class HikCameraCarNumberRecognition(HikCamera,
                                     recognition.MailNumberRecognitionRus):
     def __init__(self, ip, port, login, password, mail_token,
                  pics_folder=None, rtsp_port=554, test_mode=False,
                  auth_method="Basic", save_pics=False, photo_type_name=None):
         super().__init__(ip, port, login, password,
@@ -58,11 +62,11 @@
                          test_mode=test_mode,
                          auth_method=auth_method,
                          save_pics=save_pics, photo_type_name=photo_type_name)
         self.set_token(mail_token)
 
     def make_pic(self, name: str = None):
         res = super().make_pic(name=name)
-        if 'error' in res:
+        if not res or 'error' in res:
             return res
         res['car_number'] = self.get_result(res['photo_data'])
         return res
```

## qodex_cameras/mixins.py

```diff
@@ -60,20 +60,18 @@
         if not name:
             name = str(uuid.uuid4())
         if self.test_mode:
             with open(settings.TEST_PHOTO, 'rb') as fobj:
                 photo_data = fobj.read()
         else:
             photo_data = self.take_shot()
-            #img = Image.open(io.BytesIO(photo_data))
-            # left, upper, right, lower
-            # 2592*1944
-            #img.show()
             if not photo_data:
                 return
+            if "error" in photo_data:
+                return photo_data
         result = {'photo_data': photo_data}
         if self.save_pics:
             if not self.pics_folder:
                 self.pics_folder = settings.CUR_DIR
             photo_abs_name = os.sep.join((self.pics_folder, f"{name}.jpg"))
             functions.save_photo(photo_abs_name, photo_data)
             result['abs_path'] = photo_abs_name
@@ -82,22 +80,23 @@
     def take_shot(self):
         logging.info(f"{__name__}. Taking shot....")
         try:
             return self.get_photo_rest()
         except ConnectionError:
             logging.error(
                 f"Connection error: {traceback.format_exc()}")
+            return {"error": traceback.format_exc()}
 
 
 class HttpMakePic:
     auth_method = None
     cam_login = None
     cam_pass = None
     get_photo_url = None
-    get_pic_timeout = 5
+    get_pic_timeout = 2
 
     def get_http_photo(self):
         if self.auth_method == "Basic":
             response = requests.get(
                 self.get_photo_url,
                 auth=HTTPBasicAuth(self.cam_login, self.cam_pass),
                 timeout=self.get_pic_timeout)
```

## Comparing `qodex_cameras-2.1.7.dist-info/LICENSE` & `qodex_cameras-2.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qodex_cameras-2.1.7.dist-info/RECORD` & `qodex_cameras-2.1.8.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 qodex_cameras/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/functions.py,sha256=elNHnnx3zelcKnAOLK3E6ETMpV3PZPXfWclPRYSqiZA,166
-qodex_cameras/main.py,sha256=B-zYsIiD9j2nEA2VHG9PEwTdbMFr9FTd15_aWPV5vP8,2950
-qodex_cameras/mixins.py,sha256=DAl-7bRFCuKAQCOfwPum-O6meBmrm6r41SGSd3fLnFM,3420
+qodex_cameras/main.py,sha256=mH6cJTTieW6TJ2kATkve60Hm46V8athW8bTeZ2KUXwo,3092
+qodex_cameras/mixins.py,sha256=hWruKtza2KmdvyFHf-MFPo61Ur4igheoJAjUj0eBFXA,3402
 qodex_cameras/settings.py,sha256=xupNck2qOhJLj0WQjB47Z6dm179vhVF1FJ-dDcgX4c0,384
 qodex_cameras/video_saver.py,sha256=ebzsVuUQuKxO_Jv8Z7yFZdYx8XEI3ZkfyAo7b-Gutpg,2007
 qodex_cameras/other/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/other/pyhik_mode.py,sha256=FyG_QWVdcTi5dnSwv3Iq-L0H4PYW6wKBeVJpkYRt58Q,6078
 qodex_cameras/photos/Test.png,sha256=v54Of9PyXTQ-X6_ji_105kC2ISyuxG6UxJDBzcdV4ac,7365
 qodex_cameras/photos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/main_tests.py,sha256=2i8_idlYsYF6jL10A36VtsOPbH-HofShSKPyBkdVAPo,1372
 qodex_cameras/tests/test.png,sha256=EZ4YZtPhTRLJBM2ZMr-ZyXqVMKgYlmW-25syShwy_8s,26529
-qodex_cameras-2.1.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-qodex_cameras-2.1.7.dist-info/METADATA,sha256=UBJt9Rtn7NupQly-n00sfWhmv0GsHIxpR69weF3brSc,304
-qodex_cameras-2.1.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-qodex_cameras-2.1.7.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
-qodex_cameras-2.1.7.dist-info/RECORD,,
+qodex_cameras-2.1.8.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+qodex_cameras-2.1.8.dist-info/METADATA,sha256=-WnR9jIBrq9lLqQJwueR7AGmPBReuqmMlOgooJmb6ow,304
+qodex_cameras-2.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+qodex_cameras-2.1.8.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
+qodex_cameras-2.1.8.dist-info/RECORD,,
```

