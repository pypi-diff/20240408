# Comparing `tmp/wikiteam3-4.2.4.tar.gz` & `tmp/wikiteam3-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiteam3-4.2.4.tar", max compression
+gzip compressed data, was "wikiteam3-4.2.5.tar", max compression
```

## Comparing `wikiteam3-4.2.4.tar` & `wikiteam3-4.2.5.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0    35121 2023-01-25 14:33:50.372284 wikiteam3-4.2.4/LICENSE
--rw-r--r--   0        0        0     7298 2024-03-08 18:07:41.525229 wikiteam3-4.2.4/README.md
--rw-r--r--   0        0        0     2043 2024-03-08 20:05:36.012343 wikiteam3-4.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.130497 wikiteam3-4.2.4/wikiteam3/__init__.py
--rwxr-xr-x   0        0        0      155 2024-03-05 03:06:22.059199 wikiteam3-4.2.4/wikiteam3/dumpgenerator/__init__.py
--rw-r--r--   0        0        0       94 2023-06-27 12:10:45.130497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/__main__.py
--rw-r--r--   0        0        0      193 2023-08-04 17:15:39.832963 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/__init__.py
--rw-r--r--   0        0        0     5233 2023-12-18 15:20:41.710845 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/api.py
--rw-r--r--   0        0        0      405 2024-01-21 19:12:00.362786 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/get_json.py
--rw-r--r--   0        0        0     1110 2023-08-04 17:15:39.832963 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/handle_status_code.py
--rw-r--r--   0        0        0     3019 2023-09-25 09:46:09.055544 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/index_check.py
--rw-r--r--   0        0        0     3483 2023-09-12 18:11:18.038441 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/namespaces.py
--rw-r--r--   0        0        0     9971 2023-09-12 18:11:18.038441 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/page_titles.py
--rw-r--r--   0        0        0     5480 2024-01-21 13:10:14.771695 wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/wiki_check.py
--rw-r--r--   0        0        0       91 2023-08-04 17:15:39.832963 wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/__init__.py
--rw-r--r--   0        0        0    22335 2024-03-05 11:04:12.146959 wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/cli.py
--rw-r--r--   0        0        0     1948 2024-03-05 10:38:17.626972 wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/delay.py
--rw-r--r--   0        0        0      980 2023-12-18 15:54:18.078314 wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/greeter.py
--rw-r--r--   0        0        0     2483 2024-03-05 10:42:49.618970 wikiteam3-4.2.4/wikiteam3/dumpgenerator/config.py
--rw-r--r--   0        0        0       37 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/__init__.py
--rw-r--r--   0        0        0    12862 2024-03-05 10:44:27.474969 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/generator.py
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/__init__.py
--rw-r--r--   0        0        0     2576 2023-08-12 13:22:48.741989 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/html_regexs.py
--rw-r--r--   0        0        0     4620 2024-02-26 12:13:40.739714 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py
--rw-r--r--   0        0        0    33089 2024-03-07 11:26:40.642269 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/image.py
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/__init__.py
--rw-r--r--   0        0        0      879 2023-09-19 20:07:13.093773 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/index_php.py
--rw-r--r--   0        0        0     2770 2024-03-05 10:39:32.146971 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/site_info.py
--rw-r--r--   0        0        0      505 2024-02-26 12:13:40.743714 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/site_info_test.py
--rw-r--r--   0        0        0     1007 2023-08-16 02:54:04.801030 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/special_logs.py
--rw-r--r--   0        0        0     1009 2023-09-19 20:07:31.098123 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/special_version.py
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlexport/__init__.py
--rw-r--r--   0        0        0      498 2023-09-19 13:21:07.864884 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml.py
--rw-r--r--   0        0        0    13522 2024-01-21 19:12:00.370786 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py
--rw-r--r--   0        0        0     8991 2023-10-19 10:13:33.683870 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlrev/__init__.py
--rw-r--r--   0        0        0    22245 2023-09-25 10:01:05.148867 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py
--rw-r--r--   0        0        0     4783 2023-10-15 08:04:29.462772 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py
--rw-r--r--   0        0        0        0 2023-06-27 12:10:45.134497 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/__init__.py
--rw-r--r--   0        0        0     5780 2024-02-26 12:13:40.703714 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py
--rw-r--r--   0        0        0     5240 2023-09-12 18:11:18.042441 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py
--rw-r--r--   0        0        0      277 2023-08-18 23:41:26.686746 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_integrity.py
--rw-r--r--   0        0        0     2487 2023-08-11 17:34:23.066305 wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py
--rw-r--r--   0        0        0     1144 2024-02-26 12:13:40.703714 wikiteam3-4.2.4/wikiteam3/dumpgenerator/exceptions.py
--rw-r--r--   0        0        0       33 2023-08-04 17:15:39.840963 wikiteam3-4.2.4/wikiteam3/dumpgenerator/log/__init__.py
--rw-r--r--   0        0        0      485 2023-12-18 15:53:55.933679 wikiteam3-4.2.4/wikiteam3/dumpgenerator/log/log_error.py
--rw-r--r--   0        0        0       65 2024-03-08 20:05:36.012343 wikiteam3-4.2.4/wikiteam3/dumpgenerator/version.py
--rw-r--r--   0        0        0       83 2023-08-18 18:17:18.012394 wikiteam3-4.2.4/wikiteam3/uploader/__init__.py
--rw-r--r--   0        0        0       83 2023-08-18 18:18:57.034720 wikiteam3-4.2.4/wikiteam3/uploader/__main__.py
--rw-r--r--   0        0        0     9212 2024-03-08 18:07:41.529229 wikiteam3-4.2.4/wikiteam3/uploader/compresser.py
--rw-r--r--   0        0        0     1733 2023-08-20 13:14:28.468235 wikiteam3-4.2.4/wikiteam3/uploader/socketLock.py
--rw-r--r--   0        0        0    23068 2024-03-08 18:07:41.529229 wikiteam3-4.2.4/wikiteam3/uploader/uploader.py
--rw-r--r--   0        0        0      377 2023-08-12 15:22:07.055251 wikiteam3-4.2.4/wikiteam3/utils/__init__.py
--rw-r--r--   0        0        0     3255 2023-09-25 10:23:33.130696 wikiteam3-4.2.4/wikiteam3/utils/ia_checker.py
--rw-r--r--   0        0        0     3422 2023-08-04 17:15:48.009485 wikiteam3-4.2.4/wikiteam3/utils/identifier.py
--rw-r--r--   0        0        0     1471 2023-09-12 18:11:18.042441 wikiteam3-4.2.4/wikiteam3/utils/login/__init__.py
--rw-r--r--   0        0        0     2380 2023-08-04 17:15:39.840963 wikiteam3-4.2.4/wikiteam3/utils/login/api.py
--rw-r--r--   0        0        0     2157 2023-08-04 17:15:39.840963 wikiteam3-4.2.4/wikiteam3/utils/login/index.py
--rw-r--r--   0        0        0     6307 2024-03-08 20:05:36.012343 wikiteam3-4.2.4/wikiteam3/utils/monkey_patch.py
--rw-r--r--   0        0        0      341 2023-09-12 18:11:18.042441 wikiteam3-4.2.4/wikiteam3/utils/uprint.py
--rw-r--r--   0        0        0    38659 2024-02-26 10:00:47.663781 wikiteam3-4.2.4/wikiteam3/utils/user_agent.py
--rw-r--r--   0        0        0     4686 2024-03-05 07:01:49.623081 wikiteam3-4.2.4/wikiteam3/utils/util.py
--rw-r--r--   0        0        0      796 2023-08-04 17:15:39.840963 wikiteam3-4.2.4/wikiteam3/utils/wiki_avoid.py
--rw-r--r--   0        0        0     9042 1970-01-01 00:00:00.000000 wikiteam3-4.2.4/setup.py
--rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 wikiteam3-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35121 2024-03-06 03:04:21.649498 wikiteam3-4.2.5/LICENSE
+-rw-r--r--   0        0        0    16107 2024-03-10 09:50:28.696990 wikiteam3-4.2.5/README.md
+-rw-r--r--   0        0        0     2043 2024-04-08 13:47:32.033662 wikiteam3-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/__init__.py
+-rwxr-xr-x   0        0        0      155 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/__init__.py
+-rw-r--r--   0        0        0       94 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/__main__.py
+-rw-r--r--   0        0        0      193 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/__init__.py
+-rw-r--r--   0        0        0     5233 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/api.py
+-rw-r--r--   0        0        0      415 2024-04-08 12:30:05.560295 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/get_json.py
+-rw-r--r--   0        0        0     1110 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/handle_status_code.py
+-rw-r--r--   0        0        0     3019 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/index_check.py
+-rw-r--r--   0        0        0     3483 2024-04-08 13:47:16.853117 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/namespaces.py
+-rw-r--r--   0        0        0     9971 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/page_titles.py
+-rw-r--r--   0        0        0     5480 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/wiki_check.py
+-rw-r--r--   0        0        0       91 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/__init__.py
+-rw-r--r--   0        0        0    22478 2024-04-08 13:18:29.425069 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/cli.py
+-rw-r--r--   0        0        0     1948 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/delay.py
+-rw-r--r--   0        0        0      980 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/greeter.py
+-rw-r--r--   0        0        0     3092 2024-04-08 12:43:00.924209 wikiteam3-4.2.5/wikiteam3/dumpgenerator/config.py
+-rw-r--r--   0        0        0       37 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/__init__.py
+-rw-r--r--   0        0        0    12817 2024-04-08 12:46:20.286521 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/generator.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/__init__.py
+-rw-r--r--   0        0        0     2576 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs.py
+-rw-r--r--   0        0        0     4620 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py
+-rw-r--r--   0        0        0    32910 2024-04-08 12:59:53.869416 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/image.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/__init__.py
+-rw-r--r--   0        0        0      879 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/index_php.py
+-rw-r--r--   0        0        0     2638 2024-04-08 12:19:09.606864 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/site_info.py
+-rw-r--r--   0        0        0      505 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/site_info_test.py
+-rw-r--r--   0        0        0     1007 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_logs.py
+-rw-r--r--   0        0        0     1009 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_version.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/__init__.py
+-rw-r--r--   0        0        0      498 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml.py
+-rw-r--r--   0        0        0    13522 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py
+-rw-r--r--   0        0        0     8991 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/__init__.py
+-rw-r--r--   0        0        0    22245 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py
+-rw-r--r--   0        0        0     4783 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/__init__.py
+-rw-r--r--   0        0        0     5780 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py
+-rw-r--r--   0        0        0     5240 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py
+-rw-r--r--   0        0        0      277 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_integrity.py
+-rw-r--r--   0        0        0     2487 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py
+-rw-r--r--   0        0        0     1144 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/exceptions.py
+-rw-r--r--   0        0        0       33 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/log/__init__.py
+-rw-r--r--   0        0        0      485 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/log/log_error.py
+-rw-r--r--   0        0        0       65 2024-04-08 13:47:44.397985 wikiteam3-4.2.5/wikiteam3/dumpgenerator/version.py
+-rw-r--r--   0        0        0       83 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/uploader/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/uploader/__main__.py
+-rw-r--r--   0        0        0     9212 2024-03-08 17:33:56.605131 wikiteam3-4.2.5/wikiteam3/uploader/compresser.py
+-rw-r--r--   0        0        0     1733 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/uploader/socketLock.py
+-rw-r--r--   0        0        0    23068 2024-03-08 17:35:52.503064 wikiteam3-4.2.5/wikiteam3/uploader/uploader.py
+-rw-r--r--   0        0        0      377 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/__init__.py
+-rw-r--r--   0        0        0     3255 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/ia_checker.py
+-rw-r--r--   0        0        0     3422 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/identifier.py
+-rw-r--r--   0        0        0     1471 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/login/__init__.py
+-rw-r--r--   0        0        0     2380 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/login/api.py
+-rw-r--r--   0        0        0     2157 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/login/index.py
+-rw-r--r--   0        0        0     7701 2024-04-08 13:33:10.207323 wikiteam3-4.2.5/wikiteam3/utils/monkey_patch.py
+-rw-r--r--   0        0        0      341 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/uprint.py
+-rw-r--r--   0        0        0    38659 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/user_agent.py
+-rw-r--r--   0        0        0     4686 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/util.py
+-rw-r--r--   0        0        0      779 2024-04-08 12:19:44.152101 wikiteam3-4.2.5/wikiteam3/utils/wiki_avoid.py
+-rw-r--r--   0        0        0    18092 1970-01-01 00:00:00.000000 wikiteam3-4.2.5/PKG-INFO
```

### Comparing `wikiteam3-4.2.4/LICENSE` & `wikiteam3-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/pyproject.toml` & `wikiteam3-4.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wikiteam3"
-version = "4.2.4"
+version = "4.2.5"
 description = "Tools for downloading and preserving MediaWikis. We archive MediaWikis, from Wikipedia to tiniest wikis."
 license = "GPL-3.0-or-later"
 # authors = ["WikiTeam Contributors"] # FIXME: it's not an valid author name
 authors = ["yzqzss <yzqzss@yandex.com>"]
 maintainers = [
     # "saveweb wikiteam3 maintainers", #FIXME
     # "mediawiki-scarper maintainers",
```

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/api.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/api.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/handle_status_code.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/handle_status_code.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/index_check.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/index_check.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/namespaces.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/namespaces.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/page_titles.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/page_titles.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/api/wiki_check.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/wiki_check.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/cli.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 import http
 import http.cookiejar
 import os
 import queue
 import re
 import sys
 import traceback
-from typing import Dict, Tuple
+from typing import Tuple
 
 import requests
 from requests.adapters import DEFAULT_RETRIES as REQUESTS_DEFAULT_RETRIES
 from requests.adapters import HTTPAdapter
 import urllib3
 
 from wikiteam3.dumpgenerator.api import (
     check_retry_API,
     get_WikiEngine,
     mediawiki_get_API_and_Index,
 )
 from wikiteam3.dumpgenerator.api.index_check import check_index
 from wikiteam3.dumpgenerator.cli.delay import Delay
-from wikiteam3.dumpgenerator.config import Config, new_config
+from wikiteam3.dumpgenerator.config import Config, OtherConfig, new_config
 from wikiteam3.dumpgenerator.version import getVersion
 from wikiteam3.utils import (
     get_random_UserAgent,
     mod_requests_text,
     url2prefix_from_config,
 )
 from wikiteam3.utils.login import uniLogin
-from wikiteam3.utils.monkey_patch import WakeTLSAdapter
+from wikiteam3.utils.monkey_patch import SessionMonkeyPatch, WakeTLSAdapter
 from wikiteam3.utils.user_agent import setup_random_UserAgent
 
 
 def getArgumentParser():
     parser = argparse.ArgumentParser(description="")
 
     # General params
@@ -159,15 +159,15 @@
         "--bypass-cdn-image-compression",
         action="store_true",
         help="Bypass CDN image compression. (CloudFlare Polish, etc.)",
     )
     group_image.add_argument(
         "--image-timestamp-interval",
         metavar="2019-01-02T01:36:06Z/2023-08-12T10:36:06Z",
-        help="[BETA] Only download images uploaded in the given time interval. [format: ISO 8601 UTC interval] "
+        help="Only download images uploaded in the given time interval. [format: ISO 8601 UTC interval] "
             "(only works with api)",
     )
     group_image.add_argument(
         "--ia-wbm-booster",
         type=int,
         default=0,
         choices=[0, 1, 2, 3],
@@ -272,15 +272,15 @@
         if url and (not url.startswith("http://") and not url.startswith("https://")):
             print(url)
             print("ERROR: URLs must start with http:// or https://")
             passed = False
     
     return passed
 
-def get_parameters(params=None) -> Tuple[Config, Dict]:
+def get_parameters(params=None) -> Tuple[Config, OtherConfig]:
     # if not params:
     #     params = sys.argv
 
     parser = getArgumentParser()
     args = parser.parse_args(params)
     if checkParameters(args) is not True:
         print("\n\n")
@@ -289,14 +289,16 @@
     # print (args)
 
     ########################################
 
     # Create session
     mod_requests_text(requests) # monkey patch # type: ignore
     session = requests.Session()
+    patch_sess = SessionMonkeyPatch(session=session, hard_retries=1)
+    patch_sess.hijack()
     def print_request(r: requests.Response, *args, **kwargs):
         # TODO: use logging
         # print("H:", r.request.headers)
         for _r in r.history:
             print("Resp (history): ", _r.request.method, _r.status_code, _r.reason, _r.url)
         print(f"Resp: {r.request.method} {r.status_code} {r.reason} {r.url}")
         if r.raw._connection.sock:
@@ -531,32 +533,33 @@
         "exnamespaces": exnamespaces,
         "path": args.path and os.path.normpath(args.path) or "",
         "cookies": args.cookies or "",
         "delay": args.delay,
         "retries": int(args.retries),
     })
 
-    other = {
-        "resume": args.resume,
-        "force": args.force,
-        "session": session,
-        "stdout_log_path": args.stdout_log_path,
-        "bypass_cdn_image_compression": args.bypass_cdn_image_compression,
-        "add_referer_header": args.add_referer_header,
-        "image_timestamp_interval": args.image_timestamp_interval,
-        "ia_wbm_booster": args.ia_wbm_booster,
-
-        "assert_max_pages": args.assert_max_pages,
-        "assert_max_edits": args.assert_max_edits,
-        "assert_max_images": args.assert_max_images,
-        "assert_max_images_bytes": args.assert_max_images_bytes,
-
-        "upload": args.upload,
-        "uploader_args": args.uploader_args,
-    }
+
+    other = OtherConfig(
+        resume = args.resume,
+        force = args.force,
+        session = session,
+        stdout_log_path = args.stdout_log_path,
+        bypass_cdn_image_compression = args.bypass_cdn_image_compression,
+        add_referer_header = args.add_referer_header,
+        image_timestamp_interval = args.image_timestamp_interval,
+        ia_wbm_booster = args.ia_wbm_booster,
+
+        assert_max_pages = args.assert_max_pages,
+        assert_max_edits = args.assert_max_edits,
+        assert_max_images = args.assert_max_images,
+        assert_max_images_bytes = args.assert_max_images_bytes,
+
+        upload = args.upload,
+        uploader_args = args.uploader_args,
+    )
 
     # calculating path, if not defined by user with --path=
     if not config.path:
         config.path = "./{}-{}-wikidump".format(
             url2prefix_from_config(config=config),
             config.date,
         )
@@ -570,8 +573,9 @@
         print(
             f"There will be a {config.delay} second delay between HTTP calls in order to keep the server from timing you out."
         )
         print(
             "If you know that this is unnecessary, you can manually specify '--delay 0.0'."
         )
 
+    patch_sess.release()
     return config, other
```

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/delay.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/delay.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/cli/greeter.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/greeter.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/config.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import dataclasses
 import json
-from typing import List
+from typing import List, Optional
+
+import requests
 
 
 def _dataclass_from_dict(klass_or_obj, d: dict):
     if isinstance(klass_or_obj, type): # klass
         ret = klass_or_obj()
     else:
         ret = klass_or_obj
@@ -86,8 +88,30 @@
 
     raise FileNotFoundError(f"Config file {config_filename} not found")
 
 def save_config(config: Config, config_filename: str):
     """Save config file"""
 
     with open(f"{config.path}/{config_filename}", "w", encoding="utf-8") as outfile:
-        json.dump(dataclasses.asdict(config), outfile, indent=4, sort_keys=True)
+        json.dump(dataclasses.asdict(config), outfile, indent=4, sort_keys=True)
+
+
+@dataclasses.dataclass
+class OtherConfig:
+    resume: bool
+    force: bool 
+    session: requests.Session 
+    stdout_log_path: Optional[str] 
+    bypass_cdn_image_compression: bool 
+    add_referer_header: Optional[str] 
+    '''None, "auto", {URL}'''
+    image_timestamp_interval: Optional[str]
+    ''' 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z '''
+    ia_wbm_booster: int 
+
+    assert_max_pages: Optional[int] 
+    assert_max_edits: Optional[int] 
+    assert_max_images: Optional[int] 
+    assert_max_images_bytes: Optional[int] 
+
+    upload: bool 
+    uploader_args: List[str]
```

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/generator.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 import traceback
 from typing import Dict, Union
 
 from file_read_backwards import FileReadBackwards
 
-from wikiteam3.dumpgenerator.config import load_config, save_config
+from wikiteam3.dumpgenerator.config import OtherConfig, load_config, save_config
 from wikiteam3.dumpgenerator.config import Config
 from wikiteam3.dumpgenerator.cli import get_parameters, bye, welcome
 from wikiteam3.dumpgenerator.dump.image.image import FILENAME_LIMIT, Image
 from wikiteam3.dumpgenerator.dump.misc.index_php import save_IndexPHP
 from wikiteam3.dumpgenerator.dump.misc.special_logs import save_SpecialLog
 from wikiteam3.dumpgenerator.dump.misc.special_version import save_SpecialVersion
 from wikiteam3.dumpgenerator.dump.misc.site_info import assert_siteinfo, get_siteinfo, save_siteinfo
@@ -52,20 +52,20 @@
     @staticmethod
     def __init__(params=None):
         """Main function"""
         config_filename = DumpGenerator.configfilename
         config, other = get_parameters(params=params)
         avoid_WikiMedia_projects(config=config, other=other)
 
-        with (Tee(other["stdout_log_path"]) if other["stdout_log_path"] is not None else contextlib.nullcontext()):
+        with (Tee(other.stdout_log_path) if other.stdout_log_path else contextlib.nullcontext()):
             print(welcome())
             print("Analysing %s" % (config.api if config.api else config.index))
 
             # do not enter if resume is requested from begining
-            while not other["resume"] and os.path.isdir(config.path):
+            while not other.resume and os.path.isdir(config.path):
                 print('\nWarning!: "%s" path exists' % (config.path))
                 reply = "y" if config.failfast else ""
                 while reply.lower()[:1] not in ["y", "n"]:
                     reply = input(
                         'There is a dump in "%s", probably incomplete.\n'
                         'If you choose resume, to avoid conflicts, some parameters '
                         'you have chosen in the current session will be ignored\n'
@@ -75,80 +75,80 @@
                     )
                     reply = reply.lower()[:1]
                 if reply == "y":
                     if not os.path.isfile("{}/{}".format(config.path, config_filename)):
                         print("No config file found. I can't resume. Aborting.")
                         sys.exit(1)
                     print("You have selected: YES")
-                    other["resume"] = True
+                    other.resume = True
                     break
                 elif reply == "n":
                     print("You have selected: NO.\nbye.")
-                    # other["resume"] = False
+                    # other.resume = False
                     sys.exit(0)
 
-            if asserts_enabled := [(arg, v) for arg, v in other.items() if arg.startswith("assert_") and v is not None]:
-                site_info = get_siteinfo(config=config, session=other["session"])
+            if asserts_enabled := [(arg, v) for arg, v in other.__dict__.items() if arg.startswith("assert_") and v is not None]:
+                site_info = get_siteinfo(config=config, session=other.session)
                 assert_siteinfo(site_info, other)
                 [print(f"--{arg}: {v}, passed") for arg, v in asserts_enabled] 
 
-            if other["resume"]:
+            if other.resume:
                 print("Loading config file to resume...")
                 config = load_config(config=config, config_filename=config_filename)
             else:
-                if not other['force'] and any_recent_ia_item_exists(config, days=365):
+                if not other.force and any_recent_ia_item_exists(config, days=365):
                     print("A dump of this wiki was uploaded to IA in the last 365 days. Aborting.")
                     sys.exit(88)
 
                 os.mkdir(config.path)
                 save_config(config=config, config_filename=config_filename)
 
-            if other["resume"]:
+            if other.resume:
                 DumpGenerator.resumePreviousDump(config=config, other=other)
             else:
                 DumpGenerator.createNewDump(config=config, other=other)
 
             if config.index:
-                save_IndexPHP(config=config, session=other["session"])
-                save_SpecialVersion(config=config, session=other["session"])
+                save_IndexPHP(config=config, session=other.session)
+                save_SpecialVersion(config=config, session=other.session)
             if config.api:
-                save_siteinfo(config=config, session=other["session"])
+                save_siteinfo(config=config, session=other.session)
 
             mark_as_done(config=config, mark=ALL_DUMPED_MARK)
             bye(config.path)
-            if other["upload"]:
+            if other.upload:
                 print('Calling uploader... (--upload)')
-                retcode = subprocess.call([sys.executable, '-m', 'wikiteam3.uploader', config.path] + other["uploader_args"],
+                retcode = subprocess.call([sys.executable, '-m', 'wikiteam3.uploader', config.path] + other.uploader_args,
                     shell=False)
                 if retcode:
                     print(f'--upload: Failed: {retcode}')
                     sys.exit(retcode)
                 
                 print('--upload: Done')
 
     @staticmethod
-    def createNewDump(config: Config, other: Dict):
+    def createNewDump(config: Config, other: OtherConfig):
         # we do lazy title dumping here :)
         images = []
         print("Trying generating a new dump into a new directory...")
         if config.xml:
-            generate_XML_dump(config=config, session=other["session"])
-            check_XML_integrity(config=config, session=other["session"])
+            generate_XML_dump(config=config, session=other.session)
+            check_XML_integrity(config=config, session=other.session)
         if config.images:
-            images += Image.get_image_names(config=config, session=other["session"])
+            images += Image.get_image_names(config=config, session=other.session)
             Image.save_image_names(config=config, other=other, images=images)
             Image.generate_image_dump(
-                config=config, other=other, images=images, session=other["session"]
+                config=config, other=other, images=images, session=other.session
             )
         if config.logs:
             pass # TODO
-            # save_SpecialLog(config=config, session=other["session"])
+            # save_SpecialLog(config=config, session=other.session)
 
     @staticmethod
-    def resumePreviousDump(config: Config, other: Dict):
+    def resumePreviousDump(config: Config, other: OtherConfig):
         images = []
         print("Resuming previous dump process...")
         if config.xml:
 
             # checking xml dump
             xml_is_complete = False
             last_xml_title = None
@@ -184,21 +184,21 @@
             if xml_is_complete:
                 print("XML dump was completed in the previous session")
             elif last_xml_title:
                 # resuming...
                 print('Resuming XML dump from "%s" (revision id %s)' % (last_xml_title, last_xml_revid))
                 generate_XML_dump(
                     config=config,
-                    session=other["session"],
+                    session=other.session,
                     resume=True,
                 )
             else:
                 # corrupt? only has XML header?
                 print("XML is corrupt? Regenerating...")
-                generate_XML_dump(config=config, session=other["session"])
+                generate_XML_dump(config=config, session=other.session)
 
         if config.images:
             # load images list
             last_line = ""
             imagesFilePath = "%s/%s-%s-images.txt" % (config.path, url2prefix_from_config(config=config), config.date)
             if os.path.exists(imagesFilePath):
                 with open(imagesFilePath, "r", encoding="utf-8") as f:
@@ -215,15 +215,15 @@
                 sys.exit(9)
             if last_line == "--END--":
                 print("Image list was completed in the previous session")
             else:
                 print("Image list is incomplete. Reloading...")
                 # do not resume, reload, to avoid inconsistences, deleted images or
                 # so
-                images = Image.get_image_names(config=config, session=other["session"])
+                images = Image.get_image_names(config=config, session=other.session)
                 Image.save_image_names(config=config, other=other, images=images)
             # checking images directory
             files = set()
             du_dir: int = 0 # du -s {config.path}/images
             if os.path.exists(f"{config.path}/images"):
                 c_loaded = 0
                 for file in os.scandir(f"{config.path}/images"):
@@ -278,13 +278,13 @@
             else:
                 # we resume from previous image, which may be corrupted 
                 # by the previous session ctrl-c or abort
                 Image.generate_image_dump(
                     config=config,
                     other=other,
                     images=images,
-                    session=other["session"],
+                    session=other.session,
                 )
 
         if config.logs:
             # fix
             pass
```

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/html_regexs.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/image/image.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 import datetime
 import os
-import random
 import re
 import shutil
 import sys
 import time
 import urllib.parse
 import warnings
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import requests
 
 from wikiteam3.dumpgenerator.api import get_JSON, handle_StatusCode
 from wikiteam3.dumpgenerator.cli import Delay
-from wikiteam3.dumpgenerator.config import Config
+from wikiteam3.dumpgenerator.config import Config, OtherConfig
 from wikiteam3.dumpgenerator.dump.image.html_regexs import R_NEXT, REGEX_CANDIDATES
 from wikiteam3.dumpgenerator.exceptions import FileSha1Error, FileSizeError
 from wikiteam3.dumpgenerator.log import log_error
 from wikiteam3.dumpgenerator.version import getVersion
 from wikiteam3.utils.identifier import url2prefix_from_config
 from wikiteam3.utils.monkey_patch import SessionMonkeyPatch
 from wikiteam3.utils.util import clean_HTML, int_or_zero, sha1bytes, sha1sum, space, underscore, undo_HTML_entities
 
 NULL = "null"
 """ NULL value for image metadata """
 FILENAME_LIMIT = 240
 """ Filename not be longer than 240 **bytes**. (MediaWiki r98430 2011-09-29) """
+STDOUT_IS_TTY = sys.stdout and sys.stdout.isatty()
 
 
 WBM_EARLIEST = 1
 WBN_LATEST = 2
 WBM_BEST = 3
 
 
 def check_response(r: requests.Response) -> None:
     if r.headers.get("cf-polished", ""):
         raise RuntimeError("Found cf-polished header in response, use --bypass-cdn-image-compression to bypass it")
 
 class Image:
 
     @staticmethod
-    def generate_image_dump(config: Config, other: Dict, images: List[List],
+    def generate_image_dump(config: Config, other: OtherConfig, images: List[List],
                             session: requests.Session):
         """ Save files and descriptions using a file list """
 
-        bypass_cdn_image_compression: bool = other["bypass_cdn_image_compression"]
-        image_timestamp_interval: Optional[str] = other["image_timestamp_interval"]
-        ia_wbm_booster: int = other["ia_wbm_booster"]
-        add_referer_header: Optional[str] = other["add_referer_header"] # None, "auto", {URL}
-
         image_timestamp_intervals = None
-        if image_timestamp_interval: # 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z
-            image_timestamp_intervals = image_timestamp_interval.split("/")
+        if other.image_timestamp_interval:
+            image_timestamp_intervals = other.image_timestamp_interval.split("/")
             assert len(image_timestamp_intervals) == 2
             image_timestamp_intervals = [
                 datetime.datetime.strptime(x, "%Y-%m-%dT%H:%M:%SZ")
                 for x in image_timestamp_intervals]
 
         print("Retrieving images...")
         images_dir = Path(config.path) / "images"
@@ -83,31 +78,31 @@
             return False
 
 
         def modify_params(params: Optional[Dict] = None) -> Dict:
             """ bypass Cloudflare Polish (image optimization) """
             if params is None:
                 params = {}
-            if bypass_cdn_image_compression is True:
+            if other.bypass_cdn_image_compression is True:
                 # bypass Cloudflare Polish (image optimization)
                 # <https://developers.cloudflare.com/images/polish/>
                 params["_wiki_t"] = int(time.time()*1000)
-                params[f"_wiki_{random.randint(10,99)}_"] = "random"
+                params["_wikiteam3_nocdn"] = "init_req" # this value will be changed on hard retry
 
             return params
         
         def modify_headers(headers: Optional[Dict] = None) -> Dict:
             """ add HTTP Referer header """
             if headers is None:
                 headers = {}
-            if add_referer_header:
+            if other.add_referer_header:
                 url = config.index if config.index else config.api
                 parsed_url = urllib.parse.urlparse(
-                    add_referer_header
-                    if add_referer_header != "auto"
+                    other.add_referer_header
+                    if other.add_referer_header != "auto"
                     else url
                 )
 
                 headers["Referer"] = f"{parsed_url.scheme}://{parsed_url.netloc}/"
 
             return headers
             
@@ -139,18 +134,18 @@
                     print(f"    {filename_underscore}|timestamp is unknown: {NULL}, downloading anyway...")
                 else:
                     if not (
                         image_timestamp_intervals[0]
                         <= datetime.datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%SZ")
                         <= image_timestamp_intervals[1]
                     ):
-                        print(f"    timestamp {timestamp} is not in interval {image_timestamp_interval}: {filename_underscore}")
+                        print(f"    timestamp {timestamp} is not in interval {other.image_timestamp_interval}: {filename_underscore}")
                         continue
                     else:
-                        print(f"    timestamp {timestamp} is in interval {image_timestamp_interval}: {filename_underscore}")
+                        print(f"    timestamp {timestamp} is in interval {other.image_timestamp_interval}: {filename_underscore}")
 
             # saving file
             if filename_underscore != urllib.parse.unquote(filename_underscore):
                 print(f"WARNING:    {filename_underscore}|filename may not be unquoted: {filename_underscore}")
             if len(filename_underscore.encode('utf-8')) > FILENAME_LIMIT:
                 log_error(
                     config=config, to_stdout=True,
@@ -183,29 +178,29 @@
                         text=f"sha1 is {NULL} for {filename_underscore}, file may not in wiki site (probably deleted). "
                     )
             else:
                 # Delay(config=config, delay=config.delay + random.uniform(0, 1))
                 url = url_raw
 
                 r: Optional[requests.Response] = None
-                if ia_wbm_booster:
+                if other.ia_wbm_booster:
                     def get_ia_wbm_response() -> Optional[requests.Response]:
                         """ Get response from Internet Archive Wayback Machine
                         return None if not found / failed """
-                        if ia_wbm_booster in (WBM_EARLIEST, WBN_LATEST):
-                            ia_timestamp = ia_wbm_booster
-                        elif ia_wbm_booster == WBM_BEST:
+                        if other.ia_wbm_booster in (WBM_EARLIEST, WBN_LATEST):
+                            ia_timestamp = other.ia_wbm_booster
+                        elif other.ia_wbm_booster == WBM_BEST:
                             if timestamp != NULL:
                                 ia_timestamp = [x for x in timestamp if x.isdigit()][0:8]
                                 ia_timestamp = "".join(ia_timestamp)
                             else:
                                 print(f"ia_wbm_booster:    timestamp is {NULL}, use latest timestamp")
                                 ia_timestamp = 2
                         else:
-                            raise ValueError(f"ia_wbm_booster is {ia_wbm_booster}, but it should be 0, 1, 2 or 3")
+                            raise ValueError(f"ia_wbm_booster is {other.ia_wbm_booster}, but it should be 0, 1, 2 or 3")
 
                         available_api = "http://archive.org/wayback/available"
                         # TODO: cdx_api = "http://web.archive.org/cdx/search/cdx"
                         snap_url = f"https://web.archive.org/web/{ia_timestamp}id_/{url}"
 
                         try:
                             _r = ia_session.get(available_api, params={"url": url}, headers={"User-Agent": "wikiteam3"},
@@ -342,23 +337,26 @@
                     log_error(
                         config=config, to_stdout=True,
                         text=f"Failed to download '{filename_underscore}' with URL '{url}' due to HTTP '{r.status_code}', skipping"
                     )
 
             if not to_download: # skip printing
                 continue
-            print_msg = f"              | {len(images)}=>{filename_underscore[0:50]}"
-            print(print_msg, " "*(73 - len(print_msg)), end="\r")
+            if STDOUT_IS_TTY:
+                print_msg = f"              | {len(images)}=>{filename_underscore[0:50]}"
+                print(print_msg, " "*(73 - len(print_msg)), end="\r")
+            else:
+                print(f'{len(images)}=>{filename_underscore}')
 
         # NOTE: len(images) == 0 here
 
         patch_sess.release()
         print(f"Downloaded {c_savedImageFiles} files to 'images' dir")
         print(f"Downloaded {c_savedMismatchImageFiles} files to 'images_mismatch' dir")
-        if ia_wbm_booster and c_wbm_speedup_files:
+        if other.ia_wbm_booster and c_wbm_speedup_files:
             print(f"(WBM speedup: {c_wbm_speedup_files} files)")
 
 
     @staticmethod
     def get_image_names(config: Config, session: requests.Session):
         """Get list of image names"""
 
@@ -638,15 +636,15 @@
         else:
             print("    Found %d images" % (len(images)))
 
         return images
 
 
     @staticmethod
-    def save_image_names(config: Config, other: Dict, images: List[List]):
+    def save_image_names(config: Config, other: OtherConfig, images: List[List]):
         """Save image list in a file, including filename, url, uploader and other metadata"""
 
         images_filename = "{}-{}-images.txt".format(
             url2prefix_from_config(config=config), config.date
         )
         images_file = open(
             "{}/{}".format(config.path, images_filename), "w", encoding="utf-8"
@@ -673,21 +671,19 @@
             )
         images_file.write("--END--\n")
         images_file.close()
 
         print("Image metadata (images.txt) saved at:", images_filename)
         print(f"Estimated size of all images (images.txt): {c_images_size} bytes ({c_images_size/1024/1024/1024:.2f} GiB)")
 
-        assert_max_images: Optional[int] = other["assert_max_images"]
-        assert_max_images_bytes: Optional[int] = other["assert_max_images_bytes"]
         try:
-            assert len(images) <= assert_max_images if assert_max_images is not None else True
-            print(f"--assert_max_images: {assert_max_images}, passed")
-            assert c_images_size <= assert_max_images_bytes if assert_max_images_bytes is not None else True
-            print(f"--assert_max_images_bytes: {assert_max_images_bytes}, passed")
+            assert len(images) <= other.assert_max_images if other.assert_max_images is not None else True
+            print(f"--assert_max_images: {other.assert_max_images}, passed")
+            assert c_images_size <= other.assert_max_images_bytes if other.assert_max_images_bytes is not None else True
+            print(f"--assert_max_images_bytes: {other.assert_max_images_bytes}, passed")
         except AssertionError:
             import traceback
             traceback.print_exc()
             sys.exit(45)
 
 
     @staticmethod
```

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/index_php.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/index_php.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/site_info.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/site_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from typing import Optional
 
 import requests
 
 from wikiteam3.dumpgenerator.cli import Delay
 from wikiteam3.dumpgenerator.api import get_JSON
-from wikiteam3.dumpgenerator.config import Config
+from wikiteam3.dumpgenerator.config import Config, OtherConfig
 
 
 def save_siteinfo(config: Config, session: requests.Session):
     if os.path.exists("%s/siteinfo.json" % (config.path)):
         print("siteinfo.json exists, do not overwrite")
         return
 
@@ -21,26 +21,23 @@
     with open(
         "%s/siteinfo.json" % (config.path), "w", encoding="utf-8"
     ) as outfile:
         outfile.write(json.dumps(result, indent=4, sort_keys=True, ensure_ascii=False))
     Delay(config=config)
 
 
-def assert_siteinfo(result, other):
+def assert_siteinfo(result, other: OtherConfig):
     """ assert_max_edits, assert_max_pages, assert_max_images """
-    assert_max_edits: Optional[int] = other["assert_max_edits"]
-    assert_max_pages: Optional[int] = other["assert_max_pages"]
-    assert_max_images: Optional[int] = other["assert_max_images"]
 
     stats = result["query"]["statistics"] if "query" in result else result["statistics"]
 
     try:
-        assert stats["pages"] <= assert_max_pages if assert_max_pages is not None else True
-        assert stats["images"] <= assert_max_images if assert_max_images is not None else True
-        assert stats["edits"] <= assert_max_edits if assert_max_edits is not None else True
+        assert stats["pages"] <= other.assert_max_pages if other.assert_max_pages is not None else True
+        assert stats["images"] <= other.assert_max_images if other.assert_max_images is not None else True
+        assert stats["edits"] <= other.assert_max_edits if other.assert_max_edits is not None else True
     except AssertionError:
         import traceback
         traceback.print_exc()
         sys.exit(45)
 
 
 def get_siteinfo(config: Config, session: requests.Session):
```

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/special_logs.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_logs.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/misc/special_version.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_version.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/dumpgenerator/exceptions.py` & `wikiteam3-4.2.5/wikiteam3/dumpgenerator/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/uploader/compresser.py` & `wikiteam3-4.2.5/wikiteam3/uploader/compresser.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/uploader/socketLock.py` & `wikiteam3-4.2.5/wikiteam3/uploader/socketLock.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/uploader/uploader.py` & `wikiteam3-4.2.5/wikiteam3/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/ia_checker.py` & `wikiteam3-4.2.5/wikiteam3/utils/ia_checker.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/identifier.py` & `wikiteam3-4.2.5/wikiteam3/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/login/__init__.py` & `wikiteam3-4.2.5/wikiteam3/utils/login/__init__.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/login/api.py` & `wikiteam3-4.2.5/wikiteam3/utils/login/api.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/login/index.py` & `wikiteam3-4.2.5/wikiteam3/utils/login/index.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/monkey_patch.py` & `wikiteam3-4.2.5/wikiteam3/utils/monkey_patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import ssl
-import sys
 import time
 from typing import Optional
 import warnings
 
 import requests
 import requests.adapters
 from urllib3.util import create_urllib3_context
@@ -85,18 +84,19 @@
         )
 
 class SessionMonkeyPatch:
     """
     Monkey patch `requests.Session.send`
     """
     hijacked = False
-    def __init__(self,*, session: requests.Session, config: Config,
+    def __init__(self,*, session: requests.Session, config: Optional[Config]=None,
                  add_delay: bool=False, delay_msg: Optional[str]=None,
                  hard_retries: int=0,
-                 free_timeout_connections: bool=True, vaild_lft_sec: int=60 * 3
+                 free_timeout_connections: bool=True, vaild_lft_sec: int=60 * 3,
+                 accept_encoding: str="",
         ):
         """
         hard_retries: hard retries, default 0 (no retry)
         free_timeout_connections: regularly(`vaild_lft_sec`) clear connections pool
         """
 
         self.session = session
@@ -107,14 +107,16 @@
 
         self.hard_retries = hard_retries
 
         self.free_timeout_connections: bool = free_timeout_connections
         self.vaild_lft_sec = vaild_lft_sec
         self.last_clear_time = time.time()
 
+        self.accept_encoding = accept_encoding
+
     def clear_timeouted_pools(self):
         for adapter in self.session.adapters.values():
             adapter: requests.adapters.HTTPAdapter
             if adapter.poolmanager.pools._container.__len__() > 0 and \
                 time.time() - self.last_clear_time > self.vaild_lft_sec:
                 # TODO: logging this
                 # print('Keep-alived timeout: %d' % adapter.poolmanager.pools._container.__len__(), "connection(s) dropped.")
@@ -123,36 +125,57 @@
 
     def hijack(self):
         ''' Don't forget to call `release()` '''
 
         # Monkey patch `requests.Session.send`
         self.old_send_method = self.session.send
 
-        def new_send(request, **kwargs):
+        def new_send(request: requests.PreparedRequest, **kwargs):
             hard_retries_left = self.hard_retries + 1
             if hard_retries_left <= 0:
                 raise ValueError('hard_retries must be positive')
 
+            accept_encoding = ''
+
             while hard_retries_left > 0:
                 try:
                     if self.add_delay:
                         Delay(msg=self.delay_msg, config=self.config)
 
                     if self.free_timeout_connections:
                         self.clear_timeouted_pools()
 
+                    if _accept_encoding := accept_encoding or self.accept_encoding or request.headers.get("Accept-Encoding", ""):
+                        request.headers["Accept-Encoding"] = _accept_encoding
+
                     return self.old_send_method(request, **kwargs)
                 except (KeyboardInterrupt, requests.exceptions.ContentDecodingError): # don't retry
                     raise
                 except Exception as e:
                     hard_retries_left -= 1
                     if hard_retries_left <= 0:
                         raise
 
                     print('Hard retry... (%d), due to: %s' % (hard_retries_left, e))
+
+                    # workaround for https://wiki.erischan.org/index.php/Main_Page and other ChunkedEncodingError sites
+                    if isinstance(e, requests.exceptions.ChunkedEncodingError):
+                        accept_encoding = 'identity'
+                        print('retry with Accept-Encoding:', accept_encoding)
+
+                    # if --bypass-cdn-image-compression is enabled, retry with different url
+                    assert isinstance(request.url, str)
+                    if '_wikiteam3_nocdn=' in request.url:
+                        request.url = request.url.replace('_wikiteam3_nocdn=init_req', f'_wikiteam3_nocdn=retry_{hard_retries_left}')
+                        request.url = request.url.replace(
+                            f'_wikiteam3_nocdn=retry_{hard_retries_left + 1}',
+                            f'_wikiteam3_nocdn=retry_{hard_retries_left}'
+                            )
+                        print('--bypass-cdn-image-compression: change url to', request.url, 'on hard retry...')
+
                     time.sleep(3)
 
         self.session.send = new_send # type: ignore
         self.hijacked = True
 
     def release(self):
         ''' Undo monkey patch '''
```

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/user_agent.py` & `wikiteam3-4.2.5/wikiteam3/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/util.py` & `wikiteam3-4.2.5/wikiteam3/utils/util.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.4/wikiteam3/utils/wiki_avoid.py` & `wikiteam3-4.2.5/wikiteam3/utils/wiki_avoid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import re
 import sys
-from typing import Dict
 
-from wikiteam3.dumpgenerator.config import Config
+from wikiteam3.dumpgenerator.config import Config, OtherConfig
 
-def avoid_WikiMedia_projects(config: Config=None, other: Dict=None):
+def avoid_WikiMedia_projects(config: Config, other: OtherConfig):
     """Skip Wikimedia projects and redirect to the dumps website"""
 
     # notice about wikipedia dumps
     url = ""
     if config.api:
         url = url + config.api
     if config.index:
         url = url + config.index
     if re.findall(
         r"(?i)(wikipedia|wikisource|wiktionary|wikibooks|wikiversity|wikimedia|wikispecies|wikiquote|wikinews|wikidata|wikivoyage)\.org",
         url,
     ):
         print("PLEASE, DO NOT USE THIS SCRIPT TO DOWNLOAD WIKIMEDIA PROJECTS!")
         print("Download the dumps from http://dumps.wikimedia.org")
-        if not other["force"]:
+        if not other.force:
             print("Thanks!")
             sys.exit(2)
```

