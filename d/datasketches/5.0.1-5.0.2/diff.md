# Comparing `tmp/datasketches-5.0.1.tar.gz` & `tmp/datasketches-5.0.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasketches-5.0.1.tar", last modified: Thu Feb  8 04:30:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

