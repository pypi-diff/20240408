# Comparing `tmp/dwiqc-1.5.2-py2.py3-none-any.whl.zip` & `tmp/dwiqc-1.5.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 36596 bytes, number of entries: 25
+Zip file size: 36672 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      225 b- defN 24-Jan-23 14:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 24-Apr-03 15:44 dwiqc/__version__.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Jan-23 14:11 dwiqc/browser/__init__.py
+-rw-r--r--  2.0 unx      247 b- defN 24-Apr-08 13:57 dwiqc/__version__.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-08 13:56 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       94 b- defN 24-Jan-23 14:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     5610 b- defN 24-Jan-23 14:11 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     6898 b- defN 24-Jan-23 14:11 dwiqc/cli/install_containers.py
--rw-r--r--  2.0 unx     7114 b- defN 24-Mar-20 20:01 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     7134 b- defN 24-Apr-08 13:55 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     6157 b- defN 24-Jan-23 14:11 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      383 b- defN 24-Jan-23 14:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      346 b- defN 24-Jan-23 14:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx      280 b- defN 24-Jan-23 14:11 dwiqc/config/prequal.yaml
 -rw-r--r--  2.0 unx      240 b- defN 24-Jan-23 14:11 dwiqc/config/qsiprep.yaml
 -rw-r--r--  2.0 unx       98 b- defN 24-Jan-23 14:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 24-Jan-23 14:11 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    21296 b- defN 24-Mar-21 19:17 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4871 b- defN 24-Apr-03 14:42 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx    16340 b- defN 24-Mar-21 19:18 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     6265 b- defN 24-Apr-03 14:43 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    11891 b- defN 24-Jan-23 14:11 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     8394 b- defN 24-Apr-03 15:45 dwiqc-1.5.2.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 24-Apr-03 15:45 dwiqc-1.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      589 b- defN 24-Apr-03 15:45 dwiqc-1.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-03 15:45 dwiqc-1.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-03 15:45 dwiqc-1.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1969 b- defN 24-Apr-03 15:45 dwiqc-1.5.2.dist-info/RECORD
-25 files, 104279 bytes uncompressed, 33454 bytes compressed:  67.9%
+-rwxr-xr-x  2.0 unx     8394 b- defN 24-Apr-08 13:58 dwiqc-1.5.3.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 24-Apr-08 13:58 dwiqc-1.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      589 b- defN 24-Apr-08 13:58 dwiqc-1.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-08 13:58 dwiqc-1.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-08 13:58 dwiqc-1.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1969 b- defN 24-Apr-08 13:58 dwiqc-1.5.3.dist-info/RECORD
+25 files, 104488 bytes uncompressed, 33530 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -51,26 +51,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-1.5.2.data/scripts/dwiQC.py
+Filename: dwiqc-1.5.3.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-1.5.2.dist-info/LICENSE
+Filename: dwiqc-1.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-1.5.2.dist-info/METADATA
+Filename: dwiqc-1.5.3.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-1.5.2.dist-info/WHEEL
+Filename: dwiqc-1.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-1.5.2.dist-info/top_level.txt
+Filename: dwiqc-1.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-1.5.2.dist-info/RECORD
+Filename: dwiqc-1.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '1.5.2'
+__version__ = '1.5.3'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/browser/__init__.py

```diff
@@ -5,18 +5,25 @@
 from pathlib import Path
 import mimetypes
 import os
 logger = logging.getLogger(__name__)
 home_dir = os.path.expanduser("~")
 
 
-def snapshot(url, saveto):
-	proc1 = f'{home_dir}/.config/dwiqc/containers/chromium.sif --no-sandbox --headless --print-to-pdf={saveto} {url}'
-	output = subprocess.Popen(proc1, shell=True, stderr=subprocess.PIPE)
+def snapshot(url, saveto, container_dir):
+	proc1 = f'{container_dir}/chromium.sif --no-sandbox --headless --print-to-pdf={saveto} {url}'
+	output = subprocess.Popen(proc1, shell=True, stdout=subprocess.PIPE)
 	output.communicate()
+    code = output.returncode
+
+    if code == 0:
+        logging.info('pdf conversion successful!')
+    else:
+        logging.error('pdf conversion threw an error. exiting.')
+        sys.exit(1)
 
 def imbed_images(infile, outfile=None):
     infile = Path(infile)
     if not outfile:
         outfile = infile.with_stem(f'{infile.stem}-imbedded_images')
     os.chdir(infile.parent)
     logger.info(f'reading {infile}')
```

## dwiqc/cli/process.py

```diff
@@ -128,15 +128,15 @@
         numjobs = len(jarray.array)
         failed = len(jarray.failed)
         complete = len(jarray.complete)
         if 'prequal' in args.sub_tasks:
             prequal_eddy(args, prequal_outdir)
         if 'qsiprep' in args.sub_tasks:
             qsiprep_eddy(args, qsiprep_outdir)
-            browser.snapshot(f"{qsiprep_outdir}/qsiprep/sub-{args.sub}.html", f"{qsiprep_outdir}/qsiprep/qsiprep.pdf")
+            browser.snapshot(f"{qsiprep_outdir}/qsiprep/sub-{args.sub}.html", f"{qsiprep_outdir}/qsiprep/qsiprep.pdf", args.container_dir)
             browser.imbed_images(f"{qsiprep_outdir}/qsiprep/sub-{args.sub}.html")
         if failed:
             logger.info('%s/%s jobs failed', failed, numjobs)
             for pid,job in iter(jarray.failed.items()):
                 logger.error('%s exited with returncode %s', job.name, job.returncode)
                 with open(job.output, 'r') as fp:
                     logger.error('standard output\n%s', fp.read())
```

## Comparing `dwiqc-1.5.2.data/scripts/dwiQC.py` & `dwiqc-1.5.3.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-1.5.2.dist-info/LICENSE` & `dwiqc-1.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-1.5.2.dist-info/METADATA` & `dwiqc-1.5.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwiqc
-Version: 1.5.2
+Version: 1.5.3
 Summary: Quality Assurance Pipeline for Diffusion MR Data
 Home-page: https://github.com/harvard-nrg/dwiqc
 Author: Neuroinformatics Research Group
 Author-email: info@neuroinfo.org
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
```

## Comparing `dwiqc-1.5.2.dist-info/RECORD` & `dwiqc-1.5.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=zp8RPUe8MdTEPiDdXLPI1B172c5tkBwxqVwPI6GLUPQ,247
-dwiqc/browser/__init__.py,sha256=ZjDP9HeQSX3gbTqEXfhD1WPDymxZB04CbHfHviDFJmU,1423
+dwiqc/__version__.py,sha256=H3Mg_SwmcfTxrj48_J0TbBroeaPZh_YwywikQztXM4E,247
+dwiqc/browser/__init__.py,sha256=FXzQU8JpfBQLKgEZgo1MI2FtjFH-DCmSJqWE5e4ak3s,1612
 dwiqc/cli/__init__.py,sha256=QD5zUAU1PHaJdE14htZyZCCUOYQ1rHHMtT2v8lBF8QE,94
 dwiqc/cli/get.py,sha256=UA9W5wm-Qo-WU-agCVv0-IaqmQVKhDwo_NvbozhssOU,5610
 dwiqc/cli/install_containers.py,sha256=KJD3YRSrD37uOHEhHTWge82WQ2qzXGIh2Wfz2W-5dg4,6898
-dwiqc/cli/process.py,sha256=JaLlzWmGnFSG_Lt-Ha5l8nLnhC9wpA3Z_d2dMWsGYp8,7114
+dwiqc/cli/process.py,sha256=CpyxpCOp3LU6VIlrBsD-xOj6xL2Il_yTGrqQIg1PaDU,7134
 dwiqc/cli/tandem.py,sha256=_Vu_B_rZFgd_z1VlUDv1y7PouPJAuuPBhEO-FM0bye4,6157
 dwiqc/config/__init__.py,sha256=X33iA2gj1lDc6fsIYPUcqvZUDV--IphhJY4JTNd-Yg0,383
 dwiqc/config/dwiqc.yaml,sha256=ENgw52j0yn91y__VCQvWMLHkVa7JWuxB2HOIJ0fc3z4,346
 dwiqc/config/prequal.yaml,sha256=GNsaaGw7znyBEl7EjNVZna0mL8IB27R9TdZnAAFJfP8,280
 dwiqc/config/qsiprep.yaml,sha256=dXKCXS_3MLwE_v3PwjklNcakfTtjE9UF_alW4vari74,240
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=J1JqZLKo5uysrRM7MYxXjBhMectQiRfS0le6FGNbmHI,21296
 dwiqc/tasks/prequal_EQ.py,sha256=VU8ELYSzl7GSLNRCT7OkyRAyWBMIhKE9by1E6saNf4I,4871
 dwiqc/tasks/qsiprep.py,sha256=sW2Ae3ZIhpfuz8V1kwtjERbHwJq7ptCcZOnpltkSqeI,16340
 dwiqc/tasks/qsiprep_EQ.py,sha256=MOcJW9dRPxjhJIGHnI345i-ZTHmFRWtRccyfcuzRGUA,6265
 dwiqc/xnat/__init__.py,sha256=-rgbMvQOqHpc69rFsfNSYVG-bou_FilPmRdrjCbe9Kc,11891
-dwiqc-1.5.2.data/scripts/dwiQC.py,sha256=ck90T1qIDfn46wNJFr55csRLHIuX21Fte_muMbr3G00,8394
-dwiqc-1.5.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-1.5.2.dist-info/METADATA,sha256=Sw6D_QS3WTNk5ps592o_6HpoUWMsZVfD5krK-451ygo,589
-dwiqc-1.5.2.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-dwiqc-1.5.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-1.5.2.dist-info/RECORD,,
+dwiqc-1.5.3.data/scripts/dwiQC.py,sha256=ck90T1qIDfn46wNJFr55csRLHIuX21Fte_muMbr3G00,8394
+dwiqc-1.5.3.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-1.5.3.dist-info/METADATA,sha256=QfJk4BhxaiF1yqnSgyOCT5m4NSpJOkDAuNdPw3Jsxks,589
+dwiqc-1.5.3.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+dwiqc-1.5.3.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-1.5.3.dist-info/RECORD,,
```

