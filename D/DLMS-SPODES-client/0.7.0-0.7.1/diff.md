# Comparing `tmp/DLMS_SPODES_client-0.7.0.tar.gz` & `tmp/DLMS_SPODES_client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.7.0.tar", last modified: Fri Apr  5 11:32:59 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.7.1.tar", last modified: Mon Apr  8 06:56:11 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.7.0.tar` & `DLMS_SPODES_client-0.7.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.425579 DLMS_SPODES_client-0.7.0/
--rw-rw-rw-   0        0        0      526 2024-04-05 11:32:59.424549 DLMS_SPODES_client-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.0/README.md
--rw-rw-rw-   0        0        0      836 2024-04-05 11:05:18.000000 DLMS_SPODES_client-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 11:32:59.425579 DLMS_SPODES_client-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.278544 DLMS_SPODES_client-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.294549 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   122710 2024-04-05 07:42:39.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/client.py
--rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.231186 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.312546 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.362545 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.418579 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.420547 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5634 2024-04-05 09:00:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0    35025 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.308578 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3206 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.422546 DLMS_SPODES_client-0.7.0/test/
--rw-rw-rw-   0        0        0     7036 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.0/test/test_Client.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.523695 DLMS_SPODES_client-0.7.1/
+-rw-rw-rw-   0        0        0      526 2024-04-08 06:56:11.522696 DLMS_SPODES_client-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.1/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-08 06:55:11.000000 DLMS_SPODES_client-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 06:56:11.523695 DLMS_SPODES_client-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.360731 DLMS_SPODES_client-0.7.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.383737 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   122792 2024-04-08 06:55:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/client.py
+-rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.346698 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.407699 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.459727 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.515737 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.517727 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5634 2024-04-05 09:00:03.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0    35025 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.401733 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-08 06:56:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3206 2024-04-08 06:56:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 06:56:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-08 06:56:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-08 06:56:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-08 06:56:11.000000 DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:56:11.520701 DLMS_SPODES_client-0.7.1/test/
+-rw-rw-rw-   0        0        0     7036 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.1/test/test_Client.py
```

### Comparing `DLMS_SPODES_client-0.7.0/PKG-INFO` & `DLMS_SPODES_client-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.7.0
+Version: 0.7.1
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.0/pyproject.toml` & `DLMS_SPODES_client-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS-SPODES == 0.69.3",
     "DLMS-SPODES-communications >= 1.2.3",
     "pycryptodomex>=3.15"
```

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2113,15 +2113,18 @@
             if len(info) == 0:
                 break
             else:
                 control = frame.Control(self.settings.getNextSend(False))
         self.send_frames.extend(new_frames)
 
     def __str__(self):
-        return F"{self.objects.LDN.value if self.objects else self.__id}"
+        if not self.objects or not self.objects.LDN.value:
+            return self.__id
+        else:
+            return self.objects.LDN.value.to_str()
 
     def get_serial_number(self) -> str:
         """ return serial number as text. If serial object is absence return 'недоступен' """
         if self.objects is None:
             return "нет типа"
         obj = self.objects.serial_number
         if isinstance(obj, Data) and obj.value is not None:
```

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/servers.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client/task.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.7.1/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.0/test/test_Client.py` & `DLMS_SPODES_client-0.7.1/test/test_Client.py`

 * *Files identical despite different names*

