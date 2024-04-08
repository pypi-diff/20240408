# Comparing `tmp/shdo-0.0.7.tar.gz` & `tmp/shdo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.7.tar", last modified: Tue Apr  2 22:41:22 2024, max compression
+gzip compressed data, was "shdo-0.0.8.tar", last modified: Mon Apr  8 14:07:58 2024, max compression
```

## Comparing `shdo-0.0.7.tar` & `shdo-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:41:22.126342 shdo-0.0.7/
--rw-rw-rw-   0        0        0      329 2024-04-02 22:41:22.125343 shdo-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 22:41:22.127342 shdo-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      619 2024-04-02 22:41:17.000000 shdo-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:41:22.123331 shdo-0.0.7/shdo.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-02 22:41:21.000000 shdo-0.0.7/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 22:41:22.000000 shdo-0.0.7/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:41:21.000000 shdo-0.0.7/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-02 22:41:21.000000 shdo-0.0.7/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 22:41:21.000000 shdo-0.0.7/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16238 2024-04-02 22:41:10.000000 shdo-0.0.7/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:07:58.538776 shdo-0.0.8/
+-rw-rw-rw-   0        0        0      329 2024-04-08 14:07:58.537763 shdo-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2036 2024-04-08 14:07:04.000000 shdo-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:07:58.539692 shdo-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      619 2024-04-08 14:07:41.000000 shdo-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:07:58.537263 shdo-0.0.8/shdo.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17494 2024-04-08 12:55:30.000000 shdo-0.0.8/shdo.py
```

### Comparing `shdo-0.0.7/setup.py` & `shdo-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.0.7',
+    version='0.0.8',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
             'shdo = shdo:main',
             'shdo-pair = shdo:main',
```

### Comparing `shdo-0.0.7/shdo.py` & `shdo-0.0.8/shdo.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,36 +47,32 @@
     # start the shdo main function
     return shdo_main()
 
 
 # shdo main function
 def shdo_main():
 
-    # parse the command line parameters
-    argc = len(sys_argv)
-    argv = sys_argv
-
-    # check usage
-    if argc <= 1:
-        print("Usage: shdo <command> [parameters]")
-        return 1
-    
     # check if we're running the tool with termux
     if 'TERMUX_VERSION' not in environ:
         print("Error: You need to run this tool from Termux. If you want to run this tool anyway create the environment variable 'TERMUX_VERSION'.")
         return 1
     
-    # build the command
-    parameters = ""
-    if argc >= 3:
-        for parameter in argv[2:]:
-            parameters += f" '{parameter}'"
+    # parse the command line parameters
+    sys_argc = len(sys_argv)
+    command = None
+    if sys_argc > 1:
+        command = sys_argv[1]
+        if sys_argc > 2:
+            parameters = ""
+            if sys_argc >= 3:
+                for parameter in sys_argv[2:]:
+                    parameters += f" '{parameter}'"
 
     # run the command
-    result = run_command(argv[1], parameters, verbose=False)
+    result = run_command(command, parameters, verbose=False)
     if result is None:
         return 1
     
     # end of process
     return result
 
 
@@ -110,14 +106,20 @@
     print("shdo was successfully paired!")
     return 0
 
 
 # run an elevated command
 def run_command(command, parameters, verbose=False):
 
+    # check if the adb daemon is running
+    result = _terminal.run_command("getprop init.svc.adbd")[0].strip(' \n\t\r')
+    if result != 'running':
+        print("Error: The ADB daemon is not running. Start Wireless Debugging from the Developer Settings.")
+        return None
+
     # start the adb server
     _adb.start_server(verbose=verbose)
 
     # check if we are already connected
     if _adb.is_connected(verbose=verbose) == False:
 
         # connect to the adb server
@@ -126,77 +128,90 @@
             # print the error if needed
             print("Error: Couldn't connect to the adb server. Are you sure the adb server is paired with Termux ? Are you sure the adb wi-fi is on ?")
             
             # couldn't connect to the adb server
             return None
         
     # auto-bounce the file or executable if needed
-    if SHDO_AUTO_BOUNCE == True:
+    if SHDO_AUTO_BOUNCE == True and command is not None:
 
         # check if the command is an executable (bash, elf, ...)
         if file_exists(command) == True:
 
             # remove extra dot
             if command.startswith("./") == True:
                 filename = command[2:]
 
-            # copy the file to the bounce folder
-            if verbose == True:
-                print(f"[*] Copying the file {filename} to bounce folder...", end='', flush=True)
-            bounce_path = SHDO_BOUNCE_FOLDER_PATH + filename
-            try:
-                file_copy(filename, bounce_path)
-            except SameFileError:
-                pass
-            if verbose == True:
-                print("done.")
+            # check if we're in a Termux folder
+            if _terminal.in_termux_folder() == True:
 
-            # copy the file to the debug folder
-            if verbose == True:
-                print(f"[*] Copying the file {filename} to debug folder...", end='', flush=True)
-            debug_path = SHDO_DEBUG_FOLDER_PATH + filename
-            _adb.shell(f"cp '{bounce_path}' '{debug_path}'")
-            if verbose == True:
-                print("done.")
+                # copy the file to the bounce folder
+                if verbose == True:
+                    print(f"[*] Copying the file {filename} to bounce folder...", end='', flush=True)
+                bounce_path = SHDO_BOUNCE_FOLDER_PATH + filename
+                try:
+                    file_copy(filename, bounce_path)
+                except SameFileError:
+                    pass
+                if verbose == True:
+                    print("done.")
+
+            # check if we're in a Termux folder
+            if _terminal.in_shell_folder() == False:
+
+                # copy the file to the debug folder
+                if verbose == True:
+                    print(f"[*] Copying the file {filename} to debug folder...", end='', flush=True)
+                debug_path = SHDO_DEBUG_FOLDER_PATH + filename
+                _adb.shell(f"cp '{bounce_path}' '{debug_path}'")
+                if verbose == True:
+                    print("done.")
 
             # give execution permission to the script or executable
             if verbose == True:
                 print(f"[*] Giving the file {filename} execution permission...", end='', flush=True)
             _adb.shell(f"chmod 755 '{debug_path}'")
             if verbose == True:
                 print("done.")
             
             # change the command by its new path
             command = debug_path
 
     # build the full command
-    full_command = f"'{command}' {parameters}"
+    full_command = f"'{command}' {parameters}" if command is not None else None
         
     # run the elevated command
     return _adb.execute(full_command, verbose=verbose)
 
 
 # handle everything about android debug bridge
 class _adb:
         
     # execute an adb command
     def execute(command, verbose=False):
 
+        # build the command
+        full_command = f"adb -s 127.0.0.1:{current_adb_port} shell"
+        if command is not None:
+            full_command += f" '{command}'"
+            if verbose == True:
+                print("[*] Executing the command...\n")
+        elif verbose == True:
+            print("[*] Running the shell...\n")
+        
         # execute the command
-        if verbose == True:
-            print("[*] Executing the command...\n")
-        return system(f"adb -s 127.0.0.1:{current_adb_port} shell {command}")
+        return system(full_command)
 
 
     # run an adb command
-    def command(command):
+    def command(command, timeout=None):
 
         # run the terminal command
         command = f"adb {command}"
-        stdout, stderr = _terminal.run_command(command)
+        stdout, stderr = _terminal.run_command(command, timeout=timeout)
 
         # check if there was an error
         if stderr.startswith("adb: ") == True:
 
             # check if the device is unknown
             if stderr.find("not found") != -1:
                 return None
@@ -287,15 +302,15 @@
     
 
     # try to pair with a adb server
     def try_pair(adb_server_port, pairing_code):
         global adb_is_paired
 
         # run the adb pair command
-        result = _adb.command(f"pair 127.0.0.1:{adb_server_port} {pairing_code}")
+        result = _adb.command(f"pair 127.0.0.1:{adb_server_port} {pairing_code}", timeout=1)
         if result is None:
             return False
 
         # check if the pairing was successfull
         if result[0].find("Successfully paired to") != -1:
             adb_is_paired = True
             return True
@@ -352,15 +367,15 @@
 
     # try to connect to an adb server
     def try_connect(adb_server_port, verbose=False):
         global current_adb_port
         global connected_adb_port
 
         # run the adb connect command
-        result = _adb.command(f"connect 127.0.0.1:{adb_server_port}")
+        result = _adb.command(f"connect 127.0.0.1:{adb_server_port}", timeout=1)
         if result is None:
             if verbose == True:
                 print(f"[*] Can't connect to adb server {adb_server_port}.")
             return False
         
         # check for errors
         if result[0].find('cannot connect to') != -1:
@@ -384,24 +399,37 @@
         return True
 
 
 # handle everything about terminal
 class _terminal:
 
     # run a terminal command
-    def run_command(command):
+    def run_command(command, timeout=None):
 
         # open a process to run the command
-        process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
+        if timeout is not None:
+            process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE, timeout=timeout)
+        else:
+            process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
         stdout, stderr = process.communicate()
 
         # return the process (command) output
         stdout = stdout.decode()
         stderr = stderr.decode()
         return (stdout, stderr)
+    
+
+    # TODO: check if we are in a Termux folder
+    def in_termux_folder():
+        return False
+    
+
+    # TODO: check if we are in a Shell folder
+    def in_shell_folder():
+        return False
 
 
 # handle everything about cache
 class _cache:
         
     # load the adb server port
     def load(verbose=False):
```

