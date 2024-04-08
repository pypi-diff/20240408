# Comparing `tmp/bec_client-1.22.1.tar.gz` & `tmp/bec_client-1.22.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_client-1.22.1.tar", last modified: Thu Apr  4 14:29:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

