# Comparing `tmp/MacroQueue-0.2.4.tar.gz` & `tmp/MacroQueue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacroQueue-0.2.4.tar", last modified: Mon Apr  1 17:10:34 2024, max compression
+gzip compressed data, was "MacroQueue-0.3.0.tar", last modified: Mon Apr  8 14:46:11 2024, max compression
```

## Comparing `MacroQueue-0.2.4.tar` & `MacroQueue-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.511355 MacroQueue-0.2.4/
--rw-rw-rw-   0        0        0     1088 2024-03-19 20:51:50.000000 MacroQueue-0.2.4/LICENSE.md
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.419403 MacroQueue-0.2.4/MacroQueue/
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.460112 MacroQueue-0.2.4/MacroQueue/Bitmaps/
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.000000 MacroQueue-0.2.4/MacroQueue/Bitmaps/DownArrow.bmp
--rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.000000 MacroQueue-0.2.4/MacroQueue/Bitmaps/Remove.bmp
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.000000 MacroQueue-0.2.4/MacroQueue/Bitmaps/UpArrow.bmp
--rw-rw-rw-   0        0        0    68756 2024-03-27 14:08:48.000000 MacroQueue-0.2.4/MacroQueue/Dialogs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.480699 MacroQueue-0.2.4/MacroQueue/Functions/
--rw-rw-rw-   0        0        0     1043 2024-01-11 19:05:47.000000 MacroQueue-0.2.4/MacroQueue/Functions/BField.py
--rw-rw-rw-   0        0        0    21517 2024-04-01 13:25:42.000000 MacroQueue-0.2.4/MacroQueue/Functions/CreaTec.py
--rw-rw-rw-   0        0        0     1517 2024-03-27 16:22:52.000000 MacroQueue-0.2.4/MacroQueue/Functions/General.py
--rw-rw-rw-   0        0        0     1656 2024-03-25 14:52:53.000000 MacroQueue-0.2.4/MacroQueue/Functions/RF.py
--rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.000000 MacroQueue-0.2.4/MacroQueue/Functions/RHK.py
--rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.000000 MacroQueue-0.2.4/MacroQueue/Functions/SXM.py
--rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.000000 MacroQueue-0.2.4/MacroQueue/Functions/SXMRemote.py
--rw-rw-rw-   0        0        0    24521 2024-03-21 18:30:14.000000 MacroQueue-0.2.4/MacroQueue/GUIDesign.py
--rw-rw-rw-   0        0        0    54897 2024-04-01 15:32:11.000000 MacroQueue-0.2.4/MacroQueue/MacroQueue.py
--rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.000000 MacroQueue-0.2.4/MacroQueue/MacroQueueIcon.ico
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.491088 MacroQueue-0.2.4/MacroQueue/Macros/
--rw-rw-rw-   0        0        0    13972 2024-03-27 16:23:14.000000 MacroQueue-0.2.4/MacroQueue/Macros/CreaTecMacro.json
--rw-rw-rw-   0        0        0     7924 2022-06-13 16:55:53.000000 MacroQueue-0.2.4/MacroQueue/Macros/RHKMacro.json
--rw-rw-rw-   0        0        0      539 2024-04-01 15:21:24.000000 MacroQueue-0.2.4/MacroQueue/MakeExe.sh
--rw-rw-rw-   0        0        0      578 2024-03-19 20:16:23.000000 MacroQueue-0.2.4/MacroQueue/__init__.py
--rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.000000 MacroQueue-0.2.4/MacroQueue/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.501163 MacroQueue-0.2.4/MacroQueue.egg-info/
--rw-rw-rw-   0        0        0     3998 2024-04-01 17:10:34.000000 MacroQueue-0.2.4/MacroQueue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      819 2024-04-01 17:10:34.000000 MacroQueue-0.2.4/MacroQueue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 17:10:34.000000 MacroQueue-0.2.4/MacroQueue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-01 17:10:34.000000 MacroQueue-0.2.4/MacroQueue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 17:10:34.000000 MacroQueue-0.2.4/MacroQueue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3998 2024-04-01 17:10:34.501163 MacroQueue-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3107 2024-04-01 17:09:57.000000 MacroQueue-0.2.4/README.md
--rw-rw-rw-   0        0        0       86 2024-04-01 17:10:34.514039 MacroQueue-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2284 2024-04-01 17:10:30.000000 MacroQueue-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:10:34.501163 MacroQueue-0.2.4/test/
--rw-rw-rw-   0        0        0      562 2024-03-19 18:06:33.000000 MacroQueue-0.2.4/test/test_MainFrame.py
--rw-rw-rw-   0        0        0      774 2024-03-19 18:07:50.000000 MacroQueue-0.2.4/test/test_STMthread.py
--rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.000000 MacroQueue-0.2.4/test/test_readdata.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.612058 MacroQueue-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-19 20:51:50.000000 MacroQueue-0.3.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.554037 MacroQueue-0.3.0/MacroQueue/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.574057 MacroQueue-0.3.0/MacroQueue/Bitmaps/
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.000000 MacroQueue-0.3.0/MacroQueue/Bitmaps/DownArrow.bmp
+-rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.000000 MacroQueue-0.3.0/MacroQueue/Bitmaps/Remove.bmp
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.000000 MacroQueue-0.3.0/MacroQueue/Bitmaps/UpArrow.bmp
+-rw-rw-rw-   0        0        0    69978 2024-04-08 14:29:58.000000 MacroQueue-0.3.0/MacroQueue/Dialogs.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.584071 MacroQueue-0.3.0/MacroQueue/Functions/
+-rw-rw-rw-   0        0        0    11702 2024-04-04 18:23:56.000000 MacroQueue-0.3.0/MacroQueue/Functions/BField.py
+-rw-rw-rw-   0        0        0    14949 2024-04-04 18:21:46.000000 MacroQueue-0.3.0/MacroQueue/Functions/CreaTec.py
+-rw-rw-rw-   0        0        0     1094 2024-04-08 14:39:54.000000 MacroQueue-0.3.0/MacroQueue/Functions/General.py
+-rw-rw-rw-   0        0        0     7641 2024-04-04 18:16:32.000000 MacroQueue-0.3.0/MacroQueue/Functions/RF.py
+-rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.000000 MacroQueue-0.3.0/MacroQueue/Functions/RHK.py
+-rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.000000 MacroQueue-0.3.0/MacroQueue/Functions/SXM.py
+-rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.000000 MacroQueue-0.3.0/MacroQueue/Functions/SXMRemote.py
+-rw-rw-rw-   0        0        0      460 2024-04-08 14:35:52.000000 MacroQueue-0.3.0/MacroQueue/Functions/Testing.py
+-rw-rw-rw-   0        0        0    21014 2024-04-08 14:29:40.000000 MacroQueue-0.3.0/MacroQueue/GUIDesign.py
+-rw-rw-rw-   0        0        0    57939 2024-04-08 14:40:35.000000 MacroQueue-0.3.0/MacroQueue/MacroQueue.py
+-rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.000000 MacroQueue-0.3.0/MacroQueue/MacroQueueIcon.ico
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.597334 MacroQueue-0.3.0/MacroQueue/Macros/
+-rw-rw-rw-   0        0        0    20611 2024-04-08 12:41:13.000000 MacroQueue-0.3.0/MacroQueue/Macros/CreaTecMacro.json
+-rw-rw-rw-   0        0        0       59 2024-04-08 14:20:52.000000 MacroQueue-0.3.0/MacroQueue/Macros/RHKMacro.json
+-rw-rw-rw-   0        0        0      738 2024-04-08 14:36:30.000000 MacroQueue-0.3.0/MacroQueue/Macros/TestingMacro.json
+-rw-rw-rw-   0        0        0      565 2024-04-02 17:43:33.000000 MacroQueue-0.3.0/MacroQueue/MakeExe.sh
+-rw-rw-rw-   0        0        0      578 2024-03-19 20:16:23.000000 MacroQueue-0.3.0/MacroQueue/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.000000 MacroQueue-0.3.0/MacroQueue/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.605231 MacroQueue-0.3.0/MacroQueue.egg-info/
+-rw-rw-rw-   0        0        0     4000 2024-04-08 14:46:11.000000 MacroQueue-0.3.0/MacroQueue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2024-04-08 14:46:11.000000 MacroQueue-0.3.0/MacroQueue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:46:11.000000 MacroQueue-0.3.0/MacroQueue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-08 14:46:11.000000 MacroQueue-0.3.0/MacroQueue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 14:46:11.000000 MacroQueue-0.3.0/MacroQueue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4000 2024-04-08 14:46:11.612058 MacroQueue-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3109 2024-04-03 16:00:45.000000 MacroQueue-0.3.0/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-08 14:46:11.615081 MacroQueue-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2259 2024-04-08 14:46:09.000000 MacroQueue-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:46:11.603351 MacroQueue-0.3.0/test/
+-rw-rw-rw-   0        0        0      571 2024-04-04 18:40:22.000000 MacroQueue-0.3.0/test/test_MainFrame.py
+-rw-rw-rw-   0        0        0      920 2024-04-05 13:00:39.000000 MacroQueue-0.3.0/test/test_STMthread.py
+-rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.000000 MacroQueue-0.3.0/test/test_readdata.py
```

### Comparing `MacroQueue-0.2.4/LICENSE.md` & `MacroQueue-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Bitmaps/DownArrow.bmp` & `MacroQueue-0.3.0/MacroQueue/Bitmaps/DownArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Bitmaps/Remove.bmp` & `MacroQueue-0.3.0/MacroQueue/Bitmaps/Remove.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Bitmaps/UpArrow.bmp` & `MacroQueue-0.3.0/MacroQueue/Bitmaps/UpArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Dialogs.py` & `MacroQueue-0.3.0/MacroQueue/Dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 from functools import partial
 import numpy as np
 
 try:
     from MacroQueue.GUIDesign import MacroDialog
     from MacroQueue.GUIDesign import MacroSettingsDialog
     from MacroQueue.GUIDesign import StartMacroDialog
-    from MacroQueue.GUIDesign import ChooseSoftware
 except ModuleNotFoundError:
     from GUIDesign import MacroDialog
     from GUIDesign import MacroSettingsDialog
     from GUIDesign import StartMacroDialog
-    from GUIDesign import ChooseSoftware
 
 import pandas as pd
 class SettingsDialog(wx.Dialog):
 
     def __init__(self, parent, SettingsDict,DefaultSettingsType,title='Settings', ExpandOutput=False):
         super(SettingsDialog, self).__init__(None,title=title)
         self.ExpandOutput=ExpandOutput
@@ -1149,36 +1147,63 @@
             self.Parent.AddMacroToQueue(self.TheMacro,self.MacroName,Index=Index)
         self.Destroy()
         pass
     def OnCancel(self, event):
         self.Destroy()
 
 
-class MyChooseSoftwareDialog(ChooseSoftware):
+class MyChooseSoftwareDialog(wx.Dialog):
     def __init__(self, parent,FunctionsToLoad=None):
-        super().__init__(parent)
+        wx.Dialog.__init__ ( self, parent, id = wx.ID_ANY, title = u"Choose the STM Software", pos = wx.DefaultPosition, size = wx.DefaultSize, style = wx.DEFAULT_DIALOG_STYLE )
+
+        self.SetSizeHints( wx.DefaultSize, wx.DefaultSize )
+        self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_INACTIVECAPTION ) )
+
+        fgSizer12 = wx.FlexGridSizer( 0, 1, 0, 0 )
+        fgSizer12.SetFlexibleDirection( wx.BOTH )
+        fgSizer12.SetNonFlexibleGrowMode( wx.FLEX_GROWMODE_SPECIFIED )
+
+        self.m_ChooseSoftwareText = wx.StaticText( self, wx.ID_ANY, u"Please select the STM Software you wish to use", wx.DefaultPosition, wx.DefaultSize, 0 )
+        self.m_ChooseSoftwareText.Wrap( -1 )
+
+        fgSizer12.Add( self.m_ChooseSoftwareText, 0, wx.ALIGN_CENTER_HORIZONTAL|wx.ALL, 5 )
+
+        self.m_panel11 = wx.Panel( self, wx.ID_ANY, wx.DefaultPosition, wx.DefaultSize, wx.TAB_TRAVERSAL )
+        self.m_panel11.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_ACTIVECAPTION ) )
+
+        bSizer6 = wx.BoxSizer( wx.HORIZONTAL )
+        for i,system in enumerate(parent.Systems):
+            self.m_button = wx.Button( self.m_panel11, wx.ID_ANY, system, wx.DefaultPosition, wx.DefaultSize, 0 )
+            bSizer6.Add( self.m_button, 0, wx.ALL, 5 )
+            SetTHISSoftware = partial(self.SetSoftware,i)
+            self.m_button.Bind( wx.EVT_BUTTON,  SetTHISSoftware)
+
+
+
+        self.m_panel11.SetSizer( bSizer6 )
+        self.m_panel11.Layout()
+        bSizer6.Fit( self.m_panel11 )
+        fgSizer12.Add( self.m_panel11, 1, wx.EXPAND |wx.ALL, 5 )
+
+
+        self.SetSizer( fgSizer12 )
+        self.Layout()
+        fgSizer12.Fit( self )
+
+        self.Centre( wx.BOTH )
+
+
         self.SavedSettingsFile = self.Parent.SavedSettingsFile
         self.FunctionsToLoad = FunctionsToLoad
-    def OnRHK(self, event=None):
-        self.SetSoftware("RHK")
-    def OnCreaTec(self, event=None):
-        self.SetSoftware("CreaTec")
-    def OnSXM(self, event=None):
-        self.SetSoftware("SXM")
-    def SetSoftware(self,software=None):
-        self.Parent.m_RHKmenuItem.Check(False)
-        self.Parent.m_CreaTecmenuItem.Check(False)
-        self.Parent.m_SXMmenuItem.Check(False)
-        if software is not None:
-            if software == "RHK":
-                self.Parent.m_RHKmenuItem.Check(True)
-            if software == "CreaTec":
-                self.Parent.m_CreaTecmenuItem.Check(True)
-            if software == "SXM":
-                self.Parent.m_SXMmenuItem.Check(True)
+    def SetSoftware(self,softwareIndex=None,event=None):
+        for MenuItem in self.Parent.SystemMenuItems:
+            MenuItem.Check(False)
+        if softwareIndex is not None:
+            self.Parent.SystemMenuItems[softwareIndex].Check(True)
+            software = self.Parent.Systems[softwareIndex]
             self.Parent.Software = software
             self.Parent.MacroPath = self.Parent.MacroPaths[software]
             if self.FunctionsToLoad is None:
                 SettingsDict = {"Software":software,'Functions':['General'],'PauseAfterCancel':self.Parent.m_PauseAfterCancel.IsChecked()}
             else:
                 SettingsDict = {"Software":software,'Functions':self.FunctionsToLoad,'PauseAfterCancel':self.Parent.m_PauseAfterCancel.IsChecked()}
```

### Comparing `MacroQueue-0.2.4/MacroQueue/Functions/RHK.py` & `MacroQueue-0.3.0/MacroQueue/Functions/RHK.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Functions/SXM.py` & `MacroQueue-0.3.0/MacroQueue/Functions/SXM.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Functions/SXMRemote.py` & `MacroQueue-0.3.0/MacroQueue/Functions/SXMRemote.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/GUIDesign.py` & `MacroQueue-0.3.0/MacroQueue/GUIDesign.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 		self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_APPWORKSPACE ) )
 
 		self.m_menubar1 = wx.MenuBar( 0|wx.TRANSPARENT_WINDOW )
 		self.m_FileMenu = wx.Menu()
 		self.m_SourceMenuItem = wx.MenuItem( self.m_FileMenu, wx.ID_ANY, u"Open Source Folder", wx.EmptyString, wx.ITEM_NORMAL )
 		self.m_FileMenu.Append( self.m_SourceMenuItem )
 
-		self.m_ExitMenuItem = wx.MenuItem( self.m_FileMenu, wx.ID_ANY, u"Exit", wx.EmptyString, wx.ITEM_NORMAL )
-		self.m_FileMenu.Append( self.m_ExitMenuItem )
-
 		self.m_menubar1.Append( self.m_FileMenu, u"File" )
 
 		self.m_OptionsMenu = wx.Menu()
 		self.m_PauseAfterCancel = wx.MenuItem( self.m_OptionsMenu, wx.ID_ANY, u"Pause After Cancel", wx.EmptyString, wx.ITEM_CHECK )
 		self.m_OptionsMenu.Append( self.m_PauseAfterCancel )
 		self.m_PauseAfterCancel.Check( True )
 
@@ -57,23 +54,14 @@
 
 		self.m_menuItem8 = wx.MenuItem( self.m_Connectmenu, wx.ID_ANY, u"Disconnect"+ u"\t" + u"CTRL+D", wx.EmptyString, wx.ITEM_NORMAL )
 		self.m_Connectmenu.Append( self.m_menuItem8 )
 
 		self.m_menubar1.Append( self.m_Connectmenu, u"Connect" )
 
 		self.m_SystemMenu = wx.Menu()
-		self.m_RHKmenuItem = wx.MenuItem( self.m_SystemMenu, wx.ID_ANY, u"RHK", wx.EmptyString, wx.ITEM_CHECK )
-		self.m_SystemMenu.Append( self.m_RHKmenuItem )
-
-		self.m_CreaTecmenuItem = wx.MenuItem( self.m_SystemMenu, wx.ID_ANY, u"CreaTec", wx.EmptyString, wx.ITEM_CHECK )
-		self.m_SystemMenu.Append( self.m_CreaTecmenuItem )
-
-		self.m_SXMmenuItem = wx.MenuItem( self.m_SystemMenu, wx.ID_ANY, u"SXM", wx.EmptyString, wx.ITEM_CHECK )
-		self.m_SystemMenu.Append( self.m_SXMmenuItem )
-
 		self.m_menubar1.Append( self.m_SystemMenu, u"System" )
 
 		self.m_NotSTMMenu = wx.Menu()
 		self.m_menubar1.Append( self.m_NotSTMMenu, u"Included Functions" )
 
 		self.m_menu5 = wx.Menu()
 		self.m_menuItem10 = wx.MenuItem( self.m_menu5, wx.ID_ANY, u"Basic Usage", wx.EmptyString, wx.ITEM_NORMAL )
@@ -151,23 +139,19 @@
 		self.Centre( wx.BOTH )
 
 		# Connect Events
 		self.Bind( wx.EVT_CLOSE, self.OnClose )
 		self.Bind( wx.EVT_IDLE, self.IdleLoop )
 		self.Bind( wx.EVT_SIZE, self.OnSize )
 		self.Bind( wx.EVT_MENU, self.OpenSourceFolder, id = self.m_SourceMenuItem.GetId() )
-		self.Bind( wx.EVT_MENU, self.OnClose, id = self.m_ExitMenuItem.GetId() )
 		self.Bind( wx.EVT_MENU, self.ReloadFunctions, id = self.m_menuItem17.GetId() )
 		self.Bind( wx.EVT_MENU, self.StartMakeNewMacro, id = self.m_MakeMacroMenuItem.GetId() )
 		self.Bind( wx.EVT_MENU, self.OpenMacroFile, id = self.m_OpenMacroMenuItem.GetId() )
 		self.Bind( wx.EVT_MENU, self.AddConnectToQueue, id = self.m_menuItem7.GetId() )
 		self.Bind( wx.EVT_MENU, self.AddDisconnectToQueue, id = self.m_menuItem8.GetId() )
-		self.Bind( wx.EVT_MENU, self.OnRHKSoftware, id = self.m_RHKmenuItem.GetId() )
-		self.Bind( wx.EVT_MENU, self.OnCreaTecSoftware, id = self.m_CreaTecmenuItem.GetId() )
-		self.Bind( wx.EVT_MENU, self.OnSXMSoftware, id = self.m_SXMmenuItem.GetId() )
 		self.Bind( wx.EVT_MENU, self.BasicUseageHelp, id = self.m_menuItem10.GetId() )
 		self.Bind( wx.EVT_MENU, self.ExpandNumericalParameters, id = self.m_menuItem102.GetId() )
 		self.Bind( wx.EVT_MENU, self.MakeAMacroHelp, id = self.m_menuItem11.GetId() )
 		self.Bind( wx.EVT_MENU, self.WriteANewFunctionHelp, id = self.m_menuItem12.GetId() )
 		self.Bind( wx.EVT_MENU, self.InfoHelp, id = self.m_menuItem121.GetId() )
 		self.Bind( wx.EVT_MENU, self.License, id = self.m_menuItem1211.GetId() )
 		self.Bind( wx.EVT_TIMER, self.CheckQueue, id=wx.ID_ANY )
@@ -187,15 +171,14 @@
 
 	def OnSize( self, event ):
 		event.Skip()
 
 	def OpenSourceFolder( self, event ):
 		event.Skip()
 
-
 	def ReloadFunctions( self, event ):
 		event.Skip()
 
 	def StartMakeNewMacro( self, event ):
 		event.Skip()
 
 	def OpenMacroFile( self, event ):
@@ -203,23 +186,14 @@
 
 	def AddConnectToQueue( self, event ):
 		event.Skip()
 
 	def AddDisconnectToQueue( self, event ):
 		event.Skip()
 
-	def OnRHKSoftware( self, event ):
-		event.Skip()
-
-	def OnCreaTecSoftware( self, event ):
-		event.Skip()
-
-	def OnSXMSoftware( self, event ):
-		event.Skip()
-
 	def BasicUseageHelp( self, event ):
 		event.Skip()
 
 	def ExpandNumericalParameters( self, event ):
 		event.Skip()
 
 	def MakeAMacroHelp( self, event ):
@@ -241,82 +215,14 @@
 		event.Skip()
 
 	def ClearQueue( self, event ):
 		event.Skip()
 
 
 ###########################################################################
-## Class ChooseSoftware
-###########################################################################
-
-class ChooseSoftware ( wx.Dialog ):
-
-	def __init__( self, parent ):
-		wx.Dialog.__init__ ( self, parent, id = wx.ID_ANY, title = u"Choose the STM Software", pos = wx.DefaultPosition, size = wx.DefaultSize, style = wx.DEFAULT_DIALOG_STYLE )
-
-		self.SetSizeHints( wx.DefaultSize, wx.DefaultSize )
-		self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_INACTIVECAPTION ) )
-
-		fgSizer12 = wx.FlexGridSizer( 0, 1, 0, 0 )
-		fgSizer12.SetFlexibleDirection( wx.BOTH )
-		fgSizer12.SetNonFlexibleGrowMode( wx.FLEX_GROWMODE_SPECIFIED )
-
-		self.m_ChooseSoftwareText = wx.StaticText( self, wx.ID_ANY, u"Please select the STM Software you wish to use", wx.DefaultPosition, wx.DefaultSize, 0 )
-		self.m_ChooseSoftwareText.Wrap( -1 )
-
-		fgSizer12.Add( self.m_ChooseSoftwareText, 0, wx.ALIGN_CENTER_HORIZONTAL|wx.ALL, 5 )
-
-		self.m_panel11 = wx.Panel( self, wx.ID_ANY, wx.DefaultPosition, wx.DefaultSize, wx.TAB_TRAVERSAL )
-		self.m_panel11.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_ACTIVECAPTION ) )
-
-		bSizer6 = wx.BoxSizer( wx.HORIZONTAL )
-
-		self.m_RHKbutton = wx.Button( self.m_panel11, wx.ID_ANY, u"RHK", wx.DefaultPosition, wx.DefaultSize, 0 )
-		bSizer6.Add( self.m_RHKbutton, 0, wx.ALL, 5 )
-
-		self.m_CreaTecbutton = wx.Button( self.m_panel11, wx.ID_ANY, u"CreaTec", wx.DefaultPosition, wx.DefaultSize, 0 )
-		bSizer6.Add( self.m_CreaTecbutton, 0, wx.ALL, 5 )
-
-		self.m_SXMbutton = wx.Button( self.m_panel11, wx.ID_ANY, u"SXM", wx.DefaultPosition, wx.DefaultSize, 0 )
-		bSizer6.Add( self.m_SXMbutton, 0, wx.ALL, 5 )
-
-
-		self.m_panel11.SetSizer( bSizer6 )
-		self.m_panel11.Layout()
-		bSizer6.Fit( self.m_panel11 )
-		fgSizer12.Add( self.m_panel11, 1, wx.EXPAND |wx.ALL, 5 )
-
-
-		self.SetSizer( fgSizer12 )
-		self.Layout()
-		fgSizer12.Fit( self )
-
-		self.Centre( wx.BOTH )
-
-		# Connect Events
-		self.m_RHKbutton.Bind( wx.EVT_BUTTON, self.OnRHK )
-		self.m_CreaTecbutton.Bind( wx.EVT_BUTTON, self.OnCreaTec )
-		self.m_SXMbutton.Bind( wx.EVT_BUTTON, self.OnSXM )
-
-	def __del__( self ):
-		pass
-
-
-	# Virtual event handlers, override them in your derived class
-	def OnRHK( self, event ):
-		event.Skip()
-
-	def OnCreaTec( self, event ):
-		event.Skip()
-
-	def OnSXM( self, event ):
-		event.Skip()
-
-
-###########################################################################
 ## Class MacroDialog
 ###########################################################################
 
 class MacroDialog ( wx.Dialog ):
 
 	def __init__( self, parent ):
 		wx.Dialog.__init__ ( self, parent, id = wx.ID_ANY, title = u"Define The Macro", pos = wx.DefaultPosition, size = wx.Size( 800,600 ), style = wx.DEFAULT_DIALOG_STYLE|wx.RESIZE_BORDER )
```

### Comparing `MacroQueue-0.2.4/MacroQueue/MacroQueue.py` & `MacroQueue-0.3.0/MacroQueue/MacroQueue.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import multiprocessing as mp
 import queue
 import threading
 import importlib
 import importlib.util
 from inspect import getmembers, isfunction,getcomments
 
+import PyInstaller
 import wx
 import pyvisa
 import pythoncom
 from datetime import datetime
-
+import shutil
+ 
 from time import time as timer
 
 application_path = os.path.dirname(sys.executable) if getattr(sys, 'frozen', False) else os.path.dirname(__file__)
 sys.path.append(application_path)
 try:
     from MacroQueue.Dialogs import MyMacroDialog
     from MacroQueue.Dialogs import MyMacroSettingsDialog
@@ -30,134 +32,128 @@
     from Dialogs import MyStartMacroDialog
     from Dialogs import MyChooseSoftwareDialog
     from GUIDesign import MyFrame
     
 # from GUIDesign import MacroDialog
 from inspect import getmembers, isfunction
 
-# They all go in try/except just in case the required packages aren't installed for one of them 
-# (e.g. you can still use RHK's functions even without win32com which you need for CreaTec)
-if getattr(sys, 'frozen', False):
-    sys.path.append(os.path.dirname(sys.executable)+"\\Functions")
-else:
-    sys.path.append(os.path.dirname(__file__)+"\\Functions")
+sys.path.append(os.path.dirname(sys.executable if getattr(sys, 'frozen', False) else __file__)+"\\Functions")
 
 import json
 
+from PyInstaller.__main__ import run as PyInstall
+from functools import partial
+
 
 IconFileName = "MacroQueueIcon.ico"
 
 
 # BUG:
-# After edit macro, text on wrong side (Not reproducing?)
-# Dragging does not always work
 # Canceled during move to image start of a dIdV scan and it stopped responding.
 
 # TODO:
-# Does this work on a Mac?
 # Show number of items in queue in status bar
 
-# If a macro failed, copy it and put it and the top of the queue (Let this be an option)
-
-# Improve the help dialog
-
-# RHK functions
-# Scan - Only top down
-# RHK Scan doesn't stop
-# Set position option (absolute or relative)
-# Set bias modulation amplitude
-
-
-
-
-# Don't hold m_FunctionWindow,m_FunctionNameText in self.TheQueue.  The text only needs to be MacroLabel.  The window is only used to set the tooltip
-
-
-# Have a log dialog that can be opened (but doesn't have to be).  The log dialog shows whatever is printed (or the equivlant)
-
-# Ramping & scanning : set status bar 3
-# Progress bar: https://stackoverflow.com/questions/1883528/wxpython-progress-bar
+VersionNumber = "v0.3.0"
+# VersionNumber also in conf.py & setup.py
+Date = "4/2024"
 
-# RHK Scan time wrong
 
-
-
-# Save PDF
-
-
-# In the createc Scan, when I get the Y pixels, it crashes if I haven't set it?  There's no default value? 
-# On close, I cancel the scan.  Should I try to prevent that?
-
-VersionNumber = "v0.2.0"
 class MacroQueue(MyFrame):
-    MacroPaths = {"RHK":"Macros//RHKMacro.json","CreaTec":"Macros//CreaTecMacro.json","SXM":"Macros//SXMMacro.json"}
+    try:
+        import General
+        Systems = General.Systems
+    except:
+        Systems =['RHK','CreaTec','SXM',"Testing"]
+    NotAuxFiles = [f"{system}.py" for system in Systems]
+    NotAuxFiles.append("SXMRemote.py")
+    MacroPaths = {system:f"Macros//{system}Macro.json" for system in Systems}
 
 # Scanning, fine motion, course motion, dI/dV scans, point spectra, tip form, 
     TheQueue = []
     AddToQueue = []
     FunctionsLoaded = []
     Paused = True
     Running = False
     Software = None
     Closing = False
     Editting = False
     Functions = {}
+    SystemMenuItems = []
 # my_module = importlib.import_module('os.path')
     def __init__(self,test=False):
         self.test = test
         application_path = os.path.dirname(sys.executable) if getattr(sys, 'frozen', False) else os.path.dirname(__file__)
         os.chdir(os.path.realpath(application_path))
         self.SavedSettingsFile = 'MacroQueueSettings.csv'
 
-
         # The GUIDesign is defined in GUIDesign.py as the class MyFrame. It was made with wxFormBuilder
         MyFrame.__init__(self, parent=None) 
+        # self.m_EXEMenuItem.Enable(not getattr(sys, 'frozen', False))
+        if not getattr(sys, 'frozen', False):
+            self.m_EXEMenuItem = wx.MenuItem( self.m_FileMenu, wx.ID_ANY, u"Make Exe", wx.EmptyString, wx.ITEM_NORMAL )
+            self.m_FileMenu.Append( self.m_EXEMenuItem )
+            self.Bind( wx.EVT_MENU, self.MakeExe, id = self.m_EXEMenuItem.GetId() )
+            
+        self.m_ExitMenuItem = wx.MenuItem( self.m_FileMenu, wx.ID_ANY, u"Exit", wx.EmptyString, wx.ITEM_NORMAL )
+        self.m_FileMenu.Append( self.m_ExitMenuItem )
+        self.Bind( wx.EVT_MENU, self.OnClose, id = self.m_ExitMenuItem.GetId() )
+
+        for i,system in enumerate(self.Systems):
+            self.m_SystemmenuItem = wx.MenuItem( self.m_SystemMenu, wx.ID_ANY, system, wx.EmptyString, wx.ITEM_CHECK )
+            self.m_SystemMenu.Append( self.m_SystemmenuItem )
+            self.SystemMenuItems.append(self.m_SystemmenuItem)
+            OnTHISSoftware = partial(self.OnSoftware,i)
+            self.Bind( wx.EVT_MENU, OnTHISSoftware, id = self.m_SystemmenuItem.GetId() )
         icon_file = os.path.join(os.path.abspath(os.path.dirname(__file__)), IconFileName)
         if os.path.exists(icon_file):
             icon = wx.Icon(icon_file)
             self.SetIcon(icon)
             
         self.LoadFunctions()
 
-
-
         # Starts the STM Thread with an Incoming & Outgoing Queue.  Any time-consuming calculations/measurements should be made on this thread.
         try:
             mp.set_start_method('spawn')
         except RuntimeError:
             pass
 
 
         self.OutgoingQueue = mp.Queue()
         self.IncomingQueue = mp.Queue()
 
         self.Process = threading.Thread(target=Thread, args=(self,self.IncomingQueue,self.OutgoingQueue))
         self.Process.start()
 
         # Read the saved settings file here
-        if os.path.exists(self.SavedSettingsFile):
+        if os.path.exists(self.SavedSettingsFile) and not self.test:
             SettingsSeries = pd.read_csv(self.SavedSettingsFile,names=['key','value'])
             self.SettingsDict = SettingsSeries.set_index('key').T.iloc[0].to_dict()
             if "Functions" in self.SettingsDict.keys():
                 self.FunctionsLoaded = [string.replace(" ", "").replace("'", "") for string in (self.SettingsDict["Functions"][1:-1].split(','))]
             if "PauseAfterCancel" in self.SettingsDict.keys():
                 self.m_PauseAfterCancel.Check(self.SettingsDict['PauseAfterCancel'] != 'False')
             self.Software = self.SettingsDict["Software"]
             ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
-            ThisChooseSoftwareDialog.SetSoftware(self.Software)
+            ThisChooseSoftwareDialog.SetSoftware(self.Systems.index(self.Software))
             
             for item in self.m_NotSTMMenu.GetMenuItems():
                 if item.GetItemLabel() in self.FunctionsLoaded:
                     item.Check()
                 else:
                     item.Check(False)
         else:
-            if not test:
+            if not self.test:
                 ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self)
                 ThisChooseSoftwareDialog.ShowModal()
+            else:
+                self.Software = "CreaTec"
+                self.FunctionsLoaded = ["General"]
+                self.IncomingQueue.put(["SoftwareChange",[self.Software,self.FunctionsLoaded]])
+
         # if self.Software is None:
         #     self.OnClose()
         #     return
         
 
 
 
@@ -269,42 +265,44 @@
         self.Functions = {}
         for FunctionName in FunctionNames:
             try:
                 self.Functions[f"{FunctionName[:-3]}"] = import_source_file(os.path.abspath(f'Functions\\{FunctionName}'),FunctionName[:-3])         
                 # self.Functions[f"{FunctionName[:-3]}"] = import_source_file(os.path.abspath(f'Functions\\{FunctionName}'),os.path.abspath(f'Functions\\{FunctionName}'))         
             except Exception as e:
                 pass
-        for file in ["CreaTec.py","RHK.py","SXM.py","SXMRemote.py"]:
+        for file in self.NotAuxFiles:
             try:
                 FunctionNames.remove(file)
             except:
                 pass
         try:
             FunctionNames.insert(0, FunctionNames.pop(FunctionNames.index("General.py")))
         except:
             pass
         for file in FunctionNames:
             
             if not Reloading:
                 CheckFunction = self.m_NotSTMMenu.AppendCheckItem(wx.ID_ANY,file[:-3])
                 self.Bind(wx.EVT_MENU,self.EditLoadedFunctionFiles,CheckFunction)
+                CheckFunction.Check()
             else:
                 MenuItems = self.m_NotSTMMenu.GetMenuItems()
                 MenuLabels = [MenuItem.GetItemLabel() for MenuItem in MenuItems ]
                 if not file[:-3] in MenuLabels:
                     CheckFunction = self.m_NotSTMMenu.AppendCheckItem(wx.ID_ANY,file[:-3])
                     self.Bind(wx.EVT_MENU,self.EditLoadedFunctionFiles,CheckFunction)
+        self.EditLoadedFunctionFiles()
     def EditLoadedFunctionFiles(self,event=None):
         self.FunctionsLoaded = []
         for item in self.m_NotSTMMenu.GetMenuItems():
             if item.IsChecked():
                 self.FunctionsLoaded.append(item.GetItemLabel())
-        
-        ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
-        ThisChooseSoftwareDialog.SetSoftware(self.Software)
+        if self.Software is not None:
+            ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
+            ThisChooseSoftwareDialog.SetSoftware(self.Systems.index(self.Software))
         
     
     def MakeFunctionButtons(self):
         for child in self.m_FunctionButtonWindow.GetChildren():
             child.Destroy()
         FunctionButtonSizer = wx.FlexGridSizer(0,2,0,0)
         
@@ -782,29 +780,21 @@
         return
     def AddDisconnectToQueue(self, event=None):
         OnClose = [['OnClose',{},True],['Pause',{},True]]
         ThisStartMacroDialog = MyStartMacroDialog(self,"Disconnect",OnClose)
         ThisStartMacroDialog.AddToQueue()
         self.AddConnectToQueue()
         return
-    def OnRHKSoftware(self, event):
-        ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self)
-        ThisChooseSoftwareDialog.OnRHK()
-        return
-    def OnCreaTecSoftware(self, event):
+    def OnSoftware(self,i,event):
         ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self)
-        ThisChooseSoftwareDialog.OnCreaTec()
-        return
-    def OnSXMSoftware(self, event):
-        ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self)
-        ThisChooseSoftwareDialog.OnSXM()
-        return
+        ThisChooseSoftwareDialog.SetSoftware(i)
+
     def PauseAfterCancel(self,event):
         ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
-        ThisChooseSoftwareDialog.SetSoftware(self.Software)
+        ThisChooseSoftwareDialog.SetSoftware(self.Systems.index(self.Software))
         pass
     def ReloadFunctions(self,event):
         self.LoadFunctions(Reloading=True)
         self.IncomingQueue.put(["SoftwareChange",[self.Software,self.FunctionsLoaded]])
         pass
     def BasicUseageHelp(self, event):
         HelpMessage = "Left click on your choosen macro from the list on the main page.\n"
@@ -880,16 +870,19 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
         MyMessage = wx.MessageDialog(self,message=HelpMessage,caption="License")
         MyMessage.ShowModal()
         return
     def InfoHelp(self, event):
-        HelpMessage = f"MacroQueue {VersionNumber} (3/2024)\n"
+        HelpMessage = f"MacroQueue {VersionNumber} ({Date})\n"
         HelpMessage += "Written by Brad Goff in Jay Gupta's CME Group at the Ohio State University\n"
+        HelpMessage += "Check out https://guptagroupstm.github.io/MacroQueue for more information.\n"
+        
+
         HelpMessage += "\n"
         MyMessage = wx.MessageDialog(self,message=HelpMessage,caption="Info")
         MyMessage.ShowModal()
         return
     def WriteANewFunctionHelp(self, event):
         HelpMessage = '''Go to File -> Open Source Folder.
 Add the function to the .py file that corresponds to the software you want it to work with.
@@ -933,14 +926,43 @@
         FolderPath = os.path.realpath("Functions/")
         os.startfile(FolderPath)
         return
     def OpenMacroFile(self, event):
         FolderPath = os.path.realpath("Macros/")
         os.startfile(FolderPath)
         return
+    def MakeExe(self,event):
+        if getattr(sys, 'frozen', True):
+            MyMessage = wx.MessageDialog(self,message=f"This will package MacroQueue into an executable.  It will take a few minutes.\nWould you like to continue?.",caption="Create Exe",style=wx.YES_NO)
+            YesOrNo = MyMessage.ShowModal()
+            if YesOrNo == wx.ID_YES:
+                try:
+                    shutil.rmtree(f"{os.path.dirname(__file__)}\\dist\\")
+                except:
+                    pass
+
+                PyInstall(['--onedir','--noconsole',f'--distpath={os.path.abspath(os.path.dirname(__file__))}\\dist',f'--icon={os.path.abspath("MacroQueueIcon.ico")}',f'--add-data={os.path.abspath("MacroQueueIcon.ico")};.',f'--add-data={os.path.abspath(f"{os.path.dirname(__file__)}/Bitmaps")}/*.bmp;Bitmaps','--exclude-module=Functions',f'--add-data={os.path.abspath(f"{os.path.dirname(__file__)}/Functions")}/*.py;Functions',f'--add-data={os.path.abspath(f"{os.path.dirname(__file__)}/Macros")}/*.json;Macros',f'{os.path.abspath("MacroQueue.py")}'])
+                # python -m PyInstaller --onedir --noconsole --icon=MacroQueueIcon.ico  --add-data="MacroQueueIcon.ico;." --add-data="Bitmaps/*.bmp;Bitmaps"  --exclude-module=Functions --add-data="Functions/*.py;Functions" --add-data="Macros/*.json;Macros" --clean  MacroQueue.py
+                try:
+                    shutil.rmtree(f"{os.path.abspath(os.path.dirname(__file__))}\\__pycache__\\")
+                    shutil.rmtree(f"{os.path.abspath(os.path.dirname(__file__))}\\build\\")
+                    os.remove("MacroQueue.spec")
+                except:
+                    pass
+                shutil.move(f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\_internal\\Macros",f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\")
+                shutil.move(f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\_internal\\Functions",f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\")
+                shutil.move(f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\_internal\\Bitmaps",f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\")
+                shutil.copy(f"{os.path.abspath(os.path.dirname(__file__))}\\{self.SavedSettingsFile}",f"{os.path.abspath(os.path.dirname(__file__))}\\dist\\MacroQueue\\")
+                os.startfile(os.path.abspath(f"{os.path.dirname(__file__)}\\dist\\MacroQueue\\"))
+                pass
+        else:
+            MyMessage = wx.MessageDialog(self,message=f"MacroQueue is already an executable.",caption="Create Exe",style=wx.OK_DEFAULT)
+
+    
+
 class MyPanelDropTarget(wx.DropTarget):
     def __init__(self, window,Parent): 
         wx.DropTarget.__init__(self)
         self.window = window
         self.Parent = Parent
         self.data = wx.TextDataObject()
         self.SetDataObject(self.data)
```

### Comparing `MacroQueue-0.2.4/MacroQueue/MacroQueueIcon.ico` & `MacroQueue-0.3.0/MacroQueue/MacroQueueIcon.ico`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue/Macros/CreaTecMacro.json` & `MacroQueue-0.3.0/MacroQueue/Macros/CreaTecMacro.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.04038461538461539%*

 * *Differences: {"'Change RF'": "[['Turn Off RF Generator', OrderedDict(), False], ['Set RF Freq Mode', "*

 * *                "OrderedDict([('Mode', OrderedDict([('DefaultValue', 'CW'), ('Tooltip', ''), "*

 * *                "('Frozen', False), ('ValueType', 'Choice'), ('InRange', True), ('DefaultList', "*

 * *                "['CW', 'List', 'SWE'])]))]), False], ['Set RF Freq', OrderedDict([('Freq', "*

 * *                "OrderedDict([('DefaultValue', '1000000000.0'), ('Tooltip', 'The RF frequency in "*

 * *                "Hz in continuous wa […]*

```diff
@@ -1,717 +1,1119 @@
 {
-    "AutoPhase": [
+    "Change RF": [
         [
-            "Z Course Steps Out",
+            "Turn Off RF Generator",
+            {},
+            false
+        ],
+        [
+            "Set RF Freq Mode",
+            {
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "List",
+                        "SWE"
+                    ],
+                    "DefaultValue": "CW",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Choice"
+                }
+            },
+            false
+        ],
+        [
+            "Set RF Freq",
             {
-                "NBursts": {
-                    "DefaultValue": "3",
+                "Freq": {
+                    "DefaultValue": "1000000000.0",
                     "Frozen": false,
-                    "Tooltip": "Number of Z steps to retract",
+                    "InRange": true,
+                    "Max": 30000000000.0,
+                    "Min": 100000.0,
+                    "Name": "Freq",
+                    "Tooltip": "The RF frequency in Hz in continuous wave mode\nAcceptable range: (100000.0,30000000000.0)",
+                    "Units": "Hz",
                     "ValueType": "Numerical"
                 }
             },
-            true
+            false
+        ],
+        [
+            "Set RF Power Mode",
+            {
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "List",
+                        "SWE"
+                    ],
+                    "DefaultValue": "CW",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Choice"
+                }
+            },
+            false
+        ],
+        [
+            "Set RF Power",
+            {
+                "Power": {
+                    "DefaultValue": "-10",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Max": 27,
+                    "Min": -30,
+                    "Name": "Power",
+                    "Tooltip": "The amount of power for the RF generator in dBm in continuous wave mode\nAcceptable range: (-30,27)",
+                    "Units": "dBm",
+                    "ValueType": "Numerical"
+                }
+            },
+            false
         ],
         [
-            "AutoPhase",
+            "Turn Off RF Generator",
             {},
-            true
+            false
         ],
         [
-            "Approach",
+            "Turn On RF Generator",
             {},
-            true
+            false
         ]
     ],
-    "Course Step": [
+    "Default RF Settings": [
         [
-            "Define as Course Origin",
+            "Turn Off RF Generator",
             {},
             true
         ],
         [
-            "Burst XY",
+            "Set RF Freq Mode",
             {
-                "Burst_XY": {
-                    "DefaultValue": true,
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "List",
+                        "SWE"
+                    ],
+                    "DefaultValue": "CW",
                     "Frozen": false,
-                    "Tooltip": "Check Burst XY in the Course Positioning Form",
-                    "ValueType": "Boolean"
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
             true
         ],
         [
-            "XYCourse Step",
+            "Set RF Freq",
             {
-                "NSteps_Out": {
-                    "DefaultValue": "5",
-                    "Frozen": false,
-                    "Tooltip": "The number of Z steps to retract before course moving in X and Y",
-                    "ValueType": "Numerical"
-                },
-                "X_Position": {
-                    "DefaultValue": "10",
-                    "Frozen": false,
-                    "Tooltip": "The X position to course move to.",
-                    "ValueType": "Numerical"
-                },
-                "Y_Position": {
-                    "DefaultValue": "10",
+                "Freq": {
+                    "DefaultValue": "1000000000.0",
                     "Frozen": false,
-                    "Tooltip": "The Y position to course move to.",
+                    "InRange": true,
+                    "Max": 30000000000.0,
+                    "Min": 100000.0,
+                    "Name": "Freq",
+                    "Tooltip": "The RF frequency in Hz in continuous wave mode\nAcceptable range: (100000.0,30000000000.0)",
+                    "Units": "Hz",
                     "ValueType": "Numerical"
                 }
             },
-            true
+            false
         ],
         [
-            "Approach",
-            {},
+            "Set RF Power Mode",
+            {
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "List",
+                        "SWE"
+                    ],
+                    "DefaultValue": "CW",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Choice"
+                }
+            },
             true
         ],
         [
-            "Wait",
+            "Set RF Power",
             {
-                "WaitTime": {
-                    "DefaultValue": "120",
+                "Power": {
+                    "DefaultValue": "-10",
                     "Frozen": false,
-                    "Tooltip": "The time to wait in seconds",
-                    "Units": "s",
+                    "InRange": true,
+                    "Max": 27,
+                    "Min": -30,
+                    "Name": "Power",
+                    "Tooltip": "The amount of power for the RF generator in dBm in continuous wave mode\nAcceptable range: (-30,27)",
+                    "Units": "dBm",
                     "ValueType": "Numerical"
                 }
             },
             false
-        ]
-    ],
-    "RF Spectrum": [
+        ],
         [
-            "Fine Move Tip",
+            "Set RF Trig Dir",
             {
-                "HowToSetPosition": {
+                "Dir": {
                     "DefaultList": [
-                        "nm",
-                        "Image Coord",
-                        "Voltage"
+                        "POS",
+                        "NEG"
                     ],
-                    "DefaultValue": "nm",
+                    "DefaultValue": "POS",
                     "Frozen": false,
                     "InRange": true,
                     "Tooltip": "",
                     "ValueType": "Choice"
-                },
-                "XOffset": {
-                    "DefaultValue": "0",
+                }
+            },
+            true
+        ],
+        [
+            "Set RF Trig Type",
+            {
+                "TrigType": {
+                    "DefaultList": [
+                        "NORM",
+                        "GATE"
+                    ],
+                    "DefaultValue": "NORM",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The X position of the tip in nm, or Image Coordinate, or V",
-                    "ValueType": "Numerical"
-                },
-                "YOffset": {
-                    "DefaultValue": "0",
+                    "Name": "TrigType",
+                    "Tooltip": "NORMal trigger = edge initiates/stops sweeps; GATE trigger level starts/stops sweep.",
+                    "ValueType": "Choice"
+                }
+            },
+            true
+        ],
+        [
+            "Set RF Trig Sour",
+            {
+                "Trig": {
+                    "DefaultList": [
+                        "EXT",
+                        "IMM",
+                        "KEY",
+                        "BUS"
+                    ],
+                    "DefaultValue": "EXT",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The Y X position of the tip in nm, or Image Coordinate, or V",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
-            false
+            true
         ],
         [
-            "Set LockIn Amplitude",
+            "Set RF SWE Direction",
             {
-                "Lockin_Amp": {
-                    "DefaultValue": "100",
+                "direction": {
+                    "DefaultList": [
+                        "UP",
+                        "DOWN"
+                    ],
+                    "DefaultValue": "UP",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The lock-in voltage amplitude in mV",
-                    "Units": "mV",
-                    "ValueType": "Numerical"
+                    "Name": "direction",
+                    "Tooltip": "Up is increasing, down is decreasing.",
+                    "ValueType": "Choice"
                 }
             },
-            false
+            true
         ],
         [
-            "Set LockIn Frequency",
+            "Set RF SWE Count",
             {
-                "Lockin_Freq": {
-                    "DefaultValue": "877",
+                "Infinite": {
+                    "DefaultValue": false,
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The lock-in frequency in Hz",
-                    "Units": "Hz",
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
+                },
+                "count": {
+                    "DefaultValue": "1",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Min": 1,
+                    "Name": "count",
+                    "Tooltip": "The number of sweeps to perform after a trigger\nMinimum value: 1",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set LockIn TimeConstant",
+            "Set RF LIST Count",
             {
-                "Lockin_RC": {
-                    "DefaultValue": "100",
+                "Infinite": {
+                    "DefaultValue": false,
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The lock-in time constant in Hz",
-                    "Units": "Hz",
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
+                },
+                "count": {
+                    "DefaultValue": "1",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Min": 1,
+                    "Name": "count",
+                    "Tooltip": "The number of sweeps to perform after a trigger\nMinimum value: 1",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set RF Freq",
+            "Set RF SWE Spacing",
             {
-                "Freq": {
-                    "DefaultValue": "1000000000.0",
+                "Spacing": {
+                    "DefaultList": [
+                        "Linear",
+                        "Log"
+                    ],
+                    "DefaultValue": "Linear",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The RF frequency in Hz",
-                    "Units": "Hz",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
-            false
+            true
         ],
         [
-            "Set RF Power",
+            "Set RF LIST Blanking",
             {
-                "Power": {
-                    "DefaultValue": "0",
+                "Blanking": {
+                    "DefaultValue": false,
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The amount of power for the RF generator in dBm",
-                    "Units": "dBm",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
                 }
             },
-            false
+            true
         ],
         [
-            "Spectrum",
-            {},
+            "Set RF SWE Blanking",
+            {
+                "Blanking": {
+                    "DefaultValue": false,
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
+                }
+            },
             true
         ]
     ],
-    "Scan": [
+    "Example2": [
         [
-            "Set Recorded Channels",
+            "Wait",
             {
-                "Current": {
+                "WaitTime": {
+                    "DefaultValue": "1",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Name": "WaitTime",
+                    "Tooltip": "The time to wait",
+                    "Units": "s",
+                    "ValueType": "Numerical"
+                }
+            },
+            true
+        ],
+        [
+            "Complex Function2",
+            {
+                "SomeBoolean": {
                     "DefaultValue": true,
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "",
+                    "Name": "SomeBoolean",
+                    "Tooltip": "A Boolean parameter produces a checkbox",
                     "ValueType": "Boolean"
                 },
-                "LockInX": {
-                    "DefaultValue": false,
+                "SomeChoice": {
+                    "DefaultList": [
+                        "Choice",
+                        "Combo",
+                        "3rd",
+                        "4th"
+                    ],
+                    "DefaultValue": "Choice",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "",
-                    "ValueType": "Boolean"
+                    "Name": "SomeChoice",
+                    "Tooltip": "A Choice parameter produces a dropdown menu",
+                    "ValueType": "Choice"
                 },
-                "Topography": {
-                    "DefaultValue": true,
+                "SomeFilePath": {
+                    "DefaultValue": "C:\\",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "",
-                    "ValueType": "Boolean"
+                    "Name": "SomeFilePath",
+                    "Tooltip": "A filepath parameter produces a 'browse' button",
+                    "ValueType": "File"
+                },
+                "SomeString": {
+                    "DefaultValue": "String",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Name": "SomeString",
+                    "Tooltip": "A String parameter produces a textbox",
+                    "ValueType": "String"
                 }
             },
             true
-        ],
+        ]
+    ],
+    "RF Freq Sweep": [
         [
             "Null",
             {
                 "Index": {
                     "DefaultValue": "0",
                     "Frozen": false,
                     "InRange": true,
                     "Tooltip": "This has no impact.  It's solely used to repeat the functions.",
                     "ValueType": "Numerical"
                 }
             },
             false
         ],
         [
-            "Set NPixels",
+            "Turn Off RF Generator",
+            {},
+            true
+        ],
+        [
+            "Set RF Freq Mode",
             {
-                "NPixels": {
-                    "DefaultValue": "512",
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "LIST",
+                        "SWE"
+                    ],
+                    "DefaultValue": "SWE",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The number of pixels in each row and each column",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Scan Image Size",
+            "Set RF Power Mode",
             {
-                "HowToSetSize": {
+                "Mode": {
                     "DefaultList": [
-                        "Image Size",
-                        "Resolution"
+                        "CW",
+                        "LIST",
+                        "SWE"
                     ],
-                    "DefaultValue": "Image Size",
+                    "DefaultValue": "CW",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "Choose to set the Image Size in \u00c5 directly or the Resolution in \u00c5/pixel",
+                    "Tooltip": "",
                     "ValueType": "Choice"
-                },
-                "ImageSize": {
-                    "DefaultValue": "1000",
+                }
+            },
+            true
+        ],
+        [
+            "Set RF Freq",
+            {
+                "Freq": {
+                    "DefaultValue": "1000000000.0",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The length of a row and column in \u00c5 or \u00c5/pixel",
-                    "Units": "\u00c5",
+                    "Max": 30000000000.0,
+                    "Min": 100000.0,
+                    "Name": "Freq",
+                    "Tooltip": "The RF frequency in Hz in continuous wave mode\nAcceptable range: (100000.0,30000000000.0)",
+                    "Units": "Hz",
                     "ValueType": "Numerical"
                 }
             },
             false
         ],
         [
-            "Set Scan Speed",
+            "Set RF SWE Start",
             {
-                "HowToSetSpeed": {
-                    "DefaultList": [
-                        "nm/s",
-                        "s/line",
-                        "s/pixel"
-                    ],
-                    "DefaultValue": "s/line",
-                    "Frozen": false,
-                    "InRange": true,
-                    "Tooltip": "Choose how the Image Speed is set",
-                    "ValueType": "Choice"
-                },
-                "Speed": {
-                    "DefaultValue": "0.5",
+                "Start": {
+                    "DefaultValue": "1e9",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The speed the tip moves in nm/s, s/line, or s/pixel",
+                    "Tooltip": "",
                     "ValueType": "Numerical"
                 }
             },
             false
         ],
         [
-            "Set Scan Window Position",
+            "Set RF SWE Stop",
             {
-                "HowToSetPosition": {
-                    "DefaultList": [
-                        "nm",
-                        "Image Coord",
-                        "Voltage"
-                    ],
-                    "DefaultValue": "nm",
+                "Stop": {
+                    "DefaultValue": "20e9",
                     "Frozen": false,
                     "InRange": true,
                     "Tooltip": "",
-                    "ValueType": "Choice"
-                },
-                "XOffset": {
-                    "DefaultValue": "0",
-                    "Frozen": false,
-                    "InRange": true,
-                    "Tooltip": "The X center of the image in nm, or Image Coordinate, or V",
-                    "ValueType": "Numerical"
-                },
-                "YOffset": {
-                    "DefaultValue": "0",
-                    "Frozen": false,
-                    "InRange": true,
-                    "Tooltip": "The Y top of the image in nm, or Image Coordinate, or V",
                     "ValueType": "Numerical"
                 }
             },
             false
         ],
         [
-            "Set Setpoint",
+            "Set RF SWE Points",
             {
-                "Setpoint": {
-                    "DefaultValue": "100",
+                "points": {
+                    "DefaultValue": "5000",
                     "Frozen": false,
                     "InRange": true,
-                    "Max": 1000000.0,
-                    "Min": 0,
-                    "Name": "Setpoint",
-                    "Tooltip": "The current setpoint in pA\nAcceptable range: (0,1000000.0)",
-                    "Units": "pA",
+                    "Min": 1,
+                    "Name": "points",
+                    "Tooltip": "The number of points in a sweep.\nMinimum value: 1",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Bias",
+            "Set RF Trig Dir",
             {
-                "Bias": {
-                    "DefaultValue": "1",
+                "Dir": {
+                    "DefaultList": [
+                        "POS",
+                        "NEG"
+                    ],
+                    "DefaultValue": "POS",
                     "Frozen": false,
                     "InRange": true,
-                    "Max": 10,
-                    "Min": -10,
-                    "Name": "Bias",
-                    "Tooltip": "The bias voltage in V\nAcceptable range: (-10,10)",
-                    "Units": "V",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
-            false
+            true
         ],
         [
-            "Wait",
+            "Set RF LIST Count",
             {
-                "WaitTime": {
+                "Infinite": {
+                    "DefaultValue": false,
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
+                },
+                "count": {
                     "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The time to wait in seconds",
-                    "Units": "s",
+                    "Min": 1,
+                    "Name": "count",
+                    "Tooltip": "The number of sweeps to perform after a trigger\nMinimum value: 1",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Scan",
-            {},
+            "Set RF Trig Sour",
+            {
+                "Trig": {
+                    "DefaultList": [
+                        "EXT",
+                        "IMM",
+                        "KEY",
+                        "BUS"
+                    ],
+                    "DefaultValue": "EXT",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Choice"
+                }
+            },
             true
-        ]
-    ],
-    "Spectrum": [
+        ],
         [
-            "Fine Move Tip",
+            "Set RF Trig Type",
             {
-                "HowToSetPosition": {
+                "TrigType": {
                     "DefaultList": [
-                        "nm",
-                        "Image Coord",
-                        "Voltage"
+                        "NORM",
+                        "GATE"
                     ],
-                    "DefaultValue": "nm",
+                    "DefaultValue": "NORM",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "",
+                    "Name": "TrigType",
+                    "Tooltip": "NORMal trigger = edge initiates/stops sweeps; GATE trigger level starts/stops sweep.",
                     "ValueType": "Choice"
-                },
-                "XOffset": {
-                    "DefaultValue": "0",
+                }
+            },
+            true
+        ],
+        [
+            "Set RF SWE Blanking",
+            {
+                "Blanking": {
+                    "DefaultValue": false,
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The X position of the tip in nm, or Image Coordinate, or V",
-                    "ValueType": "Numerical"
-                },
-                "YOffset": {
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
+                }
+            },
+            true
+        ],
+        [
+            "Set RF SWE Del",
+            {
+                "delay": {
                     "DefaultValue": "0",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The Y X position of the tip in nm, or Image Coordinate, or V",
+                    "Min": 0,
+                    "Name": "delay",
+                    "Tooltip": "Delay time before going to next point.  RF Off time.\nMinimum value: 0",
+                    "Units": "s",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set LockIn Amplitude",
+            "Set RF SWE Dwell",
             {
-                "Lockin_Amp": {
-                    "DefaultValue": "100",
+                "dwell": {
+                    "DefaultValue": "0.1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The lock-in voltage amplitude in mV",
-                    "Units": "mV",
+                    "Min": 1,
+                    "Name": "dwell",
+                    "Tooltip": "Dwell time on each point.  RF On time.\nMinimum value: 1",
+                    "Units": "s",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
+        ],
+        [
+            "Turn On RF Generator",
+            {},
+            true
+        ],
+        [
+            "Set Spectrum Table to Constant Bias",
+            {},
+            true
+        ],
+        [
+            "Set Spectrum Table Trig Vaux",
+            {},
+            true
         ],
         [
-            "Set LockIn Frequency",
+            "Set Spectrum Mode",
             {
-                "Lockin_Freq": {
-                    "DefaultValue": "877",
+                "Mode": {
+                    "DefaultList": [
+                        "I(V,z)",
+                        "z(V)",
+                        "z(V,X:I)"
+                    ],
+                    "DefaultValue": "z(V)",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The lock-in frequency in Hz",
-                    "Units": "Hz",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
-            false
+            true
         ],
         [
-            "Set LockIn TimeConstant",
+            "Set Spectrum Setpoint",
             {
-                "Lockin_RC": {
-                    "DefaultValue": "100",
+                "Setpoint": {
+                    "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The lock-in time constant in Hz",
-                    "Units": "Hz",
+                    "Max": 10000.0,
+                    "Name": "Setpoint",
+                    "Tooltip": "The setpoint for constant current spectra\nMaximum value: 10000.0",
+                    "Units": "nA",
                     "ValueType": "Numerical"
+                },
+                "Use_Scan_Setpoint": {
+                    "DefaultValue": true,
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
                 }
             },
-            false
+            true
         ],
         [
-            "Set RF Freq",
+            "Set Spectra Time",
             {
-                "Freq": {
-                    "DefaultValue": "1e9",
+                "Time": {
+                    "DefaultValue": "60",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The RF frequency in Hz",
-                    "Units": "Hz",
+                    "Tooltip": "The duration of the spectrum for a single direction",
+                    "Units": "s",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set RF Power",
+            "Set Spectra NAveraging",
             {
-                "Power": {
-                    "DefaultValue": "0",
+                "N": {
+                    "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The amount of power for the RF generator in dBm",
-                    "Units": "dBm",
+                    "Tooltip": "The number of spectra to take and average.  Takes long. reduces noise.",
                     "ValueType": "Numerical"
                 }
             },
             true
         ],
         [
             "Spectrum",
             {},
             true
         ]
     ],
-    "Test": [
+    "RF Power Sweep": [
         [
-            "Exception Function",
+            "Null",
             {
-                "SomeParameter": {
-                    "DefaultValue": "5",
+                "Index": {
+                    "DefaultValue": "0",
                     "Frozen": false,
                     "InRange": true,
-                    "Max": 10,
-                    "Name": "SomeParameter",
-                    "Tooltip": "\nMaximum value: 10",
+                    "Tooltip": "This has no impact.  It's solely used to repeat the functions.",
                     "ValueType": "Numerical"
                 }
             },
+            false
+        ],
+        [
+            "Turn Off RF Generator",
+            {},
             true
-        ]
-    ],
-    "Wait": [
+        ],
         [
-            "Wait",
+            "Set RF Freq Mode",
             {
-                "WaitTime": {
-                    "DefaultValue": "10",
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "LIST",
+                        "SWE"
+                    ],
+                    "DefaultValue": "CW",
                     "Frozen": false,
-                    "Tooltip": "The time to wait in seconds",
-                    "Units": "s",
-                    "ValueType": "Numerical"
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Choice"
                 }
             },
             true
-        ]
-    ],
-    "dIdV Scan": [
+        ],
         [
-            "Set Recorded Channels",
+            "Set RF Power Mode",
             {
-                "Current": {
-                    "DefaultValue": true,
-                    "Frozen": true,
+                "Mode": {
+                    "DefaultList": [
+                        "CW",
+                        "LIST",
+                        "SWE"
+                    ],
+                    "DefaultValue": "SWE",
+                    "Frozen": false,
                     "InRange": true,
                     "Tooltip": "",
-                    "ValueType": "Boolean"
-                },
-                "LockInX": {
-                    "DefaultValue": true,
-                    "Frozen": true,
+                    "ValueType": "Choice"
+                }
+            },
+            true
+        ],
+        [
+            "Set RF Freq",
+            {
+                "Freq": {
+                    "DefaultValue": "1000000000.0",
+                    "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "",
-                    "ValueType": "Boolean"
-                },
-                "Topography": {
-                    "DefaultValue": true,
-                    "Frozen": true,
+                    "Max": 30000000000.0,
+                    "Min": 100000.0,
+                    "Name": "Freq",
+                    "Tooltip": "The RF frequency in Hz in continuous wave mode\nAcceptable range: (100000.0,30000000000.0)",
+                    "Units": "Hz",
+                    "ValueType": "Numerical"
+                }
+            },
+            false
+        ],
+        [
+            "Set RF SWE Start",
+            {
+                "Start": {
+                    "DefaultValue": "-30",
+                    "Frozen": false,
                     "InRange": true,
                     "Tooltip": "",
-                    "ValueType": "Boolean"
+                    "ValueType": "Numerical"
                 }
             },
-            true
+            false
         ],
         [
-            "Null",
+            "Set RF SWE Stop",
             {
-                "Index": {
+                "Stop": {
                     "DefaultValue": "0",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "This has no impact.  It's solely used to repeat the functions.",
+                    "Tooltip": "",
                     "ValueType": "Numerical"
                 }
             },
             false
         ],
         [
-            "Set NPixels",
+            "Set RF SWE Points",
             {
-                "NPixels": {
-                    "DefaultValue": "512",
+                "points": {
+                    "DefaultValue": "3000",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The number of pixels in each row and each column",
+                    "Min": 1,
+                    "Name": "points",
+                    "Tooltip": "The number of points in a sweep.\nMinimum value: 1",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Scan Image Size",
+            "Set RF Trig Dir",
             {
-                "HowToSetSize": {
+                "Dir": {
                     "DefaultList": [
-                        "Image Size",
-                        "Resolution"
+                        "POS",
+                        "NEG"
                     ],
-                    "DefaultValue": "Image Size",
+                    "DefaultValue": "POS",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "Choose to set the Image Size in \u00c5 directly or the Resolution in \u00c5/pixel",
+                    "Tooltip": "",
                     "ValueType": "Choice"
+                }
+            },
+            true
+        ],
+        [
+            "Set RF LIST Count",
+            {
+                "Infinite": {
+                    "DefaultValue": false,
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
                 },
-                "ImageSize": {
-                    "DefaultValue": "1000",
+                "count": {
+                    "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The length of a row and column in \u00c5 or \u00c5/pixel",
-                    "Units": "\u00c5",
+                    "Min": 1,
+                    "Name": "count",
+                    "Tooltip": "The number of sweeps to perform after a trigger\nMinimum value: 1",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Scan Speed",
+            "Set RF Trig Sour",
             {
-                "HowToSetSpeed": {
+                "Trig": {
                     "DefaultList": [
-                        "nm/s",
-                        "s/line",
-                        "s/pixel"
+                        "EXT",
+                        "IMM",
+                        "KEY",
+                        "BUS"
                     ],
-                    "DefaultValue": "s/line",
+                    "DefaultValue": "EXT",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "Choose how the Image Speed is set",
+                    "Tooltip": "",
                     "ValueType": "Choice"
-                },
-                "Speed": {
-                    "DefaultValue": "1",
+                }
+            },
+            true
+        ],
+        [
+            "Set RF Trig Type",
+            {
+                "TrigType": {
+                    "DefaultList": [
+                        "NORM",
+                        "GATE"
+                    ],
+                    "DefaultValue": "NORM",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The speed the tip moves in nm/s, s/line, or s/pixel",
+                    "Name": "TrigType",
+                    "Tooltip": "NORMal trigger = edge initiates/stops sweeps; GATE trigger level starts/stops sweep.",
+                    "ValueType": "Choice"
+                }
+            },
+            true
+        ],
+        [
+            "Set RF SWE Blanking",
+            {
+                "Blanking": {
+                    "DefaultValue": false,
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
+                }
+            },
+            true
+        ],
+        [
+            "Set RF SWE Del",
+            {
+                "delay": {
+                    "DefaultValue": "0",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Min": 0,
+                    "Name": "delay",
+                    "Tooltip": "Delay time before going to next point.  RF Off time.\nMinimum value: 0",
+                    "Units": "s",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Scan Window Position",
+            "Set RF SWE Dwell",
             {
-                "HowToSetPosition": {
+                "dwell": {
+                    "DefaultValue": "0.1",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Min": 1,
+                    "Name": "dwell",
+                    "Tooltip": "Dwell time on each point.  RF On time.\nMinimum value: 1",
+                    "Units": "s",
+                    "ValueType": "Numerical"
+                }
+            },
+            true
+        ],
+        [
+            "Turn On RF Generator",
+            {},
+            true
+        ],
+        [
+            "Set Spectrum Table to Constant Bias",
+            {},
+            true
+        ],
+        [
+            "Set Spectrum Table Trig Vaux",
+            {},
+            true
+        ],
+        [
+            "Set Spectrum Mode",
+            {
+                "Mode": {
                     "DefaultList": [
-                        "nm",
-                        "Image Coord",
-                        "Voltage"
+                        "I(V,z)",
+                        "z(V)",
+                        "z(V,X:I)"
                     ],
-                    "DefaultValue": "Voltage",
+                    "DefaultValue": "z(V)",
                     "Frozen": false,
                     "InRange": true,
                     "Tooltip": "",
                     "ValueType": "Choice"
-                },
-                "XOffset": {
-                    "DefaultValue": "0",
+                }
+            },
+            true
+        ],
+        [
+            "Set Spectrum Setpoint",
+            {
+                "Setpoint": {
+                    "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The X center of the image in nm, or Image Coordinate, or V",
+                    "Max": 10000.0,
+                    "Name": "Setpoint",
+                    "Tooltip": "The setpoint for constant current spectra\nMaximum value: 10000.0",
+                    "Units": "nA",
                     "ValueType": "Numerical"
                 },
-                "YOffset": {
-                    "DefaultValue": "0",
+                "Use_Scan_Setpoint": {
+                    "DefaultValue": true,
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The Y top of the image in nm, or Image Coordinate, or V",
-                    "ValueType": "Numerical"
+                    "Tooltip": "",
+                    "ValueType": "Boolean"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Setpoint",
+            "Set Spectra Time",
             {
-                "Setpoint": {
-                    "DefaultValue": "100",
+                "Time": {
+                    "DefaultValue": "60",
                     "Frozen": false,
                     "InRange": true,
-                    "Max": 1000000.0,
-                    "Min": 0,
-                    "Name": "Setpoint",
-                    "Tooltip": "The current setpoint in pA\nAcceptable range: (0,1000000.0)",
-                    "Units": "pA",
+                    "Tooltip": "The duration of the spectrum for a single direction",
+                    "Units": "s",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "Set Bias",
+            "Set Spectra NAveraging",
             {
-                "Bias": {
+                "N": {
                     "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Max": 10,
-                    "Min": -10,
-                    "Name": "Bias",
-                    "Tooltip": "The bias voltage in V\nAcceptable range: (-10,10)",
-                    "Units": "V",
+                    "Tooltip": "The number of spectra to take and average.  Takes long. reduces noise.",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
+        ],
+        [
+            "Spectrum",
+            {},
+            true
+        ]
+    ],
+    "Test": [
+        [
+            "Null",
+            {
+                "Index": {
+                    "DefaultValue": "0,3,1",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "This has no impact.  It's solely used to repeat the functions.",
+                    "ValueType": "Numerical"
+                }
+            },
+            true
         ],
         [
             "Wait",
             {
                 "WaitTime": {
                     "DefaultValue": "1",
                     "Frozen": false,
                     "InRange": true,
-                    "Tooltip": "The time to wait in seconds",
+                    "Name": "WaitTime",
+                    "Tooltip": "The time to wait",
                     "Units": "s",
                     "ValueType": "Numerical"
                 }
             },
-            false
+            true
         ],
         [
-            "dIdV Scan",
-            {},
+            "Print",
+            {
+                "Number": {
+                    "DefaultValue": "10,20",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Tooltip": "",
+                    "ValueType": "Numerical"
+                }
+            },
             true
+        ],
+        [
+            "Complex Function",
+            {
+                "SomeBoolean": {
+                    "DefaultValue": true,
+                    "Frozen": false,
+                    "InRange": true,
+                    "Name": "SomeBoolean",
+                    "Tooltip": "A Boolean parameter produces a checkbox",
+                    "ValueType": "Boolean"
+                },
+                "SomeChoice": {
+                    "DefaultList": [
+                        "Choice",
+                        "Combo",
+                        "3rd",
+                        "4th"
+                    ],
+                    "DefaultValue": "Choice",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Name": "SomeChoice",
+                    "Tooltip": "A Choice parameter produces a dropdown menu",
+                    "ValueType": "Choice"
+                },
+                "SomeFilePath": {
+                    "DefaultValue": "C:\\",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Name": "SomeFilePath",
+                    "Tooltip": "A filepath parameter produces a 'browse' button",
+                    "ValueType": "File"
+                },
+                "SomeString": {
+                    "DefaultValue": "String",
+                    "Frozen": false,
+                    "InRange": true,
+                    "Name": "SomeString",
+                    "Tooltip": "A String parameter produces a textbox",
+                    "ValueType": "String"
+                }
+            },
+            false
         ]
     ]
 }
```

### Comparing `MacroQueue-0.2.4/MacroQueue/MakeExe.sh` & `MacroQueue-0.3.0/MacroQueue/MakeExe.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 rm -r .\\dist\\
 python -m PyInstaller --onedir --noconsole --icon=MacroQueueIcon.ico  --add-data="MacroQueueIcon.ico;." --add-data="Bitmaps/*.bmp;Bitmaps"  --exclude-module=Functions --add-data="Functions/*.py;Functions" --add-data="Macros/*.json;Macros" --clean  MacroQueue.py
 rm -r .\\__pycache__\\
 rm -r .\\build\\
 rm MacroQueue.spec
 mv .\\dist\\MacroQueue\\_internal\\Macros .\\dist\\MacroQueue\\
 mv .\\dist\\MacroQueue\\_internal\\Functions .\\dist\\MacroQueue\\
-mv .\\dist\\MacroQueue\\_internal\\Bitmaps .\\dist\\MacroQueue\\
+mv .\\dist\\MacroQueue\\_internal\\Bitmaps .\\dist\\MacroQueue\\
+start \\dist\\MacroQueue
```

### Comparing `MacroQueue-0.2.4/MacroQueue/__init__.py` & `MacroQueue-0.3.0/MacroQueue/__init__.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.4/MacroQueue.egg-info/PKG-INFO` & `MacroQueue-0.3.0/MacroQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MacroQueue
-Version: 0.2.4
+Version: 0.3.0
 Summary: Automating Scanning Probe Microscopy
 Home-page: https://github.com/guptagroupstm/STMMacroQueue
-Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.0.tar.gz
 Author: Brad Goff
 Author-email: guptagroupstm@gmail.com
 License: MIT
 Keywords: Automation,Scanning Probe Microscopy,Macro,Queue
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -29,20 +29,21 @@
 
 Users can easily add python functions to control new and existing equipment.  Although any arbitary python function can be added, the base functions were created with the functional programming paradigm in mind, so the functions are small and each perform a single task.  For example, the function "Set RF Frequency", changes the frequency on the RF generator and records the new value.  This allows the functions to be reused for many types of measurements.
 
 The functions can be grouped into macros for each type of measurement.  Macros are added to a queue with different values for each parameter (e.g. bias, magnetic field, etc.) to perform measurements throughout a parameter space.  Each measurement is performed consecutively on a seperate thread to enable measurements in the queue to be modified.
 These features allow users to easily control several instruments in sync, perform a long series of measurements with minimal input, and add new instruments to a system. 
 The goal of MacroQueue is to provide a GUI that allow users to perform measurements in high-dimensional parameter spaces without requiring coding ability while still providing users with coding ability the flexibility to write arbitrarily complex functions.  
 
+Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
+
 
 ![Brief image of MacroQueue](https://raw.githubusercontent.com/guptagroupstm/MacroQueue/main/docs_src/source/ReadMe.png)
 
 ![Brief image of MacroQueue](https://raw.githubusercontent.com/guptagroupstm/MacroQueue/main/docs_src/source/ExpandingFigure.png)
 
-Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
 
 ## Installation
 
 See the [install documentation](https://guptagroupstm.github.io/MacroQueue/Install.html). System requirements are also found in this page.
 
 ## Contributing
```

### Comparing `MacroQueue-0.2.4/MacroQueue.egg-info/SOURCES.txt` & `MacroQueue-0.3.0/MacroQueue.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 MacroQueue/Functions/BField.py
 MacroQueue/Functions/CreaTec.py
 MacroQueue/Functions/General.py
 MacroQueue/Functions/RF.py
 MacroQueue/Functions/RHK.py
 MacroQueue/Functions/SXM.py
 MacroQueue/Functions/SXMRemote.py
+MacroQueue/Functions/Testing.py
 MacroQueue/Macros/CreaTecMacro.json
 MacroQueue/Macros/RHKMacro.json
+MacroQueue/Macros/TestingMacro.json
 test/test_MainFrame.py
 test/test_STMthread.py
 test/test_readdata.py
```

### Comparing `MacroQueue-0.2.4/PKG-INFO` & `MacroQueue-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MacroQueue
-Version: 0.2.4
+Version: 0.3.0
 Summary: Automating Scanning Probe Microscopy
 Home-page: https://github.com/guptagroupstm/STMMacroQueue
-Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.0.tar.gz
 Author: Brad Goff
 Author-email: guptagroupstm@gmail.com
 License: MIT
 Keywords: Automation,Scanning Probe Microscopy,Macro,Queue
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -29,20 +29,21 @@
 
 Users can easily add python functions to control new and existing equipment.  Although any arbitary python function can be added, the base functions were created with the functional programming paradigm in mind, so the functions are small and each perform a single task.  For example, the function "Set RF Frequency", changes the frequency on the RF generator and records the new value.  This allows the functions to be reused for many types of measurements.
 
 The functions can be grouped into macros for each type of measurement.  Macros are added to a queue with different values for each parameter (e.g. bias, magnetic field, etc.) to perform measurements throughout a parameter space.  Each measurement is performed consecutively on a seperate thread to enable measurements in the queue to be modified.
 These features allow users to easily control several instruments in sync, perform a long series of measurements with minimal input, and add new instruments to a system. 
 The goal of MacroQueue is to provide a GUI that allow users to perform measurements in high-dimensional parameter spaces without requiring coding ability while still providing users with coding ability the flexibility to write arbitrarily complex functions.  
 
+Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
+
 
 ![Brief image of MacroQueue](https://raw.githubusercontent.com/guptagroupstm/MacroQueue/main/docs_src/source/ReadMe.png)
 
 ![Brief image of MacroQueue](https://raw.githubusercontent.com/guptagroupstm/MacroQueue/main/docs_src/source/ExpandingFigure.png)
 
-Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
 
 ## Installation
 
 See the [install documentation](https://guptagroupstm.github.io/MacroQueue/Install.html). System requirements are also found in this page.
 
 ## Contributing
```

### Comparing `MacroQueue-0.2.4/README.md` & `MacroQueue-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 Users can easily add python functions to control new and existing equipment.  Although any arbitary python function can be added, the base functions were created with the functional programming paradigm in mind, so the functions are small and each perform a single task.  For example, the function "Set RF Frequency", changes the frequency on the RF generator and records the new value.  This allows the functions to be reused for many types of measurements.
 
 The functions can be grouped into macros for each type of measurement.  Macros are added to a queue with different values for each parameter (e.g. bias, magnetic field, etc.) to perform measurements throughout a parameter space.  Each measurement is performed consecutively on a seperate thread to enable measurements in the queue to be modified.
 These features allow users to easily control several instruments in sync, perform a long series of measurements with minimal input, and add new instruments to a system. 
 The goal of MacroQueue is to provide a GUI that allow users to perform measurements in high-dimensional parameter spaces without requiring coding ability while still providing users with coding ability the flexibility to write arbitrarily complex functions.  
 
+Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
+
 
 ![Brief image of MacroQueue](https://raw.githubusercontent.com/guptagroupstm/MacroQueue/main/docs_src/source/ReadMe.png)
 
 ![Brief image of MacroQueue](https://raw.githubusercontent.com/guptagroupstm/MacroQueue/main/docs_src/source/ExpandingFigure.png)
 
-Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
 
 ## Installation
 
 See the [install documentation](https://guptagroupstm.github.io/MacroQueue/Install.html). System requirements are also found in this page.
 
 ## Contributing
```

### Comparing `MacroQueue-0.2.4/setup.py` & `MacroQueue-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,24 @@
    import pypandoc
    long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
 # read the contents of your README file
   from pathlib import Path
   this_directory = Path(__file__).parent
   long_description = (this_directory / "README.md").read_text()
-print(long_description)
 setup(
   name = 'MacroQueue',         # How you named your package folder (MyLib)
   packages = ['MacroQueue'],   # Chose the same as "name"
-  version = '0.2.4',      # Start with a small number and increase it with every change you make
+  version = '0.3.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Automating Scanning Probe Microscopy',   # Give a short description about your library
   author = 'Brad Goff',                   # Type in your name
   author_email = 'guptagroupstm@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/guptagroupstm/STMMacroQueue',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.2.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.0.tar.gz',    # I explain this later on
   keywords = ['Automation', 'Scanning Probe Microscopy', 'Macro',"Queue"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pandas',
           'wxPython',
           'pyvisa',
           'PyWin32',
           'pyinstaller'
```

### Comparing `MacroQueue-0.2.4/test/test_MainFrame.py` & `MacroQueue-0.3.0/test/test_MainFrame.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import wx
 import unittest
 import multiprocessing as mp
 import sys
 import os
 application_path = os.path.dirname(__file__)
 sys.path.append(os.path.realpath(application_path+'\\..\\MacroQueue\\'))
-from MacroQueue import *
+from MacroQueue import MacroQueue
 
 class MainFrame_test(unittest.TestCase):
     def test_GUI(self):
         app = wx.App() 
         MyMainFrame = MacroQueue(test=True)
         MyMainFrame.CheckQueue(event=None)
         MyMainFrame.IdleLoop(event=None)
```

### Comparing `MacroQueue-0.2.4/test/test_STMthread.py` & `MacroQueue-0.3.0/test/test_STMthread.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 
 class STMThread_test(unittest.TestCase):
     def test_thread(self):
         mp.freeze_support()
         self.app = wx.App() 
         self.MyMainFrame = MacroQueue(test=True)
-        TestMacro = [ [{'Name':"test","Parameters":[]},False] ]
+        TestMacro = [ [{'Name':"Print","Parameters":{"Number":5}},True] ]
         self.MyMainFrame.IncomingQueue.put(("StartFunction",TestMacro))
         Message = self.MyMainFrame.OutgoingQueue.get()
+        self.assertEqual(f"{Message}","('SetStatus', ('Function: Print', 1))")
+        Message = self.MyMainFrame.OutgoingQueue.get()
         self.assertEqual(f"{Message}","('FunctionFinished', None)")
         self.MyMainFrame.OnClose()
 
         pass
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `MacroQueue-0.2.4/test/test_readdata.py` & `MacroQueue-0.3.0/test/test_readdata.py`

 * *Files identical despite different names*

