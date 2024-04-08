# Comparing `tmp/smartcard_identifier-1.7.3.tar.gz` & `tmp/smartcard_identifier-1.8.1.tar.gz`

## Comparing `smartcard_identifier-1.7.3.tar` & `smartcard_identifier-1.8.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/Makefile
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/macOS/com.shortstorybox.SmartcardIdentifier.plist
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/macOS/distribution.xml
--rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/macOS/scripts/postinstall
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/macOS/scripts/preinstall
--rwxr-xr-x   0        0        0     5968 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/src/smartcard_identifier.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/LICENSE
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/pyproject.toml
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 smartcard_identifier-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/Makefile
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/com.shortstorybox.SmartcardIdentifier.plist
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/distribution.xml
+-rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/scripts/postinstall
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/scripts/preinstall
+-rwxr-xr-x   0        0        0     5980 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/src/smartcard_identifier.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/LICENSE
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/PKG-INFO
```

### Comparing `smartcard_identifier-1.7.3/Makefile` & `smartcard_identifier-1.8.1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	rm -rf dist/
 	python3 -m pip install build
 	python3 -m build
 
 .PHONY: lint
 lint:
 	python3 -m pip install ruff black isort
-	python3 -m ruff src/
+	python3 -m ruff check src/
 	@python3 -m black --check src/ || (echo "Please run 'make format' to fix formatting issues."; exit 1)
 	@python3 -m isort src/ || (echo "Please run 'make format' to fix formatting issues."; exit 1)
 
 .PHONY: format
 format:
 	python3 -m pip install black isort
 	python3 -m black src/
```

### Comparing `smartcard_identifier-1.7.3/macOS/distribution.xml` & `smartcard_identifier-1.8.1/macOS/distribution.xml`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.7.3/src/smartcard_identifier.py` & `smartcard_identifier-1.8.1/src/smartcard_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
             SUCCESS = (0x90, 0x00)
             if (sw1, sw2) == SUCCESS:
                 card_id = hexlify(bytes(response)).decode("ascii").upper()
                 if print_only:
                     print(card_id)
                 else:
-                    simulate_keypress(card_id, use_linux_uinput=use_linux_uinput)
+                    simulate_keypress(card_id + "\n", use_linux_uinput=use_linux_uinput)
             else:
                 sys.stderr.write("Failed to read card ID\n")
                 sys.stderr.flush()
         finally:
             card.connection.disconnect()
 
 
@@ -129,15 +129,15 @@
     )
     group.add_argument(
         "--uinput",
         action="store_true",
         help="Use uinput to simulate keypresses. Requires user to be in the 'input' group, or to run as root. (Linux only)",
     )
     group.add_argument(
-        "--print",
+        "--stdout",
         action="store_true",
         help="Print the card ID to stdout instead of simulating keypresses.",
     )
     args = parser.parse_args()
     if args.test_permissions:
         if platform_system() != "Darwin":
             sys.exit("ERROR: --test-permissions is only supported on macOS")
@@ -155,24 +155,24 @@
             shutil.which("ydotool") or sys.exit(
                 "Please install `ydotool`, e.g.:\n\n    $ sudo apt-get install ydotoold ydotool"
             )
         elif args.x11:
             shutil.which("xdotool") or sys.exit(
                 "Please install `xdotool`, e.g.:\n\n    $ sudo apt-get install xdotool"
             )
-        elif args.print:
+        elif args.stdout:
             pass
         else:
             parser.print_help()
-            sys.exit("ERROR: You must specify either --x11 or --uinput or --print")
+            sys.exit("ERROR: You must specify either --x11 or --uinput or --stdout")
 
     def do_run(*_, **__):
-        run(print_only=args.print, use_linux_uinput=args.uinput)
+        run(print_only=args.stdout, use_linux_uinput=args.uinput)
 
-    if args.print:
+    if args.stdout:
         # Disable keyboard echoing on the terminal, which can cause confusion
         # if the script is running at the same time somewhere else
         _raw_input = getpass._raw_input
         try:
             getpass._raw_input = do_run
             getpass.getpass("")
         finally:
```

### Comparing `smartcard_identifier-1.7.3/.gitignore` & `smartcard_identifier-1.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.7.3/LICENSE` & `smartcard_identifier-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.7.3/README.md` & `smartcard_identifier-1.8.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -38,7 +38,20 @@
 
 
 To build & publish a release, first increment the version in pyproject.toml,
 then run the following to build and upload to Github and PyPI:
 
     $ make release
 
+# Notes
+
+If you run into the following error installing via `pip3 install smartcard-identifier` on macOS:
+
+    × Building wheel for pyscard (pyproject.toml) did not run successfully.
+    │ exit code: 1
+    ╰─> [5 lines of output]
+        running bdist_wheel
+        running build
+        running build_py
+        Install swig and try again
+
+then you can fix the above error by running `brew install swig`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smartcard_identifier-1.7.3/pyproject.toml` & `smartcard_identifier-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "smartcard-identifier"
-version = "1.7.3"
+version = "1.8.1"
 authors = [
   { name="Samuel Hoffstaetter", email="sam@shortstorybox.com" },
 ]
 description = "Read smart card ID number and emulate a keyboard to paste it as text."
 readme = "README.md"
 requires-python = ">=3.3"
 classifiers = [
```

### Comparing `smartcard_identifier-1.7.3/PKG-INFO` & `smartcard_identifier-1.8.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smartcard-identifier
-Version: 1.7.3
+Version: 1.8.1
 Summary: Read smart card ID number and emulate a keyboard to paste it as text.
 Project-URL: Homepage, https://github.com/shortstorybox/smartcard-identifier
 Project-URL: Issues, https://github.com/shortstorybox/smartcard-identifier/issues
 Author-email: Samuel Hoffstaetter <sam@shortstorybox.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
@@ -55,7 +55,20 @@
 
 
 To build & publish a release, first increment the version in pyproject.toml,
 then run the following to build and upload to Github and PyPI:
 
     $ make release
 
+# Notes
+
+If you run into the following error installing via `pip3 install smartcard-identifier` on macOS:
+
+    × Building wheel for pyscard (pyproject.toml) did not run successfully.
+    │ exit code: 1
+    ╰─> [5 lines of output]
+        running bdist_wheel
+        running build
+        running build_py
+        Install swig and try again
+
+then you can fix the above error by running `brew install swig`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

