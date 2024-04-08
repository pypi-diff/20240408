# Comparing `tmp/ampapi-1.3.8.tar.gz` & `tmp/ampapi-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.3.8.tar", last modified: Mon Jan  8 01:37:05 2024, max compression
+gzip compressed data, was "ampapi-1.3.9.tar", last modified: Thu Feb  8 23:51:44 2024, max compression
```

## Comparing `ampapi-1.3.8.tar` & `ampapi-1.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-01-08 01:37:05.979270 ampapi-1.3.8/
--rwxrwxr-x   0 dylan     (1000) dylan     (1000)    35149 2023-11-23 22:20:37.000000 ampapi-1.3.8/LICENSE
--rwxrwxr-x   0 dylan     (1000) dylan     (1000)     1070 2023-11-23 22:20:37.000000 ampapi-1.3.8/LICENSE-API
--rw-r--r--   0 dylan     (1000) dylan     (1000)     6229 2024-01-08 01:37:05.979270 ampapi-1.3.8/PKG-INFO
--rwxrwxr-x   0 dylan     (1000) dylan     (1000)     5666 2024-01-06 01:31:09.000000 ampapi-1.3.8/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-01-08 01:37:05.971269 ampapi-1.3.8/ampapi/
--rwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-11-23 22:20:37.000000 ampapi-1.3.8/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     5519 2024-01-06 04:16:44.000000 ampapi-1.3.8/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-01-08 01:37:05.975269 ampapi-1.3.8/ampapi/apimodules/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    60174 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/ADSModule.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    65874 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/Core.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1091 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/EmailSenderPlugin.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    16942 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/FileManagerPlugin.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1205 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/GenericModule.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     7086 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/LocalFileBackupPlugin.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    16373 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/MinecraftModule.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1081 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/RCONPlugin.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-11-23 22:20:37.000000 ampapi-1.3.8/ampapi/apimodules/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2877 2024-01-08 01:36:55.000000 ampapi-1.3.8/ampapi/apimodules/steamcmdplugin.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-01-08 01:37:05.979270 ampapi-1.3.8/ampapi/modules/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     5121 2024-01-06 01:31:25.000000 ampapi-1.3.8/ampapi/modules/ADS.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2865 2024-01-06 01:27:34.000000 ampapi-1.3.8/ampapi/modules/CommonAPI.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2477 2024-01-06 05:44:06.000000 ampapi-1.3.8/ampapi/modules/GenericModule.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1752 2023-11-23 22:20:37.000000 ampapi-1.3.8/ampapi/modules/Minecraft.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-11-23 22:20:37.000000 ampapi-1.3.8/ampapi/modules/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    32044 2024-01-08 01:35:42.000000 ampapi-1.3.8/ampapi/types.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-01-08 01:37:05.979270 ampapi-1.3.8/ampapi.egg-info/
--rw-r--r--   0 dylan     (1000) dylan     (1000)     6229 2024-01-08 01:37:05.000000 ampapi-1.3.8/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      711 2024-01-08 01:37:05.000000 ampapi-1.3.8/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2024-01-08 01:37:05.000000 ampapi-1.3.8/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2024-01-08 01:37:05.000000 ampapi-1.3.8/ampapi.egg-info/top_level.txt
--rwxrwxr-x   0 dylan     (1000) dylan     (1000)      111 2023-11-23 22:20:37.000000 ampapi-1.3.8/pyproject.toml
--rwxrwxr-x   0 dylan     (1000) dylan     (1000)      626 2024-01-08 01:37:05.979270 ampapi-1.3.8/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-02-08 23:51:44.125724 ampapi-1.3.9/
+-rwxrwxr-x   0 dylan     (1000) dylan     (1000)    35149 2023-11-23 22:20:37.000000 ampapi-1.3.9/LICENSE
+-rwxrwxr-x   0 dylan     (1000) dylan     (1000)     1070 2023-11-23 22:20:37.000000 ampapi-1.3.9/LICENSE-API
+-rw-r--r--   0 dylan     (1000) dylan     (1000)     6229 2024-02-08 23:51:44.125724 ampapi-1.3.9/PKG-INFO
+-rwxrwxr-x   0 dylan     (1000) dylan     (1000)     5666 2024-01-06 01:31:09.000000 ampapi-1.3.9/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-02-08 23:51:44.121724 ampapi-1.3.9/ampapi/
+-rwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-11-23 22:20:37.000000 ampapi-1.3.9/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     5519 2024-01-06 04:16:44.000000 ampapi-1.3.9/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-02-08 23:51:44.121724 ampapi-1.3.9/ampapi/apimodules/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    60174 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/ADSModule.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    65874 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/Core.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1091 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/EmailSenderPlugin.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    16942 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/FileManagerPlugin.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1205 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/GenericModule.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     7086 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/LocalFileBackupPlugin.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    16373 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/MinecraftModule.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1081 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/RCONPlugin.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-11-23 22:20:37.000000 ampapi-1.3.9/ampapi/apimodules/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     2877 2024-02-08 23:51:33.000000 ampapi-1.3.9/ampapi/apimodules/steamcmdplugin.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-02-08 23:51:44.125724 ampapi-1.3.9/ampapi/modules/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     5121 2024-01-06 01:31:25.000000 ampapi-1.3.9/ampapi/modules/ADS.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     2865 2024-01-06 01:27:34.000000 ampapi-1.3.9/ampapi/modules/CommonAPI.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     2477 2024-01-06 05:44:06.000000 ampapi-1.3.9/ampapi/modules/GenericModule.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1752 2023-11-23 22:20:37.000000 ampapi-1.3.9/ampapi/modules/Minecraft.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-11-23 22:20:37.000000 ampapi-1.3.9/ampapi/modules/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    35271 2024-02-08 23:44:22.000000 ampapi-1.3.9/ampapi/types.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2024-02-08 23:51:44.125724 ampapi-1.3.9/ampapi.egg-info/
+-rw-r--r--   0 dylan     (1000) dylan     (1000)     6229 2024-02-08 23:51:44.000000 ampapi-1.3.9/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      711 2024-02-08 23:51:44.000000 ampapi-1.3.9/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2024-02-08 23:51:44.000000 ampapi-1.3.9/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2024-02-08 23:51:44.000000 ampapi-1.3.9/ampapi.egg-info/top_level.txt
+-rwxrwxr-x   0 dylan     (1000) dylan     (1000)      111 2023-11-23 22:20:37.000000 ampapi-1.3.9/pyproject.toml
+-rwxrwxr-x   0 dylan     (1000) dylan     (1000)      626 2024-02-08 23:51:44.125724 ampapi-1.3.9/setup.cfg
```

### Comparing `ampapi-1.3.8/LICENSE` & `ampapi-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/LICENSE-API` & `ampapi-1.3.9/LICENSE-API`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/PKG-INFO` & `ampapi-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.3.8
+Version: 1.3.9
 Summary: An API that allows you to communicate with AMP installations from within Python.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-py
 Author: Dylan Sperrer - p0t4t0sandwich - thepotatoking3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.3.8/README.md` & `ampapi-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/ampapi.py` & `ampapi-1.3.9/ampapi/ampapi.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/ADSModule.py` & `ampapi-1.3.9/ampapi/apimodules/ADSModule.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/Core.py` & `ampapi-1.3.9/ampapi/apimodules/Core.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/EmailSenderPlugin.py` & `ampapi-1.3.9/ampapi/apimodules/EmailSenderPlugin.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/FileManagerPlugin.py` & `ampapi-1.3.9/ampapi/apimodules/FileManagerPlugin.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/GenericModule.py` & `ampapi-1.3.9/ampapi/apimodules/GenericModule.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/LocalFileBackupPlugin.py` & `ampapi-1.3.9/ampapi/apimodules/LocalFileBackupPlugin.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/MinecraftModule.py` & `ampapi-1.3.9/ampapi/apimodules/MinecraftModule.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/RCONPlugin.py` & `ampapi-1.3.9/ampapi/apimodules/RCONPlugin.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/apimodules/steamcmdplugin.py` & `ampapi-1.3.9/ampapi/apimodules/steamcmdplugin.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/modules/ADS.py` & `ampapi-1.3.9/ampapi/modules/ADS.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/modules/CommonAPI.py` & `ampapi-1.3.9/ampapi/modules/CommonAPI.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/modules/GenericModule.py` & `ampapi-1.3.9/ampapi/modules/GenericModule.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/modules/Minecraft.py` & `ampapi-1.3.9/ampapi/modules/Minecraft.py`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/ampapi/types.py` & `ampapi-1.3.9/ampapi/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -381,15 +381,15 @@
     ContainerCPUs: int
     SpecificDockerImage: str
     Metrics: dict[str, Metric]
     ApplicationEndpoints: list[EndpointInfo]
     DeploymentArgs: dict[str, str]
     DisplayImageSource: str
 
-    def __init__(self, InstanceID: UUID, TargetID: UUID, InstanceName: str, FriendlyName: str, Module: str, AMPVersion: AMPVersionAlias, IsHTTPS: bool, IP: str, Port: int, Daemon: bool, DaemonAutostart: bool, ExcludeFromFirewall: bool, Running: bool, AppState: State, Tags: list[str], DiskUsageMB: int, ReleaseStream: str, ManagementMode: str, Suspended: bool, IsContainerInstance: bool, ContainerMemoryMB: int, ContainerMemoryPolicy: str, ContainerCPUs: int, Metrics: dict[str, Metric], ApplicationEndpoints: list[EndpointInfo], DeploymentArgs: dict[str, str], DisplayImageSource: str = "", Description: str = "", ModuleDisplayName: str = "", SpecificDockerImage: str = "") -> None:
+    def __init__(self, InstanceID: UUID, TargetID: UUID, InstanceName: str, FriendlyName: str, Module: str, AMPVersion: AMPVersionAlias, IsHTTPS: bool, IP: str, Port: int, Daemon: bool, DaemonAutostart: bool, ExcludeFromFirewall: bool, Running: bool, AppState: State, Tags: list[str], DiskUsageMB: int, ReleaseStream: str, ManagementMode: str, Suspended: bool, IsContainerInstance: bool, ContainerMemoryMB: int, ContainerMemoryPolicy: str, ContainerCPUs: int, ApplicationEndpoints: list[EndpointInfo], DeploymentArgs: dict[str, str], Metrics: dict[str, Metric] = {}, DisplayImageSource: str = "", Description: str = "", ModuleDisplayName: str = "", SpecificDockerImage: str = "") -> None:
         """
         Initializes the Instance object
         Author: p0t4t0sandwich
         """
         self.InstanceID = InstanceID
         self.TargetID = TargetID
         self.InstanceName = InstanceName
@@ -416,68 +416,165 @@
         self.ContainerMemoryPolicy = ContainerMemoryPolicy
         self.ContainerCPUs = ContainerCPUs
         self.Metrics = {i : Metric(**Metrics[i]) for i in Metrics}
         self.ApplicationEndpoints = [EndpointInfo(**ApplicationEndpoints[i]) for i in range(len(ApplicationEndpoints))]
         self.DeploymentArgs = DeploymentArgs
         self.DisplayImageSource = DisplayImageSource
 
+class GlibcInfo():
+    """
+    Glibc information object
+    Author: Kei
+    """
+    Major : int
+    Minor : int
+    Build : int
+    Revision : int
+    MajorRevision : int
+    MinorRevision : int
+
+    def __init__(self, Major: int, Minor: int, Build: int, Revision: int, MajorRevision: int, MinorRevision: int) -> None:
+        """
+        Initializes the GlibcInfo object
+        Author: Kei
+        """
+        self.Major = Major
+        self.Minor = Minor
+        self.Build = Build
+        self.Revision = Revision
+        self.MajorRevision = MajorRevision
+        self.MinorRevision = MinorRevision
+
+# Type alias for State
+# Author: Kei
+GlibcInfoAlias = GlibcInfo
+
 class PlatformInfo():
     """
     Platform information object
     Author: p0t4t0sandwich
+    :param IsSharedSetup: If the setup is shared
+    :type IsSharedSetup: bool
+    :param AdminRights: Admin right status
+    :type AdminRights: int
     :param CPUInfo: The CPU information object
     :type CPUInfo: CPUInfo
     :param InstalledRAMMB: The installed RAM in MB
     :type InstalledRAMMB: int
     :param OS: The OS
     :type OS: int
     :param PlatformName: The platform name
     :type PlatformName: str
+    :param HardwarePlatformName: The hardware platform name
+    :type HardwarePlatformName: str
     :param SystemType: The system type
     :type SystemType: int
     :param Virtualization: The virtualization
     :type Virtualization: int
+    :param InstalledGlibcVersion: Version of Glibc installed
+    :type InstalledGlibcVersion: GlibcInfo
     """
+    IsSharedSetup: bool
+    AdminRights: int
     CPUInfo: CPUInfoAlias
     InstalledRAMMB: int
     OS: int
     PlatformName: str
+    HardwarePlatformName: str
     SystemType: int
     Virtualization: int
+    InstalledGlibcVersion: GlibcInfo
 
-    def __init__(self, CPUInfo: CPUInfoAlias, InstalledRAMMB: int, OS: int, PlatformName: str, SystemType: int, Virtualization: int) -> None:
+    def __init__(self, IsSharedSetup : bool, AdminRights : int, CPUInfo: CPUInfoAlias, InstalledRAMMB: int, OS: int, PlatformName: str, HardwarePlatformName : str, SystemType: int, Virtualization: int, InstalledGlibcVersion : GlibcInfoAlias) -> None:
         """
         Initializes the PlatformInfo object
         Author: p0t4t0sandwich
         """
+        self.IsSharedSetup = IsSharedSetup
+        self.AdminRights = AdminRights
         self.CPUInfo = CPUInfoAlias(**CPUInfo)
         self.InstalledRAMMB = InstalledRAMMB
         self.OS = OS
         self.PlatformName = PlatformName
+        self.HardwarePlatformName = HardwarePlatformName
         self.SystemType = SystemType
         self.Virtualization = Virtualization
+        self.InstalledGlibcVersion = GlibcInfoAlias(**InstalledGlibcVersion)
 
 # Type alias for PlatformInfo
 # Author: p0t4t0sandwich
 PlatformInfoAlias = PlatformInfo
 
+class FitnessInfo():
+    """
+    Fitness information object
+    Author: Kei
+    :param Available: Availability
+    :type Available: bool
+    :param TotalServices: Service count.
+    :type TotalServices: int
+    :param FreeRAMMB: Unallocated RAM in MB.
+    :type FreeRAMMB: int
+    :param FreeDiskMB: Unallocated disk space in MB.
+    :type FreeDiskMB: int
+    :param CPUServiceRatio: CPU service ratio.
+    :type CPUServiceRatio: float
+    :param ThreadQueueLength: Thread queue length.
+    :type ThreadQueueLength: int
+    :param LoadAvg: Load average.
+    :type LoadAvg: float
+    :param ReminaingInstanceSlots: Remaining instance slots.
+    :type ReminaingInstanceSlots: int
+    :param Score: Fitness score.
+    :type Score: float
+    """
+    Available: bool
+    TotalServices: int
+    FreeRAMMB: int
+    FreeDiskMB: int
+    CPUServiceRatio: float
+    ThreadQueueLength: int
+    LoadAvg: float
+    ReminaingInstanceSlots: int
+    Score: float
+
+    def __init__(self, Available: bool, TotalServices: int, FreeRAMMB: int, FreeDiskMB: int, CPUServiceRatio: float, ThreadQueueLength: int, LoadAvg: float, ReminaingInstanceSlots: int, Score: float) -> None:
+        """
+        Initializes the FitnessInfo object
+        """
+        self.Available = Available
+        self.TotalServices = TotalServices
+        self.FreeRAMMB = FreeRAMMB
+        self.FreeDiskMB = FreeDiskMB
+        self.CPUServiceRatio = CPUServiceRatio
+        self.ThreadQueueLength = ThreadQueueLength
+        self.LoadAvg = LoadAvg
+        self.ReminaingInstanceSlots = ReminaingInstanceSlots
+        self.Score = Score
+
+# Type alias for FitnessInfo
+# Author: Kei        
+FitnessInfoAlias = FitnessInfo
+
 class IADSInstance():
     """
     An ADS instance object
     Author: p0t4t0sandwich
     :param Id: The ADS instance ID
     :type Id: int
     :param InstanceId: The instance ID
     :type InstanceId: UUID
     :param FriendlyName: The friendly name
     :type FriendlyName: str
     :param Description: The description
     :type Description: str
     :param Disabled: Whether the instance is disabled
     :type Disabled: bool
+    :param Fitness: Fitness of the instance.
+    :type Fitness: FitnessInfo
     :param IsRemote: Whether the instance is remote
     :type IsRemote: bool
     :param Platform: The platform information object
     :type PlatformInfo: Platform
     :param Datastores: The datastores
     :type Datastores: list[InstanceDatastore]
     :param CreatesInContainers: Whether the instance creates in containers
@@ -496,53 +593,51 @@
     :type AvailableIPs: list[str]
     """
     Id: int
     InstanceId: UUID
     FriendlyName: str
     Description: str
     Disabled: bool
+    Fitness: FitnessInfo
     IsRemote: bool
     Platform: PlatformInfo
     Datastores: list[InstanceDatastore]
     CreatesInContainers: bool
-    State: State
+    State: StateAlias
     StateReason: str
     CanCreate: bool
     LastUpdated: str
     AvailableInstances: list[Instance]
     AvailableIPs: list[str]
     Tags: list[str]
     TagsList: list[str]
     URL: str
 
-    def __init__(self, Id: int, InstanceId: UUID, FriendlyName: str, Disabled: bool, IsRemote: bool, Datastores: list[InstanceDatastore], CreatesInContainers: bool, State: StateAlias, StateReason: str, CanCreate: bool, LastUpdated: str, AvailableInstances: list[Instance], AvailableIPs: list[str], Platform: PlatformInfo = None, Description: str = "", Tags: list[str] = [], TagsList: list[str] = [], URL: str = "") -> None:
+    def __init__(self, Id: int, InstanceId: UUID, FriendlyName: str, Disabled: bool, Fitness:FitnessInfo, IsRemote: bool, Datastores: list[InstanceDatastore], CreatesInContainers: bool, State: StateAlias, CanCreate: bool, LastUpdated: str, AvailableInstances: list[Instance], AvailableIPs: list[str], Platform: PlatformInfo = None, Description: str = "", Tags: list[str] = [], TagsList: list[str] = [], URL: str = "", StateReason: str = "") -> None:
         """
         Initializes the IADSInstance object
         Author: p0t4t0sandwich
         """
         self.Id = Id
         self.InstanceId = InstanceId
         self.FriendlyName = FriendlyName
         self.Description = Description
         self.Disabled = Disabled
+        self.Fitness = Fitness
         self.IsRemote = IsRemote
         if Platform != None:
             self.Platform = PlatformInfo(**Platform)
         else:
             self.Platform = Platform
         self.Datastores = [InstanceDatastore(**Datastores[i]) for i in range(len(Datastores))]
         self.CreatesInContainers = CreatesInContainers
         self.State = State
         self.StateReason = StateReason
         self.CanCreate = CanCreate
         self.LastUpdated = LastUpdated
-
-        # for i in AvailableInstances:
-        #     print(i.keys())
-
         self.AvailableInstances = [Instance(**AvailableInstances[i]) for i in range(len(AvailableInstances))]
         self.AvailableIPs = AvailableIPs
         self.URL = URL
 
 class UserInfo():
     """
     Information about the user
```

### Comparing `ampapi-1.3.8/ampapi.egg-info/PKG-INFO` & `ampapi-1.3.9/ampapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.3.8
+Version: 1.3.9
 Summary: An API that allows you to communicate with AMP installations from within Python.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-py
 Author: Dylan Sperrer - p0t4t0sandwich - thepotatoking3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.3.8/ampapi.egg-info/SOURCES.txt` & `ampapi-1.3.9/ampapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampapi-1.3.8/setup.cfg` & `ampapi-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.3.8
+version = 1.3.9
 author = Dylan Sperrer - p0t4t0sandwich - thepotatoking3452
 author_email = p0t4t0sandwich@gmail.com
 description = An API that allows you to communicate with AMP installations from within Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-py
 classifiers =
```

