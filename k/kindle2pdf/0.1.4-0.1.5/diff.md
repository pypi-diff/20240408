# Comparing `tmp/kindle2pdf-0.1.4.tar.gz` & `tmp/kindle2pdf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kindle2pdf-0.1.4.tar", max compression
+gzip compressed data, was "kindle2pdf-0.1.5.tar", max compression
```

## Comparing `kindle2pdf-0.1.4.tar` & `kindle2pdf-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      718 2024-04-06 15:42:50.462637 kindle2pdf-0.1.4/README.md
--rw-r--r--   0        0        0    14333 2024-04-07 08:08:12.007062 kindle2pdf-0.1.4/kindle2pdf.py
--rw-r--r--   0        0        0      461 2024-04-07 07:31:26.444428 kindle2pdf-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 kindle2pdf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-04-07 18:34:12.317348 kindle2pdf-0.1.5/README.md
+-rw-r--r--   0        0        0    14619 2024-04-08 06:53:13.897941 kindle2pdf-0.1.5/kindle2pdf.py
+-rw-r--r--   0        0        0      461 2024-04-08 06:55:02.809198 kindle2pdf-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 kindle2pdf-0.1.5/PKG-INFO
```

### Comparing `kindle2pdf-0.1.4/README.md` & `kindle2pdf-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kindle2pdf-0.1.4/kindle2pdf.py` & `kindle2pdf-0.1.5/kindle2pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 logger = logging.getLogger("kindle2pdf")
 logger.setLevel(logging.INFO)
 handler = logging.StreamHandler()
 handler.setLevel(logging.INFO)
 logger.addHandler(handler)
 
 
+class Kindle2PDFError(Exception):
+    """Base class for other Kindle2PDF exceptions"""
+
+
 class Kindle2PDF:
     """
     A class to convert Kindle book content to a PDF file.
 
     Attributes:
         asin (str): Amazon Standard Identification Number of the book.
         session (dict): A dictionary containing session information for book rendering.
@@ -88,18 +92,17 @@
             "https://read.amazon.com/service/web/register/getDeviceToken",
             params=params,
             cookies=cookies,
             headers=headers,
             timeout=60,
         )
         if response.status_code != 200:
-            logger.error(
+            raise Kindle2PDFError(
                 "Ensure you have logged in recently to https://read.amazon.com in Chrome."
             )
-            return {}
 
         device_session_token = response.json()["deviceSessionToken"]
 
         headers = {"x-adp-session-token": device_session_token}
 
         params = {
             "asin": self.asin,
@@ -111,17 +114,22 @@
             params=params,
             cookies=cookies,
             headers=headers,
             timeout=60,
         )
         response = response.json()
 
+        if response.get("downloadRestrictionReason"):
+            code = response["downloadRestrictionReason"]["reasonCode"]
+            raise Kindle2PDFError(
+                f"Book {self.asin} is not available for download ({code})."
+            )
         if not response.get("isOwned", False):
-            logger.error("Book %s is not owned by you.", self.asin)
-            return {}
+            raise Kindle2PDFError(f"Book {self.asin} is not owned by you.")
+
         auth = response["karamelToken"]
         metadata_url = response["metadataUrl"]
 
         response = requests.get(metadata_url, timeout=60)
         response = response.text[
             response.text.find("loadMetadata(")
             + len("loadMetadata(") : response.text.rfind(");")
@@ -379,16 +387,14 @@
 
                 end_pos = self.render_pdf(
                     jsons=jsons,
                     images=images,
                     pdf_canvas=pdf_canvas,
                     progress=progress,
                 )
-                progress.n = end_pos
-                progress.refresh()
                 start_pos = end_pos + 1
 
         pdf_canvas.save()
 
 
 def main() -> int:
     """
@@ -405,16 +411,20 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("asin", help="ASIN of the book to convert")
     parser.add_argument("--output", help="Optional output PDF file path")
     parser.add_argument(
         "--font-size", help="Font size to use for rendering", default=12
     )
     args = parser.parse_args()
-    kindle2pdf = Kindle2PDF(asin=args.asin, font_size=args.font_size)
-    if not kindle2pdf.session:
+
+    try:
+        kindle2pdf = Kindle2PDF(asin=args.asin, font_size=args.font_size)
+        kindle2pdf.render_book(output_path=args.output)
+    except Kindle2PDFError as e:
+        logger.error(e)
         return 1
-    kindle2pdf.render_book(output_path=args.output)
+
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `kindle2pdf-0.1.4/PKG-INFO` & `kindle2pdf-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kindle2pdf
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Robert Dargavel Smith
 Author-email: teticio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

