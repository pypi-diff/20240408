# Comparing `tmp/gattlib-py-0.5.2.tar.gz` & `tmp/gattlib-py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattlib-py-0.5.2.tar", last modified: Thu Apr  4 22:06:43 2024, max compression
+gzip compressed data, was "gattlib-py-0.6.0.tar", last modified: Sun Apr  7 22:52:28 2024, max compression
```

## Comparing `gattlib-py-0.5.2.tar` & `gattlib-py-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:43.713917 gattlib-py-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 22:06:43.713917 gattlib-py-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:43.713917 gattlib-py-0.5.2/gattlib/
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 22:06:43.000000 gattlib-py-0.5.2/gattlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/gatt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/mainloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/gattlib/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:43.713917 gattlib-py-0.5.2/gattlib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 22:06:43.000000 gattlib-py-0.5.2/gattlib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 22:06:43.000000 gattlib-py-0.5.2/gattlib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:06:43.000000 gattlib-py-0.5.2/gattlib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 22:06:43.000000 gattlib-py-0.5.2/gattlib_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 22:06:43.000000 gattlib-py-0.5.2/gattlib_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:06:43.713917 gattlib-py-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-04 21:49:19.000000 gattlib-py-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:52:28.012049 gattlib-py-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-07 22:52:28.008049 gattlib-py-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:52:28.008049 gattlib-py-0.6.0/gattlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 22:52:27.000000 gattlib-py-0.6.0/gattlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/gatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/gattlib/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:52:28.008049 gattlib-py-0.6.0/gattlib_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-07 22:52:28.000000 gattlib-py-0.6.0/gattlib_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 22:52:28.000000 gattlib-py-0.6.0/gattlib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:52:28.000000 gattlib-py-0.6.0/gattlib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 22:52:28.000000 gattlib-py-0.6.0/gattlib_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 22:52:28.000000 gattlib-py-0.6.0/gattlib_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:52:28.012049 gattlib-py-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-07 22:34:30.000000 gattlib-py-0.6.0/setup.py
```

### Comparing `gattlib-py-0.5.2/PKG-INFO` & `gattlib-py-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.5.2/gattlib/__init__.py` & `gattlib-py-0.6.0/gattlib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,29 +100,29 @@
 # } gattlib_advertisement_data_t;
 class GattlibAdvertisementData(Structure):
     _fields_ = [("uuid", GattlibUuid),
                 ("data", c_void_p),
                 ("data_length", c_size_t)]
 
 
-# int gattlib_adapter_open(const char* adapter_name, void** adapter);
+# int gattlib_adapter_open(const char* adapter_name, gattlib_adapter_t** adapter);
 gattlib_adapter_open = gattlib.gattlib_adapter_open
 gattlib_adapter_open.argtypes = [c_char_p, POINTER(c_void_p)]
 
-# const char *gattlib_adapter_get_name(void* adapter)
+# const char *gattlib_adapter_get_name(gattlib_adapter_t* adapter)
 gattlib_adapter_get_name = gattlib.gattlib_adapter_get_name
 gattlib_adapter_get_name.argtypes = [c_void_p]
 gattlib_adapter_get_name.restype = c_char_p
 
-# void gattlib_discovered_device_python_callback(void *adapter, const char* addr, const char* name, void *user_data)
+# void gattlib_discovered_device_python_callback(gattlib_adapter_t* adapter, const char* addr, const char* name, void *user_data)
 gattlib_discovered_device_python_callback = gattlib.gattlib_discovered_device_python_callback
 gattlib_discovered_device_python_callback.argtypes = [c_void_p, c_char_p, c_char_p, py_object]
 gattlib_discovered_device_python_callback.restype = c_void_p
 
-# void gattlib_connected_device_python_callback(void *adapter, const char *dst, gatt_connection_t* connection, int error, void* user_data);
+# void gattlib_connected_device_python_callback(gattlib_adapter_t* adapter, const char *dst, gattlib_connection_t* connection, int error, void* user_data);
 gattlib_connected_device_python_callback = gattlib.gattlib_connected_device_python_callback
 gattlib_connected_device_python_callback.argtypes = [c_void_p, c_char_p, c_void_p, c_int, py_object]
 gattlib_connected_device_python_callback.restype = c_void_p
 
 # void gattlib_disconnected_device_python_callback(void *user_data)
 gattlib_disconnected_device_python_callback = gattlib.gattlib_disconnected_device_python_callback
 gattlib_disconnected_device_python_callback.argtypes = [py_object]
@@ -134,91 +134,91 @@
 gattlib_notification_device_python_callback.restype = c_void_p
 
 # void* gattlib_python_callback_args(PyObject* python_callback, PyObject* python_args) {
 gattlib_python_callback_args = gattlib.gattlib_python_callback_args
 gattlib_python_callback_args.argtypes = [py_object, py_object]
 gattlib_python_callback_args.restype = c_void_p
 
-# int gattlib_adapter_scan_enable_with_filter_non_blocking(void *adapter, uuid_t **uuid_list, int16_t rssi_threshold, uint32_t enabled_filters,
+# int gattlib_adapter_scan_enable_with_filter_non_blocking(gattlib_adapter_t* adapter, uuid_t **uuid_list, int16_t rssi_threshold, uint32_t enabled_filters,
 #        gattlib_discovered_device_t discovered_device_cb, size_t timeout, void *user_data)
 gattlib_adapter_scan_enable_with_filter_non_blocking = gattlib.gattlib_adapter_scan_enable_with_filter_non_blocking
 gattlib_adapter_scan_enable_with_filter_non_blocking.argtypes = [c_void_p, POINTER(POINTER(GattlibUuid)), c_int16, c_uint32, c_void_p, c_size_t, c_void_p]
 
-# int gattlib_adapter_scan_eddystone(void *adapter, int16_t rssi_threshold, uint32_t eddsytone_types,
+# int gattlib_adapter_scan_eddystone(gattlib_adapter_t* adapter, int16_t rssi_threshold, uint32_t eddsytone_types,
 #        gattlib_discovered_device_with_data_t discovered_device_cb, size_t timeout, void *user_data)
 gattlib_adapter_scan_eddystone = gattlib.gattlib_adapter_scan_eddystone
 gattlib_adapter_scan_eddystone.argtypes = [c_void_p, c_int16, c_uint32, py_object, c_size_t, py_object]
 
-# int gattlib_connect(void *adapter, const char *dst, unsigned long options, gatt_connect_cb_t connect_cb, void* user_data)
+# int gattlib_connect(gattlib_adapter_t* adapter, const char *dst, unsigned long options, gatt_connect_cb_t connect_cb, void* user_data)
 gattlib_connect = gattlib.gattlib_connect
 gattlib_connect.argtypes = [c_void_p, c_char_p, c_ulong, c_void_p, c_void_p]
 
-# int gattlib_disconnect(gatt_connection_t* connection, bool wait_disconnection);
+# int gattlib_disconnect(gattlib_connection_t* connection, bool wait_disconnection);
 gattlib_disconnect = gattlib.gattlib_disconnect
 gattlib_disconnect.argtypes = [c_void_p, c_bool]
 
-# int gattlib_discover_primary(gatt_connection_t* connection, gattlib_primary_service_t** services, int* services_count);
+# int gattlib_discover_primary(gattlib_connection_t* connection, gattlib_primary_service_t** services, int* services_count);
 gattlib_discover_primary = gattlib.gattlib_discover_primary
 gattlib_discover_primary.argtypes = [c_void_p, POINTER(POINTER(GattlibPrimaryService)), POINTER(c_int)]
 
-# int gattlib_discover_char(gatt_connection_t* connection, gattlib_characteristic_t** characteristics, int* characteristic_count);
+# int gattlib_discover_char(gattlib_connection_t* connection, gattlib_characteristic_t** characteristics, int* characteristic_count);
 gattlib_discover_char = gattlib.gattlib_discover_char
 gattlib_discover_char.argtypes = [c_void_p, POINTER(POINTER(GattlibCharacteristic)), POINTER(c_int)]
 
-# int gattlib_read_char_by_uuid(gatt_connection_t* connection, uuid_t* uuid, void** buffer, size_t* buffer_len);
+# int gattlib_read_char_by_uuid(gattlib_connection_t* connection, uuid_t* uuid, void** buffer, size_t* buffer_len);
 gattlib_read_char_by_uuid = gattlib.gattlib_read_char_by_uuid
 gattlib_read_char_by_uuid.argtypes = [c_void_p, POINTER(GattlibUuid), POINTER(c_void_p), POINTER(c_size_t)]
 
 # void gattlib_characteristic_free_value(void* buffer);
 gattlib_characteristic_free_value = gattlib.gattlib_characteristic_free_value
 gattlib_characteristic_free_value.argtypes = [c_void_p]
 
-# int gattlib_write_char_by_uuid(gatt_connection_t* connection, uuid_t* uuid, const void* buffer, size_t buffer_len)
+# int gattlib_write_char_by_uuid(gattlib_connection_t* connection, uuid_t* uuid, const void* buffer, size_t buffer_len)
 gattlib_write_char_by_uuid = gattlib.gattlib_write_char_by_uuid
 gattlib_write_char_by_uuid.argtypes = [c_void_p, POINTER(GattlibUuid), c_void_p, c_size_t]
 
-# int gattlib_write_without_response_char_by_uuid(gatt_connection_t* connection, uuid_t* uuid, const void* buffer, size_t buffer_len)
+# int gattlib_write_without_response_char_by_uuid(gattlib_connection_t* connection, uuid_t* uuid, const void* buffer, size_t buffer_len)
 gattlib_write_without_response_char_by_uuid = gattlib.gattlib_write_without_response_char_by_uuid
 gattlib_write_without_response_char_by_uuid.argtypes = [c_void_p, POINTER(GattlibUuid), c_void_p, c_size_t]
 
-# int gattlib_write_char_by_uuid_stream_open(gatt_connection_t* connection, uuid_t* uuid, gatt_stream_t **stream, uint16_t *mtu)
+# int gattlib_write_char_by_uuid_stream_open(gattlib_connection_t* connection, uuid_t* uuid, gattlib_stream_t **stream, uint16_t *mtu)
 gattlib_write_char_by_uuid_stream_open = gattlib.gattlib_write_char_by_uuid_stream_open
 gattlib_write_char_by_uuid_stream_open.argtypes = [c_void_p, POINTER(GattlibUuid), POINTER(c_void_p), POINTER(c_uint16)]
 
-# int gattlib_notification_start(gatt_connection_t* connection, const uuid_t* uuid);
+# int gattlib_notification_start(gattlib_connection_t* connection, const uuid_t* uuid);
 gattlib_notification_start = gattlib.gattlib_notification_start
 gattlib_notification_start.argtypes = [c_void_p, POINTER(GattlibUuid)]
 
-# int gattlib_notification_stop(gatt_connection_t* connection, const uuid_t* uuid);
+# int gattlib_notification_stop(gattlib_connection_t* connection, const uuid_t* uuid);
 gattlib_notification_stop = gattlib.gattlib_notification_stop
 gattlib_notification_stop.argtypes = [c_void_p, POINTER(GattlibUuid)]
 
-# int gattlib_register_notification(gatt_connection_t* connection, gattlib_event_handler_t notification_handler, void* user_data);
+# int gattlib_register_notification(gattlib_connection_t* connection, gattlib_event_handler_t notification_handler, void* user_data);
 gattlib_register_notification = gattlib.gattlib_register_notification
 gattlib_register_notification.argtypes = [c_void_p, c_void_p, c_void_p]
 
-# int gattlib_register_on_disconnect(gatt_connection_t *connection, PyObject *handler, PyObject *user_data)
+# int gattlib_register_on_disconnect(gattlib_connection_t *connection, PyObject *handler, PyObject *user_data)
 gattlib_register_on_disconnect = gattlib.gattlib_register_on_disconnect
 gattlib_register_on_disconnect.argtypes = [c_void_p, c_void_p, c_void_p]
 
-# int gattlib_get_rssi(gatt_connection_t *connection, int16_t *rssi)
+# int gattlib_get_rssi(gattlib_connection_t *connection, int16_t *rssi)
 gattlib_get_rssi = gattlib.gattlib_get_rssi
 gattlib_get_rssi.argtypes = [c_void_p, POINTER(c_int16)]
 
-# int gattlib_get_rssi_from_mac(void *adapter, const char *mac_address, int16_t *rssi)
+# int gattlib_get_rssi_from_mac(gattlib_adapter_t* adapter, const char *mac_address, int16_t *rssi)
 gattlib_get_rssi_from_mac = gattlib.gattlib_get_rssi_from_mac
 gattlib_get_rssi_from_mac.argtypes = [c_void_p, c_char_p, POINTER(c_int16)]
 
-# int gattlib_get_advertisement_data(gatt_connection_t *connection,
+# int gattlib_get_advertisement_data(gattlib_connection_t *connection,
 # 		 gattlib_advertisement_data_t **advertisement_data, size_t *advertisement_data_count,
 # 		 uint16_t *manufacturer_id, uint8_t **manufacturer_data, size_t *manufacturer_data_size)
 gattlib_get_advertisement_data = gattlib.gattlib_get_advertisement_data
 gattlib_get_advertisement_data.argtypes = [c_void_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(c_uint16), POINTER(c_void_p), POINTER(c_size_t)]
 
-# int gattlib_get_advertisement_data_from_mac(void *adapter, const char *mac_address,
+# int gattlib_get_advertisement_data_from_mac(gattlib_adapter_t* adapter, const char *mac_address,
 #        gattlib_advertisement_data_t **advertisement_data, size_t *advertisement_data_length,
 #        uint16_t *manufacturer_id, uint8_t **manufacturer_data, size_t *manufacturer_data_size)
 gattlib_get_advertisement_data_from_mac = gattlib.gattlib_get_advertisement_data_from_mac
 gattlib_get_advertisement_data_from_mac.argtypes = [c_void_p, c_char_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(c_uint16), POINTER(c_void_p), POINTER(c_size_t)]
 
 # int gattlib_mainloop_python(PyObject *handler, PyObject *user_data)
 gattlib_mainloop = gattlib.gattlib_mainloop_python
```

### Comparing `gattlib-py-0.5.2/gattlib/adapter.py` & `gattlib-py-0.6.0/gattlib/adapter.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.2/gattlib/device.py` & `gattlib-py-0.6.0/gattlib/device.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.2/gattlib/exception.py` & `gattlib-py-0.6.0/gattlib/exception.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.2/gattlib/gatt.py` & `gattlib-py-0.6.0/gattlib/gatt.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.2/gattlib/mainloop.py` & `gattlib-py-0.6.0/gattlib/mainloop.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.2/gattlib/uuid.py` & `gattlib-py-0.6.0/gattlib/uuid.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.2/gattlib_py.egg-info/PKG-INFO` & `gattlib-py-0.6.0/gattlib_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.5.2/setup.py` & `gattlib-py-0.6.0/setup.py`

 * *Files identical despite different names*

