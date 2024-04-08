# Comparing `tmp/dtactions-1.5.7.tar.gz` & `tmp/dtactions-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtactions-1.5.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dtactions-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dtactions-1.5.7.tar` & `dtactions-1.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2548 2023-10-08 16:59:10.396689 dtactions-1.5.7/README.md
--rw-r--r--   0        0        0     1427 2023-10-08 16:59:10.400689 dtactions-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     2026 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/README.md
--rw-r--r--   0        0        0     6640 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/__init__.py
--rw-r--r--   0        0        0    24945 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/autohotkeyactions.py
--rw-r--r--   0        0        0    62583 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/messagefunctions.py
--rw-r--r--   0        0        0    67137 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/monitorfunctions.py
--rw-r--r--   0        0        0    21534 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/natlinkclipboard.py
--rw-r--r--   0        0        0      196 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/samples/autohotkey/getintoforeground.ahk
--rw-r--r--   0        0        0       48 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/samples/autohotkey/showmessageswindow.ahk
--rw-r--r--   0        0        0    11847 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/samples/unimacro/unimacroactions.ini
--rw-r--r--   0        0        0    45180 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/scintillacon.py
--rw-r--r--   0        0        0     1366 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/sendkeys.py
--rw-r--r--   0        0        0        0 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/__init__.py
--rw-r--r--   0        0        0     5751 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/actionbases.py
--rw-r--r--   0        0        0     2519 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/code-actions.py
--rw-r--r--   0        0        0    16039 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/excel-actions.py
--rw-r--r--   0        0        0     4918 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/frescobaldi-actions.py
--rw-r--r--   0        0        0     3233 2023-10-08 16:59:10.400689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/komodo-actions.py
--rw-r--r--   0        0        0     2862 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/notreadykomodo-actions.py
--rw-r--r--   0        0        0      773 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/pythonwin-actions.py
--rw-r--r--   0        0        0     1521 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/uedit32-actions.py
--rw-r--r--   0        0        0     1655 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/uedit64-actions.py
--rw-r--r--   0        0        0     1084 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/actionclasses/win32pad-actions.py
--rw-r--r--   0        0        0     4576 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/ding.wav
--rw-r--r--   0        0        0    15004 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/extenvvars.py
--rw-r--r--   0        0        0    75728 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/inivars.py
--rw-r--r--   0        0        0    78484 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/newactions.py
--rw-r--r--   0        0        0    79429 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/unimacroactions.py
--rw-r--r--   0        0        0    62644 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/unimacroutils.py
--rw-r--r--   0        0        0       15 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/usc_functions.py
--rw-r--r--   0        0        0    39529 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/unimacro/utilsqh.py
--rw-r--r--   0        0        0    14962 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/vocola_sendkeys/ExtendedSendDragonKeys.py
--rw-r--r--   0        0        0    20101 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/vocola_sendkeys/SendInput.py
--rw-r--r--   0        0        0      303 2023-10-08 16:59:10.404689 dtactions-1.5.7/src/dtactions/vocola_sendkeys/ext_keys.py
--rw-r--r--   0        0        0     3463 1970-01-01 00:00:00.000000 dtactions-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     2670 2024-04-08 15:24:46.297453 dtactions-1.6.1/README.md
+-rw-r--r--   0        0        0     1444 2024-04-08 15:24:46.297453 dtactions-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2026 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/README.md
+-rw-r--r--   0        0        0     6678 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/__init__.py
+-rw-r--r--   0        0        0    25528 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/autohotkeyactions.py
+-rw-r--r--   0        0        0    62583 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/messagefunctions.py
+-rw-r--r--   0        0        0    67137 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/monitorfunctions.py
+-rw-r--r--   0        0        0    21534 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/natlinkclipboard.py
+-rw-r--r--   0        0        0      196 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/samples/autohotkey/getintoforeground.ahk
+-rw-r--r--   0        0        0       48 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/samples/autohotkey/showmessageswindow.ahk
+-rw-r--r--   0        0        0    11847 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/samples/unimacro/unimacroactions.ini
+-rw-r--r--   0        0        0    45180 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/scintillacon.py
+-rw-r--r--   0        0        0     1497 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/sendkeys.py
+-rw-r--r--   0        0        0        0 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/__init__.py
+-rw-r--r--   0        0        0     5751 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/actionbases.py
+-rw-r--r--   0        0        0     2519 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/code-actions.py
+-rw-r--r--   0        0        0    16039 2024-04-08 15:24:46.297453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/excel-actions.py
+-rw-r--r--   0        0        0     4918 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/frescobaldi-actions.py
+-rw-r--r--   0        0        0     3233 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/komodo-actions.py
+-rw-r--r--   0        0        0     2862 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/notreadykomodo-actions.py
+-rw-r--r--   0        0        0      773 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/pythonwin-actions.py
+-rw-r--r--   0        0        0     1521 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/uedit32-actions.py
+-rw-r--r--   0        0        0     1655 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/uedit64-actions.py
+-rw-r--r--   0        0        0     1084 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/actionclasses/win32pad-actions.py
+-rw-r--r--   0        0        0     4576 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/ding.wav
+-rw-r--r--   0        0        0    17802 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/extenvvars.py
+-rw-r--r--   0        0        0    76714 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/inivars.py
+-rw-r--r--   0        0        0    78484 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/newactions.py
+-rw-r--r--   0        0        0    79623 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/unimacroactions.py
+-rw-r--r--   0        0        0    62741 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/unimacroutils.py
+-rw-r--r--   0        0        0       15 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/usc_functions.py
+-rw-r--r--   0        0        0    25505 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/unimacro/utilsqh.py
+-rw-r--r--   0        0        0    14962 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/vocola_sendkeys/ExtendedSendDragonKeys.py
+-rw-r--r--   0        0        0    20101 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/vocola_sendkeys/SendInput.py
+-rw-r--r--   0        0        0      303 2024-04-08 15:24:46.301453 dtactions-1.6.1/src/dtactions/vocola_sendkeys/ext_keys.py
+-rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 dtactions-1.6.1/PKG-INFO
```

### Comparing `dtactions-1.5.7/README.md` & `dtactions-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 You can run `py -m pip install dtactions[test]` or `py -m pip install dtactions[natlink_test]` if you don't have the prequisites like pytest.  
 
 You can run pytest from project root folder to run the tests that don't depend on natlink being installed.  For the natlink-dependent tests, run 
 `py -m pytest natlink_test`.  
 
 ## Notes About Packaging for Developers
 
-The package is specified in `pyproject.toml` and built with [flit](https://pypi.org/project/flit/). 
+The package is specified in `pyproject.toml` and uses  [flit](https://pypi.org/project/flit/) as the underlying build tool. 
 
-`py -m flit build` (or just `flit build`) builds the package.  A github action publishes to  publishes to [Python Packaging Index](https://pypi.org/). 
+Too build the package locally, 
+
+`py -m flit build` (or just `flit build`) builds the package. You can also use `python -m build` if you have build installed.   A github action publishes to  publishes to [Python Packaging Index](https://pypi.org/). 
 
 
  
 Version numbers of the packages must be increased before your publish to [Python Packaging Index](https://pypi.org/).
```

### Comparing `dtactions-1.5.7/pyproject.toml` & `dtactions-1.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 maintainers  = [{name = "Quintijn Hoogenboom", email="q.hoogenboom@antenna.nl"}, {name = "LexiconCode", email = "CasterVoice@protonmail.com"}]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 readme = "README.md"
 
 dependencies= [
 	"pywin32 >= 300",
-	"debugpy"
+	"debugpy",
+	"platformdirs"
 ]
 
 classifiers=[	"Development Status :: 4 - Beta",
 				"Topic :: Multimedia :: Sound/Audio :: Speech",
 				"Topic :: Scientific/Engineering :: Human Machine Interfaces",
 				]
```

### Comparing `dtactions-1.5.7/src/dtactions/README.md` & `dtactions-1.6.1/src/dtactions/README.md`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/__init__.py` & `dtactions-1.6.1/src/dtactions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 status = natlinkstatus.DtactionsStatus()
 status.getDtactionsDirectory()
 status.getDtactionsUserDirectory()
 ```
 
 """
 ## version to be updated when a new release is sent to pypi:
-__version__ = '1.5.7'     # streamlining __init__ a bit oct 23
+__version__ = '1.6.1'     # new middle number with extenvvar.py and requirement of natlink, april 24
 ##----------------------
 import sys
 import os
 from pathlib import Path, WindowsPath
 
 def getDtactionsDirectory():
     """return the root directory of dtactions
```

### Comparing `dtactions-1.5.7/src/dtactions/autohotkeyactions.py` & `dtactions-1.6.1/src/dtactions/autohotkeyactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,25 +63,36 @@
 
 def do_ahk_script(script, filename=None):
     """try autohotkey integration
     """
     filename = filename or 'tempscript.ahk'
     if not ahk_is_active():
         print('ahk is not active, cannot run script')
-        return
+        return 0
     #print 'AHK with script: %s'% script
+    if script.strip().endswith('.ahk'):
+        script = script.strip()
+        scriptPath = ahkscriptfolder/script
+        if scriptPath.is_file():
+            call_ahk_script_path(scriptPath)
+            return 1
+        print(f'not a valid filepath for AHK script: "{str(scriptPath)}"')
+        return 0
+    
     scriptPath = ahkscriptfolder/filename
+            
     if isinstance(script, (list, tuple)):
         script = '\n'.join(script)         
     if not script.endswith('\n'):
         script += '\n'
     
-    with open(scriptPath, 'w') as fp:
+    with open(scriptPath, 'w', encoding='utf-8') as fp:
         fp.write(script)
     call_ahk_script_path(scriptPath)
+    return 1
 
 def call_ahk_script_path(scriptPath):
     """call the specified ahk script  
     
     you can call .ahk scripts or .exe compiled files,
     but .exe files seem not to give better performance...
     
@@ -92,15 +103,15 @@
     if scriptPath.endswith('.ahk'):
         result = subprocess.call([ahkexe, scriptPath, ""])
     elif scriptPath.endswith('exe'):
         result = subprocess.call([scriptPath, "", ""])
     else:
         raise ValueError(f'autohotkeyactions, call_ahk_script_path: path should end with ".ahk", or ".exe"\n    path: {scriptPath}')
     if result:
-        print('non-zero result of call_ahk_script_path "%s": %s'% (scriptPath, result))
+        print(f'non-zero result of call_ahk_script_path "{scriptPath}": {result}')
 
 ProgInfo = collections.namedtuple('ProgInfo', 'progpath prog title toporchild classname hndle'.split(' '))
 
 def getProgInfo():
     """get the prog info, like natlink.getCurrentModule enhanced with toporchild and classname
     
     returns program info as namedtuple (progpath, prog, title, toporchild, classname, hndle)
@@ -146,15 +157,15 @@
 """
     script = script.replace('##proginfofile##', str(info_file))
     return script
 
 def getProgInfoResult(info_file):
     """extract the contents of the info_file, and return the progInfo
     """
-    with open(info_file, 'r') as fp:
+    with open(info_file, 'r', encoding='utf-8') as fp:
         progInfo = fp.read().split('\n')
         
     # note ahk returns 5 lines, but ProgInfo has 6 items.   
     if len(progInfo) == 5:
         # make hndle decimal number:
         progpath, title, toporchild, classname, hndle = progInfo
         if hndle:
@@ -285,15 +296,16 @@
     ## do the replacements:
     script = script.replace('##waitForStart##', str(waitForStart))
     script = script.replace('##proginfofile##', str(ProgInfoFile))
     script = script.replace('##ErrorFile##', str(ErrorFile))
 
     ## do the script!!
     do_ahk_script(script)
-    message = open(ErrorFile, 'r').read().strip()
+    with open(ErrorFile, 'r', encoding='utf-8') as fp:
+        message = fp.read().strip()
     if message:
         return message  
 
     # see if there is an error message:
     errors = readErrorMessagesFile()
     if errors:
         return errors
@@ -464,15 +476,15 @@
         wHndle := wHndle + 0
         FileDelete, ##hndlefile##
         FileAppend, %wHndle%, ##hndlefile##
     '''
     script = script.replace('##hndlefile##', str(HndleFile))
     do_ahk_script(script, filename="getforegroundwindow.ahk")
 
-    with open(HndleFile, 'r') as fp:
+    with open(HndleFile, 'r', encoding='utf-8') as fp:
         gotHndle = fp.read().strip()
     try:
         if gotHndle:
             hndleInt = int(gotHndle)
             return hndleInt
         mess = 'autohotkeyactions, GetForegroundWindow did not return a window hndle'
         return mess
@@ -517,15 +529,16 @@
         mess = f'Error with SetForegroundWindow to {hndle}'
         return mess
 
     if not Path(ProgInfoFile).is_file():
         mess = f'Error with SetForegroundWindow to {hndle}, InfoFile cannot be found'
         return mess
         
-    winHndle = open(ProgInfoFile, 'r').read().strip()
+    with open(ProgInfoFile, 'r', encoding='utf-8') as fp:
+        winHndle = fp.read().strip()
     if winHndle:
         try:
             winHndle = int(winHndle)
         except ValueError:
             mess = f'ahk script getIntoForeground to "{hndle}" did not return correct winHndle: {winHndle}'
             return mess
             
@@ -609,23 +622,23 @@
 
 def clearErrorMessagesFile():
     """make an empty ErrorMessagesFile
     
     return the path of the ErrorMessagesFile
     """
     ErrorFile = ahkscriptfolder/"errormessagefromahk.txt"
-    with open(ErrorFile, 'w') as f:
+    with open(ErrorFile, 'w', encoding='utf-8') as f:
         f.write('\n')
     return ErrorFile
 
 def readErrorMessagesFile():
     """get the error messages if any
     """
     ErrorFile = ahkscriptfolder/"errormessagefromahk.txt"
-    with open(ErrorFile, 'r') as f:
+    with open(ErrorFile, 'r', encoding='utf-8') as f:
         mess = f.read()
     if mess.strip():
         return f'autohotkeyactions.ahkBringup failed:\n===={mess}'
     return ''
 
 
 
@@ -720,12 +733,14 @@
     test()
     print(f'ahk_is_active: {ahk_is_active()}')
     Result = getProgInfo()
     print(f'\nresult of getProgModInfo: (start)\n{repr(Result)}')
     Result = ahkBringup("notepad")
     print(f'\nresult of ahkBringup("notepad"):\n{repr(Result)}')
     if Result.hndle:
-        killWindow(Result.hndle)
+        killWindow(Result.hndle, silent=False)
+    Result = do_ahk_script('showmessageswindow.ahk')
+    pass
```

### Comparing `dtactions-1.5.7/src/dtactions/messagefunctions.py` & `dtactions-1.6.1/src/dtactions/messagefunctions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/monitorfunctions.py` & `dtactions-1.6.1/src/dtactions/monitorfunctions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/natlinkclipboard.py` & `dtactions-1.6.1/src/dtactions/natlinkclipboard.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/samples/unimacro/unimacroactions.ini` & `dtactions-1.6.1/src/dtactions/samples/unimacro/unimacroactions.ini`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/scintillacon.py` & `dtactions-1.6.1/src/dtactions/scintillacon.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/actionbases.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/actionbases.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/code-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/code-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/excel-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/excel-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/frescobaldi-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/frescobaldi-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/komodo-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/komodo-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/notreadykomodo-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/notreadykomodo-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/pythonwin-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/pythonwin-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/uedit32-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/uedit32-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/uedit64-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/uedit64-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/actionclasses/win32pad-actions.py` & `dtactions-1.6.1/src/dtactions/unimacro/actionclasses/win32pad-actions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/ding.wav` & `dtactions-1.6.1/src/dtactions/unimacro/ding.wav`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/extenvvars.py` & `dtactions-1.6.1/src/dtactions/unimacro/extenvvars.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,433 +3,480 @@
 #   (c) Copyright 1999 by Joel Gould
 #   Portions (c) Copyright 1999 by Dragon Systems, Inc.
 #
 #pylint:disable=E0611, E0401, R0911, R0912, W0702, C0116
 #pylint:disable=C0209
 """extenvvars.py
 
-Keep track of environment variables, including added "fake" variables like DROPBOX, "This PC", etc.
+Keep track of environment variables, including added "fake" variables like DROPBOX
 
- Quintijn Hoogenboom, January 2008/September 2015/November 2022 (python3)
+ Quintijn Hoogenboom, January 2008/September 2015/November 2022 (python3)/March 24
 
 
 """
 import os
+from os.path import normpath, isfile, isdir, join
+import copy
 import re
+from pathlib import Path
 from win32com.shell import shell, shellcon
-from natlinkcore import natlinkstatus
-status = natlinkstatus.NatlinkStatus()
+import platformdirs
+try:
+    import natlink
+    natlinkAvailable = True
+except ImportError:
+    natlinkAvailable = False
+    
+if natlinkAvailable:
+    if not natlink.isNatSpeakRunning():
+        natlinkAvailable = False
+        
+if natlinkAvailable:
+    from natlinkcore import natlinkstatus
+    status = natlinkstatus.NatlinkStatus()
+    status_dict_full = copy.copy(status.getNatlinkStatusDict())
+    
+    status_dict = {key.upper():value for (key, value) in status_dict_full.items() if os.path.isdir(value)}
+    del status_dict_full
+else:
+    status = None
+    status_dict = None
 # for extended environment variables:
 reEnv = re.compile('(%[A-Z_]+%)', re.I)
 
-# keep track of found env variables, fill, if you wish, with
-# getAllFolderEnvironmentVariables.
-# substitute back with substituteEnvVariableAtStart.
-# and substite forward with expandEnvVariableAtStart
-# in all cases a private envDict can be user, or the global dict recentEnv
-#
-# to collect all env variables, call getAllFolderEnvironmentVariables, see below
-recentEnv = {}
-
-def addToRecentEnv(name, value):
-    """to be filled for NATLINK variables from natlinkstatus
-    """
-    recentEnv[name] = value
+class ExtEnvVars:
+    """gives and "remembers" environment variables, with extensions
+    
+    several sorts of env variables are handled:
+    
+    Environment variables, like %xxxx%:
+    - os.environ
+    - all from natlinkstatus.py (if available) (like %natlink% or %unimacro%)
 
-def deleteFromRecentEnv(name):
-    """to possibly delete from recentEnv, from natlinkstatus
-    """
-    if name in recentEnv:
-        del recentEnv[name]
 
-def getFolderFromLibraryName(fName):
-    """from windows library names extract the real folder
-    
-    the CabinetWClass and #32770 controls return "Documents", "Dropbox", "Desktop" etc.
-    try to resolve these throug the extended env variables.
+    Libraries, that are returned from a getFolderFromActiveWindow (_folders grammar of unimacro):
+        - several from "Libraries" (like Music, Documents), via platformdirs
+        - others from "CSIDL_variables" directly
     """
-    if fName.startswith("Docum"):  # Documents in Dutch and English
-        return getExtendedEnv("PERSONAL")
-    if fName in ["Muziek", "Music"]:
-        return getExtendedEnv("MYMUSIC")
-    if fName in ["Pictures", "Afbeeldingen"]:
-        return getExtendedEnv("MYPICTURES")
-    if fName in ["Videos", "Video's"]:
-        return getExtendedEnv("MYVIDEO")
-    if fName in ['OneDrive']:
-        return getExtendedEnv("OneDrive")
-    if fName in ['Desktop', "Bureaublad"]:
-        return getExtendedEnv("DESKTOP")
-    if fName in ['Quick access', 'Snelle toegang']:
-        templatesfolder = getExtendedEnv('TEMPLATES')
-        if os.path.isdir(templatesfolder):
-            QuickAccess = os.path.normpath(os.path.join(templatesfolder, "..", "Libraries"))
-            if os.path.isdir(QuickAccess):
-                return QuickAccess
-    if fName == 'Dropbox':
-        return getDropboxFolder()
-    if fName in ['Download', 'Downloads']:
-        personal = getExtendedEnv('PERSONAL')
-        userDir = os.path.normpath(os.path.join(personal, '..'))
-        if os.path.isdir(userDir):
-            tryDir = os.path.normpath(os.path.join(userDir, fName))
-            if os.path.isdir(tryDir):
-                return tryDir
-    usersHome = os.path.normpath(os.path.join(r"C:\Users", fName))
-    if os.path.isdir(usersHome):
-        return usersHome
-    if fName in ["This PC", "Deze pc"]:
-        return "\\"
-    print('cannot find folder for Library name: %s'% fName)
-    return ""
-
-
-def getDropboxFolder(containsFolder=None):
-    """get the dropbox folder, or the subfolder which is specified.
-    
-    Searching is done in all 'C:\\Users' folders, and in the root of "C:"
-    (See DirsToTry)
-    
-    raises OSError if more folders are found (should not happen, I think)
-    if containsFolder is not passed, the dropbox main folder is returned
-    if containsFolder is passed, this folder is returned if it is found in the dropbox folder
     
-    otherwise None is returned.
-    """
-    results = []
-    root = 'C:\\Users'
-    dirsToTry = [ os.path.join(root, s) for s in os.listdir(root) if os.path.isdir(os.path.join(root,s)) ]
-    dirsToTry.append('C:\\')
-    for root in dirsToTry:
-        if not os.path.isdir(root):
-            continue
-        try:
-            subs = os.listdir(root)
-        except WindowsError:
-            continue
-        if 'Dropbox' in subs:
-            subAbs = os.path.join(root, 'Dropbox')
-            subsub = os.listdir(subAbs)
-            if not ('.dropbox' in subsub and os.path.isfile(os.path.join(subAbs,'.dropbox'))):
-                continue
-            if containsFolder:
-                result = matchesStart(subsub, containsFolder, caseSensitive=False)
-                if result:
-                    results.append(os.path.join(subAbs,result))
-            else:
-                results.append(subAbs)
-    if not results:
-        return ''
-    if len(results) > 1:
-        raise OSError('getDropboxFolder, more dropbox folders found: %s')
-    return results[0]                 
+    def __init__(self):
+        self.recentEnv = {}
+        self.homeDir = self.getHome()        # starting at least reventEnv dict.
 
-def matchesStart(listOfDirs, checkDir, caseSensitive):
-    """return result from list if checkDir matches, mostly case insensitive
-    """
-    if not caseSensitive:
-        checkDir = checkDir.lower()
-    for l in listOfDirs:
-        if not caseSensitive:
-            ll = l.lower()
-        else:
-            ll = l
-        if ll.startswith(checkDir):
-            return l
-    return False   
+    def addToRecentEnv(self, name, value):
+        """to be filled for NATLINK variables from natlinkstatus and other env variables, sort of caching mechanism
         
-            
+        empty values can be cached...
+        """
+        if not value:
+            self.recentEnv[name] = None
+            return
+        value = str(value)
+        if not isdir(value):
+            self.recentEnv[name] = None
+            raise ValueError('extenvvars, addToRecentEnv: not a valid path for for name: "%s": "%s"'% (name, value))
+        self.recentEnv[name] = value
+
+    def deleteFromRecentEnv(self, name):
+        """to possibly delete from recentEnv, from natlinkstatus
+        """
+        if name in self.recentEnv:
+            del self.recentEnv[name]
 
-def getExtendedEnv(var, envDict=None, displayMessage=1):
-    """get from environ or windows CSLID
+    def getFolderFromLibraryName(self, name):
+        """from windows library names extract the real folder
+        
+        the CabinetWClass and #32770 controls return "Documents", "Dropbox", "Desktop" etc.
+        try to resolve these throug the extended env variables,
+        - with platformdirs
+        - with more special trick
+        """
+        if name in self.recentEnv:
+            return self.recentEnv[name]
+        
+        if name == "~":
+            home_dir = Path().home()
+            self.addToRecentEnv("~", home_dir)
+            return self.recentEnv["~"]
+        
+        
+        ## these are NOT cached:
+        if name.startswith("Docum"):  # Documents in Dutch and English
+            return platformdirs.windows.get_win_folder("CSIDL_PERSONAL")
+        if name in ["Muziek", "Music"]:
+            return platformdirs.windows.get_win_folder("CSIDL_MYMUSIC")
+        if name in ["Pictures", "Afbeeldingen"]:
+            return platformdirs.windows.get_win_folder("CSIDL_MYPICTURES")
+        if name in ["Videos", "Video's"]:
+            return platformdirs.windows.get_win_folder("CSIDL_MYVIDEO")
+        if name in ['Desktop', "Bureaublad"]:
+            return platformdirs.windows.get_win_folder("CSIDL_DESKTOPDIRECTORY")
+        if name in ['Download', 'Downloads']:
+            return platformdirs.windows.get_win_folder("CSIDL_DOWNLOADS")
+        if name in ['APPDATA']:
+            return platformdirs.windows.get_win_folder("CSIDL_APPDATA")
+        if name in ['COMMON_APPDATA']:
+            return platformdirs.windows.get_win_folder("CSIDL_COMMON_APPDATA")
+        if name in ['LOCAL_APPDATA']:
+            return platformdirs.windows.get_win_folder("CSIDL_LOCAL_APPDATA")
+        
+        ## extra cases:
+        # if name in ['Quick access', 'Snelle toegang']:
+        #     templatesfolder =self. getExtendedEnv('TEMPLATES')
+        #     if isdir(templatesfolder):
+        #         QuickAccess = normpath(join(templatesfolder, "..", "Libraries"))
+        #         if isdir(QuickAccess):
+        #             return QuickAccess
+        if name.upper() == 'DROPBOX':
+            return self.getDropboxFolder()
+        if name.upper() in ['ONEDRIVE']:
+            return self.getExtendedEnv("OneDrive")
+        
+        if name in ["This PC", "Deze pc"]:
+            return "\\"
+        print('getFolderFromLibraryName, cannot find folder for Library name: %s'% name)
+        return ""
 
-    HOME is environ['HOME'] or CSLID_PERSONAL
-    ~ is HOME
+    def getHome(self):
+        """get the home directory, with pathlib.Path().home()
+        
+        If env variable HOME is there, and points to another directory, give a warning. 
+        
+        result is cached in recentEnv dict.
+        
+        """
+        if "~" in self.recentEnv:
+            return self.recentEnv["~"]
+
+        Home = str(Path().home())
+        if Home and isdir(Home):
+            self.addToRecentEnv("~", Home)   # cache as a str
+        HomeFromEnv = os.environ.get("HOME", "")
+        if HomeFromEnv and isdir(HomeFromEnv):
+            self.addToRecentEnv("HOME", HomeFromEnv)
+            if HomeFromEnv != Home:
+                print(f'Warning: "~" and "HOME" point to different directories\n\t"~": "{Home}"\n\t"HOME": "{HomeFromEnv}"')
+        else:
+            self.addToRecentEnv("HOME", Home)
+        return self.recentEnv["~"]
+            
 
-    DROPBOX added via getDropboxFolder is this module (QH, December 1, 2018)
+    def getDropboxFolder(self):
+        """get the dropbox folder, or the subfolder which is specified.
+        
+        searched is in home directory of the user...
+        
+        raises OSError if more folders are found (should not happen, I think)
+        if containsFolder is not passed, the dropbox main folder is returned
+        if containsFolder is passed, this folder is returned if it is found in the dropbox folder
+        
+        otherwise None is returned.
+        """
+        if "DROPBOX" in self.recentEnv:
+            return self.recentEnv["DROPBOX"]
+
+        dirsToTry = [ "%DROPBOX%", "~", 'C:\\']    #### for s in os.listdir(root) if isdir(join(root,s)) ]
+        for root in dirsToTry:
+            result = self.getDropboxFolder2(root)
+            if result:
+                self.addToRecentEnv("DROPBOX", result)
+                return self.recentEnv["DROPBOX"]
+        return False 
+            
+    def getDropboxFolder2(self, root):
+        """helper function
+        """
+        
+        if root.startswith("%"):
+            root = root.strip("% ").upper()
+            root = os.environ.get(root, "")
+        
+        if root and not isdir(root):
+            return False
+        
+        if root.lower().endswith("dropbox"):
+            return root
+        next_dir = join(root, "dropbox")
+        if isdir(next_dir):
+            return next_dir
+        return False
+    
+    def matchesStart(self, listOfDirs, checkDir, caseSensitive):
+        """return result from list if checkDir matches, mostly case insensitive
+        """
+        if not caseSensitive:
+            checkDir = checkDir.lower()
+        for l in listOfDirs:
+            if not caseSensitive:
+                ll = l.lower()
+            else:
+                ll = l
+            if ll.startswith(checkDir):
+                return l
+        return False   
+        
+            
 
-    Also the directories that are configured inside Natlink can be retrieved, via natlinkstatus.py
-    Natlink_SettingsDir, DragonflyUserDirectory, VocolaDirectory, AhkUserDir
+    def getExtendedEnv(self, var, noCache=False, displayMessage=True):
+        r"""get from os.environ or windows CSLID
     
-    Note: these settings are case sensitive! You can leave out Dir or Directory.
+        HOME is os.environ['HOME'] or CSLID_PERSONAL
+        ~ is HOME (this is doubtful, str(pathlib.Path.home()) gives 'C:\Users\User', also when HOME points to another directory
     
-    As envDict for recent results either a private (passed in) dict is taken, or
-    the global recentEnv.
-
-    This is merely for "caching results"
-
-    """
-    if envDict is None:
-        myEnvDict = recentEnv
-    else:
-        myEnvDict = envDict
-##    var = var.strip()
-    var = var.strip("% ")
-
-    result = getDirectoryFromNatlinkstatus(var)
-    if result:
-        return result
-    var = var.upper()
-    
-    if var == "~":
-        var = 'HOME'
-
-    if var in myEnvDict:
-        return myEnvDict[var]
-
-    if var in os.environ:
-        myEnvDict[var] = os.environ[var]
-        return myEnvDict[var]
-
-    if var == 'DROPBOX':
-        result = getDropboxFolder()
+        DROPBOX added via self.getDropboxFolder is this module (QH, December 1, 2018)
+    
+        Also the directories that are configured inside Natlink can be retrieved, via natlinkstatus.py
+        Natlink_SettingsDir, DragonflyUserDirectory, VocolaDirectory, AhkUserDir:
+        
+        Note: these settings are case sensitive! You can leave out Dir or Directory.
+    
+        """
+        var = var.strip("% ")
+    
+        if var in  self.recentEnv:
+            return self.recentEnv[var]
+    
+        # Note the Natlink variables must conform to "Unimacro" etc. Best don't append "Dir" or "Directory":
+        # It is tried to append ("Dir" or "Directory" (or nothing) to it in the call
+        # Don't capitalise these variables!!)
+        result = self.getDirectoryFromNatlinkstatus(var)
         if result:
+            self.recentEnv[var] = result
             return result
-        raise ValueError('getExtendedEnv, cannot find path for "DROPBOX"')
-
-    if var == 'NOTEPAD':
-        windowsDir = getExtendedEnv("WINDOWS")
-        notepadPath = os.path.join(windowsDir, 'notepad.exe')
-        if os.path.isfile(notepadPath):
-            return notepadPath
-        raise ValueError('getExtendedEnv, cannot find path for "NOTEPAD"')
-
-    # try to get from CSIDL system call:
-    if var == 'HOME':
-        var2 = 'PERSONAL'
-    else:
-        var2 = var
-        
-    try:
-        CSIDL_variable =  'CSIDL_%s'% var2
-        shellnumber = getattr(shellcon,CSIDL_variable, -1)
-    except:
-        print('getExtendedEnv, cannot find in environ or CSIDL: "%s"'% var2)
-        return ''
-    if shellnumber < 0:
-        # on some systems have SYSTEMROOT instead of SYSTEM:
-        if var == 'SYSTEM':
-            return getExtendedEnv('SYSTEMROOT', envDict=envDict)
-        return ''
-        # raise ValueError('getExtendedEnv, cannot find in environ or CSIDL: "%s"'% var2)
-    try:
-        result = shell.SHGetFolderPath (0, shellnumber, 0, 0)
-    except:
-        if displayMessage:
-            print('getExtendedEnv, cannot find in environ or CSIDL: "%s"'% var2)
-        return ''
-
-    
-    result = str(result)
-    result = os.path.normpath(result)
-    myEnvDict[var] = result
-    # on some systems apparently:
-    if var == 'SYSTEMROOT':
-
-        myEnvDict['SYSTEM'] = result
-    return result
-
-def getDirectoryFromNatlinkstatus(envvar):
-    """see if directory can can be retrieved from envvar
-    """
-    # try if function in natlinkstatus:
-    for extra in ('', 'Directory', 'Dir'):
-        var2 = envvar + extra
-        if var2 in status.__dict__:
-            funcName = f'get{var2}'
-            func = getattr(status, funcName)
-            result = func()
+      
+        
+        
+        if var == "~":
+            var = 'HOME'
+        
+        if var in os.environ:
+            result = os.environ[var]
+            self.addToRecentEnv(var, result)
+            return self.recentEnv[var]
+    
+        if var == 'DROPBOX':
+            result = self.getDropboxFolder()
             if result:
+                self.addToRecentEnv(var, result)
                 return result
-    return None
-
-
-
-def clearRecentEnv():
-    """for testing, clears above global dictionary
-    """
-    recentEnv.clear()
-
-def getAllFolderEnvironmentVariables(fillRecentEnv=None):
-    """return, as a dict, all the environ AND all CSLID variables that result into a folder
+            raise ValueError('getExtendedEnv, cannot find path for "DROPBOX"')
     
-    Now also implemented:  Also include NATLINK, UNIMACRO, VOICECODE, DRAGONFLY, VOCOLAUSERDIR, UNIMACROUSERDIR
-    This is done by calling from natlinkstatus, see there and example in natlinkmain.
-
-    Optionally put them in recentEnv, if you specify fillRecentEnv to 1 (True)
-
-    """
-    #pylint:disable=W0603
-    D = {}
+        if var == 'NOTEPAD':
+            windowsDir =self. getExtendedEnv("WINDOWS")
+            notepadPath = join(windowsDir, 'notepad.exe')
+            if isfile(notepadPath):
+                return notepadPath
+            raise ValueError('getExtendedEnv, cannot find path for "NOTEPAD"')
+    
+        # try to get from CSIDL system call:
+        try:
+            CSIDL_variable =  'CSIDL_%s'% var
+            shellnumber = getattr(shellcon,CSIDL_variable, -1)
+        except:
+            print('getExtendedEnv, cannot find in os.environ or CSIDL: "%s"'% var)
+            return ''
+        if shellnumber < 0:
+            # on some systems have SYSTEMROOT instead of SYSTEM:
+            if var == 'SYSTEM':
+                return self.getExtendedEnv('SYSTEMROOT')
+            return ''
+        try:
+            result = shell.SHGetFolderPath (0, shellnumber, 0, 0)
+        except:
+            if displayMessage:
+                print('getExtendedEnv, cannot find in os.environ or CSIDL: "%s"'% var)
+            return ''
+        if noCache:
+            return result
+        self.addToRecentEnv(var, result)
+        return self.recentEnv[var]
 
-    for k in dir(shellcon):
-        if k.startswith("CSIDL_"):
-            kStripped = k[6:]
+    def getDirectoryFromNatlinkstatus(self, envvar):
+        """see if directory can can be retrieved from envvar
+        """
+        # if natlink not available:
+        if not natlinkAvailable:
+            # print(f'natlink not available for get "{envvar}"')
+            return None
+    
+        # try if function in natlinkstatus:
+        if not status:
+            return None
+        for extra in ('', 'Directory', 'Dir'):
+            var2 = envvar + extra
+            if var2 in status.__dict__:
+                funcName = f'get{var2}'
+                func = getattr(status, funcName)
+                result = func()
+                if result:
+                    return result
+        return None
+    
+    
+    
+    def clearRecentEnv(self):
+        """for testing, clears above global dictionary
+        """
+        self.recentEnv.clear()
+    
+    def getAllFolderEnvironmentVariables(self, displayMessage=False):
+        """return, as a dict, all the os.environ AND all CSLID variables that result into a folder
+        
+        Now also implemented:  Also include NATLINK, UNIMACRO, VOICECODE, DRAGONFLY, VOCOLAUSERDIR, UNIMACROUSERDIR
+        This is done by calling from natlinkstatus, see there and example in natlinkmain.
+    
+        Optionally put them in recentEnv, if you specify fillRecentEnv to 1 (True)
+    
+        """
+        D = {}
+    
+        for k in dir(shellcon):
+            if k.startswith("CSIDL_"):
+                kStripped = k[6:]
+                try:
+                    v =self.getExtendedEnv(kStripped, noCache=True, displayMessage=displayMessage)    ## displayMessage=False)
+                except ValueError:
+                    continue
+                if len(str(v)) > 2 and isdir(v):
+                    D[kStripped] = v
+        # os.environ overrules CSIDL:
+        for k, v in os.environ.items():
+            if isdir(v):
+                v = normpath(v)
+                if k in D and D[k] != v:
+                    print('warning, CSIDL also exists for key: %s, take os.environ value: %s'% (k, v))
+                D[k] = v
+        return D
+    def substituteEnvVariableAtStart(self, filepath, envDict=None): 
+        r"""try to substitute back one of the (preused) environment variables back
+    
+        into the start of a filename
+    
+        if ~ (HOME) is D:\My documents,
+        the path "D:\My documents\folder\file.txt" should return "~\folder\file.txt"
+    
+        pass in a dict of possible environment variables, which can be taken from recent calls, or
+        from  envDict = getAllFolderEnvironmentVariables().
+    
+        Alternatively you can call getAllFolderEnvironmentVariables once, and use the recentEnv
+        of this module! getAllFolderEnvironmentVariables(fillRecentEnv)
+    
+        If you do not pass such a dict, recentEnv is taken, but this recentEnv holds only what has been
+        asked for in the session, so no complete list!
+    
+        """
+        if envDict is None:
+            envDict = self.recentEnv
+        Keys = list(envDict.keys())
+        # sort, longest result first, shortest keyname second:
+        decorated = [(-len(envDict[k]), len(k), k) for k in Keys]
+        decorated.sort()
+        Keys = [k for (dummy1,dummy2, k) in decorated]
+        for k in Keys:
+            val = envDict[k]
+            if filepath.lower().startswith(val.lower()):
+                if k in ("HOME", "PERSONAL"):
+                    k = "~"
+                else:
+                    k = "%" + k + "%"
+                filepart = filepath[len(val):]
+                filepart = filepart.strip('/\\ ')
+                return join(k, filepart)
+        # no hit, return original:
+        return filepath
+           
+    def expandEnvVariableAtStart(self, filepath, envDict=None): 
+        """try to substitute environment variable into a path name
+    
+        """
+        filepath = filepath.strip()
+    
+        if filepath.startswith('~'):
+            folderpart =self. getExtendedEnv('~', envDict)
+            filepart = filepath[1:]
+            filepart = filepart.strip('/\\ ')
+            return normpath(join(folderpart, filepart))
+        if reEnv.match(filepath):
+            envVar = reEnv.match(filepath).group(1)
+            # get the envVar...
             try:
-                v = getExtendedEnv(kStripped, displayMessage=None)
+                folderpart =self. getExtendedEnv(envVar, envDict)
             except ValueError:
-                continue
-            if len(v) > 2 and os.path.isdir(v):
-                D[kStripped] = v
-            elif v == '.':
-                D[kStripped] = os.getcwd
-    # os.environ overrules CSIDL:
-    for k in os.environ:
-        v = os.environ[k]
-        if os.path.isdir(v):
-            v = os.path.normpath(v)
-            if k in D and D[k] != v:
-                print('warning, CSIDL also exists for key: %s, take os.environ value: %s'% (k, v))
-            D[k] = v
-    if isinstance(fillRecentEnv, dict):
-        recentEnv.update(D)
-    return D
-
-#def setInRecentEnv(key, value):
-#    if key in recentEnv:
-#        if recentEnv[key] == value:
-#            print 'already set (the same): %s, %s'% (key, value)
-#        else:
-#            print 'already set (but different): %s, %s'% (key, value)
-#        return
-#    print 'setting in recentEnv: %s to %s'% (key, value)
-#    recentEnv[key] = value
-
-def substituteEnvVariableAtStart(filepath, envDict=None): 
-    r"""try to substitute back one of the (preused) environment variables back
-
-    into the start of a filename
-
-    if ~ (HOME) is D:\My documents,
-    the path "D:\My documents\folder\file.txt" should return "~\folder\file.txt"
-
-    pass in a dict of possible environment variables, which can be taken from recent calls, or
-    from  envDict = getAllFolderEnvironmentVariables().
-
-    Alternatively you can call getAllFolderEnvironmentVariables once, and use the recentEnv
-    of this module! getAllFolderEnvironmentVariables(fillRecentEnv)
-
-    If you do not pass such a dict, recentEnv is taken, but this recentEnv holds only what has been
-    asked for in the session, so no complete list!
-
-    """
-    if envDict is None:
-        envDict = recentEnv
-    Keys = list(envDict.keys())
-    # sort, longest result first, shortest keyname second:
-    decorated = [(-len(envDict[k]), len(k), k) for k in Keys]
-    decorated.sort()
-    Keys = [k for (dummy1,dummy2, k) in decorated]
-    for k in Keys:
-        val = envDict[k]
-        if filepath.lower().startswith(val.lower()):
-            if k in ("HOME", "PERSONAL"):
-                k = "~"
+                print('invalid (extended) environment variable: %s'% envVar)
             else:
-                k = "%" + k + "%"
-            filepart = filepath[len(val):]
-            filepart = filepart.strip('/\\ ')
-            return os.path.join(k, filepart)
-    # no hit, return original:
-    return filepath
-       
-def expandEnvVariableAtStart(filepath, envDict=None): 
-    """try to substitute environment variable into a path name
-
-    """
-    filepath = filepath.strip()
-
-    if filepath.startswith('~'):
-        folderpart = getExtendedEnv('~', envDict)
-        filepart = filepath[1:]
-        filepart = filepart.strip('/\\ ')
-        return os.path.normpath(os.path.join(folderpart, filepart))
-    if reEnv.match(filepath):
-        envVar = reEnv.match(filepath).group(1)
-        # get the envVar...
-        try:
-            folderpart = getExtendedEnv(envVar, envDict)
-        except ValueError:
-            print('invalid (extended) environment variable: %s'% envVar)
-        else:
-            # OK, found:
-            filepart = filepath[len(envVar)+1:]
+                # OK, found:
+                filepart = filepath[len(envVar)+1:]
+                filepart = filepart.strip('/\\ ')
+                return normpath(join(folderpart, filepart))
+        # no match
+        return filepath
+        
+    def expandEnvVariables(self, filepath, envDict=None): 
+        """try to substitute environment variable into a path name,
+    
+        ~ only at the start,
+    
+        %XXX% can be anywhere in the string.
+    
+        """
+        filepath = filepath.strip()
+        
+        if filepath.startswith('~'):
+            folderpart =self. getExtendedEnv('~', envDict)
+            filepart = filepath[1:]
             filepart = filepart.strip('/\\ ')
-            return os.path.normpath(os.path.join(folderpart, filepart))
-    # no match
-    return filepath
+            filepath = normpath(join(folderpart, filepart))
+        
+        if reEnv.search(filepath):
+            List = reEnv.split(filepath)
+            #print 'parts: %s'% List
+            List2 = []
+            for part in List:
+                if not part:
+                    continue
+                if part == "~" or (part.startswith("%") and part.endswith("%")):
+                    try:
+                        folderpart = self.getExtendedEnv(part, envDict)
+                    except ValueError:
+                        folderpart = part
+                    List2.append(folderpart)
+                else:
+                    List2.append(part)
+            List2 = [str(item) for item in List2]
+            filepath = ''.join(List2)
+            return normpath(filepath)
+        # no match
+        return filepath
     
-def expandEnvVariables(filepath, envDict=None): 
-    """try to substitute environment variable into a path name,
-
-    ~ only at the start,
-
-    %XXX% can be anywhere in the string.
-
-    """
-    filepath = filepath.strip()
     
-    if filepath.startswith('~'):
-        folderpart = getExtendedEnv('~', envDict)
-        filepart = filepath[1:]
-        filepart = filepart.strip('/\\ ')
-        filepath = os.path.normpath(os.path.join(folderpart, filepart))
-    
-    if reEnv.search(filepath):
-        List = reEnv.split(filepath)
-        #print 'parts: %s'% List
-        List2 = []
-        for part in List:
-            if not part:
-                continue
-            if part == "~" or (part.startswith("%") and part.endswith("%")):
-                try:
-                    folderpart = getExtendedEnv(part, envDict)
-                except ValueError:
-                    folderpart = part
-                List2.append(folderpart)
-            else:
-                List2.append(part)
-        filepath = ''.join(List2)
-        return os.path.normpath(filepath)
-    # no match
-    return filepath
-
-def printAllEnvVariables():
-    for k in sorted(recentEnv.keys()):
-        print("%s\t%s"% (k, recentEnv[k]))
-
+    
+    def printAllEnvVariables(self):
+        for k in sorted(self.recentEnv.keys()):
+            print("%s\t%s"% (k, self.recentEnv[k]))
+    
 if __name__ == "__main__":
-    Vars = getAllFolderEnvironmentVariables()
-    for kk in sorted(Vars):
-        print('%s: %s'% (kk, Vars[kk]))
-        if not os.path.isdir(Vars[kk]):
-            print('----- not a directory: %s (%s)'% (Vars[kk], kk))
+    env = ExtEnvVars()
+    Vars = env.getAllFolderEnvironmentVariables()
+    print('recentEnv: ')
+    print(env.recentEnv)
+    print('='*80)
+    
 
     print('testing       expandEnvVariableAtStart')
-    print('also see expandEnvVar in natlinkstatus!!')
-    for p in ("D:\\natlink\\unimacro", "~/unimacroqh",
+    print('also see expandEnvVar in natlinkstatus!! and test_extenvvars.py in dtactions/test')
+    for p in ("~", "%home%", "D:\\natlink\\unimacro", "~/unimacroqh",
               "%HOME%/personal",
               "%WINDOWS%\\folder\\strange testfolder"):
-        expanded = expandEnvVariableAtStart(p)
+        expanded = env.expandEnvVariableAtStart(p)
         print('expandEnvVariablesAtStart: %s: %s'% (p, expanded))
+        
     print('testing       expandEnvVariables')  
-    for p in ("%DROPBOX%/QuintijnHerold/jachthutten", "D:\\%username%", "%NATLINK%\\unimacro", "%UNIMACROUSER%",
-              "%HOME%/personal", "%HOME%", "%personal%"
+    p = "%UNIMACROUSER%"
+    expanded = env.expandEnvVariables(p)
+
+
+    for p in ("%NATLINK%\\unimacro", "%DROPBOX%/QuintijnHerold/jachthutten", "D:\\%username%",  "%UNIMACROUSER%", "%HOME%/personal", "%HOME%", "%personal%"
               "%WINDOWS%\\folder\\strange testfolder"):
-        expanded = expandEnvVariables(p)
+        expanded = env.expandEnvVariables(p)
         print('expandEnvVariables: %s: %s'% (p, expanded))
 
-    # testIniSection = NatlinkstatusInifileSection()
-    # print testIniSection.keys()
-    # testIniSection.set("test", "een test")
-    # testval = testIniSection.get("test")
-    # print 'testval: %s'% testval
-    # testIniSection.delete("test")
-    # testval = testIniSection.get("test")
-    # print 'testval: %s'% testval
-    print('recentEnv: %s'% len(recentEnv))
-    np = getExtendedEnv("NOTEPAD")
-    print(np)
-    for lName in ['Snelle toegang', 'Quick access', 'Documenten', 'Documents', 'Muziek', 'Afbeeldingen', 'Dropbox', 'OneDrive', 'Desktop', 'Bureaublad']:
-        f = getFolderFromLibraryName(lName)
-        print('folder from library name %s: %s'% (lName, f))
+
```

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/inivars.py` & `dtactions-1.6.1/src/dtactions/unimacro/inivars.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,24 @@
     state = 1: normal string, including spaces
     state = 2: inside a quoted string, that everything go except
     the quote that is maintained in hadQuote
     state = 3: after a quoted string, waits for a separator or
     the end of the string. Raises error if anything else than a
     space his met
 
+    # edge cases:
+    
+    >>> list(getIniList("''''''"))
+    ['abc']
+    >>> list(getIniList("'"))
+    ["'"]
+    
+    # single item, single quotes
+    >>> list(getIniList('a'))
+    ['a']
     >>> list(getIniList("a; c"))
     ['a', 'c']
     >>> list(getIniList("a;c"))
     ['a', 'c']
     >>> list(getIniList("a; c;"))
     ['a', 'c', '']
     >>> list(getIniList("'a\\"b'; c"))
@@ -225,14 +235,17 @@
     ['a ', ' c ']
 
     """
     i =  0
     l = len(t)
     state = 0
     hadQuote = ''
+    if l == 1:
+        yield t
+        return
 ##    print '---------------------------length: %s'% l
     for j in range(l):
         c = t[j]
 ##        print 'do c: |%s|, index: %s'% (c, j)
         if c in ("'", '"'):
             if state == 0:
                 # starting quoted state
@@ -1432,61 +1445,83 @@
 
 
         >>> import os
         >>> try: os.remove('getint.ini')
         ... except: pass
         >>> ini = IniVars('getint.ini')
         >>> ini.set('s', 'three', 3)
+        >>> ini.set('s', 'booltrue', 'T')
+        >>> ini.set('s', 'boolfalse', 'F')
         >>> ini.getInt('s', 'three')
         3
         >>> ini.getInt('s', 'unknown')
         0
         >>> ini.getInt('s', 'unknowndefault', 11)
         11
         
+
+        ##Edge cases: if t T f F (bool)return 1 or 0
+        ## two error cases for less errors in practice...
+        >>> ini.getInt('s', 'booltrue')
+        ini method getInt, got "T", return 1
+        1
+        >>> ini.getInt('s', 'boolfalse')
+        ini method getInt, got "F", return 0
+        0
+        
+        
         """
         try:
             i = self[section][key]
         except (KeyError, TypeError):
             return default
 
         if isinstance(i, int):
             return i
         if isinstance(i, str):
             if i:
                 try:
                     return int(i)
                 except ValueError as exc:
+                    if i in ('t', 'T'):
+                        print('ini method getInt, got "%s", return 1'% i)
+                        return 1
+                    if i in ('f', 'F'):
+                        print('ini method getInt, got "%s", return 0'% i)
+                        return 0
                     raise IniError('ini method getInt, value not a valid integer: %s (section: %s, key: %s)'% (section, key, i)) from exc
             else:
                 return default
         raise IniError('invalid type for getInt (probably intermediate set without write: %s)(section: %s, key: %s'%
                        (repr(i), section, key))
 
     def getBool(self, section, key, default=False):
         """get a value and convert into boolean
 
 t, T, true, True, Waar, waar, w, W, 1 -->> True
 empty, o, f, F, False, false, Onwaar, o, none -->> False
         
+        Errors: return False
+        
+        
         """
         try:
             i = self[section][key]
         except (KeyError, TypeError):
             return default
         if not i:
             return False
         i = str(i)
         if i.lower()[0] in ['t', 'w', '1']:
             return True
         if i.lower()[0] in ['f', 'o', '0']:
             return False
-        raise IniError('inivars, getBool, unexpected value: "%s" (section: %s, key: %s)'%
-                         (i, section, key))
-
+        print('inivars, getBool, unexpected value: "%s" (section: %s, key: %s), return False'% (i, section, key))
+        return False
+    
     def getFloat(self, section, key, default=0.0):
         """get a value and convert into a float
 
 
         >>> import os
         >>> try: os.remove('getfloat.ini')
         ... except: pass
```

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/newactions.py` & `dtactions-1.6.1/src/dtactions/unimacro/newactions.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/unimacroactions.py` & `dtactions-1.6.1/src/dtactions/unimacro/unimacroactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2301,13 +2301,22 @@
         print('_actions, OSError, cannot write debug statements to: %s'% debugFile)
 else:
     try:
         os.remove(debugFile)
     except OSError:
         pass
 
+
+def try_SCLIP():
+    ''' try by running this script, ensure cursor is on a safe place (bottom, or here after a #
+    '''
+    do_SCLIP('hello')
+    do_SCLIP('9123456789')
+    # now comes the error:
+    do_SCLIP('123456789')
+
+
 if __name__ == '__main__':
-    _s = 551345646373737373
-    do_SCLIP(_s)
-    # UnimacroBringUp("edit", r"C:\Users\Gebruiker\Documents\.natlink\UnimacroGrammars\_brackets.txt")
+    try_SCLIP()
     
-    
+    # UnimacroBringUp("edit", r"C:\Users\Gebruiker\Documents\.natlink\UnimacroGrammars\_brackets.txt")
+
```

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/unimacroutils.py` & `dtactions-1.6.1/src/dtactions/unimacro/unimacroutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #  
 """a set of utility functions in dtactions/unimacro
 
 Previous this was natlinkutilsqh.py in unimacro
 
 """
-#pylint:disable=C0302, C0116, C0321, R0912, R0913, R0914, R0915, W0613, C0209, W0602
+#pylint:disable=C0302, C0116, C0321, R0912, R0913, R0914, R0915, W0613, C0209, W0602, W0621, R1715, W0702
 #pylint:disable=E1101
 import time
 import re
 import os
 import os.path
 import sys
 import collections
@@ -45,16 +45,15 @@
 
 # default Waiting Times:
 defaultWaitingTime = 0.1        # 100 milliseconds
 visibleWaitFactor = 3                 # default for Wait and W
 longWaitFactor = 10                   # times 3 for visible wait
 shortWaitFactor = 0.3                 # times 10 for long wait
                                 # times 0.3 for short wait
-#debugMode 0 = not, -1 == dvcMode, 1 is light, 2 = normal, 3 = heavy
-debugMode = 1
+debugMode = 0     #-1
 
 pendingExecScripts = []
 
 ProgInfo = collections.namedtuple('ProgInfo', 'progpath prog title toporchild classname hndle'.split(' '))
 
 
 
@@ -205,15 +204,15 @@
     """returns program info as namedtuple (progpath, prog, title, toporchild, classname, hndle)
 
 
     now length 6, including the classname, but also a named tuple!!
 
     prog always lowercase
     
-    title now with capital letters.
+    title now with mixed (lower and upper case) letters.
 
     toporchild 'top' or 'child', or '' if no valid window
     """
     #pylint:disable=W0702
     if modInfo is None:
         try:
             modInfo = natlink.getCurrentModule()
@@ -223,15 +222,15 @@
             return progInfo
     
     _hndle = modInfo[2]
     if not _hndle:
         ## assume desktop, no foreground window, treat as top...
         return ProgInfo("", "", "", "top", "", 0)
     progpath = modInfo[0]
-    prog = Path(modInfo[0].lower()).stem
+    prog = Path(modInfo[0].lower()).stem  
     title = modInfo[1]
     if isTopWindow(modInfo[2]):
         toporchild = 'top'
     else:
         toporchild = 'child'
          
     HNDLE = int(modInfo[2])
@@ -730,15 +729,15 @@
         else:
             btn = mouse
     else:
         #print 'no click, mouseState: %s'% mouseState
         btn = 0
         nclick = 0
     #nClick = nClick or nclick   # take things from "mouse" if nClick  not used
-    #print 'btn: %s, nClick: %s, current mouseState: %s'% (btn, nClick, mouseState)
+    print('btn: %s, nClick: %s, current mouseState: %s'% (btn, nClick, mouseState))
     if onlyMove:
         print('onlyMove to %s, %x'% (xp, yp))
         natlink.playEvents([(natlinkutils.wm_mousemove, xp, yp)])
     elif not mouseState:  # ongecompliceerd
         if nClick > 0:
             natlink.playEvents([(natlinkutils.wm_mousemove, xp, yp)])
             if btn:
@@ -807,26 +806,32 @@
     return mouse, None 
 
 ##buttons = makedict(left=1, right=2, middle=4)
 ##joelsButtons = ['', 'left', 'right', 'middle']
 def buttonClick(button='left', nclick=1, modifiers=None):
     """do a natspeak buttonclick, but release mouse first if necessary
     """
-    # make button numeric:
-    #if button in buttons:
-    #    button = buttons[button]
-    #if button not in [1, 2, 4]:
-    #    raise UnimacroError('buttonClick invalid button: %s'% button)
-    #if nclick not in [1,2]:
-    #    raise UnimacroError('buttonClick invalid number of clicks: %s'% nclick)
+     # make button numeric:
+    buttons = {'left':1, 'right':2, 'middle':4}
+    if button in buttons:
+        button = buttons[button]
+    if button not in [1, 2, 4]:
+        raise UnimacroError('buttonClick invalid button: %s'% button)
+    if nclick not in [1,2]:
+        raise UnimacroError('buttonClick invalid number of clicks: %s'% nclick)
     if mouseState:
         releaseMouse()
         
-    natlinkutils.buttonClick(button, nclick, modifiers)
-    #natlink.execScript("ButtonClick %s,%s"%(button, nclick))
+    # natlinkutils.buttonClick(button, nclick, modifiers)
+    if button == 1 and nclick == 1:
+        script = 'ButtonClick'
+    else:
+        script = f'ButtonClick {button},{nclick}'
+    print(f'buttonClick via execScript: "{script}"')
+    natlink.execScript(script)
     
 
 
 def releaseMouse():
     """restores the default mouseState
     """
      #pylint:disable=W0603
@@ -1421,31 +1426,21 @@
     """
     if not w:
         return
     isInActiveVoc = (natlink.getWordInfo(w,0) is not None)
     if isInActiveVoc:
         natlink.deleteWord(w)
 
-if DEBUG:
-    fOutName = 'c:\\DEBUG '+__name__+'.txt'
-    debugFile = open(fOutName, 'w', encoding='utf-8')
-    print('DEBUG uitvoer naar: %s'% fOutName)
-
 def debugPrint(t):
     """print to debug file (is this working???)
     """
     if not DEBUG:
         return
-    if isinstance(t, str):
-        debugFile.write(t)
-    else:
-        debugFile.write(repr(t))
-    debugFile.write('\n')
-    debugFile.flush()
-
+    print(t)
+    
 def GetForegroundWindow():
     """return the handle of the current foreground window
     """
     return win32gui.GetForegroundWindow()
     
 
 def SetForegroundWindow(h, waitingTime=0.1, nWait=3, debug=None):
@@ -1684,44 +1679,46 @@
     # global previousClipboardText
     if previousClipboardText:
         t = previousClipboardText.pop()
     else:
         print('No "previousClipboardText" available, empty clipboard...')
         t = None
         return
-    for _i in range(10):
-        try:
-            win32clipboard.OpenClipboard()
-            break
-        except:
-            time.sleep(0.1)
-            continue
-        else:
-            print("could not restore clipboard")
-            return
-    win32clipboard.EmptyClipboard()
-    if t:
-        win32clipboard.SetClipboardData(format_unicode, t)
-    win32clipboard.CloseClipboard()
+    try:
+        for _i in range(10):
+            try:
+                win32clipboard.OpenClipboard()
+                break
+            except:
+                time.sleep(0.1)
+                continue
+            else:
+                print("could not restore clipboard")
+                return
+        win32clipboard.EmptyClipboard()
+        if t:
+            win32clipboard.SetClipboardData(format_unicode, t)
+    finally:
+        win32clipboard.CloseClipboard()
 
 def getClipboard():
-    """get clipboard through natlink, and strips off backslash r
+    """get clipboard through natlink, and strips off backslash r   
 
     """
     #pylint:disable=W0702       
     # t0 = time.time()
     t = None
     for _i in range(3):
         try:
             t = natlink.getClipboard()
             if not t is None:
                 # print ' at try', i
                 break
         except:
-            print('getClipboard, got no text')
+            print('getClipboard, but apparently empty')
             shortWait()
         else:
             break
 
     if t:
         # print 'got clipboard: "%s"'% repr(t)
         t = t.replace('\r', '')
@@ -1732,19 +1729,23 @@
 
 
 def setClipboard(t, format=1):
     """set clipboard with text
     format = win32con.CF_UNICODETEXT (13): as unicode
 
     """
-    #pylint:disable=W0622    
-    win32clipboard.OpenClipboard()
-    win32clipboard.EmptyClipboard()
-    win32clipboard.SetClipboardData(format, t)
-    win32clipboard.CloseClipboard()
+    #pylint:disable=W0622
+    try:
+        win32clipboard.OpenClipboard()
+        win32clipboard.EmptyClipboard()
+        win32clipboard.SetClipboardData(format, t)
+    except:
+        print(f'exception in unimacroutils/setClipboard of "{t}"')
+    finally:
+        win32clipboard.CloseClipboard()
 
 def checkLists(one, two):
     """returns to lists, only in first, only in second
 
     if lists are equal 2 empty lists are returned
     """
     onlyone = []
```

### Comparing `dtactions-1.5.7/src/dtactions/unimacro/utilsqh.py` & `dtactions-1.6.1/src/dtactions/unimacro/utilsqh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,16 @@
 """utility functions from Quintijn, used in unimacro and in local programs.
    in python3 also the path module as subclass of the standard path class
 """
 #pylint:disable=C0116, C0302,  W0613, R0912, R0914, R0915, R0911, W0702
-import sys
 import unicodedata
 import os
 import re
-import traceback
 import collections
-import time
 from pathlib import Path
-
-# skip the string.maketrans business, ook de fixwordquotes
-# _allchars = string.maketrans('', '')
-# ## string translator functions:
-# def translator(frm=b'', to=b'', delete=b'', keep=None):
-#     """closure function to implement the string.translate functie
-#     python cookbook (2), ch 1 recipe 9
-# obsolete, test for doctest unicode functions...
-# 
-# # functions below, see also testUtilsqh.py in unittest.
-# >>> fixwordquotes(b'\x91aa\x92')
-# b"'aa'"
-# >>> fixwordquotes(b'\x93bb\x94')
-# b'"bb"'
-# 
-# ## do these via unicode:
-# >>> normalizeaccentedchars('d\\u00e9sir\\u00e9 //\u00ddf..# -..e.')
-# 'desire //Yf..# -..e.'
-# 
-# # this one should go before normalizeaccentedchars
-# #(and after splitting of the extension and folder parts)
-# >>> fixdotslash('abc/-.def this is no extension.')
-# 'abc_-_def this is no extension_'
-# 
-# ## do via unicode:
-# ## normalise a inivars key (or section)
-# >>> fixinivarskey('abcd')
-# 'abcd'
-# >>> fixinivarskey("abcd e'f  g")
-# 'abcd e_f g'
-# >>> fixinivarskey("##$$abcd)e'f  g*")
-# 'abcd_e_f g'
-# """
-#     if len(to) == 1:
-#         to = to * len(frm)
-#     trans = string.maketrans(frm, to)
-#     if keep is not None:
-#         delete = _allchars.translate(_allchars, keep.translate(_allchars, delete))
-#     def translate(s):
-#         return s.translate(trans)
-#     return translate
-# 
-# fixwordquotes = translator(b'\x91\x92\x93\x94\x95\x96', b"''\"\"  ")
-
-###removenoncharacters = translator('
-# def fixinivarskey(s):
-#     """remove all non letters to underscore, remove leading underscore
-#     remove double spaces
-#     """
-#     if isinstance(s, str):
-#         s = str(s)
-#     t = translate_non_alphanumerics(s)
-#     t = t.strip("_ ")
-#     while '  ' in t:
-#         t = t.replace('  ', ' ')
-#     return t
     
 def unifyaccentedchars(to_translate):
     """change acuted characters with combining code to single characters
     
 The combining variant (s3) is converted into the one character shorter variant s1, apart from the capitals.
 This is done by the NFC variant of the normalize function
     
@@ -144,79 +85,20 @@
                     # print('c cedilla, change to "s" (%s)'% to_translate)
                     shaved.pop()
                     shaved.append("s")
                 else:
                     # print("c cedilla, but NO C, ignore (%s)"% to_translate)
                     pass
             else:
-                print('(yet) unknown combining char %s in "%s", ignore'% (comb, to_translate))
+                print(f'(yet) unknown combining char {comb} in "{to_translate}", ignore')
             last = ""
         else:
             shaved.append(c)
             last = c
     return ''.join(shaved)
-    # shaved = ''.join(c for c in norm_txt if not unicodedata.combining(c))
-    # return shaved
-    
-# def convertToBinary(unicodeString, encoding=None):
-#     """convert a str (unicodeString) to bytes
-#     
-#     encode encoding (list of strings or string).
-#     when encoding is None: take ['ascii', 'cp1252', 'latin-1']
-#     
-# ## \u0041 is A
-# ##unichr(233) or \u00e9 is e accent acute
-#     
-# # >>> t = '\u0041-xyz-' + unichr(233) + '-abc-'
-# >>> t = '\u0041-xyz-\u00e9-abc-'
-# >>> convertToBinary(t)
-# b'A-xyz-\\xe9-abc-'
-# >>> convertToBinary(t+'ascii', 'ascii')
-# convertToBinary, cannot convert to printable string with encoding: ['ascii']
-# return with "?": b'A-xyz-?-abc-ascii'
-# b'A-xyz-?-abc-ascii'
-# >>> convertToBinary(t+'cp1252', 'cp1252')
-# b'A-xyz-\\xe9-abc-cp1252'
-# >>> byteslatin1 = convertToBinary(t+'latin-1', 'latin-1')
-# >>> byteslatin1
-# b'A-xyz-\\xe9-abc-latin-1'
-# >>> bytesutf8 = convertToBinary(t+'utf-8', 'utf-8')
-# >>> bytesutf8
-# b'A-xyz-\\xc3\\xa9-abc-utf-8'
-# >>> convertToBinary(t+'ascii + cp1252', ['ascii', 'cp1252'])
-# b'A-xyz-\\xe9-abc-ascii + cp1252'
-# >>> convertToBinary(convertToBinary(t+'double convert'))
-# b'A-xyz-\\xe9-abc-double convert'
-# >>> convertToBinary(byteslatin1)
-# b'A-xyz-\\xe9-abc-latin-1'
-# >>> convertToBinary(bytesutf8)
-# b'A-xyz-\\xe9-abc-utf-8'
-# 
-# ## \x92 (PU2) is from cp1252 (windows convention): 
-# >>> convertToBinary('fondationnimba rapportsd\x92archive index.html')
-# b'fondationnimba rapportsd\\x92archive index.html'
-#     """
-#     # a binary string can hold accented characters:
-#     if type(unicodeString) == bytes:
-#         unicodeString = convertToUnicode(unicodeString)
-#     if encoding is None:
-#         encoding = ['ascii', 'cp1252', 'latin-1']
-#     elif encoding and type(encoding) in (str, bytes):
-#         encoding = [encoding]
-#     res = ''
-#     for enc in encoding:
-#         try:
-#             res = unicodeString.encode(enc)
-#             break
-#         except UnicodeEncodeError:
-#             pass
-#     else:
-#         res = unicodeString.encode('ascii', 'replace')
-#         print('convertToBinary, cannot convert to printable string with encoding: %s\nreturn with "?": %s'% (encoding, res))
-#     return res
 
 class peek_ahead:
     """ An iterator that supports a peek operation.
     
     Improved for python3 after QH's example: Adapted for python 3 by Paulo Roma.
     
     this is a merge of example 19.18 of python cookbook part 2, peek ahead more steps
@@ -399,14 +281,15 @@
             self.count += n
         self.preview = self._cache[0]
         return result
 
     def next(self,n=None):
         """python2 compatibility
         """
+        #pylint:disable=C2801
         return self.__next__(n)
     
     def isFirst(self):
         """returns true if iter is at first position
         """
         return self.count == 0
 
@@ -473,42 +356,14 @@
                 line = line.rstrip()
                 Next = (len(line) - len(line.lstrip()), line.lstrip())
             except StopIteration:
                 # store sentinel, to identify end of iter:
                 Next = self.sentinel
             self._cache.append(Next)
      
-
-def isSubList(largerList, smallerList):
-    """returns 1 if smallerList is a sub list of largerList
-
->>> isSubList([1,2,4,3,2,3], [2,3])
-True
->>> isSubList([1,2,3,2,2,2,2], [2])
-True
->>> isSubList([1,2,3,2], [2,4])
-False
-    """
-    if not smallerList:
-        raise ValueError("isSubList: smallerList is empty: %s"% smallerList)
-    item0 = smallerList[0]
-    lenSmaller = len(smallerList)
-    lenLarger = len(largerList)
-    if lenSmaller > lenLarger:
-        return False  # can not be sublist
-    # get possible relevant indexes for first item
-    indexes0 = [i for (i,item) in enumerate(largerList) if item == item0 and i <= lenLarger-lenSmaller]
-    if not indexes0:
-        return False
-    for start in indexes0:
-        _slice = largerList[start:start+lenSmaller]
-        if _slice == smallerList:
-            return True
-    return False
-
 # helper string functions:
 def replaceExt(fileName, ext):
     """change extension of file
 
 >>> replaceExt("a.psd", ".jpg")
 'a.jpg'
 >>> replaceExt("a/b/c/d.psd", "jpg")
@@ -528,45 +383,15 @@
 '.psd'
 >>> getExt("abcd")
 ''
 >>> getExt("a/b/xyz")
 ''
     """
     _a, ext = os.path.splitext(fileName)
-    return str(ext)
-
-def fileHasImageExtension(fileName):
-    """return True if fileName has extension .jpg, .jpeg or .png
->>> fileHasImageExtension(u"a.JPG")
-True
->>> fileHasImageExtension(u"yyy.JPEG")
-True
->>> fileHasImageExtension(u"C:/a/b/d/e/xxx.png")
-True
->>> fileHasImageExtension(u"a.txt")
-False
-
-    """
-    ext = getExt(fileName)
-    if not ext:
-        return None
-    return ext.lower() in [".jpg", ".jpeg", ".png"]
-
-def fileHasJpgExtension(fileName):
-    """return True if fileName has extension .jpg, .jpeg
->>> fileHasJpgExtension(u"a.JPG")
-True
->>> fileHasJpgExtension(u"yyy.PNG")
-False
-
-    """
-    ext = getExt(fileName)
-    if not ext:
-        return None
-    return ext.lower() in [".jpg", ".jpeg"]
+    return ext
 
 def removeFromStart(text, toRemove, ignoreCase=None):
     """returns the text with "toRemove" stripped from the start if it matches
 >>> removeFromStart('abcd', 'a')
 'bcd'
 >>> removeFromStart('abcd', 'not')
 'abcd'
@@ -586,14 +411,15 @@
         toRemove = toRemove.lower()
     else:
         text2 = text
     if text2.startswith(toRemove):
         return text[len(toRemove):]
     return text
 
+
 def removeFromEnd(text, toRemove, ignoreCase=None):
     """returns the text with "toRemove" stripped from the end if it matches
 
 >>> removeFromEnd('a.jpg', '.jpg')
 'a'
 >>> removeFromEnd('b.jpg', '.gif')
 'b.jpg'
@@ -707,85 +533,17 @@
 'short__t.html'
 >>> appendBeforeExt("http://a/b/c/d/long.html", '__b')
 'http://a/b/c/d/long__b.html'
     """
     base, ext = os.path.splitext(text)
     return base + toAppend + ext
 
-def getBaseFolder(globalsDict):
-    """get in a module the folder of this module.
-
-    either sys.argv[0] (when run direct) or
-    __file__, which can be empty. In that case take the working directory
-    """
-    baseFolder = ""
-    if globalsDict['__name__']  == "__main__":
-        baseFolder = os.path.split(sys.argv[0])[0]
-        print('baseFolder from argv: %s'% baseFolder)
-    elif globalsDict['__file__']:
-        baseFolder = os.path.split(globalsDict['__file__'])[0]
-        print('baseFolder from __file__: %s'% baseFolder)
-    if not baseFolder or baseFolder == '.':
-        baseFolder = os.getcwd()
-    return baseFolder
-
 Classes = ('ExploreWClass', 'CabinetWClass')
 
 
-def partition_range(max_range):
-    """partition for milla website in lengths of 3 or 4
-    
->>> partition_range(3)
-[[0], [1], [2]]
->>> partition_range(5)
-[[0], [1], [2], [3, 4]]
->>> partition_range(8)
-[[0, 1], [2, 3], [4, 5], [6, 7]]
->>> partition_range(12)
-[[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]]
-
-    """
-    lst = list(range(max_range))
-    if max_range <= 4:
-        return [[i] for i in lst]
-    if max_range == 5:
-        L = [[i] for i in range(4)]
-        L[3].append(4)
-        return L
-    if max_range == 6:
-        return [[0, 1], [2, 3], [4, 5]]
-    if max_range == 7:
-        return [[0], [1, 2], [3, 4], [5, 6]]
-    if max_range == 8:
-        return [[0, 1], [2, 3], [4, 5], [6, 7]]
-    return [lst] # alle images achter elkaar, scrollen afhankelijk van de browser
-    
-
-
-
-        
-
-def unravelList(menu):
-    """unravel from menu list to dropdown list order
-    
->>> unravelList([1, [2, [3, 4, 5], 6], 7, 8])
-[[1, 7, 8], [2, 6], [3, 4, 5]]
-
-    """
-    L, M = [], None
-    for elt in menu:
-        if isinstance(elt, list):
-            M = unravelList(elt)
-        else:
-            L.append(elt)
-    if M and isinstance(M, list):
-        M.insert(0, L)
-        return M
-    return [L]
-
 ## to pathqh:
 # # def toUnixName(t, glueChar="", lowercase=1, canHaveExtension=1, canHaveFolders=1, mayBeEmpty=False):
     
 def sendkeys_escape(Str):
     """escape with {} keys that have a special meaning in sendkeys
     + ^ % ~ { } [ ]
 
@@ -806,196 +564,14 @@
     """Escape one character in the set or return if different"""
     if s in ('+', '^', '%', '~', '{' , '}' , '[' , ']' ) :
         result = '{%s}' % s
     else:
         result = s
     return str(result)
 
-def print_exc_plus(filename=None, skiptypes=None, takemodules=None,
-                   specials=None):
-    """ Print the usual traceback information, followed by a listing of
-    all the local variables in each frame.
-    
-    
-    """
-    #print('specials:', specials')
-    # normal traceback:
-    traceback.print_exc()
-    tb = sys.exc_info()[2]
-    while tb.tb_next:
-        tb = tb.tb_next
-    stack = []
-    f = tb.tb_frame
-    while f:
-        stack.append(f)
-        f = f.f_back
-    stack.reverse()
-    traceback.print_exc()
-    L = []
-    # keys that are in specialsSitegen are recorded in next array:
-    specialsDict = {}
-    push = L.append
-
-    push('traceback date/time: %s'% time.asctime(time.localtime(time.time())))
-    pagename = ''
-    menuname = ''
-    for frame in stack:
-        if takemodules and not [_f for _f in [frame.f_code.co_filename.find(t) > 0 for t in takemodules] if _f]:
-            continue
-        functionname = frame.f_code.co_name
-        push('\nFrame "%s" in %s at line %s' % (frame.f_code.co_name,
-                                frame.f_code.co_filename,
-                                frame.f_lineno))
-        keys = []
-        values = []
-        for key, value in list(frame.f_locals.items()):
-            if key[0:2] == '__':
-                continue
-            try:
-                v = repr(value)
-            except:
-                continue
-            if skiptypes and [_f for _f in [v.find(s) == 1 for s in skiptypes] if _f]:
-                continue
-            keys.append(key)
-            if functionname == 'go' and key == 'self':
-                if v.find('Menu instance') > 0:
-                    menuname = value.name
-                    push('menu name: %s'% menuname)
-            if functionname == 'makePage' and key == 'self':
-                if v.find('Page instance') > 0:
-                    pagename = value.name
-                    push('page name: %s'% pagename)
-
-            # we must _absolutely_ avoid propagating exceptions, and value
-            # COULD cause any exception, so we MUST catch any...:
-            v = v.replace('\n', '|')
-            values.append(v)
-        if keys:
-            maxlenkeys = max(15, max(list(map(len, keys))))
-            allowedlength = 80-maxlenkeys
-            kv = list(zip(keys, values))
-            kv.sort()
-            for k,v in kv:
-                if v.startswith('<built-in method'):
-                    continue
-                if len(v) > allowedlength:
-                    half = allowedlength//2
-                    v = v[:half] + " ... " + v[-half:]
-                push(k.rjust(maxlenkeys) + " = " + v)
-    if specials:
-        stack.reverse()
-        for frame in stack:
-            if 'self' in frame.f_locals:
-                push('\ncontents of self (%s)'% repr(frame.f_locals['self']))
-                inst = frame.f_locals['self']
-                keys, values = [], []
-                for key in dir(inst):
-                    value = getattr(inst, key)
-                    if key[0:2] == '__':
-                        continue
-                    try:
-                        v = repr(value)
-                    except:
-                        continue
-                    if skiptypes and [_f for _f in [v.find(s) == 1 for s in skiptypes] if _f]:
-                        continue
-                    # specials for eg sitegen
-                    if specials and key in specials:
-                        #print('found specialskey: %s: %s'% (key, v)')
-                        specialsDict[key] = v
-                    keys.append(key)
-                    # we must _absolutely_ avoid propagating exceptions, and value
-                    # COULD cause any exception, so we MUST catch any...:
-                    v = v.replace('\n', '|')
-                    values.append(v)
-                if not keys:
-                    break
-                maxlenkeys = max(15, max(list(map(len, keys))))
-                allowedlength = 80-maxlenkeys
-                for k,v in zip(keys, values):
-                    if v and len(v) > allowedlength:
-                        half = allowedlength//2
-                        v = v[:half] + " ... " + v[-half:]
-                    push(k.rjust(maxlenkeys) + " = " + str(v))
-                break
-            print('no self of HTMLDoc found')
-
-    callback = []
-
-    if menuname:
-        push('menu: %s'% menuname)
-        callback.append('menu: %s'% menuname)
-    elif pagename == 'index':
-        push('menu: top')
-        callback.append('menu: top')
-        
-    if pagename:
-        push('page: %s'% pagename)
-        callback.append('page: %s'% pagename)
-    push('\ntype: %s, value: %s\n'% (sys.exc_info()[0], sys.exc_info()[1]))
-    callback.append('error: %s'%sys.exc_info()[1])
-
-    print('\nerror occurred:')
-    callback = '\n'.join(callback)
-    print(callback)
-
-    sys.stderr.write('\n'.join(L))
-    sys.stderr.write(callback)
-    if filename:
-        print("skip writing to file %s"% filename)
-        # with open(filename, 'w') as fout:
-        #     fout.write("\n".join(L))
-        #     print("written traceback in %s"% filename)    
-    #print('result specialsDict: %s'% specialsDict')
-    return callback, specialsDict
-
-def cleanTraceback(tb, filesToSkip=None):
-    """strip boilerplate in traceback (unittest)
-
-    the purpose is to skip the lines "Traceback" (only if filesToSkip == True),
-    and to skip traceback lines from modules that are in filesToSkip.
-
-    in use with unimacro unittest and voicecode unittesting.
-
-    filesToSkip are (can be "unittest.py" and "TestCaseWithHelpers.py"
-
-    """
-    L = tb.split('\n')
-    snip = "  ..." # leaving a sign of the stripping!
-    if filesToSkip:
-        singleLineSkipping = ["Traceback (most recent call last):"]
-    else:
-        singleLineSkipping = None
-    M = []
-    skipNext = 0
-    for line in L:
-        # skip the traceback line:
-        if singleLineSkipping and line in singleLineSkipping:
-            continue
-        # skip trace lines from one one the filesToSkip and the next one
-        # UNLESS there are no leading spaces, in case we hit on the error line itself.
-        if skipNext and line.startswith(" "):
-            skipNext = 0
-            continue
-        if filesToSkip:
-            for f in filesToSkip:
-                if line.find(f + '", line') >= 0:
-                    skipNext = 1
-                    if M and  M[-1] == snip:
-                        pass
-                    else:
-                        M.append(snip)
-                    break
-            else:
-                skipNext = 0
-                M.append(line)
-
-    return '\n'.join(M)
-
 def getSublists(L, maxLen, sepLen):
     """generator function, that gives pieces of the list, up to
     the maximum length, accounting for the separator length
     """
     if not L:
         yield L
         return
@@ -1203,25 +779,25 @@
 
     # if input string is a number, return string directly
     try:
         i = int(t)
         if t == '0':
             return 0
         if t.startswith('0'):
-            print('warning convertToPythonArg, could be int, but assume string: %s'% t)
-            return '%s'% t
+            print(f'warning convertToPythonArg, could be int, but assume string: {t}')
+            return str(t)
         return i
     except ValueError:
         pass
     try:
         f = float(t)
         if t.find(".") >= 0:
             return f
-        print('warning convertToPythonArg, can be float, but assume string: %s'% t)
-        return '%s'% t
+        print(f'warning convertToPythonArg, can be float, but assume string: {t}')
+        return str(t)
     except ValueError:
         pass
 
     # now proceeding with strings:    
     if hasDoubleQuotes.match(t):
         return t[1:-1]
     if hasSingleQuotes.match(t):
```

### Comparing `dtactions-1.5.7/src/dtactions/vocola_sendkeys/ExtendedSendDragonKeys.py` & `dtactions-1.6.1/src/dtactions/vocola_sendkeys/ExtendedSendDragonKeys.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/src/dtactions/vocola_sendkeys/SendInput.py` & `dtactions-1.6.1/src/dtactions/vocola_sendkeys/SendInput.py`

 * *Files identical despite different names*

### Comparing `dtactions-1.5.7/PKG-INFO` & `dtactions-1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dtactions
-Version: 1.5.7
+Version: 1.6.1
 Summary: dtactions __init__
 Keywords: dragon,speech,dictation,dictation-toolbox,natlink
 Author-email: Quintijn Hoogenboom <q.hoogenboom@antenna.nl>
 Maintainer-email: Quintijn Hoogenboom <q.hoogenboom@antenna.nl>, LexiconCode <CasterVoice@protonmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Dist: pywin32 >= 300
 Requires-Dist: debugpy
+Requires-Dist: platformdirs
 Requires-Dist: pyenvutils ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pytest >=7.1.2 ; extra == "test"
 Project-URL: Home, https://github.com/dictation-toolbox/dtactions
 Project-URL: Readthedocs, https://dtactions.readthedocs.io/en/latest/sendkeys.html
 Provides-Extra: dev
 Provides-Extra: test
@@ -65,16 +66,18 @@
 You can run `py -m pip install dtactions[test]` or `py -m pip install dtactions[natlink_test]` if you don't have the prequisites like pytest.  
 
 You can run pytest from project root folder to run the tests that don't depend on natlink being installed.  For the natlink-dependent tests, run 
 `py -m pytest natlink_test`.  
 
 ## Notes About Packaging for Developers
 
-The package is specified in `pyproject.toml` and built with [flit](https://pypi.org/project/flit/). 
+The package is specified in `pyproject.toml` and uses  [flit](https://pypi.org/project/flit/) as the underlying build tool. 
 
-`py -m flit build` (or just `flit build`) builds the package.  A github action publishes to  publishes to [Python Packaging Index](https://pypi.org/). 
+Too build the package locally, 
+
+`py -m flit build` (or just `flit build`) builds the package. You can also use `python -m build` if you have build installed.   A github action publishes to  publishes to [Python Packaging Index](https://pypi.org/). 
 
 
  
 Version numbers of the packages must be increased before your publish to [Python Packaging Index](https://pypi.org/).
```

