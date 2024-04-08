# Comparing `tmp/omdeventhandler-0.5.0.tar.gz` & `tmp/omdeventhandler-1.0.tar.gz`

## Comparing `omdeventhandler-0.5.0.tar` & `omdeventhandler-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0     6905 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/bin/eventhandler
--rw-r--r--   0        0        0    11211 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/baseclass.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/bash/runner.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/default/decider.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/nsc_web/runner.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/omd_site_self_heal/decider.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/ssh/runner.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/test_classes.py
--rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/test_notify.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/test_package.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/eventhandler/example/runner.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     6740 2020-02-02 00:00:00.000000 omdeventhandler-1.0/bin/eventhandler
+-rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/baseclass.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/bash/runner.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/default/decider.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/nsc_web/runner.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/omd_site_self_heal/decider.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/ssh/runner.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/test_classes.py
+-rw-r--r--   0        0        0     8552 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/test_notify.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/test_package.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/pythonpath/local/lib/python/eventhandler/example/runner.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdeventhandler-1.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omdeventhandler-1.0/README.md
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 omdeventhandler-1.0/pyproject.toml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 omdeventhandler-1.0/PKG-INFO
```

### Comparing `omdeventhandler-0.5.0/bin/eventhandler` & `omdeventhandler-1.0/bin/eventhandler`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                       help='Show logs at stdout',
                       default=False)
     parser.add_argument('--debug', action='store_true',
                       dest="debug",
                       help='Increase the log level to DEBUG',
                       default=False)
     parser.add_argument('--version', action='version',
-                      version=f'%(prog)%s 0.5.0')
+                      version=f'%(prog)%s 1.0')
 
     args = parser.parse_args()
     if not any(vars(args).values()):
         parser.print_help()
         parser.exit()
 
     if os.path.exists(os.environ["OMD_ROOT"]+"/var/log/eventhandler.debug"):
@@ -143,12 +143,8 @@
             logger = logging.getLogger(logger_name)
             if args.debug:
                 traceback.print_exc(file=sys.stdout)
             logger.critical("there is no class for forwarder {} and formatter {}".format(args.forwarder, args.formatter))
             sys.exit(1)
     
     success = runner.handle(args.eventopt)
-    if args.forwarder:
-        if success != None:
-            args.eventopt["eventhandler_success"] = success
-            runner.forwarder.forward(args.eventopt)
     sys.exit(1 if success == False else 0)
```

### Comparing `omdeventhandler-0.5.0/src/eventhandler/baseclass.py` & `omdeventhandler-1.0/src/eventhandler/baseclass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABCMeta, abstractmethod
 import os
+import re
 import socket
 import traceback
 import signal
 import functools
 import errno
 import fcntl
 import time
@@ -134,14 +135,17 @@
             return decided_event
         except Exception as e:
             logger.critical("when deciding based on this {} with this {} there was an error <{}>".format(str(raw_event), instance.__class__.__name__+"@"+instance.__module_file__, str(e)))
             return None
 
     def handle(self, raw_event):
         success = False
+        if "SERVICEDESC" in raw_event:
+            if re.match(r'(Return\ code\ of|Timed\ Out|timed\ out|check_by_ssh:\ Remote\ command|service\ check\ orphaned)', raw_event["SERVICEDESC"]):
+                return True
         try:
             decided_event = self.decide_and_prepare_event(raw_event)
             if decided_event.is_discarded:
                 if not decided_event.is_discarded_silently:
                     if not decided_event.summary:
                         decided_event.summary = str(raw_event)
                     logger.info("discarded: {}".format(decided_event.summary))
@@ -154,15 +158,33 @@
                 decided_event
             except NameError:
                 logger.critical("raw event {} caused error {}".format(str(raw_event), str(e)))
             decided_event = None
             success = None
         if decided_event:
             self.overwrite_attributes(decided_event.payload)
-            success = self.run_decided(decided_event)
+            success, stdout, stderr = self.run_decided(decided_event)
+            if hasattr(self, "forwarder"):
+                raw_event["NOTIFICATIONTYPE"] = "EVENTHANDLER"
+                raw_event["NOTIFICATIONAUTHOR"] = self.runner_name
+                raw_event["NOTIFICATIONCOMMENT"] = "stdout: {}, stderr: {}".format(stdout if stdout else "-", stderr if stderr else "-")
+                if "SERVICEDESC" in raw_event:
+                    if success:
+                        raw_event["SERVICESTATE"] = "OK"
+                    else:
+                        raw_event["SERVICESTATE"] = "CRITICAL"
+                else:
+                    if success:
+                        raw_event["HOSTSTATE"] = "UP"
+                    else:
+                        raw_event["HOSTSTATE"] = "DOWN"
+                raw_event["eventhandler_success"] = success
+                if success != None:
+                    # none means, python runner has aborted intentionally
+                    self.forwarder.forward(raw_event)
         return success
 
     def overwrite_attributes(self, payload):
         # paload can overwrite runneropts
         for k in payload:
             if hasattr(self, k):
                 setattr(self, k, payload[k])
@@ -198,23 +220,23 @@
             success = False
             decide_exception_msg = str(e)
 
         if success:
             if self.baseclass_logs_summary:
                 logger.info("{}".format(decided_event.summary))
                 logger.debug("stdout {}, stderr {}".format(stdout if stdout else "", stderr if stderr else ""))
-            return True
+            return True, stdout, stderr
         else:
             if stderr:
                 logger.critical("run failed: stdout {}, stderr {}, event {}".format(stdout if stdout else "", stderr if stderr else "", decided_event.summary))
             elif decide_exception_msg:
                 logger.critical("run failed: exception <{}>, event was <{}>".format(decide_exception_msg, decided_event.summary))
             elif self.baseclass_logs_summary:
                 logger.critical("run failed: stdout {}, stderr {}, exitcode {}, event {}".format(stdout if stdout else "", stderr if stderr else "", exit_code, decided_event.summary))
-            return False
+            return False, stdout, stderr
 
 
     def no_more_logging(self):
         # this is called in the runner. If the runner already wrote
         # it's own logs and writing the summary by the baseclass is not
         # desired.
         self.baseclass_logs_summary = False
```

### Comparing `omdeventhandler-0.5.0/src/eventhandler/default/decider.py` & `omdeventhandler-1.0/src/eventhandler/default/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.5.0/src/eventhandler/nsc_web/runner.py` & `omdeventhandler-1.0/src/eventhandler/nsc_web/runner.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.5.0/src/eventhandler/omd_site_self_heal/decider.py` & `omdeventhandler-1.0/src/eventhandler/omd_site_self_heal/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.5.0/src/eventhandler/ssh/runner.py` & `omdeventhandler-1.0/src/eventhandler/ssh/runner.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.5.0/tests/test_classes.py` & `omdeventhandler-1.0/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.5.0/tests/test_notify.py` & `omdeventhandler-1.0/tests/test_notify.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
     assert payload["signature"] == "no_"+random_string
     assert payload["description"] == "i_describe_an_eventhandler"
     assert os.path.exists(omd_root+"/var/log/notificationforwarder_webhook_evtnot.log")
     with open(omd_root+"/var/log/notificationforwarder_webhook_evtnot.log") as f:
         notlog = f.read().strip()
     assert "signature=no_"+random_string in notlog
     assert "eventhandler for vongsrv04/some_service succeeded" in notlog
+    assert "notificationtype=EVENTHANDLER" in notlog
+    assert "notificationauthor=example_evthdl" in notlog
 
 
 def test_eventhandler_failure_notification(server_fixture):
     tic = time.time()
     random_string = ''.join(secrets.choice(string.ascii_letters + string.digits) for _ in range(10))
     command = """PYTHONPATH=$PYTHONPATH OMD_SITE=my_devel_site OMD_ROOT={} {} \\
         --runner example \\
```

### Comparing `omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py` & `omdeventhandler-1.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py` & `omdeventhandler-1.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,10 +8,13 @@
         json_payload = {
             'timestamp': time.time(),
         }
         json_payload['description'] = event.eventopts['description']
         if 'signature' in event.eventopts:
             json_payload['signature'] = event.eventopts['signature']
         event.payload = json_payload
+        ident = "notificationtype={},notificationauthor={}".format(
+            event.eventopts["NOTIFICATIONTYPE"],
+            event.eventopts["NOTIFICATIONAUTHOR"])
         # ! event.eventopts["eventhandler_success"] is a string !
         # all eventopts are cast to strings, so "True" or "False"
-        event.summary = "eventhandler for {}/{} {} (signature={})".format(event.eventopts["HOSTNAME"], event.eventopts["SERVICEDESC"], "succeeded" if event.eventopts["eventhandler_success"] == "True" else "failed", event.eventopts["signature"])
+        event.summary = "eventhandler for {}/{} {} (signature={}), ident={}".format(event.eventopts["HOSTNAME"], event.eventopts["SERVICEDESC"], "succeeded" if event.eventopts["eventhandler_success"] == "True" else "failed", event.eventopts["signature"], ident)
```

### Comparing `omdeventhandler-0.5.0/pyproject.toml` & `omdeventhandler-1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 packages = ["src/eventhandler"]
 
 [tool.hatch.build.targets.wheel.force-include]
 "./bin/eventhandler" = "eventhandler/bin_folder/eventhandler"
 
 [project]
 name = "omdeventhandler"
-version = "0.5.0"
+version = "1.0"
 authors = [
   { name="Gerhard Lausser", email="lausser@yahoo.com" },
 ]
 description = "A framework for event handlers for OMD"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `omdeventhandler-0.5.0/PKG-INFO` & `omdeventhandler-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omdeventhandler
-Version: 0.5.0
+Version: 1.0
 Summary: A framework for event handlers for OMD
 Project-URL: Homepage, https://github.com/lausser/noteventificationforhandlerwarder
 Project-URL: Bug Tracker, https://github.com/lausser/noteventificationforhandlerwarder/issues
 Author-email: Gerhard Lausser <lausser@yahoo.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

