# Comparing `tmp/dcx-0.75.0.tar.gz` & `tmp/dcx-0.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcx-0.75.0.tar", last modified: Wed Mar 20 19:19:34 2024, max compression
+gzip compressed data, was "dcx-0.76.0.tar", last modified: Mon Apr  8 16:25:18 2024, max compression
```

## Comparing `dcx-0.75.0.tar` & `dcx-0.76.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-20 19:19:34.675376 dcx-0.75.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.75.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-03-20 19:19:34.675214 dcx-0.75.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.75.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-03-20 19:19:32.000000 dcx-0.75.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-03-20 19:19:34.675413 dcx-0.75.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-20 19:19:34.673047 dcx-0.75.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-20 19:19:34.673723 dcx-0.75.0/src/dcx/
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.75.0/src/dcx/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)    63636 2024-03-20 19:19:24.000000 dcx-0.75.0/src/dcx/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-20 19:19:34.675065 dcx-0.75.0/src/dcx.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-03-20 19:19:34.000000 dcx-0.75.0/src/dcx.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-03-20 19:19:34.000000 dcx-0.75.0/src/dcx.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-03-20 19:19:34.000000 dcx-0.75.0/src/dcx.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-03-20 19:19:34.000000 dcx-0.75.0/src/dcx.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-03-20 19:19:34.000000 dcx-0.75.0/src/dcx.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.418844 dcx-0.76.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.76.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:25:18.418657 dcx-0.76.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.76.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-08 16:25:16.000000 dcx-0.76.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-08 16:25:18.418886 dcx-0.76.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.416234 dcx-0.76.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.417042 dcx-0.76.0/src/dcx/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.76.0/src/dcx/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)    64762 2024-04-08 16:14:29.000000 dcx-0.76.0/src/dcx/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:25:18.418488 dcx-0.76.0/src/dcx.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-08 16:25:18.000000 dcx-0.76.0/src/dcx.egg-info/top_level.txt
```

### Comparing `dcx-0.75.0/PKG-INFO` & `dcx-0.76.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.75.0
+Version: 0.76.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcx-0.75.0/pyproject.toml` & `dcx-0.76.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcx"
-version = "0.75.0"
+version = "0.76.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "Minimalistic selenium wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dcx-0.75.0/src/dcx/__main__.py` & `dcx-0.76.0/src/dcx/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 import rich
 from rich.console import Console
 
 from selenium.webdriver.firefox.options import Options as FFOptions
 from selenium.webdriver.chrome.options import Options as CHOptions
 from selenium.webdriver.edge.options import Options as EDOptions
+from selenium.webdriver.safari.options import Options as SAOptions
+
 from selenium import webdriver
 
 from selenium.webdriver.common.keys import Keys as KEYS
 from selenium.webdriver.common.by import By as BY
 
 from selenium.webdriver.support.ui import WebDriverWait as WDW
 from selenium.webdriver.support.ui import Select as SEL
@@ -47,16 +49,18 @@
 figlet = base64.b64decode(const_figlet).decode()
 parser = argparse.ArgumentParser(prog="dcx", epilog=epilog, formatter_class=argparse.RawTextHelpFormatter, description="DAISY CHAINED XPATH processor (v%s) - commandline tool to run JSON defined selenium scripts.\n\n%s\n" % (const_appversion, figlet))
 parser.add_argument("--gen", action="store_true", help="Generate a play.js and play.env if non existing and QUIT")
 parser.add_argument("--format", action="store_true", help="Only reformat play.js and exit")
 parser.add_argument("--no-dev", action="store_true", help="Disable Developer Tools Auto-Open (Only Firefox)")
 parser.add_argument("--no-img", action="store_true", help="Disable screenshots")
 parser.add_argument("--log", action="store_true", help="Don't flush directory 'log'")
+parser.add_argument("--reg", action="store_true", help="Extract reg as reg.zip to the CWD after execution")
 parser.add_argument("--local-chrome", action="store_true", help="Use local 'Google Chrome' and not 'Firefox'")
 parser.add_argument("--local-edge", action="store_true", help="Use local 'Google Chrome' and not 'Firefox'")
+parser.add_argument("--local-safari", action="store_true", help="Use local 'Safari' and not 'Firefox'")
 parser.add_argument("--remote-edge", action="store_true", help="Use remote edge")
 parser.add_argument("--remote-firefox", action="store_true", help="Use remote firefox")
 parser.add_argument("--remote-chrome", action="store_true", help="Use remote chrome")
 parser.add_argument("--remote-host", nargs=1, type=str, default=["127.0.0.1"], help="Default is 127.0.0.1")
 parser.add_argument("--remote-port", nargs=1, type=int, default=[4444], help="Default is 4444")
 parser.add_argument("--unzip-profile", nargs=1, type=str, help="PK-Zipped profile contents (flat) -- FIREFOX ONLY")
 parser.add_argument("--zip-profile", metavar="ZIP_PREFIX", nargs=1, type=str, help="ZIP Profile after execution (leave out the '.zip' !) -- FIREFOX ONLY")
@@ -279,14 +283,19 @@
     driver = webdriver.Chrome(options=chrome_options)
 
 if args.local_edge:
     driver_mode = "local-edge"
     chrome_options = EDOptions()
     driver = webdriver.Edge(options=chrome_options)
 
+if args.local_safari:
+    driver_mode = "local-safari"
+    chrome_options = SAOptions()
+    driver = webdriver.Safari(options=chrome_options)
+
 if driver == None:
     if args.headless:
         opts.add_argument("--headless")
     
     if args.unzip_profile:
         unzip_profile_filename = args.unzip_profile[0]
         logging.info("Unzipping profile %s" % unzip_profile_filename)
@@ -370,15 +379,20 @@
         ac = ['_' for x in href if x=="/"]
         if len(ac) >= min_slashes:
             all_href[href] = True
     return sorted(list(all_href.keys()))
 
 play = None
 
-def process_report():
+def process_report(logbasedir_):
+    if args.reg:
+        if os.path.exists("reg.zip"):
+            os.unlink("reg.zip")
+        shutil.make_archive("reg", "zip", os.path.join(logbasedir_, "reg"))
+
     if args.report:
         logging.info("Building report...")
         report_filename = os.path.join(logbasedir, args.report_filename[0])
         import turbowriter
         import PIL.Image
         
         pdf = turbowriter.DINA3()
@@ -558,15 +572,15 @@
             print("  %s = %s" % (x, reg_read(x)))
     if data == "q":
         print("QUIT")
         if args.zip_profile:
             postrun_profile_zip = args.zip_profile[0]
             shutil.make_archive(postrun_profile_zip, "zip", profiledir_actual)
 
-        process_report()
+        process_report(logbasedir)
 
         driver.quit()
         if args.log == False:
             shutil.rmtree(logbasedir)
         sys.exit(0)
 
 # src=["b", "n"], l=2, idx=1
@@ -929,14 +943,25 @@
                 if play_part[1] == "js64str":###ntcommand
                     varname = play_part[2]
                     code_plain = base64.b64decode(play_part[3]).decode("utf-8")
                     res = str(driver.execute_script(code_plain))
                     reg_write(varname, res)
                     unknown_command=False
 
+                if play_part[1] == "reg_href":###ntcommand
+                    varname = play_part[2]
+                    newdata = driver.execute_script('return location.href;').strip()
+                    olddata=""
+                    if "+" in varname:
+                        # append mode
+                        varname = varname.replace("+", "")
+                        olddata = reg_read(varname)
+                    reg_write(varname, olddata + newdata)
+                    unknown_command=False
+
                 if play_part[1] == "reg_str":###ntcommand
                     varname = play_part[2]
                     newdata = expand_column(play_part, 3)
                     olddata=""
                     if "+" in varname:
                         # append mode
                         varname = varname.replace("+", "")
@@ -996,30 +1021,30 @@
                         print()
                         input_data = input("$ ").strip().split("\n")[0].strip()
                         print()
                         print("*"*68)
                         lel[0].send_keys(input_data)
                         unknown_command=False
 
+                    if play_part[1] == "enter": ###tcommand
+                        lel[0].send_keys("\r")
+                        unknown_command=False
+
                     if play_part[1] == "input_password_type": ###tcommand
                         input_caption = expand_column(play_part, 2)
                         print("*"*68)
                         print("** %s" % input_caption)
                         print("*"*68)
                         print()
                         input_data = getpass.getpass()
                         print()
                         print("*"*68)
                         lel[0].send_keys(input_data)
                         unknown_command=False
 
-                    if play_part[1] == "enter": ###tcommand
-                        lel[0].send_keys("\n")
-                        unknown_command=False
-
                     if play_part[1] == "submit": ###tcommand
                         lel[0].submit()
                         unknown_command=False
 
                     if play_part[1] == "input_setvalue": ###tcommand
                         input_caption = expand_column(play_part, 2)
                         print("*"*68)
@@ -1175,15 +1200,15 @@
 # driver.save_screenshot("test.png")
 
 if args.zip_profile:
     postrun_profile_zip = args.zip_profile[0]
     shutil.make_archive(postrun_profile_zip, "zip", profiledir_actual)
 
 
-process_report()
+process_report(logbasedir)
 
 driver.quit()
 logging.info("finished")
 
 
 if args.post_bash == None:
     logging.info("no POST task")
```

### Comparing `dcx-0.75.0/src/dcx.egg-info/PKG-INFO` & `dcx-0.76.0/src/dcx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.75.0
+Version: 0.76.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

