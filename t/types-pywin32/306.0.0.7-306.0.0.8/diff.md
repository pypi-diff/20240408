# Comparing `tmp/types-pywin32-306.0.0.7.tar.gz` & `tmp/types-pywin32-306.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pywin32-306.0.0.7.tar", last modified: Fri Dec  8 02:21:53 2023, max compression
+gzip compressed data, was "types-pywin32-306.0.0.8.tar", last modified: Tue Dec 19 02:20:54 2023, max compression
```

## Comparing `types-pywin32-306.0.0.7.tar` & `types-pywin32-306.0.0.8.tar`

### file list

```diff
@@ -1,415 +1,415 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/_win32typing-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/_win32typing-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)   210297 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/_win32typing-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/afxres-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/afxres-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/afxres-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/commctrl-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/commctrl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/commctrl-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/dde-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/dde-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/dde-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/isapi-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/isapi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/isapi-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/isapi-stubs/isapicon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/isapi-stubs/simple.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/isapi-stubs/threaded_extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/mmapfile-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/mmapfile-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/mmapfile-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.329028 types-pywin32-306.0.0.7/mmsystem-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/mmsystem-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/mmsystem-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/ntsecuritycon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/ntsecuritycon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/ntsecuritycon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/odbc-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/odbc-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/odbc-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/perfmon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/perfmon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/perfmon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/pythoncom-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/pythoncom-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/pythoncom-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/pythonwin-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/pythonwin-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/pythonwin-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/pythonwin-stubs/dde.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/pythonwin-stubs/win32ui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/pythonwin-stubs/win32uiole.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/pywintypes-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/pywintypes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/pywintypes-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/regutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/regutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/regutil-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/servicemanager-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/servicemanager-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/servicemanager-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/sspicon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/sspicon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/sspicon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/timer-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/timer-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/timer-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/types_pywin32.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-12-08 02:21:53.000000 types-pywin32-306.0.0.7/types_pywin32.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2023-12-08 02:21:53.000000 types-pywin32-306.0.0.7/types_pywin32.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 02:21:53.000000 types-pywin32-306.0.0.7/types_pywin32.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-08 02:21:53.000000 types-pywin32-306.0.0.7/types_pywin32.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.333028 types-pywin32-306.0.0.7/win2kras-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win2kras-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win2kras-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.341028 types-pywin32-306.0.0.7/win32-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/_wincerapi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13033 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/afxres.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35998 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/commctrl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22380 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/mmsystem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16244 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/ntsecuritycon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/pywintypes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/regutil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/sspicon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win2kras.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   101683 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32con.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    54316 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32cryptcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32evtlogutil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32gui_struct.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    33390 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32inetcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14831 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32netcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32pdhquery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32serviceutil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/win32timezone.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    77893 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/winerror.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17966 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/winioctlcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    31295 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/winnt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/winperf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/lib/winxptheme.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/mmapfile.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/odbc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/perfmon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/servicemanager.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/timer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32clipboard.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32console.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32cred.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32evtlog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32file.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24668 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32gui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32help.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32inet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32job.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32lz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32net.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32pdh.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32print.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32process.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32profile.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32ras.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20333 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32trace.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32ts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/win32wnet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32-stubs/winxpgui.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32api-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32api-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32api-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32clipboard-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32clipboard-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32clipboard-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32com-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32com-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32com-stubs/adsi/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/adsi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/adsi/adsi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/adsi/adsicon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32com-stubs/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/authorization/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/authorization/authorization.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.345028 types-pywin32-306.0.0.7/win32com-stubs/axcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axcontrol/axcontrol.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/axdebug/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/adb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/axdebug.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/codecontainer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/contexts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/debugger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/documents.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/expressions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/gateways.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/stackframe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axdebug/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/axscript/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/asputil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/axscript.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/axscript/client/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/client/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/axscript/server/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/server/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/server/axsite.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/axscript/server/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/bits/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/bits/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/bits/bits.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/client/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/client/dynamic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/client/gencache.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/directsound/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/directsound/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/directsound/directsound.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/ifilter/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/ifilter/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/ifilter/ifilter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/ifilter/ifiltercon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.349028 types-pywin32-306.0.0.7/win32com-stubs/internet/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/internet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/internet/inetcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/internet/internet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32com-stubs/mapi/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/_exchdapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/emsabtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/exchange.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/mapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/mapitags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/mapi/mapiutil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/olectl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32com-stubs/propsys/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/propsys/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/propsys/propsys.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/propsys/pscon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32com-stubs/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/server/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/server/connect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/server/dispatcher.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/server/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/server/policy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/server/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32com-stubs/shell/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/shell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/shell/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/shell/shellcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/storagecon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32com-stubs/taskscheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/taskscheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/taskscheduler/taskscheduler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/universal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32com-stubs/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32comext-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32comext-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32comext-stubs/adsi/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/adsi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/adsi/adsi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/adsi/adsicon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32comext-stubs/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/authorization/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/authorization/authorization.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.353028 types-pywin32-306.0.0.7/win32comext-stubs/axcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axcontrol/axcontrol.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/adb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/axdebug.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/codecontainer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/contexts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/debugger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/documents.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/expressions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/gateways.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/stackframe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axdebug/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/axscript/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/asputil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/axscript.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/axscript/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/client/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/client/pyscript.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/axscript/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/server/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/server/axsite.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/axscript/server/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/bits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/bits/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/bits/bits.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/directsound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/directsound/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/directsound/directsound.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/ifilter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/ifilter/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/ifilter/ifilter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/ifilter/ifiltercon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.357028 types-pywin32-306.0.0.7/win32comext-stubs/internet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/internet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/internet/inetcon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/internet/internet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32comext-stubs/mapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/_exchdapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    34766 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/emsabtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/exchange.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/mapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26668 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/mapitags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/mapi/mapiutil.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32comext-stubs/propsys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/propsys/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/propsys/propsys.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23479 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/propsys/pscon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32comext-stubs/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/shell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18642 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/shell/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    34194 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/shell/shellcon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32comext-stubs/taskscheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/taskscheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-12-08 02:21:42.000000 types-pywin32-306.0.0.7/win32comext-stubs/taskscheduler/taskscheduler.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32con-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32con-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32con-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32console-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32console-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32console-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32cred-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32cred-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32cred-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32crypt-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32crypt-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32crypt-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32cryptcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32cryptcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32cryptcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32event-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32event-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32event-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.361028 types-pywin32-306.0.0.7/win32evtlog-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32evtlog-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32evtlog-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32evtlogutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32evtlogutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32evtlogutil-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32file-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32file-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32file-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32gui-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32gui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32gui-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32gui_struct-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32gui_struct-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32gui_struct-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32help-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32help-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32help-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32inet-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32inet-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32inet-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32inetcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32inetcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32inetcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32job-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32job-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32job-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32lz-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32lz-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32lz-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32net-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32net-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32net-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32netcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32netcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32netcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32pdh-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32pdh-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32pdh-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32pdhquery-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32pdhquery-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32pdhquery-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32pipe-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32pipe-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32pipe-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.365028 types-pywin32-306.0.0.7/win32print-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32print-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32print-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32process-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32process-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32process-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32profile-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32profile-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32profile-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32ras-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32ras-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32ras-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32security-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32security-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32security-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32service-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32service-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32service-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32serviceutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32serviceutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32serviceutil-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32timezone-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32timezone-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32timezone-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32trace-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32trace-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32trace-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32transaction-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32transaction-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32transaction-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32ts-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32ts-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32ts-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32ui-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32ui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32ui-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32uiole-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32uiole-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32uiole-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/win32wnet-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32wnet-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/win32wnet-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.369028 types-pywin32-306.0.0.7/winerror-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winerror-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winerror-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/winioctlcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winioctlcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winioctlcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/winnt-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winnt-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winnt-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/winperf-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winperf-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winperf-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/winxpgui-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winxpgui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winxpgui-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 02:21:53.373028 types-pywin32-306.0.0.7/winxptheme-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winxptheme-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 02:21:52.000000 types-pywin32-306.0.0.7/winxptheme-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/_win32typing-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/_win32typing-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)   210278 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/_win32typing-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/afxres-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/afxres-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/afxres-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/commctrl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/commctrl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/commctrl-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/dde-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/dde-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/dde-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/isapi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/isapi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/isapi-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/isapi-stubs/isapicon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/isapi-stubs/simple.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/isapi-stubs/threaded_extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/mmapfile-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/mmapfile-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/mmapfile-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/mmsystem-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/mmsystem-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/mmsystem-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/ntsecuritycon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/ntsecuritycon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/ntsecuritycon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/odbc-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/odbc-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/odbc-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/perfmon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/perfmon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/perfmon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.205495 types-pywin32-306.0.0.8/pythoncom-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/pythoncom-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/pythoncom-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/pythonwin-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/pythonwin-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/pythonwin-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/pythonwin-stubs/dde.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/pythonwin-stubs/win32ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/pythonwin-stubs/win32uiole.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/pywintypes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/pywintypes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/pywintypes-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/regutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/regutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/regutil-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/servicemanager-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/servicemanager-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/servicemanager-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/sspicon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/sspicon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/sspicon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/timer-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/timer-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/timer-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/types_pywin32.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-12-19 02:20:54.000000 types-pywin32-306.0.0.8/types_pywin32.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2023-12-19 02:20:54.000000 types-pywin32-306.0.0.8/types_pywin32.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:20:54.000000 types-pywin32-306.0.0.8/types_pywin32.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-19 02:20:54.000000 types-pywin32-306.0.0.8/types_pywin32.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.209495 types-pywin32-306.0.0.8/win2kras-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win2kras-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win2kras-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.213495 types-pywin32-306.0.0.8/win32-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/_wincerapi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.217495 types-pywin32-306.0.0.8/win32-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/afxres.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35998 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/commctrl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22380 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/mmsystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16244 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/ntsecuritycon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/pywintypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/regutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13870 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/sspicon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win2kras.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   101683 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32con.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    54316 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32cryptcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32evtlogutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32gui_struct.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    33390 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32inetcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32netcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32pdhquery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32serviceutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/win32timezone.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    77893 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/winerror.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17966 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/winioctlcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    31295 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/winnt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/winperf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/lib/winxptheme.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/mmapfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/odbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/perfmon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/servicemanager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/timer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32clipboard.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32console.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32cred.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32evtlog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25244 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32help.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32inet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32job.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32lz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32net.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32pdh.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32print.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32process.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32profile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32ras.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20333 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32trace.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32ts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/win32wnet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32-stubs/winxpgui.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.217495 types-pywin32-306.0.0.8/win32api-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32api-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32api-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32clipboard-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32clipboard-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32clipboard-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32com-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32com-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32com-stubs/adsi/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/adsi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/adsi/adsi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/adsi/adsicon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32com-stubs/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/authorization/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/authorization/authorization.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32com-stubs/axcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axcontrol/axcontrol.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32com-stubs/axdebug/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/adb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/axdebug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/codecontainer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/contexts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/debugger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/documents.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/expressions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/gateways.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/stackframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axdebug/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.221495 types-pywin32-306.0.0.8/win32com-stubs/axscript/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/asputil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/axscript.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/axscript/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/client/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/axscript/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/server/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/server/axsite.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/axscript/server/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/bits/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/bits/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/bits/bits.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/client/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/client/dynamic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/client/gencache.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/directsound/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/directsound/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/directsound/directsound.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/ifilter/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/ifilter/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/ifilter/ifilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/ifilter/ifiltercon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/internet/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/internet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/internet/inetcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/internet/internet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/mapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/_exchdapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/emsabtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/exchange.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/mapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/mapitags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/mapi/mapiutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/olectl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.225495 types-pywin32-306.0.0.8/win32com-stubs/propsys/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/propsys/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/propsys/propsys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/propsys/pscon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32com-stubs/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/server/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/server/connect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/server/dispatcher.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/server/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/server/policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/server/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32com-stubs/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/shell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/shell/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/shell/shellcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/storagecon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32com-stubs/taskscheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/taskscheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/taskscheduler/taskscheduler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/universal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32com-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32comext-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32comext-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32comext-stubs/adsi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/adsi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/adsi/adsi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/adsi/adsicon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32comext-stubs/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/authorization/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/authorization/authorization.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32comext-stubs/axcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axcontrol/axcontrol.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.229496 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/adb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/axdebug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/codecontainer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/contexts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/debugger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/documents.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/expressions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/gateways.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/stackframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axdebug/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/axscript/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/asputil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/axscript.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/axscript/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/client/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/client/pyscript.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/axscript/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/server/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/server/axsite.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/axscript/server/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/bits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/bits/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/bits/bits.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/directsound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/directsound/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/directsound/directsound.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/ifilter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/ifilter/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/ifilter/ifilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/ifilter/ifiltercon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/internet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/internet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/internet/inetcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/internet/internet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/mapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/_exchdapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    34766 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/emsabtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/exchange.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/mapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26668 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/mapitags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/mapi/mapiutil.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.233496 types-pywin32-306.0.0.8/win32comext-stubs/propsys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/propsys/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/propsys/propsys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23479 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/propsys/pscon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32comext-stubs/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/shell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/shell/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    34194 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/shell/shellcon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32comext-stubs/taskscheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/taskscheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-12-19 02:20:33.000000 types-pywin32-306.0.0.8/win32comext-stubs/taskscheduler/taskscheduler.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32con-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32con-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32con-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32console-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32console-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32console-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32cred-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32cred-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32cred-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32crypt-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32crypt-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32crypt-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32cryptcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32cryptcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32cryptcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32event-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32event-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32event-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32evtlog-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32evtlog-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32evtlog-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32evtlogutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32evtlogutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32evtlogutil-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32file-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32file-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32file-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32gui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32gui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32gui-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32gui_struct-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32gui_struct-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32gui_struct-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32help-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32help-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32help-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.237496 types-pywin32-306.0.0.8/win32inet-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32inet-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32inet-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32inetcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32inetcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32inetcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32job-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32job-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32job-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32lz-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32lz-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32lz-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32net-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32net-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32net-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32netcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32netcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32netcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32pdh-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32pdh-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32pdh-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32pdhquery-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32pdhquery-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32pdhquery-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32pipe-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32pipe-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32pipe-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32print-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32print-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32print-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32process-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32process-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32process-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32profile-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32profile-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32profile-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32ras-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32ras-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32ras-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32security-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32security-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32security-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32service-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32service-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32service-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.241496 types-pywin32-306.0.0.8/win32serviceutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32serviceutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32serviceutil-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32timezone-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32timezone-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32timezone-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32trace-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32trace-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32trace-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32transaction-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32transaction-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32transaction-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32ts-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32ts-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32ts-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32ui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32ui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32ui-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32uiole-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32uiole-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32uiole-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/win32wnet-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32wnet-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/win32wnet-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/winerror-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winerror-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winerror-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/winioctlcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winioctlcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winioctlcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/winnt-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winnt-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winnt-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/winperf-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winperf-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winperf-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/winxpgui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winxpgui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winxpgui-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:20:54.245496 types-pywin32-306.0.0.8/winxptheme-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winxptheme-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-19 02:20:53.000000 types-pywin32-306.0.0.8/winxptheme-stubs/__init__.pyi
```

### Comparing `types-pywin32-306.0.0.7/CHANGELOG.md` & `types-pywin32-306.0.0.8/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 306.0.0.8 (2023-12-19)
+
+pywin32 annotations improvements (#11177)
+
 ## 306.0.0.7 (2023-12-08)
 
 Fix `pywin32`'s `PyCBitmap.GetBitmapBits` method (#11108)
 
 ## 306.0.0.6 (2023-10-29)
 
 Type `pywin32`'s `win32.win32print.StartDocPrinter` method (#10898)
```

### Comparing `types-pywin32-306.0.0.7/PKG-INFO` & `types-pywin32-306.0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pywin32
-Version: 306.0.0.7
+Version: 306.0.0.8
 Summary: Typing stubs for pywin32
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pywin32.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-pywin32` aims to provide accurate annotations
 for `pywin32==306.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pywin32. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `acfdebfeb83c110d8ffefcfa7cc68bf3ab94817f` and was tested
+This package was generated from typeshed commit `7bdf6ba85ceeebfaf68f632fe0a02f08ce457694` and was tested
 with mypy 1.7.1, pyright 1.1.339, and
-pytype 2023.11.29.
+pytype 2023.12.8.
```

### Comparing `types-pywin32-306.0.0.7/_win32typing-stubs/__init__.pyi` & `types-pywin32-306.0.0.8/_win32typing-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Not available at runtime. Contains type definitions that are otherwise not exposed and not part of a specific module.
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from collections.abc import Iterable
 from typing import overload
 from typing_extensions import Literal, Self, final
 
 class ArgNotFound: ...
 class PyOleEmpty: ...
 class PyOleMissing: ...
@@ -4025,15 +4025,15 @@
 class PyIOleInPlaceSiteWindowless:
     def CanWindowlessActivate(self) -> None: ...
     def GetCapture(self) -> None: ...
     def SetCapture(self, fCapture) -> None: ...
     def GetFocus(self) -> None: ...
     def SetFocus(self, fFocus) -> None: ...
     def GetDC(self, grfFlags, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete]) -> None: ...
-    def ReleaseDC(self, hDC) -> None: ...
+    def ReleaseDC(self, __hDC: PyCDC) -> None: ...
     def InvalidateRect(self, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete], fErase) -> None: ...
     def InvalidateRgn(self, hRgn, fErase) -> None: ...
     def ScrollRect(self, dx, dy) -> None: ...
     def AdjustRect(self) -> None: ...
     def OnDefWindowMessage(self, msg, wParam, lParam) -> None: ...
 
 class PyIOleInPlaceUIWindow:
@@ -4784,17 +4784,17 @@
 class PyAssocCObject: ...
 
 class PyAssocObject:
     def AttachObject(self) -> None: ...
     def GetAttachedObject(self): ...
 
 class PyCBitmap:
-    def CreateCompatibleBitmap(self, dc: PyCDC, width, height) -> None: ...
+    def CreateCompatibleBitmap(self, __dc: PyCDC, __width: int, __height: int) -> None: ...
     def GetSize(self) -> tuple[Incomplete, Incomplete]: ...
-    def GetHandle(self) -> PyGdiHANDLE: ...
+    def GetHandle(self, *args: Unused) -> int: ...
     def LoadBitmap(self, idRes, obDLL: PyDLL | None = ...) -> None: ...
     def LoadBitmapFile(self, fileObject) -> None: ...
     def LoadPPMFile(self, fileObject, cols, rows) -> None: ...
     def Paint(
         self,
         dcObject: PyCDC,
         arg: tuple[Incomplete, Incomplete, Incomplete, Incomplete],
@@ -4915,28 +4915,23 @@
         self,
         rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete],
         pointStart: tuple[Incomplete, Incomplete],
         pointEnd: tuple[Incomplete, Incomplete],
     ) -> None: ...
     def BeginPath(self) -> None: ...
     def BitBlt(
-        self,
-        destPos: tuple[Incomplete, Incomplete],
-        size: tuple[Incomplete, Incomplete],
-        dc: PyCDC,
-        srcPos: tuple[Incomplete, Incomplete],
-        rop,
+        self, __destPos: tuple[int, int], __size: tuple[int, int], __dc: PyCDC, __srcPos: tuple[int, int], __rop: int
     ) -> None: ...
     def Chord(
         self,
         rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete],
         pointStart: tuple[Incomplete, Incomplete],
         pointEnd: tuple[Incomplete, Incomplete],
     ) -> None: ...
-    def CreateCompatibleDC(self, dcFrom: PyCDC | None = ...) -> PyCDC: ...
+    def CreateCompatibleDC(self, __dcFrom: PyCDC | None = ...) -> PyCDC: ...
     def CreatePrinterDC(self, printerName: str | None = ...) -> None: ...
     def DeleteDC(self) -> None: ...
     def DPtoLP(self, point: tuple[Incomplete, Incomplete], x, y) -> tuple[Incomplete, Incomplete]: ...
     def Draw3dRect(self, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete], colorTopLeft, colorBotRight) -> None: ...
     def DrawFocusRect(self, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete]) -> None: ...
     def DrawFrameControl(self, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete], typ, state) -> None: ...
     def DrawIcon(self, point: tuple[Incomplete, Incomplete], hIcon: int) -> None: ...
@@ -4965,15 +4960,15 @@
     def GetCurrentPosition(self) -> tuple[Incomplete, Incomplete]: ...
     def GetDeviceCaps(self, index): ...
     def GetHandleAttrib(self): ...
     def GetHandleOutput(self): ...
     def GetMapMode(self): ...
     def GetNearestColor(self, color): ...
     def GetPixel(self, x, y) -> None: ...
-    def GetSafeHdc(self): ...
+    def GetSafeHdc(self) -> int: ...
     def GetTextExtent(self, text: str) -> tuple[Incomplete, Incomplete]: ...
     def GetTextExtentPoint(self, text: str) -> tuple[Incomplete, Incomplete]: ...
     def GetTextFace(self) -> str: ...
     def GetTextMetrics(self): ...
     def GetViewportExt(self) -> tuple[Incomplete, Incomplete]: ...
     def GetViewportOrg(self) -> tuple[Incomplete, Incomplete]: ...
     def GetWindowExt(self) -> tuple[Incomplete, Incomplete]: ...
@@ -4994,15 +4989,15 @@
     def Rectangle(self): ...
     def RectVisible(self, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete]): ...
     def RestoreDC(self, saved) -> None: ...
     def SaveDC(self): ...
     def ScaleWindowExt(self) -> tuple[Incomplete, Incomplete]: ...
     def ScaleViewportExt(self) -> tuple[Incomplete, Incomplete]: ...
     def SelectClipRgn(self): ...
-    def SelectObject(self, ob): ...
+    def SelectObject(self, __ob: PyCBitmap) -> PyCBitmap: ...
     def SetBkColor(self, color): ...
     def SetBkMode(self, mode): ...
     def SetBrushOrg(self, point: tuple[Incomplete, Incomplete]) -> tuple[Incomplete, Incomplete]: ...
     def SetGraphicsMode(self, mode): ...
     def SetMapMode(self, newMode): ...
     def SetPixel(self, x, y, color) -> None: ...
     def SetPolyFillMode(self, point: tuple[Incomplete, Incomplete]): ...
@@ -5852,15 +5847,15 @@
     def GetTopLevelFrame(self) -> PyCWnd: ...
     def GetTopLevelOwner(self) -> PyCWnd: ...
     def GetTopLevelParent(self) -> PyCWnd: ...
     def GetTopWindow(self) -> PyCWnd: ...
     def GetWindow(self, _type) -> PyCWnd: ...
     def GetWindowDC(self) -> PyCDC: ...
     def GetWindowPlacement(self): ...
-    def GetWindowRect(self) -> tuple[Incomplete, Incomplete, Incomplete, Incomplete]: ...
+    def GetWindowRect(self) -> tuple[int, int, int, int]: ...
     def GetWindowText(self) -> str: ...
     def HideCaret(self) -> None: ...
     def HookAllKeyStrokes(self, obHandler) -> None: ...
     def HookKeyStroke(self, obHandler, ch): ...
     def HookMessage(self, obHandler, message): ...
     def InvalidateRect(self, arg: tuple[Incomplete, Incomplete, Incomplete, Incomplete], bErase: int = ...) -> None: ...
     def InvalidateRgn(self, region: PyCRgn, bErase: int = ...) -> None: ...
@@ -5890,15 +5885,15 @@
     def OnWndMsg(self, msg, wParam, lParam) -> tuple[Incomplete, Incomplete]: ...
     def PreCreateWindow(self, createStruct): ...
     def PumpWaitingMessages(self, firstMsg, lastMsg) -> None: ...
     def RedrawWindow(
         self, _object: PyCRgn, flags, rect: tuple[Incomplete, Incomplete, Incomplete, Incomplete] | None = ...
     ) -> None: ...
     def ReleaseCapture(self) -> None: ...
-    def ReleaseDC(self, dc: PyCDC) -> None: ...
+    def ReleaseDC(self, __dc: PyCDC) -> None: ...
     def RepositionBars(self, idFirst, idLast, idLeftOver) -> None: ...
     def RunModalLoop(self, flags): ...
     def PostMessage(self, idMessage, wParam: int = ..., lParam: int = ...) -> None: ...
     def SendMessageToDescendants(self, idMessage, wParam: int = ..., lParam: int = ..., bDeep: int = ...) -> None: ...
     def SendMessage(self, idMessage, idMessage1, ob, wParam: int = ..., lParam: int = ...) -> None: ...
     def SetActiveWindow(self) -> PyCWnd: ...
     def SetForegroundWindow(self) -> None: ...
```

### Comparing `types-pywin32-306.0.0.7/isapi-stubs/isapicon.pyi` & `types-pywin32-306.0.0.8/isapi-stubs/isapicon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/isapi-stubs/threaded_extension.pyi` & `types-pywin32-306.0.0.8/isapi-stubs/threaded_extension.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/pythoncom-stubs/__init__.pyi` & `types-pywin32-306.0.0.8/pythoncom-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/pythonwin-stubs/dde.pyi` & `types-pywin32-306.0.0.8/pythonwin-stubs/dde.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/pythonwin-stubs/win32ui.pyi` & `types-pywin32-306.0.0.8/pythonwin-stubs/win32ui.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 
 import _win32typing
 
 class error(Exception): ...
 
 def ComparePath(path1: str, path2: str): ...
 def CreateMDIFrame() -> _win32typing.PyCMDIFrameWnd: ...
 def CreateMDIChild() -> _win32typing.PyCMDIChildWnd: ...
-def CreateBitmap() -> _win32typing.PyCBitmap: ...
+def CreateBitmap(*args: Unused) -> _win32typing.PyCBitmap: ...
 def CreateBitmapFromHandle(): ...
 def CreateBrush() -> _win32typing.PyCBrush: ...
 def CreateButton() -> _win32typing.PyCButton: ...
 def CreateColorDialog(
     initColor: int = ..., flags: int = ..., parent: _win32typing.PyCWnd | None = ...
 ) -> _win32typing.PyCColorDialog: ...
 def CreateControl(
@@ -24,15 +24,15 @@
     bStorage,
     obPersist: Incomplete | None = ...,
     licKey: str | None = ...,
 ) -> _win32typing.PyCWnd: ...
 def CreateControlBar() -> _win32typing.PyCControlBar: ...
 def CreateCtrlView(doc: _win32typing.PyCDocument, className: str, style: int = ...) -> _win32typing.PyCCtrlView: ...
 def CreateDC() -> None: ...
-def CreateDCFromHandle(hwnd: int) -> _win32typing.PyCDC: ...
+def CreateDCFromHandle(__hwnd: int | _win32typing.PyHANDLE) -> _win32typing.PyCDC: ...
 def CreateDialog(idRes, dll: _win32typing.PyDLL | None = ...) -> _win32typing.PyCDialog: ...
 def CreateDialogBar() -> _win32typing.PyCDialogBar: ...
 def CreateDialogIndirect(oblist) -> _win32typing.PyCDialog: ...
 def CreatePrintDialog(
     idRes, bPrintSetupOnly, dwFlags, parent: _win32typing.PyCWnd | None = ..., dll: _win32typing.PyDLL | None = ...
 ) -> _win32typing.PyCPrintDialog: ...
 def CreateDocTemplate(idRes) -> _win32typing.PyCDocTemplate: ...
```

### Comparing `types-pywin32-306.0.0.7/pythonwin-stubs/win32uiole.pyi` & `types-pywin32-306.0.0.8/pythonwin-stubs/win32uiole.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/setup.py` & `types-pywin32-306.0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-pywin32` aims to provide accurate annotations
 for `pywin32==306.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pywin32. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `acfdebfeb83c110d8ffefcfa7cc68bf3ab94817f` and was tested
+This package was generated from typeshed commit `7bdf6ba85ceeebfaf68f632fe0a02f08ce457694` and was tested
 with mypy 1.7.1, pyright 1.1.339, and
-pytype 2023.11.29.
+pytype 2023.12.8.
 '''.lstrip()
 
 setup(name=name,
-      version="306.0.0.7",
+      version="306.0.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pywin32.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['win32timezone-stubs', 'winxptheme-stubs', 'winperf-stubs', 'win32com-stubs', 'winioctlcon-stubs', 'win32netcon-stubs', 'winxpgui-stubs', 'perfmon-stubs', 'win32ts-stubs', 'win32ui-stubs', 'win32clipboard-stubs', 'win32cred-stubs', 'win32trace-stubs', 'win32pdhquery-stubs', 'ntsecuritycon-stubs', 'pywintypes-stubs', 'win32security-stubs', 'win32console-stubs', 'win32api-stubs', 'win32inetcon-stubs', 'win32cryptcon-stubs', 'win32job-stubs', 'win2kras-stubs', 'win32help-stubs', 'dde-stubs', 'regutil-stubs', 'win32gui-stubs', 'win32pipe-stubs', 'win32gui_struct-stubs', 'win32service-stubs', 'win32print-stubs', 'servicemanager-stubs', 'win32profile-stubs', 'odbc-stubs', 'commctrl-stubs', 'win32evtlog-stubs', 'win32comext-stubs', 'winnt-stubs', 'pythonwin-stubs', 'afxres-stubs', 'win32crypt-stubs', 'win32serviceutil-stubs', 'mmsystem-stubs', 'win32inet-stubs', 'win32process-stubs', 'win32ras-stubs', 'win32lz-stubs', 'win32file-stubs', 'win32transaction-stubs', 'win32pdh-stubs', '_win32typing-stubs', 'win32net-stubs', 'win32wnet-stubs', 'win32event-stubs', 'sspicon-stubs', 'mmapfile-stubs', 'win32evtlogutil-stubs', 'winerror-stubs', 'win32-stubs', 'win32con-stubs', 'isapi-stubs', 'win32uiole-stubs', 'timer-stubs', 'pythoncom-stubs'],
-      package_data={'win32timezone-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxptheme-stubs': ['__init__.pyi', 'METADATA.toml'], 'winperf-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32com-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'client/__init__.pyi', 'client/build.pyi', 'client/dynamic.pyi', 'client/gencache.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'olectl.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'server/__init__.pyi', 'server/connect.pyi', 'server/dispatcher.pyi', 'server/exception.pyi', 'server/policy.pyi', 'server/util.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'storagecon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'universal.pyi', 'util.pyi', 'METADATA.toml'], 'winioctlcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32netcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxpgui-stubs': ['__init__.pyi', 'METADATA.toml'], 'perfmon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ts-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32clipboard-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cred-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32trace-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdhquery-stubs': ['__init__.pyi', 'METADATA.toml'], 'ntsecuritycon-stubs': ['__init__.pyi', 'METADATA.toml'], 'pywintypes-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32security-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32console-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32api-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inetcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cryptcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32job-stubs': ['__init__.pyi', 'METADATA.toml'], 'win2kras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32help-stubs': ['__init__.pyi', 'METADATA.toml'], 'dde-stubs': ['__init__.pyi', 'METADATA.toml'], 'regutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pipe-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui_struct-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32service-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32print-stubs': ['__init__.pyi', 'METADATA.toml'], 'servicemanager-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32profile-stubs': ['__init__.pyi', 'METADATA.toml'], 'odbc-stubs': ['__init__.pyi', 'METADATA.toml'], 'commctrl-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32evtlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32comext-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/client/pyscript.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'METADATA.toml'], 'winnt-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythonwin-stubs': ['__init__.pyi', 'dde.pyi', 'win32ui.pyi', 'win32uiole.pyi', 'METADATA.toml'], 'afxres-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32crypt-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32serviceutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmsystem-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inet-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32process-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32lz-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32file-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32transaction-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdh-stubs': ['__init__.pyi', 'METADATA.toml'], '_win32typing-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32net-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32wnet-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32event-stubs': ['__init__.pyi', 'METADATA.toml'], 'sspicon-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmapfile-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32evtlogutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'winerror-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32-stubs': ['__init__.pyi', '_wincerapi.pyi', 'lib/__init__.pyi', 'lib/afxres.pyi', 'lib/commctrl.pyi', 'lib/mmsystem.pyi', 'lib/ntsecuritycon.pyi', 'lib/pywintypes.pyi', 'lib/regutil.pyi', 'lib/sspicon.pyi', 'lib/win2kras.pyi', 'lib/win32con.pyi', 'lib/win32cryptcon.pyi', 'lib/win32evtlogutil.pyi', 'lib/win32gui_struct.pyi', 'lib/win32inetcon.pyi', 'lib/win32netcon.pyi', 'lib/win32pdhquery.pyi', 'lib/win32serviceutil.pyi', 'lib/win32timezone.pyi', 'lib/winerror.pyi', 'lib/winioctlcon.pyi', 'lib/winnt.pyi', 'lib/winperf.pyi', 'lib/winxptheme.pyi', 'mmapfile.pyi', 'odbc.pyi', 'perfmon.pyi', 'servicemanager.pyi', 'timer.pyi', 'win32api.pyi', 'win32clipboard.pyi', 'win32console.pyi', 'win32cred.pyi', 'win32crypt.pyi', 'win32event.pyi', 'win32evtlog.pyi', 'win32file.pyi', 'win32gui.pyi', 'win32help.pyi', 'win32inet.pyi', 'win32job.pyi', 'win32lz.pyi', 'win32net.pyi', 'win32pdh.pyi', 'win32pipe.pyi', 'win32print.pyi', 'win32process.pyi', 'win32profile.pyi', 'win32ras.pyi', 'win32security.pyi', 'win32service.pyi', 'win32trace.pyi', 'win32transaction.pyi', 'win32ts.pyi', 'win32wnet.pyi', 'winxpgui.pyi', 'METADATA.toml'], 'win32con-stubs': ['__init__.pyi', 'METADATA.toml'], 'isapi-stubs': ['__init__.pyi', 'isapicon.pyi', 'simple.pyi', 'threaded_extension.pyi', 'METADATA.toml'], 'win32uiole-stubs': ['__init__.pyi', 'METADATA.toml'], 'timer-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythoncom-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['win32evtlog-stubs', 'win32netcon-stubs', 'isapi-stubs', 'win32inet-stubs', 'win32pdhquery-stubs', 'win32con-stubs', 'win32uiole-stubs', 'win32wnet-stubs', 'pywintypes-stubs', 'winxpgui-stubs', 'win32ts-stubs', 'win32gui-stubs', 'win32process-stubs', 'winioctlcon-stubs', 'winerror-stubs', 'perfmon-stubs', 'win32lz-stubs', 'win32help-stubs', 'win32crypt-stubs', 'pythonwin-stubs', 'win32print-stubs', 'win32-stubs', 'win32com-stubs', 'win32api-stubs', 'winxptheme-stubs', 'win32gui_struct-stubs', 'commctrl-stubs', 'win32service-stubs', 'win32transaction-stubs', 'mmapfile-stubs', 'win32net-stubs', 'servicemanager-stubs', 'win32ras-stubs', 'win32pipe-stubs', 'sspicon-stubs', 'win32file-stubs', 'mmsystem-stubs', 'winnt-stubs', 'timer-stubs', 'win32trace-stubs', 'win32clipboard-stubs', 'win32serviceutil-stubs', 'win32security-stubs', 'pythoncom-stubs', 'ntsecuritycon-stubs', 'win32console-stubs', 'winperf-stubs', 'win32pdh-stubs', 'win32job-stubs', 'dde-stubs', 'win32timezone-stubs', 'win32profile-stubs', 'regutil-stubs', '_win32typing-stubs', 'win32cryptcon-stubs', 'win32inetcon-stubs', 'win2kras-stubs', 'win32ui-stubs', 'win32comext-stubs', 'win32evtlogutil-stubs', 'win32cred-stubs', 'win32event-stubs', 'afxres-stubs', 'odbc-stubs'],
+      package_data={'win32evtlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32netcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'isapi-stubs': ['__init__.pyi', 'isapicon.pyi', 'simple.pyi', 'threaded_extension.pyi', 'METADATA.toml'], 'win32inet-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdhquery-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32con-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32uiole-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32wnet-stubs': ['__init__.pyi', 'METADATA.toml'], 'pywintypes-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxpgui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ts-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32process-stubs': ['__init__.pyi', 'METADATA.toml'], 'winioctlcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'winerror-stubs': ['__init__.pyi', 'METADATA.toml'], 'perfmon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32lz-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32help-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32crypt-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythonwin-stubs': ['__init__.pyi', 'dde.pyi', 'win32ui.pyi', 'win32uiole.pyi', 'METADATA.toml'], 'win32print-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32-stubs': ['__init__.pyi', '_wincerapi.pyi', 'lib/__init__.pyi', 'lib/afxres.pyi', 'lib/commctrl.pyi', 'lib/mmsystem.pyi', 'lib/ntsecuritycon.pyi', 'lib/pywintypes.pyi', 'lib/regutil.pyi', 'lib/sspicon.pyi', 'lib/win2kras.pyi', 'lib/win32con.pyi', 'lib/win32cryptcon.pyi', 'lib/win32evtlogutil.pyi', 'lib/win32gui_struct.pyi', 'lib/win32inetcon.pyi', 'lib/win32netcon.pyi', 'lib/win32pdhquery.pyi', 'lib/win32serviceutil.pyi', 'lib/win32timezone.pyi', 'lib/winerror.pyi', 'lib/winioctlcon.pyi', 'lib/winnt.pyi', 'lib/winperf.pyi', 'lib/winxptheme.pyi', 'mmapfile.pyi', 'odbc.pyi', 'perfmon.pyi', 'servicemanager.pyi', 'timer.pyi', 'win32api.pyi', 'win32clipboard.pyi', 'win32console.pyi', 'win32cred.pyi', 'win32crypt.pyi', 'win32event.pyi', 'win32evtlog.pyi', 'win32file.pyi', 'win32gui.pyi', 'win32help.pyi', 'win32inet.pyi', 'win32job.pyi', 'win32lz.pyi', 'win32net.pyi', 'win32pdh.pyi', 'win32pipe.pyi', 'win32print.pyi', 'win32process.pyi', 'win32profile.pyi', 'win32ras.pyi', 'win32security.pyi', 'win32service.pyi', 'win32trace.pyi', 'win32transaction.pyi', 'win32ts.pyi', 'win32wnet.pyi', 'winxpgui.pyi', 'METADATA.toml'], 'win32com-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'client/__init__.pyi', 'client/build.pyi', 'client/dynamic.pyi', 'client/gencache.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'olectl.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'server/__init__.pyi', 'server/connect.pyi', 'server/dispatcher.pyi', 'server/exception.pyi', 'server/policy.pyi', 'server/util.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'storagecon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'universal.pyi', 'util.pyi', 'METADATA.toml'], 'win32api-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxptheme-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui_struct-stubs': ['__init__.pyi', 'METADATA.toml'], 'commctrl-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32service-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32transaction-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmapfile-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32net-stubs': ['__init__.pyi', 'METADATA.toml'], 'servicemanager-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pipe-stubs': ['__init__.pyi', 'METADATA.toml'], 'sspicon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32file-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmsystem-stubs': ['__init__.pyi', 'METADATA.toml'], 'winnt-stubs': ['__init__.pyi', 'METADATA.toml'], 'timer-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32trace-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32clipboard-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32serviceutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32security-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythoncom-stubs': ['__init__.pyi', 'METADATA.toml'], 'ntsecuritycon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32console-stubs': ['__init__.pyi', 'METADATA.toml'], 'winperf-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdh-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32job-stubs': ['__init__.pyi', 'METADATA.toml'], 'dde-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32timezone-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32profile-stubs': ['__init__.pyi', 'METADATA.toml'], 'regutil-stubs': ['__init__.pyi', 'METADATA.toml'], '_win32typing-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cryptcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inetcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win2kras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32comext-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/client/pyscript.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'METADATA.toml'], 'win32evtlogutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cred-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32event-stubs': ['__init__.pyi', 'METADATA.toml'], 'afxres-stubs': ['__init__.pyi', 'METADATA.toml'], 'odbc-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       python_requires=">=3.7",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-pywin32-306.0.0.7/types_pywin32.egg-info/PKG-INFO` & `types-pywin32-306.0.0.8/types_pywin32.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pywin32
-Version: 306.0.0.7
+Version: 306.0.0.8
 Summary: Typing stubs for pywin32
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pywin32.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-pywin32` aims to provide accurate annotations
 for `pywin32==306.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pywin32. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `acfdebfeb83c110d8ffefcfa7cc68bf3ab94817f` and was tested
+This package was generated from typeshed commit `7bdf6ba85ceeebfaf68f632fe0a02f08ce457694` and was tested
 with mypy 1.7.1, pyright 1.1.339, and
-pytype 2023.11.29.
+pytype 2023.12.8.
```

### Comparing `types-pywin32-306.0.0.7/types_pywin32.egg-info/SOURCES.txt` & `types-pywin32-306.0.0.8/types_pywin32.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/types_pywin32.egg-info/top_level.txt` & `types-pywin32-306.0.0.8/types_pywin32.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/_wincerapi.pyi` & `types-pywin32-306.0.0.8/win32-stubs/_wincerapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/afxres.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/afxres.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/commctrl.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/commctrl.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/mmsystem.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/mmsystem.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/ntsecuritycon.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/ntsecuritycon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/pywintypes.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/pywintypes.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/regutil.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/regutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/sspicon.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/sspicon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win2kras.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win2kras.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32con.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32con.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32cryptcon.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32cryptcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32evtlogutil.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32evtlogutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32gui_struct.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32gui_struct.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32inetcon.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32inetcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32netcon.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32netcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32pdhquery.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32pdhquery.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32serviceutil.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32serviceutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/win32timezone.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/win32timezone.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/winerror.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/winerror.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/winioctlcon.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/winioctlcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/winnt.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/winnt.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/winperf.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/winperf.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/lib/winxptheme.pyi` & `types-pywin32-306.0.0.8/win32-stubs/lib/winxptheme.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/odbc.pyi` & `types-pywin32-306.0.0.8/win32-stubs/odbc.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/servicemanager.pyi` & `types-pywin32-306.0.0.8/win32-stubs/servicemanager.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32api.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32api.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 def GetSystemDefaultLangID(): ...
 def GetSystemDefaultLCID(): ...
 def GetSystemDirectory() -> str: ...
 def GetSystemFileCacheSize(): ...
 def SetSystemFileCacheSize(MinimumFileCacheSize, MaximumFileCacheSize, Flags=...) -> None: ...
 def GetSystemInfo(): ...
 def GetNativeSystemInfo(): ...
-def GetSystemMetrics(index): ...
+def GetSystemMetrics(__index: int) -> int: ...
 def GetSystemPowerStatus() -> dict[str, int]: ...
 def GetSystemTime(): ...
 def GetTempFileName(path: str, prefix: str, nUnique): ...
 def GetTempPath() -> str: ...
 def GetThreadLocale(): ...
 def GetTickCount() -> int: ...
 def GetTimeFormat(locale, flags, time: _win32typing.PyTime, _format: str) -> str: ...
```

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32clipboard.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32clipboard.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32console.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32console.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32cred.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32cred.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32crypt.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32crypt.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32event.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32event.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32evtlog.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32evtlog.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32file.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32file.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32gui.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32gui.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,26 @@
     hDC, xLeft, yTop, hIcon, cxWidth, cyWidth, istepIfAniCur, hbrFlickerFreeDraw: _win32typing.PyGdiHANDLE, diFlags
 ) -> None: ...
 def CreateIconIndirect(iconinfo: _win32typing.PyICONINFO): ...
 def CreateIconFromResource(bits: str, fIcon, ver: int = ...) -> int: ...
 def LoadImage(
     __hinst: int, __name: str, __type: int, __cxDesired: int, __cyDesired: int, __fuLoad: int
 ) -> _win32typing.PyGdiHANDLE: ...
-def DeleteObject(handle: _win32typing.PyGdiHANDLE) -> None: ...
-def BitBlt(hdcDest, x, y, width, height, hdcSrc, nXSrc, nYSrc, dwRop) -> None: ...
+def DeleteObject(__handle: int | _win32typing.PyGdiHANDLE) -> None: ...
+def BitBlt(
+    __hdcDest: int | _win32typing.PyGdiHANDLE,
+    __x: int,
+    __y: int,
+    __width: int,
+    __height: int,
+    __hdcSrc: int | _win32typing.PyGdiHANDLE | None,
+    __nXSrc: int,
+    __nYSrc: int,
+    __dwRop: int,
+) -> None: ...
 def StretchBlt(hdcDest, x, y, width, height, hdcSrc, nXSrc, nYSrc, nWidthSrc, nHeightSrc, dwRop) -> None: ...
 def PatBlt(hdc: int, XLeft, YLeft, Width, Height, Rop) -> None: ...
 def SetStretchBltMode(hdc: int, StretchMode): ...
 def GetStretchBltMode(hdc: int): ...
 def TransparentBlt(
     Dest: int, XOriginDest, YOriginDest, WidthDest, HeightDest, Src: int, XOriginSrc, YOriginSrc, WidthSrc, HeightSrc, Transparent
 ) -> None: ...
@@ -163,21 +173,25 @@
 def GetActiveWindow(): ...
 def SetForegroundWindow(__hwnd: int) -> None: ...
 def GetForegroundWindow() -> int: ...
 def GetClientRect(hwnd: int) -> tuple[int, int, int, int]: ...
 def GetDC(hwnd: int): ...
 def SaveDC(hdc: int): ...
 def RestoreDC(hdc: int, SavedDC) -> None: ...
-def DeleteDC(hdc) -> None: ...
-def CreateCompatibleDC(dc): ...
-def CreateCompatibleBitmap(hdc, width, height) -> _win32typing.PyGdiHANDLE: ...
-def CreateBitmap(width, height, cPlanes, cBitsPerPixel, bitmap_bits) -> _win32typing.PyGdiHANDLE: ...
-def SelectObject(hdc, _object): ...
+def DeleteDC(__hdc: int | _win32typing.PyHANDLE) -> None: ...
+def CreateCompatibleDC(__dc: int | _win32typing.PyHANDLE | None) -> int: ...
+def CreateCompatibleBitmap(
+    __hdc: int | _win32typing.PyHANDLE | None, __width: int, __height: int
+) -> _win32typing.PyGdiHANDLE: ...
+def CreateBitmap(
+    __width: int, __height: int, __cPlanes: int, __cBitsPerPixel: int, __bitmap_bits: None
+) -> _win32typing.PyGdiHANDLE: ...
+def SelectObject(__hdc: int | _win32typing.PyHANDLE | None, __object: int | _win32typing.PyHANDLE | None) -> int: ...
 def GetCurrentObject(hdc: int, ObjectType) -> int: ...
-def GetWindowRect(hwnd: int) -> tuple[int, int, int, int]: ...
+def GetWindowRect(__hwnd: int | _win32typing.PyHANDLE) -> tuple[int, int, int, int]: ...
 def GetStockObject(Object) -> int: ...
 def PostQuitMessage(__rc: int) -> None: ...
 def WaitMessage() -> None: ...
 def SetWindowPos(__hWnd: int, __InsertAfter: int | None, __X: int, __Y: int, __cx: int, __cy: int, __Flags: int) -> None: ...
 def GetWindowPlacement(__hwnd: int) -> tuple[int, int, tuple[int, int], tuple[int, int], tuple[int, int, int, int]]: ...
 def SetWindowPlacement(hWnd: int, placement) -> None: ...
 def RegisterClass(__wndClass: _win32typing.PyWNDCLASS) -> _win32typing.PyResourceId: ...
@@ -356,26 +370,26 @@
 def CreateRoundRectRgn(LeftRect, TopRect, RightRect, BottomRect, WidthEllipse, HeightEllipse): ...
 def CreateRectRgnIndirect(rc: _win32typing.PyRECT): ...
 def CreateEllipticRgnIndirect(rc: _win32typing.PyRECT): ...
 def CreateWindowEx(
     dwExStyle, className: str, windowTitle: str, style, x, y, width, height, parent, menu, hinstance, reserved
 ): ...
 def GetParent(child: int) -> int: ...
-def SetParent(__child: int, __child1: int | None | _win32typing.PyHANDLE) -> int: ...
+def SetParent(__child: int, __child1: int | _win32typing.PyHANDLE | None) -> int: ...
 def GetCursorPos() -> tuple[Incomplete, Incomplete]: ...
 def GetDesktopWindow(): ...
 def GetWindow(__hWnd: int, __uCmd: int) -> int: ...
-def GetWindowDC(hWnd: int) -> int: ...
+def GetWindowDC(__hWnd: int | _win32typing.PyHANDLE | None) -> int: ...
 def IsIconic(__hWnd: int) -> int: ...
 def IsWindow(__hWnd: int) -> int: ...
 def IsChild(__hWndParent: int, hWnd: int) -> int: ...
 def ReleaseCapture() -> None: ...
 def GetCapture(): ...
 def SetCapture() -> None: ...
-def ReleaseDC(hWnd: int, hDC): ...
+def ReleaseDC(__hWnd: int | _win32typing.PyHANDLE | None, __hDC: int | _win32typing.PyHANDLE | None) -> Literal[0, 1]: ...
 def CreateCaret(hWnd: int, hBitmap: _win32typing.PyGdiHANDLE, nWidth, nHeight) -> None: ...
 def DestroyCaret() -> None: ...
 def ScrollWindowEx(
     hWnd: int, dx, dy, rcScroll: _win32typing.PyRECT, rcClip: _win32typing.PyRECT, hrgnUpdate, flags
 ) -> tuple[Incomplete, _win32typing.PyRECT]: ...
 def SetScrollInfo(hwnd: int, nBar, scollInfo: _win32typing.PySCROLLINFO, bRedraw=...) -> None: ...
 def GetScrollInfo(hwnd: int, nBar, mask) -> _win32typing.PySCROLLINFO: ...
```

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32help.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32help.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32inet.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32inet.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32job.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32job.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32net.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32net.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32pdh.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32pdh.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32pipe.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32print.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32print.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 def AddPrinterConnection(printer: str): ...
 def DeletePrinterConnection(printer: str): ...
 def EnumPrinters(flags, name: str | None = ..., level: int = ...): ...
 def GetDefaultPrinter() -> str: ...
 def GetDefaultPrinterW() -> str: ...
 def SetDefaultPrinter(printer: str): ...
 def SetDefaultPrinterW(Printer: str): ...
-def StartDocPrinter(__hprinter: _win32typing.PyPrinterHANDLE | int, __level: Literal[1], __tuple: tuple[str, str, str]): ...
+def StartDocPrinter(
+    __hprinter: _win32typing.PyPrinterHANDLE | int, __level: Literal[1], __tuple: tuple[str, str, str | None]
+) -> int: ...
 def EndDocPrinter(hPrinter: _win32typing.PyPrinterHANDLE): ...
 def AbortPrinter(hPrinter: _win32typing.PyPrinterHANDLE) -> None: ...
 def StartPagePrinter(hprinter: _win32typing.PyPrinterHANDLE) -> None: ...
 def EndPagePrinter(hprinter: _win32typing.PyPrinterHANDLE) -> None: ...
 def StartDoc(hdc: int, docinfo): ...
 def EndDoc(hdc: int) -> None: ...
 def AbortDoc(hdc: int) -> None: ...
 def StartPage(hdc: int) -> None: ...
 def EndPage(hdc: int) -> None: ...
-def WritePrinter(hprinter: _win32typing.PyPrinterHANDLE, buf: str): ...
+def WritePrinter(__hprinter: int | _win32typing.PyPrinterHANDLE, __buf: bytes | bytearray | memoryview) -> int: ...
 def EnumJobs(hPrinter: _win32typing.PyPrinterHANDLE, FirstJob, NoJobs, Level=...): ...
 def GetJob(hPrinter: _win32typing.PyPrinterHANDLE, JobID, Level: int = ...): ...
 def SetJob(hPrinter: _win32typing.PyPrinterHANDLE, JobID, Level, JobInfo, Command): ...
 def DocumentProperties(
     HWnd: int,
     hPrinter: _win32typing.PyPrinterHANDLE,
     DeviceName: str,
```

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32process.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32process.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32profile.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32profile.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32ras.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32ras.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32security.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32security.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32service.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32service.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32trace.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32trace.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32transaction.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32ts.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32ts.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32-stubs/win32wnet.pyi` & `types-pywin32-306.0.0.8/win32-stubs/win32wnet.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/client/__init__.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/client/build.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/client/build.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/client/dynamic.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/client/dynamic.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/olectl.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/olectl.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/server/connect.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/server/connect.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/server/dispatcher.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/server/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/server/exception.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/server/exception.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/server/policy.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/server/policy.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/server/util.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/server/util.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/storagecon.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/storagecon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32com-stubs/universal.pyi` & `types-pywin32-306.0.0.8/win32com-stubs/universal.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/adsi/__init__.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/adsi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/adsi/adsi.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/adsi/adsi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/adsi/adsicon.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/adsi/adsicon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axcontrol/axcontrol.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axcontrol/axcontrol.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/adb.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/adb.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/axdebug.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/axdebug.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/codecontainer.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/codecontainer.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/contexts.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/contexts.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/debugger.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/debugger.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/documents.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/documents.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/expressions.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/expressions.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/gateways.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/gateways.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axdebug/stackframe.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axdebug/stackframe.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axscript/axscript.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axscript/axscript.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axscript/client/error.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axscript/client/error.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/axscript/server/axsite.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/axscript/server/axsite.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/bits/bits.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/bits/bits.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/directsound/directsound.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/directsound/directsound.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/ifilter/ifilter.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/ifilter/ifilter.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/ifilter/ifiltercon.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/ifilter/ifiltercon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/internet/inetcon.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/internet/inetcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/internet/internet.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/internet/internet.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/mapi/_exchdapi.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/mapi/_exchdapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/mapi/emsabtags.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/mapi/emsabtags.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/mapi/mapi.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/mapi/mapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/mapi/mapitags.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/mapi/mapitags.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/mapi/mapiutil.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/mapi/mapiutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/propsys/propsys.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/propsys/propsys.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/propsys/pscon.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/propsys/pscon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/shell/shell.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/shell/shell.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 ) -> _win32typing.PyIPropertyBag: ...
 def SHILCreateFromPath(Path: str, Flags) -> tuple[_win32typing.PyIDL, Incomplete]: ...
 def SHCreateShellItem(
     pidlParent: _win32typing.PyIDL, sfParent: _win32typing.PyIShellFolder, Child: _win32typing.PyIDL
 ) -> _win32typing.PyIShellItem: ...
 def SHOpenFolderAndSelectItems(Folder: _win32typing.PyIDL, Items: tuple[_win32typing.PyIDL, ...], Flags=...) -> None: ...
 def SHCreateStreamOnFileEx(File, Mode, Attributes, Create, Template: Incomplete | None = ...) -> _win32typing.PyIStream: ...
-def SetCurrentProcessExplicitAppUserModelID(AppID) -> None: ...
-def GetCurrentProcessExplicitAppUserModelID(): ...
+def SetCurrentProcessExplicitAppUserModelID(__AppID: str) -> None: ...
+def GetCurrentProcessExplicitAppUserModelID() -> str: ...
 def SHParseDisplayName(
     Name, Attributes, BindCtx: _win32typing.PyIBindCtx | None = ...
 ) -> tuple[_win32typing.PyIDL, Incomplete]: ...
 def SHCreateItemFromIDList(*args, **kwargs): ...  # incomplete
 def SHCreateShellItemArrayFromIDLists(*args, **kwargs): ...  # incomplete
 def SHGetIDListFromObject(*args, **kwargs): ...  # incomplete
 def SHGetNameFromIDList(*args, **kwargs): ...  # incomplete
```

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/shell/shellcon.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/shell/shellcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.7/win32comext-stubs/taskscheduler/taskscheduler.pyi` & `types-pywin32-306.0.0.8/win32comext-stubs/taskscheduler/taskscheduler.pyi`

 * *Files identical despite different names*

