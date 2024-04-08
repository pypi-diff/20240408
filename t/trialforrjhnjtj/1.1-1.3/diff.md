# Comparing `tmp/trialforrjhnjtj-1.1.tar.gz` & `tmp/trialforrjhnjtj-1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trialforrjhnjtj-1.1.tar", last modified: Sun Apr  7 18:41:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

