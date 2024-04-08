# Comparing `tmp/TSMasterAPI-2.3.3.tar.gz` & `tmp/TSMasterAPI-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.3.3.tar", last modified: Fri Mar 29 08:56:38 2024, max compression
+gzip compressed data, was "TSMasterAPI-2.3.4.tar", last modified: Mon Apr  8 07:04:19 2024, max compression
```

## Comparing `TSMasterAPI-2.3.3.tar` & `TSMasterAPI-2.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 08:56:38.118583 TSMasterAPI-2.3.3/
--rw-rw-rw-   0        0        0     1048 2024-03-29 08:56:38.117555 TSMasterAPI-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.3.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-29 08:56:38.099057 TSMasterAPI-2.3.3/TSMasterAPI/
--rw-rw-rw-   0        0        0   156886 2024-03-27 14:19:32.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSAPI.py
--rw-rw-rw-   0        0        0     5911 2024-03-27 14:19:32.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSCallback.py
--rw-rw-rw-   0        0        0     1373 2024-03-27 14:19:32.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0    10672 2024-03-27 14:19:32.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSEnum.py
--rw-rw-rw-   0        0        0    24356 2024-01-28 12:49:52.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSFibex_parse.py
--rw-rw-rw-   0        0        0   121282 2024-03-27 14:19:32.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    30819 2024-03-27 14:19:32.000000 TSMasterAPI-2.3.3/TSMasterAPI/TSStruct.py
--rw-rw-rw-   0        0        0       20 2024-03-11 02:15:54.000000 TSMasterAPI-2.3.3/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 08:56:38.115011 TSMasterAPI-2.3.3/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1048 2024-03-29 08:56:38.000000 TSMasterAPI-2.3.3/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-03-29 08:56:38.000000 TSMasterAPI-2.3.3/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 08:56:38.000000 TSMasterAPI-2.3.3/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-29 08:56:38.000000 TSMasterAPI-2.3.3/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.3.3/license.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 08:56:38.119100 TSMasterAPI-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1415 2024-03-29 08:56:35.000000 TSMasterAPI-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:04:19.128554 TSMasterAPI-2.3.4/
+-rw-rw-rw-   0        0        0     1048 2024-04-08 07:04:19.127524 TSMasterAPI-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.3.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 07:04:19.099397 TSMasterAPI-2.3.4/TSMasterAPI/
+-rw-rw-rw-   0        0        0   159436 2024-04-04 04:16:38.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSAPI.py
+-rw-rw-rw-   0        0        0     6329 2024-04-04 04:16:38.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSCallback.py
+-rw-rw-rw-   0        0        0     1373 2024-04-04 04:16:38.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0    10672 2024-04-04 04:16:38.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSEnum.py
+-rw-rw-rw-   0        0        0    24356 2024-01-28 11:49:52.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0   121282 2024-04-04 04:16:38.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    31142 2024-04-04 04:16:38.000000 TSMasterAPI-2.3.4/TSMasterAPI/TSStruct.py
+-rw-rw-rw-   0        0        0       20 2024-03-11 02:15:54.000000 TSMasterAPI-2.3.4/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:04:19.123266 TSMasterAPI-2.3.4/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1048 2024-04-08 07:04:18.000000 TSMasterAPI-2.3.4/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-08 07:04:18.000000 TSMasterAPI-2.3.4/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 07:04:18.000000 TSMasterAPI-2.3.4/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 07:04:18.000000 TSMasterAPI-2.3.4/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.3.4/license.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 07:04:19.128554 TSMasterAPI-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1415 2024-04-08 07:03:48.000000 TSMasterAPI-2.3.4/setup.py
```

### Comparing `TSMasterAPI-2.3.3/PKG-INFO` & `TSMasterAPI-2.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.3.3
+Version: 2.3.4
 Summary: Use TSMaster hardware
 Home-page: UNKNOWN
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
```

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSAPI.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -2760,14 +2760,19 @@
 #arg[1] mac
 #arg[2] ipaddr
 tssocket_remove_device_ex = dll.tssocket_remove_device_ex
 tssocket_remove_device_ex.restype = s32
 tssocket_remove_device_ex.argtypes = [s32,pchar,pchar]
 
 #arg[0] ANetworkIndex
+tssocket_get_errno = dll.tssocket_get_errno
+tssocket_get_errno.restype = s32
+tssocket_get_errno.argtypes = [s32]
+
+#arg[0] ANetworkIndex
 tssocket_dhcp_start = dll.tssocket_dhcp_start
 tssocket_dhcp_start.restype = s32
 tssocket_dhcp_start.argtypes = [s32]
 
 #arg[0] ANetworkIndex
 #arg[1] maxfdp1
 #arg[2] readset
@@ -3182,14 +3187,31 @@
 #arg[0] s
 tssocket_unregister_udp_receivefrom_eventsv2 = dll.tssocket_unregister_udp_receivefrom_eventsv2
 tssocket_unregister_udp_receivefrom_eventsv2.restype = s32
 tssocket_unregister_udp_receivefrom_eventsv2.argtypes = [s32]
 
 #arg[0] s
 #arg[1] AEvent
+tssocket_register_udp_receivefrom_eventv3 = dll.tssocket_register_udp_receivefrom_eventv3
+tssocket_register_udp_receivefrom_eventv3.restype = s32
+tssocket_register_udp_receivefrom_eventv3.argtypes = [s32,TSSocketReceiveEventV3_Win32]
+
+#arg[0] s
+#arg[1] AEvent
+tssocket_unregister_udp_receivefrom_eventv3 = dll.tssocket_unregister_udp_receivefrom_eventv3
+tssocket_unregister_udp_receivefrom_eventv3.restype = s32
+tssocket_unregister_udp_receivefrom_eventv3.argtypes = [s32,TSSocketReceiveEventV3_Win32]
+
+#arg[0] s
+tssocket_unregister_udp_receivefrom_eventsv3 = dll.tssocket_unregister_udp_receivefrom_eventsv3
+tssocket_unregister_udp_receivefrom_eventsv3.restype = s32
+tssocket_unregister_udp_receivefrom_eventsv3.argtypes = [s32]
+
+#arg[0] s
+#arg[1] AEvent
 tssocket_register_tcp_receive_eventv2 = dll.tssocket_register_tcp_receive_eventv2
 tssocket_register_tcp_receive_eventv2.restype = s32
 tssocket_register_tcp_receive_eventv2.argtypes = [s32,TSSocketReceiveEventV2_Win32]
 
 #arg[0] s
 #arg[1] AEvent
 tssocket_unregister_tcp_receive_eventv2 = dll.tssocket_unregister_tcp_receive_eventv2
@@ -4692,7 +4714,53 @@
 rpc_client_receive_sync.argtypes = [size_t,psize_t,pu8,s32]
 
 #arg[0] AMasked
 mask_fpu_exceptions = dll.mask_fpu_exceptions
 mask_fpu_exceptions.restype = s32
 mask_fpu_exceptions.argtypes = [cbool]
 
+#arg[0] AActivate
+rpc_tsmaster_activate_server = dll.rpc_tsmaster_activate_server
+rpc_tsmaster_activate_server.restype = s32
+rpc_tsmaster_activate_server.argtypes = [cbool]
+
+#arg[0] ATSMasterAppName
+#arg[1] AHandle
+rpc_tsmaster_create_client = dll.rpc_tsmaster_create_client
+rpc_tsmaster_create_client.restype = s32
+rpc_tsmaster_create_client.argtypes = [pchar,psize_t]
+
+#arg[0] AHandle
+#arg[1] AActivate
+rpc_tsmaster_activate_client = dll.rpc_tsmaster_activate_client
+rpc_tsmaster_activate_client.restype = s32
+rpc_tsmaster_activate_client.argtypes = [size_t,cbool]
+
+#arg[0] AHandle
+rpc_tsmaster_delete_client = dll.rpc_tsmaster_delete_client
+rpc_tsmaster_delete_client.restype = s32
+rpc_tsmaster_delete_client.argtypes = [size_t]
+
+#arg[0] AHandle
+rpc_tsmaster_cmd_start_simulation = dll.rpc_tsmaster_cmd_start_simulation
+rpc_tsmaster_cmd_start_simulation.restype = s32
+rpc_tsmaster_cmd_start_simulation.argtypes = [size_t]
+
+#arg[0] AHandle
+rpc_tsmaster_cmd_stop_simulation = dll.rpc_tsmaster_cmd_stop_simulation
+rpc_tsmaster_cmd_stop_simulation.restype = s32
+rpc_tsmaster_cmd_stop_simulation.argtypes = [size_t]
+
+#arg[0] AHandle
+#arg[1] ACompleteName
+#arg[2] AValue
+rpc_tsmaster_cmd_write_system_var = dll.rpc_tsmaster_cmd_write_system_var
+rpc_tsmaster_cmd_write_system_var.restype = s32
+rpc_tsmaster_cmd_write_system_var.argtypes = [size_t,pchar,pchar]
+
+#arg[0] AHandle
+#arg[1] AAddr
+#arg[2] ASizeBytes
+rpc_tsmaster_cmd_transfer_memory = dll.rpc_tsmaster_cmd_transfer_memory
+rpc_tsmaster_cmd_transfer_memory.restype = s32
+rpc_tsmaster_cmd_transfer_memory.argtypes = [size_t,pu8,size_t]
+
```

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSCallback.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSCallback.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,22 @@
 # Arg[3] ARemoteEndPoint
 # Arg[4] AData
 # Arg[5] ASize
 TSSocketReceiveEventV2 = WINFUNCTYPE(None,ps32,s32,s32,pchar,pu8,s32)
 # Arg[0] AObj
 # Arg[1] ASocket
 # Arg[2] AResult
+# Arg[3] ADstEndPoint
+# Arg[4] ASrcEndPoint
+# Arg[5] AData
+# Arg[6] ASize
+TSSocketReceiveEventV3 = WINFUNCTYPE(None,ps32,s32,s32,pchar,pchar,pu8,s32)
+# Arg[0] AObj
+# Arg[1] ASocket
+# Arg[2] AResult
 # Arg[3] AData
 # Arg[4] ASize
 TSSocketTransmitEvent = WINFUNCTYPE(None,ps32,s32,s32,pu8,s32)
 # Arg[0] AObj
 # Arg[1] ASocket
 # Arg[2] AClientSocket
 # Arg[3] AResult
@@ -117,14 +125,22 @@
 # Arg[3] ARemoteEndPoint
 # Arg[4] AData
 # Arg[5] ASize
 TSSocketReceiveEventV2_Win32 = WINFUNCTYPE(None,ps32,s32,s32,pchar,pu8,s32)
 # Arg[0] AObj
 # Arg[1] ASocket
 # Arg[2] AResult
+# Arg[3] ADstEndPoint
+# Arg[4] ASrcEndPoint
+# Arg[5] AData
+# Arg[6] ASize
+TSSocketReceiveEventV3_Win32 = WINFUNCTYPE(None,ps32,s32,s32,pchar,pchar,pu8,s32)
+# Arg[0] AObj
+# Arg[1] ASocket
+# Arg[2] AResult
 # Arg[3] AData
 # Arg[4] ASize
 TSSocketTransmitEvent_Win32 = WINFUNCTYPE(None,ps32,s32,s32,pu8,s32)
 # Arg[0] AObj
 # Arg[1] AProgress100
 TReadProgressCallback = WINFUNCTYPE(None,ps32,double)
 # Arg[0] AObj
```

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSEnum.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSEnum.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSFibex_parse.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSFibex_parse.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI/TSStruct.py` & `TSMasterAPI-2.3.4/TSMasterAPI/TSStruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,14 +882,29 @@
 ('msg_iovlen',s32),
 ('msg_control',ps32),
 ('msg_controllen',u32),
 ('msg_flags',s32),
 ]
 Pts_msghdr = POINTER(Tts_msghdr)
 
+class Tts_cmsghdr(Structure):
+    _pack_ = 1
+    _fields_ =[('cmsg_len',u32),
+('cmsg_level',s32),
+('cmsg_type',s32),
+]
+Pts_cmsghdr = POINTER(Tts_cmsghdr)
+
+class Tts_in_pktinfo(Structure):
+    _pack_ = 1
+    _fields_ =[('ipi_ifindex',u32),
+('ipi_addr',Ts_in_addr),
+]
+Pts_in_pktinfo = POINTER(Tts_in_pktinfo)
+
 class Tts_pollfd(Structure):
     _pack_ = 1
     _fields_ =[('fd',s32),
 ('events',s16),
 ('revents',s16),
 ]
 Pts_pollfd = POINTER(Tts_pollfd)
```

### Comparing `TSMasterAPI-2.3.3/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.3.4/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.3.3
+Version: 2.3.4
 Summary: Use TSMaster hardware
 Home-page: UNKNOWN
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
```

### Comparing `TSMasterAPI-2.3.3/license.txt` & `TSMasterAPI-2.3.4/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.3.3/setup.py` & `TSMasterAPI-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.3.3',  # 版本号
+      version='2.3.4',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

