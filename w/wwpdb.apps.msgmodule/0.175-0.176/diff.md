# Comparing `tmp/wwpdb.apps.msgmodule-0.175.tar.gz` & `tmp/wwpdb.apps.msgmodule-0.176.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.msgmodule-0.175.tar", last modified: Thu Nov 30 00:12:37 2023, max compression
+gzip compressed data, was "wwpdb.apps.msgmodule-0.176.tar", last modified: Mon Apr  8 20:33:10 2024, max compression
```

## Comparing `wwpdb.apps.msgmodule-0.175.tar` & `wwpdb.apps.msgmodule-0.176.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.535766 wwpdb.apps.msgmodule-0.175/
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2023-11-30 00:12:37.535766 wwpdb.apps.msgmodule-0.175/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      301 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2023-11-30 00:12:37.535766 wwpdb.apps.msgmodule-0.175/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2326 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.527766 wwpdb.apps.msgmodule-0.175/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.531766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.531766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      151 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.531766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)    37932 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/depict/MessagingDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26771 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/depict/MessagingTemplates.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.531766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     1491 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/DateUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4420 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7771 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/MessagingDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7384 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/MessagingDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)   267971 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/MessagingIo.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.531766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/models/
--rw-r--r--   0 vsts      (1001) docker     (127)    17412 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/models/Message.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.535766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/util/
--rw-r--r--   0 vsts      (1001) docker     (127)     5316 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/util/AutoMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22343 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/util/ExtractMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.535766 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    82359 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/webapp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4918 2023-11-30 00:10:48.000000 wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-30 00:12:37.535766 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2023-11-30 00:12:37.000000 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1072 2023-11-30 00:12:37.000000 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-30 00:12:37.000000 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-30 00:12:22.000000 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2023-11-30 00:12:37.000000 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2023-11-30 00:12:37.000000 wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      301 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2326 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.352669 wwpdb.apps.msgmodule-0.176/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      151 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)    38649 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26771 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingTemplates.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1491 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/DateUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4420 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7771 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7384 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   269531 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingIo.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17412 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/Message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5613 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/AutoMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27867 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/ExtractMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    83116 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4918 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1072 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 20:32:52.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.msgmodule-0.175/PKG-INFO` & `wwpdb.apps.msgmodule-0.176/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.msgmodule
-Version: 0.175
+Version: 0.176
 Summary: wwPDB messaging module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.msgmodule-0.175/setup.py` & `wwpdb.apps.msgmodule-0.176/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/depict/MessagingDepict.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingDepict.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         #
         self.absltSessionPath = None
         self.absltEdtrSessionPath = None
         self.rltvSessionPath = None
         self.rltvEdtrSessionPath = None
         #
         self.__expMethodList = []
-        if self.__verbose:
-            logger.info("CStrack+++ initiate MessagingDepict class")
+        # if self.__verbose:
+        #     logger.info("CStrack+++ initiate MessagingDepict class")
 
     def doRender(self, p_reqObj, p_bIsWorkflow):
         """Render HTML used as starter page/container for the wwPDB Messaging interface
         Once this content is in the browser, AJAX calls are made to populate the page
         with content when needed.
 
         :Params:
@@ -201,26 +201,30 @@
                 myD["display_title"] = "GROUP/DEPOSITION IDS"
                 myD["display_identifier"] = groupId + "/" + myD["identifier"]
             #
         #
         tmpltFile = "msging_launch_embed_tmplt.html" if embeddedVw.lower() == "true" else "msging_launch_tmplt.html"
 
         oL.append(self.processTemplate(tmpltPth=tmpltPath, fn=tmpltFile, parameterDict=myD))
+        logger.info("CStrack+++ use html template of *%s*", tmpltFile)
         #
         return oL
 
     def getMsgTmplts(self, p_reqObj, p_bIsWorkflow):
         """Get
 
         :Helpers:
 
         :Returns:
 
         """
         #
+        logger.info("CStrack+++ dump input web request obj for templates generation")
+        logger.info("".join(p_reqObj.dump()))
+
         oL = []
         #
         strParamDict = {}
         #
         if self.__verbose:
             logging.info("-- Starting.")
         #
@@ -236,16 +240,16 @@
                 strParamDict["identifier"] = "D_000000"
             else:
                 strParamDict["identifier"] = depId
         #
         if self.__verbose:
             logger.info("\n -- dep_id is:%s", depId)
         #
-        if self.__verbose:
-            logger.info("CStrack+++ call MessagingIo class from MessagingDepict.getMsgTmplts()")
+        # if self.__verbose:
+        #     logger.info("CStrack+++ call MessagingIo class from MessagingDepict.getMsgTmplts()")
         msgingIo = MessagingIo(p_reqObj, self.__verbose, self.__lfh)
         msgingIo.initializeDataStore()  # THIS CALL MUST BE MADE HERE TO SUPPORT ALL DOWNSTREAM PROCESSING IN NEED OF DATA PARSED FROM THE COORDINATE FILE
         msgingIo.getMsgTmpltDataItems(strParamDict)
         starterMsgBody = msgingIo.getStarterMsgBody()
         #
         strParamDict["starter_msg_body"] = starterMsgBody if starterMsgBody is not None else ""
         strParamDict["msg_tmplt_default"] = (MessagingTemplates.msgTmplt_default_em % strParamDict) if b_em else (MessagingTemplates.msgTmplt_default % strParamDict)
@@ -255,15 +259,15 @@
         # strParamDict["msg_tmplt_approval-impl"] = (
         #     (MessagingTemplates.msgTmplt_approvalImplicit_em % strParamDict) if b_em else (MessagingTemplates.msgTmplt_approvalImplicit % strParamDict)
         # )  # noqa: E501
         strParamDict["msg_tmplt_reminder"] = (MessagingTemplates.msgTmplt_reminder_em % strParamDict) if b_em else (MessagingTemplates.msgTmplt_reminder % strParamDict)
 
         # CS 2022-02-27 add map-only withdrawn template;
         # CS 2023-10-20 start, further seperate all scenarios of EM model-map, model-only, and map-only. The selection process needs to be optimized later.
-        logger.info("strParamDict: %s", strParamDict)
+        # logger.info("strParamDict: %s", strParamDict)
         if b_em:
             logger.info("CStrack+++ EM-ENTRY")
             if strParamDict.get("pdb_id", "") == "[PDBID NOT AVAIL]":  # EM map-only
                 logger.info("CStrack+++ EM-MAP-ONLY")
                 strParamDict["msg_tmplt_withdrawn"] = MessagingTemplates.msgTmplt_withdrawn_em_map_only % strParamDict
                 strParamDict["msg_tmplt_approval-expl"] = MessagingTemplates.msgTmplt_approvalExplicit_em % strParamDict
                 strParamDict["msg_tmplt_approval-impl"] = MessagingTemplates.msgTmplt_approvalImplicit_em % strParamDict
@@ -313,16 +317,24 @@
             strParamDict["msg_tmplt_system-unlocked"] = MessagingTemplates.msgTmplt_systemUnlockedPostRel % strParamDict
         else:
             strParamDict["msg_tmplt_system-unlocked"] = (
                 (MessagingTemplates.msgTmplt_systemUnlocked_em % strParamDict) if b_em else (MessagingTemplates.msgTmplt_systemUnlocked % strParamDict)
             )  # noqa: E501
         strParamDict["msg_tmplt_maponly-authstatus-em"] = (MessagingTemplates.msgTmplt_mapOnly_authStatus_em % strParamDict) if b_em else ""
 
+        logger.info("CStrack+++ dump parameter dict for templates")
+        logger.info("\n".join(list(strParamDict.keys())))
+        # logger.info(strParamDict["msg_tmplt_vldtn"])
+        # logger.info(strParamDict["msg_tmplt_approval-expl"])
+
         oL.append(self.processTemplate(tmpltPth=tmpltPath, fn="msg_tmplts.html", parameterDict=strParamDict))
+        logger.info("CStrack+++ use html template of *msg_tmplts.html*")
         #
+        logger.info(''.join(oL))
+
         return oL
 
     def doRenderAllCorrespondence(self, p_reqObj):
         """Render HTML used as starter page/container for the wwPDB Messaging interface
         Once this content is in the browser, AJAX calls are made to populate the page
         with content when needed.
 
@@ -365,14 +377,15 @@
         myD["identifier"] = depId
         myD["session_url_prefix"] = self.rltvEdtrSessionPath
 
         tmpltFile = "msging_launch_commhstry_tmplt.html"
         # tmpltFile = "msging_launch_embed_tmplt.previewMsg.html" if embeddedVw.lower() == "true" else "msging_launch_tmplt.previewMsg.20150622.html"
 
         oL.append(self.processTemplate(tmpltPth=tmpltPath, fn=tmpltFile, parameterDict=myD))
+        logger.info("CStrack+++ use html template of *%s*", tmpltFile)
         #
         return oL
 
     def doRenderDisplayMsg(self, p_reqObj, p_bIsWorkflow, p_msgDict):
         """Render HTML used to display individual message
 
         :Params:
@@ -441,16 +454,16 @@
             myD["content_type_hdr"] = "Communications with Depositor"
         else:
             myD["content_type_hdr"] = "Complete Correspondence History"
 
         ############################################################################
         # get message template data from MessagingIo
         ############################################################################
-        if self.__verbose:
-            logger.info("CStrack+++ call MessagingIo class from MessagingDepict.doRenderDisplayMsg()")
+        # if self.__verbose:
+        #     logger.info("CStrack+++ call MessagingIo class from MessagingDepict.doRenderDisplayMsg()")
         msgingIo = MessagingIo(p_reqObj, self.__verbose, self.__lfh)
         msgingIo.getMsgTmpltDataItems(myD)
 
         if len(p_msgDict["files_referenced"]) > 0:
             htmlStr = ""
             for fileRef in p_msgDict["files_referenced"]:
                 filePathSplitArr = fileRef["relative_file_url"].split("/")
@@ -487,14 +500,16 @@
 
         logger.info("p_msgDict is:  %r", p_msgDict)
         logger.info("myD is:  %r", myD)
 
         tmpltFile = "display_msg_tmplt.html"
         oL.append(self.processTemplate(tmpltPth=tmpltPath, fn=tmpltFile, parameterDict=myD))
         #
+        logger.info("CStrack+++ use html template of *%s*", tmpltFile)
+
         return oL
 
     # ####### BEGIN -- Specific to DataTable Implementation ##################
     # NOTE: consider encapsulating DataTable functionality as separate class
 
     def getJsonDataTable(self, p_msgRcrdList, p_msgColList, p_iDisplayStart=0):
         """Generate contents of json object expected by DataTables for populating display
@@ -543,16 +558,16 @@
 
         """
         dtblConfigDict = {}
         depId = p_reqObj.getValue("identifier")
         sContentType = p_reqObj.getValue("content_type")
         bCommHstryRqstd = True if sContentType == "commhstry" else False
         #
-        if self.__verbose:
-            logger.info("CStrack+++ call MessagingIo class from MessagingDepict.getDataTableTemplate()")
+        # if self.__verbose:
+        #     logger.info("CStrack+++ call MessagingIo class from MessagingDepict.getDataTableTemplate()")
         msgingIo = MessagingIo(p_reqObj, self.__verbose, self.__lfh)
         bOk, msgColList = msgingIo.getMsgColList(bCommHstryRqstd)
         #
         if bOk:
             ###############################################################################################
             # FIRST: obtain any config info needed by DataTables plugin
             ###############################################################################################
```

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/depict/MessagingTemplates.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingTemplates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/DateUtil.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/DateUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/EmHeaderUtils.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/MessagingDataExport.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/MessagingDataImport.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/io/MessagingIo.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingIo.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 #    2023-10-20    CS     For map-only, add "auth_rel_status_code_map" key for msg dict, get value from _em_depui.depositor_hold_instructions
 #    2023-10-20    CS     Update release letter for pdb ids being superseded, for both autoMsg and UI, add "spr_to_replace_pdb_ids" to msg dict
 #    2023-11-01    CS     Update file attachement list process to not to append validation report files if already in workingFileRefsList
 #    2023-11-02    CS     Update to include PDB extension id in letter, add pdb_ext_id in msg dict
 #    2023-11-06    CS     Update logic for __getDefaultMsgTmpltType(), i.e. default message pop-up for StatusMod
 #    2023-11-20    EP     Add anyUnactionApprovalWithoutCorrection() to determine if any pendingapproval without corrections that need to be acted upon
 #    2023-11-23    EP     autoMsg() add support for explicit-approved autogenerated message
+#    2024-04-04    CS     Add context_type to autoMsg() and sendSingle() to match frontend message-to-depositor drop-down list
 ##
 """
 Class to manage persistence/retrieval of messaging data
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Raul Sala"
@@ -1249,16 +1250,18 @@
         msgOrigCommRef.setOrigAttachments(origAttachments)
         nextOrdinalId = mIIo.nextOrigCommReferenceOrdinal()
         msgOrigCommRef.setOrdinalId(id=nextOrdinalId)
         mIIo.appendOrigCommReference(msgOrigCommRef.get())
 
     def autoMsg(self, p_depIdList, p_tmpltType="release-publ", p_isEmdbEntry=False, p_sender="auto"):
         """
-        Method to enable release message to be automatically sent by another server-side python module (e.g. Release module)
-        (i.e. as opposed to being invoked via URL request)
+        Send message based on template type p_tmpltType, invoked by 'auto' batch operation rather than frontend UI selection.
+        Originally deleveloped as a  method to enable release message to be automatically sent by another server-side
+        python module (e.g. Release module) (i.e. as opposed to being invoked via URL request).
+        The message is then archived in notes-from-annotator.
 
         :Helpers:
 
         :Returns:
 
         """
         #
@@ -1272,15 +1275,15 @@
         self.__reqObj.setValue("filesource", "archive")
 
         if p_isEmdbEntry:
             self.__reqObj.setValue("expmethod", "ELECTRON MICROSCOPY")
         #
         rtrnDict = {}
         #
-        contextType = None
+        contextType = p_tmpltType  # CS 2024-04-04 record message type
         contextVal = None
         #
         # Added by ZF
         #
         statusApi = StatusDbApi(siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
         for depId in p_depIdList:  # for depId,tmpltType in p_depIdList:
 
@@ -1301,15 +1304,15 @@
 
             # defaults for EM
             self.__reqObj.setValue("em_entry", "false")
             self.__reqObj.setValue("em_map_only", "false")
             self.__reqObj.setValue("em_map_and_model", "false")
 
             useAnnotatorName = False
-            if p_tmpltType in ["remind-unlocked", "implicit-approved"]:
+            if p_tmpltType in ["remind-unlocked", "approval-impl"]:  # CS 2024-04-04 change implicit-approved to approval-impl to match frontend drop-down
                 useAnnotatorName = True
 
             # Trigger lookup of annotator initial to name if desired by template
             if useAnnotatorName:
                 self.__reqObj.setValue("useAnnotatorName", "True")
 
             # qualifying name of database file, in case code calling this function does so with list of depIDs
@@ -1370,21 +1373,21 @@
             elif p_tmpltType == "remind-unlocked":
                 msgTmplt = MessagingTemplates.msgTmplt_remindUnlocked
                 attachFiles = False
                 isNote = True
                 # Need all ids
                 accstr = templateDict["accession_ids"]
                 subject = "ARCHIVED: Please attend to your unlocked deposition session - " + accstr
-            elif p_tmpltType == "implicit-approved":
+            elif p_tmpltType == "approval-impl":  # CS 2024-04-04 change implicit-approved to approval-impl to match frontend drop-down
                 msgTmplt = MessagingTemplates.msgTmplt_approvalImplicit_em if p_isEmdbEntry else MessagingTemplates.msgTmplt_approvalImplicit
                 attachFiles = False
                 # Need all ids
                 accstr = templateDict["accession_ids"]
                 subject = "Implicit Approval of Your Structure - " + accstr
-            elif p_tmpltType == "explicit-approved":
+            elif p_tmpltType == "approval-expl":  # CS 2024-04-04 change explicit-approved to approval-expl to match frontend drop-down
                 msgTmplt = MessagingTemplates.msgTmplt_approvalExplicit_em if p_isEmdbEntry else MessagingTemplates.msgTmplt_approvalExplicit
                 attachFiles = False
                 # Need all ids
                 accstr = templateDict["accession_ids"]
                 subject = "Explicit Approval of Your Structure - " + accstr
             elif p_tmpltType == "obsolete":
                 otypes = templateDict["obs_id_types"]
@@ -1394,15 +1397,15 @@
                         msgTmplt = MessagingTemplates.msgTmplt_obsolete_map_model
                     else:
                         msgTmplt = MessagingTemplates.msgTmplt_obsolete_map_only
                 else:
                     msgTmplt = MessagingTemplates.msgTmplt_obsolete_model
                 subject = "Obsoletion of " + templateDict["obs_ids"]
                 attachFiles = False
-            elif p_tmpltType == "remind-feedback":
+            elif p_tmpltType == "reminder":  # CS 2024-04-04 change type from remind-feedback to reminder to match frontend drop-down
                 msgTmplt = MessagingTemplates.msgTmplt_reminder_em if p_isEmdbEntry else MessagingTemplates.msgTmplt_reminder
                 attachFiles = False
                 isNote = True
                 # Need all ids
                 accstr = templateDict["accession_ids"]
                 subject = "ARCHIVED: Still awaiting feedback for " + accstr
 
@@ -1469,16 +1472,27 @@
                 rtrnDict[depId]["append_msg"] = sMsg
             #
             if self.__verbose:
                 logger.info("pdbx_model_updated is: %s", rtrnDict[depId]["pdbx_model_updated"])
         #
         return rtrnDict
 
-    def sendSingle(self, depId, subject, msg, p_sender="auto", p_testemail=None):
-        """Sends a single message for depId with subject and msg.  If p_testemail is set - will send notification there"""
+    def sendSingle(self, depId, subject, msg, p_sender="auto", p_testemail=None, p_tmpltType="other"):  # CS 2024-04-04 add p_tmpltType arg
+        """Sends a single message for depId with subject and msg. If p_testemail is set - will send notification there
+        Different from autoMsg, this function sends customized message pre-composed and passed by subject and msg args.
+        Although template type p_tmpltType is an arg, the message doesn't base on the template type which is only provided for record.
+        The message is then archived in notes-from-annotator.
+        The function is invoked by programmatic process rather than frontend UI selection including the following:
+        (1) WFM manager use the function to send confirmation message
+        (2) AutoMessage uses this to send auto messages
+        (3) OnholdEntryReminder
+        (4) SessionExpiringNotice
+        (5) CitationRequest
+
+        """
         logger.info("Depid %s", depId)
         logger.info("Subject %s", subject)
         logger.info("Message %s", msg)
         logger.info("Test email %s", p_testemail)
 
         self.__reqObj.setValue("content_type", "msgs")  # as opposed to "notes"
         self.__reqObj.setValue("filesource", "archive")
@@ -1493,15 +1507,15 @@
 
         # No files are being attached
         fileRefList = []
 
         # We are archiving notes
         isNote = True
 
-        contextType = None
+        contextType = p_tmpltType  # CS 2024-04-04 record message type, following frontend message-to-depositor drop-down list, default at "other"
         contextVal = None
 
         messageDict = {
             "deposition_data_set_id": depId,
             "sender": p_sender,
             "context_type": contextType,
             "context_value": contextVal,
```

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/models/Message.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/Message.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/util/AutoMessage.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/AutoMessage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##
 # File:  AutoMessage.py
 # Date:  28-Jun-2019 E. Peisach
 #
 # Update:
 """
 Support for automatic scripts to send template drive email messages and archive in normal message stream/notes
-
+Auto messages are archived in notes-from-annotator
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Ezra Peisach"
 __email__ = "peisach@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 
@@ -57,21 +57,21 @@
         return mio
 
     def sendRemindUnlocked(self, depidlist):
         self._sendReminderBulk(depidlist, p_tmplt="remind-unlocked")
 
     def sendRemindFeedback(self, depidlist):
         """ Sends a reminder that depositor has not responded to validation report """
-        self._sendReminderBulk(depidlist, p_tmplt="remind-feedback")
+        self._sendReminderBulk(depidlist, p_tmplt="reminder")
 
     def sendImplicitApproved(self, depidlist):
-        self._sendReminderBulk(depidlist, p_tmplt="implicit-approved")
+        self._sendReminderBulk(depidlist, p_tmplt="approval-impl")  # CS 2024-04-04 change implicit-approved to approval-impl to match frontend drop-down
 
     def sendExplicitApproved(self, depidlist):
-        self._sendReminderBulk(depidlist, p_tmplt="explicit-approved")
+        self._sendReminderBulk(depidlist, p_tmplt="approval-expl")  # CS 2024-04-04 change explicit-approved to approval-expl to match frontend drop-down
 
     def _sendReminderBulk(self, depidlist, p_tmplt):
         """Sends the bulk messages - handling setting EM flag"""
 
         (pdbents, emdents) = self._splitents(depidlist)
 
         mio = self.__getmsgio()
@@ -107,30 +107,31 @@
             expmeths = self._getExptl(depid)
             if "ELECTRON MICROSCOPY" in expmeths:
                 ements.append(depid)
             else:
                 pdbents.append(depid)
         return (pdbents, ements)
 
-    def sendSingleMessage(self, depid, subject, msg, testemail=None):
+    def sendSingleMessage(self, depid, subject, msg, testemail=None, p_tmpltType="other"):
         """Sends a message to depid, without using templates. No attachments.
 
         Args:
            depid (str): Deposition id
            subject (str): Subject string for message
            msg (str): Multiline message to send
            testemail (str): If set overrides entry recipients for testing
+           p_tmpltType as template type
 
         returns:
            bool:  True if successfule or else false
         """
 
         mio = self.__getmsgio()
-        ret = mio.sendSingle(depid, subject, msg, p_testemail=testemail)
-        ret = True
+        ret = mio.sendSingle(depid, subject, msg, p_testemail=testemail, p_tmpltType=p_tmpltType)
+        # ret = True
         return ret
 
     def tagMessageStatus(self, depId, msgidlist, actionReqd="N", forReleaseFlg="N"):
         """Tags a message"""
 
         ret = True
         mio = self.__getmsgio(depId)
```

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/util/ExtractMessage.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/ExtractMessage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 # File:  ExtractMessage.py
 # Date:  28-Jun-2019 E. Peisach
 #
 # Update:
 #    2023-11-10    CS     Refactor code to add general process to parse message file; Add functions to retrieve datetime of last messages of various type.
 #    2023-11-23    EP     Add getApprovalNoCorrectSubjects() and getPendingDepositorMessages()
+#    2024-04-04    CS     Use context_type and context_value to find target message, and default to subject/title parsing as was used previously.
 #
 ##
 """
 Support for automatic extracting information from send messages
 
 
 """
@@ -124,14 +125,101 @@
                             maxOrdId = ordinalId
                             ret = self.convertStrToDatetime(str(row[idxLastCommDate]))
 
                 except Exception as e:
                     logger.error("Error processing message file for %s, %s", self.__depid, e)
         return ret
 
+    # CS 2024-04-04 add search below by context_type
+    def __selectLastMsgByContextType(self, l_context_type_to_search):
+        """ return datetime of the lastest message based on context type
+
+        input: arg l_context_type_to_search is a list of the context types to search for.
+        list is used because some searches invole multiple context_type, e.g. ["release-publ", "release-nopubl"]
+
+        output: return datetime
+
+        """
+        ret = None
+        dc0 = self.__lc[0]
+        catObj = dc0.getObj("pdbx_deposition_message_info")
+        if catObj is None:
+            logger.warning("cannot find pdbx_deposition_message_info category in the message file for %s", self.__depid)
+            return None
+        else:
+            itDict = {}
+            itNameList = catObj.getItemNameList()
+            for idxIt, itName in enumerate(itNameList):
+                itDict[str(itName).lower()] = idxIt
+                #
+            idxOrdinalId = itDict["_pdbx_deposition_message_info.ordinal_id"]
+            idxLastCommDate = itDict["_pdbx_deposition_message_info.timestamp"]
+            idxContextType = itDict["_pdbx_deposition_message_info.context_type"]
+
+            maxOrdId = 0
+            for row in catObj.getRowList():
+                try:
+                    ordinalId = int(row[idxOrdinalId])
+                    context_type_recorded = row[idxContextType]
+
+                    if context_type_recorded in l_context_type_to_search:
+                        if ordinalId > maxOrdId:
+                            maxOrdId = ordinalId
+                            ret = self.convertStrToDatetime(str(row[idxLastCommDate]))
+
+                except Exception as e:
+                    logger.error("Error processing message file for %s, %s", self.__depid, e)
+        return ret
+
+    # CS 2024-04-04 add validation letter search below by context_type/context_value
+    def __getLastValidationByContextType(self):
+        """Returns (datetime, major issue)  of the last time a validation was sent as determined by
+        context_type and context_value
+        """
+
+        lastvalid = None
+        major = None
+
+        dc0 = self.__lc[0]
+        catObj = dc0.getObj("pdbx_deposition_message_info")
+        if catObj is None:
+            logger.warning("cannot find pdbx_deposition_message_info category in the message file for %s", self.__depid)
+            return None
+        else:
+            itDict = {}
+            itNameList = catObj.getItemNameList()
+            for idxIt, itName in enumerate(itNameList):
+                itDict[str(itName).lower()] = idxIt
+                #
+            idxOrdinalId = itDict["_pdbx_deposition_message_info.ordinal_id"]
+            idxLastCommDate = itDict["_pdbx_deposition_message_info.timestamp"]
+            idxContextType = itDict["_pdbx_deposition_message_info.context_type"]
+            idxContextValue = itDict["_pdbx_deposition_message_info.context_value"]
+
+            maxOrdId = 0
+            for row in catObj.getRowList():
+                try:
+                    ordinalId = int(row[idxOrdinalId])
+                    context_type_recorded = row[idxContextType]
+                    context_value_recorded = row[idxContextValue]
+
+                    if context_type_recorded == "vldtn":
+                        if ordinalId > maxOrdId:
+                            maxOrdId = ordinalId
+                            lastvalid = self.convertStrToDatetime(str(row[idxLastCommDate]))
+                            if context_value_recorded == "major-issue-in-validation":
+                                major = True
+                            else:
+                                major = False
+
+                except Exception as e:
+                    logger.error("Error processing message file for %s, %s", self.__depid, e)
+
+        return (lastvalid, major)
+
     def convertStrToDatetime(self, s_datetime):
         return datetime.datetime.strptime(str(s_datetime), "%Y-%m-%d %H:%M:%S")
 
     def getLastMsgDatetime(self, depid, to_from="both", b_use_cache=True, test_folder=None):
         """Return last message date as python datetime, either to or from depositor.
         System-sent messages in archived notes file are not counted.
         """
@@ -170,40 +258,52 @@
     def getLastAutoReminderDatetime(self, depid, b_use_cache=True, test_folder=None):
         """ Return date of last reminder in notes as python datetime.
         Notes only records automatically-sent messages unless annotators specifically archived a message.
         """
         ret = None
         self.__readMsgFile(depid, contentType="notes-from-annotator", b_use_cache=b_use_cache, test_folder=test_folder)
         if len(self.__lc) >= 1:
-            ret = self.__selectLastMsgByTitlePhrase(phrase='Still awaiting feedback for')
+            ret_by_context_type = self.__selectLastMsgByContextType(["reminder"])  # CS 2024-04-04 search by context_type first
+            if ret_by_context_type:
+                ret = ret_by_context_type
+            else:
+                ret = self.__selectLastMsgByTitlePhrase(phrase='Still awaiting feedback for')
         else:
             logger.info("Deposition %s empty message file", depid)
 
         return ret
 
     def getLastManualReminderDatetime(self, depid, b_use_cache=True, test_folder=None):
         """Return date of last reminder message to depositor as python datetime.
         System-sent messages in archived notes file are not counted.
         """
         ret = None
         self.__readMsgFile(depid, contentType="messages-to-depositor", b_use_cache=b_use_cache, test_folder=test_folder)
         if len(self.__lc) >= 1:
-            ret = self.__selectLastMsgByTitlePhrase(phrase='Still awaiting feedback for')
+            ret_by_context_type = self.__selectLastMsgByContextType(["reminder"])  # CS 2024-04-04 search by context_type first
+            if ret_by_context_type:
+                ret = ret_by_context_type
+            else:
+                ret = self.__selectLastMsgByTitlePhrase(phrase='Still awaiting feedback for')
         else:
             logger.info("Deposition %s empty message file", depid)
 
         return ret
 
     def getLastReleaseNoticeDatetime(self, depid, b_use_cache=True, test_folder=None):
         """Return date of last release notice to depositor as python datetime.
         """
         ret = None
         self.__readMsgFile(depid, contentType="messages-to-depositor", b_use_cache=b_use_cache, test_folder=test_folder)
         if len(self.__lc) >= 1:
-            ret = self.__selectLastMsgByTitlePhrase(phrase='Release of')
+            ret_by_context_type = self.__selectLastMsgByContextType(["release-publ", "release-nopubl"])  # CS 2024-04-04 search by context_type first
+            if ret_by_context_type:
+                ret = ret_by_context_type
+            else:
+                ret = self.__selectLastMsgByTitlePhrase(phrase='Release of')
         else:
             logger.info("Deposition %s empty message file", depid)
 
         return ret
 
     def getLastUnlockDatetime(self, depid, b_use_cache=True, test_folder=None):
         """Return date of last unlock message to depositor as python datetime.
@@ -254,22 +354,24 @@
                 itNameList = catObj.getItemNameList()
                 for idxIt, itName in enumerate(itNameList):
                     itDict[str(itName).lower()] = idxIt
                     #
                 idxOrdinalId = itDict["_pdbx_deposition_message_info.ordinal_id"]
                 idxLastCommDate = itDict["_pdbx_deposition_message_info.timestamp"]
                 idxMsgSubj = itDict["_pdbx_deposition_message_info.message_subject"]
+                idxContextType = itDict["_pdbx_deposition_message_info.context_type"]
 
                 maxUnlockOrdId = 0
                 for row in catObj.getRowList():
                     try:
                         ordinalId = int(row[idxOrdinalId])
                         msgsubj = row[idxMsgSubj]
+                        context_type_recorded = row[idxContextType]
 
-                        if msgsubj == "System Unlocked":
+                        if context_type_recorded == "system-unlocked" or msgsubj == "System Unlocked":
                             if ordinalId > maxUnlockOrdId:
                                 maxUnlockOrdId = ordinalId
                                 ret = str(row[idxLastCommDate])
 
                     except Exception as e:
                         logger.error("Error processing %s %s", depid, str(e))
 
@@ -304,14 +406,22 @@
 
         lastvalid = None
         major = None
 
         self.__readMsgFile(depid, contentType="messages-to-depositor", b_use_cache=b_use_cache, test_folder=test_folder)
 
         if len(self.__lc) >= 1:
+            logger.info("start searching for last validation letter by context_type")
+            (lastvalid, major) = self.__getLastValidationByContextType()  # CS 2024-04-04 first search by context_type/context_value
+            if lastvalid:
+                logger.info("found last validation letter by context_type")
+                return (lastvalid, major)  # return if find message by context_type/context_value
+
+            logger.info("fail to find last validation letter by context_type, default to search by subject/text parsing")
+
             c0 = self.__lc[0]
             catObj = c0.getObj("pdbx_deposition_message_file_reference")
             if catObj is None:
                 logger.debug("Deposition %s no pdbx_deposition_message_file_reference category", depid)
                 return (None, None)
 
             # Get list of msgids of validtion report
@@ -390,16 +500,16 @@
                     else:
                         pass  # ignore message not sent; ignore message not with validation report attached
                 except Exception as e:
                     logger.exception("Error processing %s %s", depid, str(e))
         else:
             logger.debug("Deposition %s empty message file", depid)
 
+        logger.info("finished searching for last validation letter by subject/text parsing")
         logger.info("Returning (%s, %s)", lastvalid, major)
-
         return (lastvalid, major)
 
     def _majorValidation(self, msgText):
         """Returns true if there appears to be a major error in the validation test - otherwise False"""
 
         ret = False
         if re.search("Some major issues", msgText, re.IGNORECASE) is not None:
```

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # 2016-02-03    RPS    Calling checkGlobalMsgStatus() after a message requiring "notes" flag is archived by email handler, so that flag is properly refreshed for display in WFM UI
 # 2016-02-17    RPS    Introducing use of Message model class to increase encapsulation, improve code organization.
 # 2016-08-09    RPS    Introducing support for standalone correspondence viewer. Providing means for detecting presence of notes archived via BMRB emails.
 # 2016-09-07    RPS    Providing separate, dedicated means for activating/deactivating UI flag for detecting presence of
 #                      notes archived via BMRB emails (vs. standard annotator authored notes).
 # 2016-09-14    ZF     Added __checkGroupDeposition() function to support for group deposition
 # 2023-11-20    EP     Added __checkAnyApprovalFlags() and set approriate database flags if set
+# 2024-04-04    CS     Add process on context_type/context_value of message-to-depositor recorded by frontend JavaScript and passed here through wsgi message submit URL
 ##
 """
 wwPDB Messaging web request and response processing modules.
 
 This software was developed as part of the World Wide Protein Data Bank
 Common Deposition and Annotation System Project
 
@@ -56,14 +57,15 @@
 __version__ = "V0.07"
 
 import ntpath
 import os
 import sys
 import time
 import traceback
+import re
 
 try:
     from html import unescape
 except ImportError:
     from HTMLParser import HTMLParser
 
 from wwpdb.utils.session.WebRequest import InputRequest, ResponseContent
@@ -1341,15 +1343,23 @@
 
         """
         #
         #
         self.__getSession()
         #
         rtrnDict = {}
-        #
+
+        # CS 2024-04-04 start processing context_value, add "major-issue-in-validation" if frontend submitted validation message contains major issue
+        if self.__reqObj.getValue("context_type") == "vldtn":
+            if not self.__reqObj.getValue("context_value").strip():
+                message_text = self.__reqObj.getValue("message")
+                if re.search("major issue", message_text.lower()) and re.search("outstanding issue", message_text.lower()):
+                    self.__reqObj.setValue("context_value", "major-issue-in-validation")
+        # CS 2024-04-04 end
+
         self.__reqObj.setReturnFormat(return_format="json")
         self.__reqObj.setValue("message_state", p_msgState)  # setting here for downstream processing, used only for processing purposes
         # NOTE: this field is not part of the PdbxMessage data structure, and thus is not persisted to data file.
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         #
         msgObj = Message.fromReqObj(self.__reqObj, self.__verbose, self.__lfh)
         #
```

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb/apps/msgmodule/webapp/wsgi.py` & `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/PKG-INFO` & `wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.msgmodule
-Version: 0.175
+Version: 0.176
 Summary: wwPDB messaging module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.msgmodule-0.175/wwpdb.apps.msgmodule.egg-info/SOURCES.txt` & `wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

