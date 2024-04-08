# Comparing `tmp/hich_restrict-0.1.2-py3-none-any.whl.zip` & `tmp/hich_restrict-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6905 bytes, number of entries: 10
+Zip file size: 6919 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 hich_restrict/__init__.py
--rw-r--r--  2.0 unx     1300 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
+-rw-r--r--  2.0 unx     1331 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
 -rw-r--r--  2.0 unx     4202 b- defN 80-Jan-01 00:00 hich_restrict/contacts.py
 -rw-r--r--  2.0 unx     4343 b- defN 80-Jan-01 00:00 hich_restrict/fragments.py
 -rw-r--r--  2.0 unx     3761 b- defN 80-Jan-01 00:00 hich_restrict/restrict_manager.py
 -rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 hich_restrict/timer.py
--rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.2.dist-info/RECORD
-10 files, 16307 bytes uncompressed, 5501 bytes compressed:  66.3%
+-rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.3.dist-info/RECORD
+10 files, 16338 bytes uncompressed, 5515 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: hich_restrict/restrict_manager.py
 Comment: 
 
 Filename: hich_restrict/timer.py
 Comment: 
 
-Filename: hich_restrict-0.1.2.dist-info/METADATA
+Filename: hich_restrict-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: hich_restrict-0.1.2.dist-info/WHEEL
+Filename: hich_restrict-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: hich_restrict-0.1.2.dist-info/entry_points.txt
+Filename: hich_restrict-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: hich_restrict-0.1.2.dist-info/RECORD
+Filename: hich_restrict-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hich_restrict/__main__.py

```diff
@@ -14,14 +14,16 @@
 @click.option("--output-pairs",
     type=str,
     help="Filename for output .pairs file")
 @click.argument("frag-file")
 @click.argument("input-pairs")
 def cli(frag_file_format, output_pairs, frag_file, input_pairs):
     """
+    hich-restrict v 0.1.3
+    
     frag-file: a non-compressed plaintext file containing fragments. All
     fragments from a particular chromosome must be in one contiguous block,
     with ascending coordinates. All fragments in a chromosome must be
     adjacent (frag_n start = frag_n-1 end + 1).
 
     input-pairs: a text file containing pairs in .pairs format. Can be
     plaintext or compressed with gzip (.gz, .gzip) or lz4 (.lz4).
```

## Comparing `hich_restrict-0.1.2.dist-info/RECORD` & `hich_restrict-0.1.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 hich_restrict/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hich_restrict/__main__.py,sha256=E2qjk90I-smYKcc7z4aLFQSTHqS1enDBMjb3OpivV58,1300
+hich_restrict/__main__.py,sha256=Qy6eE7SYZv7brHAvm-fRzwRqV7vqmxlLRfF9bIDESy4,1331
 hich_restrict/contacts.py,sha256=088NMTKygzd43V2vPlkfj3_Fzybw04YIBInUoVWd0BM,4202
 hich_restrict/fragments.py,sha256=oY7ceSjTIYauV1gElRvKrnF1LCJqwfNr7VqcfIvmNZ8,4343
 hich_restrict/restrict_manager.py,sha256=M2Ll_VylhjRhUSWcRxibpTnw78__rDc6oVosm3T28go,3761
 hich_restrict/timer.py,sha256=VhkDub_yc5dQmXwHfKRQjFuFD_S64bpMl9akkSbNrOA,1289
-hich_restrict-0.1.2.dist-info/METADATA,sha256=6w3uaija3FU7uhhocbmpqZY5sVb3GzBQ6hV88NgZlM4,445
-hich_restrict-0.1.2.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-hich_restrict-0.1.2.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
-hich_restrict-0.1.2.dist-info/RECORD,,
+hich_restrict-0.1.3.dist-info/METADATA,sha256=tpN5yYDZaG3EsuLirJ3wVux6H8U672OsiUwU4xhABD4,445
+hich_restrict-0.1.3.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+hich_restrict-0.1.3.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
+hich_restrict-0.1.3.dist-info/RECORD,,
```

