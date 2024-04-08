# Comparing `tmp/langcheck-0.5.0.tar.gz` & `tmp/langcheck-0.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcheck-0.5.0.tar", last modified: Mon Mar 11 08:28:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

