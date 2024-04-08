# Comparing `tmp/sqlmap-1.8.3.tar.gz` & `tmp/sqlmap-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlmap-1.8.3.tar", last modified: Fri Mar  1 10:22:25 2024, max compression
+gzip compressed data, was "dist/sqlmap-1.8.4.tar", last modified: Mon Apr  8 08:49:45 2024, max compression
```

## Comparing `sqlmap-1.8.3.tar` & `sqlmap-1.8.4.tar`

### file list

```diff
@@ -1,780 +1,781 @@
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28978 2024-03-01 10:22:24.000000 sqlmap-1.8.3/MANIFEST.in
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4952 2024-03-01 10:22:25.000000 sqlmap-1.8.3/PKG-INFO
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5308 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/README.md
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/wininetpton/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      319 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/wininetpton/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2775 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/wininetpton/win_inet_pton.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/clientform/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   126727 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/clientform/clientform.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/clientform/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/multipart/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4513 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/multipart/multipartpost.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/multipart/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/socks/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17437 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/socks/socks.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/socks/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1401 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/socks/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10510 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/escsm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3749 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/eucjpprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2766 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/utf8prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11102 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langturkishmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5110 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/charsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3413 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/mbcharsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13546 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/euckrfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/version.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1754 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/gb2312prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/cp949prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9411 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/chardistribution.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1661 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/enums.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11345 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langhebrewmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12688 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langgreekmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3950 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/escprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3590 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/codingstatemachine.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31621 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/euctwfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5370 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/latin1prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12839 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langbulgarianmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31254 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/big5freq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1748 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/euckrprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25777 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/jisfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1757 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/big5prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25481 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/mbcssm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12485 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/universaldetector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    20715 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/gb2312freq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3774 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/sjisprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1134 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/compat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3546 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/sbcsgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1559 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3787 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/charsetgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19643 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/jpcntx.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17948 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langcyrillicmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12592 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langhungarianmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1747 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/euctwprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/sbcharsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2012 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/mbcsgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11290 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/langthaimodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13838 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/chardet/hebrewprober.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/odict/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4283 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/odict/ordereddict.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      156 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/odict/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/keepalive/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      730 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/keepalive/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22807 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/keepalive/keepalive.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/magic/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6723 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/magic/magic.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/magic/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/ansistrm/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5329 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/ansistrm/ansistrm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/ansistrm/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/identywaf/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25913 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/identywaf/identYwaf.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61564 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/identywaf/data.json
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      270 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/identywaf/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1078 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/identywaf/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/prettyprint/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1357 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/prettyprint/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4215 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/prettyprint/prettyprint.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/bottle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   170898 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/bottle/bottle.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        5 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/bottle/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/fcrypt/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/fcrypt/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26757 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/fcrypt/fcrypt.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/pydes/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27500 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/pydes/pyDes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      720 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/pydes/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/beautifulsoup/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80038 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1673 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/beautifulsoup/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/six/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34581 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/six/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/termcolor/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/termcolor/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5246 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/termcolor/termcolor.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2524 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/ansi.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2065 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/initialise.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6356 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/winterm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      240 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10243 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/ansitowin32.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5365 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/thirdparty/colorama/win32.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    16703 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/.pylintrc
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/procs/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      269 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/create_new_xp_cmdshell.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      246 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/configure_openrowset.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/disable_xp_cmdshell_2000.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       70 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/enable_xp_cmdshell_2000.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      163 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/activate_sp_oacreate.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      333 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/run_statement_as_user.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      197 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/dns_request.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      236 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mssqlserver/configure_xp_cmdshell.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      187 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/procs/postgresql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      536 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/postgresql/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/procs/mysql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       73 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mysql/write_file_limit.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       85 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/mysql/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/procs/oracle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2010 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/oracle/read_file_export_extension.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      397 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/procs/oracle/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.1/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.5/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/12/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3257 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/11/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2563 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2561 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2562 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/10/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.1/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2729 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.5/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/11/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2020 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2018 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2016 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/10/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4231 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4773 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4755 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4766 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/64/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3200 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/32/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2512 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/64/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5267 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/32/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4549 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/shell/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/shell/stagers/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      379 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.php_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.asp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      529 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.aspx_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1321 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.jsp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      686 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/shell/backdoors/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      243 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/backdoors/backdoor.asp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      469 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/backdoors/backdoor.php_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      417 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/backdoors/backdoor.aspx_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      359 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/shell/backdoors/backdoor.jsp_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/txt/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68896 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/smalldict.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18539 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/common-outputs.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    44074 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/common-tables.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   399831 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/user-agents.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48329 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/common-files.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14646 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/keywords.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26013 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/common-columns.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)  6076425 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/txt/wordlist.tx_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/html/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5763 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/html/index.html
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/xml/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9507 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/errors.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19304 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/union_query.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5482 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/inline_query.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68050 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/error_based.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    79693 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/time_blind.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24754 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/stacked_queries.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    60087 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/payloads/boolean_blind.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   141162 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/queries.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/sharepoint.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1649 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/x-powered-by.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1448 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/set-cookie.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      233 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/x-aspnet-version.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   101453 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/mssql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      805 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/servlet-engine.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3897 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/generic.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      327 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/postgresql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31443 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/server.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      158 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/oracle.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2956 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/banner/mysql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15092 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/data/xml/boundaries.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/tamper/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1879 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/between.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/symboliclogical.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/misunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      753 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/schemasplit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      906 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/dunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1127 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/least.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1211 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/substring2leftright.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1007 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/concat2concatws.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3046 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/luanginx.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      944 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/apostrophemask.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2589 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2mssqlblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      700 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/0eunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1197 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/randomcomments.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1802 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/plus2concat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      963 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/varnish.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1314 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/multiplespaces.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1597 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/versionedkeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2mssqlhash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      639 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/informationschemacomment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/ord2ascii.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1737 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/versionedmorekeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      523 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/apostrophenullencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1413 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/percentage.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      825 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/sp_password.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      766 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/equaltorlike.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2250 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/plus2fnconcat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/halfversionedmorekeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2morecomment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/modsecurityzeroversioned.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1135 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/greatest.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1290 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/bluecoat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1065 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/uppercase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1584 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2hash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1455 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/overlongutf8more.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      680 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/decentities.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1264 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2dash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1292 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/modsecurityversioned.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      715 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/hexentities.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1388 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/charencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/equaltolike.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1218 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/chardoubleencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      985 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/scientific.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1351 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2comment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1306 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/unmagicquotes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1285 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/xforwardedfor.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1282 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2plus.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1215 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/charunicodeescape.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      511 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/unionalltounion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2218 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2morehash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1744 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/ifnull2casewhenisnull.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      468 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/escapequotes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/ifnull2ifisnull.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      758 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/commentbeforeparentheses.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      868 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/sleep2getlock.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1002 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/lowercase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1225 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/commalessmid.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/charunicodeencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1168 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2mysqldash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1377 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/hex2char.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1736 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/randomcase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1000 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/appendnullbyte.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      519 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/base64encode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1663 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2randomblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/binary.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2113 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/if2case.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1444 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/overlongutf8.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1977 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/space2mysqlblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      849 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/htmlencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      970 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/tamper/commalesslimit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      258 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25751 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/sqlmap.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/doc/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34109 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/CHANGELOG.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25122 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/THANKS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      190 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/AUTHORS
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/doc/translations/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3281 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-it-IT.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4227 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-uk-UA.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3289 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-ko-KR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3149 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-rs-RS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4882 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-in-HI.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3786 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-fa-IR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4092 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-bg-BG.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4218 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-ru-RU.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3138 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-id-ID.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3332 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-fr-FR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3175 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-pt-BR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3180 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-hr-HR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3167 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-nl-NL.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3240 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-sk-SK.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3561 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-vi-VN.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3226 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-pl-PL.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4248 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-gr-GR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2921 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-zh-CN.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3609 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-ja-JP.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6026 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-ka-GE.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3029 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-tr-TR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3184 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-de-DE.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3435 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/translations/README-es-MX.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14763 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/doc/THIRD-PARTY.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22364 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/sqlmap.conf
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18886 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/generic/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2654 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2484 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5055 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/custom.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    30708 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/entries.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27907 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/search.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1730 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18208 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29216 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/users.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1723 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6887 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/misc.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    54885 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/databases.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12371 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/generic/filesystem.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1701 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2204 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5279 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/presto/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1445 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2784 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5276 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2537 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18049 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2583 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      889 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6499 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6913 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      950 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17312 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2525 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2130 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      670 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1011 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5843 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      919 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      691 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/access/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2609 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      520 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1035 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      703 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/raima/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1322 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1830 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      995 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2636 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      907 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/derby/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2397 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3135 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      900 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cache/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      459 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1920 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      689 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2992 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1080 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1151 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4990 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1103 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1894 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2549 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9202 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3792 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1858 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      807 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2591 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      428 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1016 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5448 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1304 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3005 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      265 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2095 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1044 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5124 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12785 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1113 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7731 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1022 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1902 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1272 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3284 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/informix/filesystem.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      589 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2657 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2427 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2673 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2371 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      503 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2590 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      669 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      615 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1935 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5871 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      880 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/db2/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1835 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      726 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2541 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1580 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      500 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3324 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      869 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      663 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/h2/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6002 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2817 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      886 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1101 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3880 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2301 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      632 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2538 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11670 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2558 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      638 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/enumeration.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/connector.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      687 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/syntax.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      987 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/takeover.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2627 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/fingerprint.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      950 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      679 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2054 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3083 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      644 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3176 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1541 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2517 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      923 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2613 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/controller/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8896 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/controller/handler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7233 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/controller/action.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    75900 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/controller/checks.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/controller/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    36817 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/controller/controller.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/utils/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7984 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/search.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4686 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/httpd.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48979 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/hash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2325 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/getch.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5207 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/sqlalchemy.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8450 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/hashdb.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2935 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/xrange.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/versioncheck.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3337 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/progress.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2674 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/purge.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10977 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/crawler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8030 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/har.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15901 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/brute.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7369 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/pivotdumptable.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34342 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/api.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3190 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/safe2bin.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1111 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/timeout.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5564 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/deps.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18275 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/utils/sgmllib.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/request/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18899 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/basic.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6017 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/dns.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3229 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/direct.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8399 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/redirecthandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      942 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/rangehandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/methodrequest.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5815 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/httpshandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      633 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/templates.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1384 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/basicauthhandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1566 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/chunkedhandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1158 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/pkihandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24808 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/inject.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80562 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/connect.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7788 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/request/comparison.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/techniques/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/techniques/error/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    21157 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/error/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/error/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/techniques/dns/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5061 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/dns/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1125 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/dns/test.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/dns/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/techniques/blind/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/blind/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34684 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/blind/inference.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/techniques/union/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    23147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/union/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18664 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/union/test.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/techniques/union/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/core/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      728 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/data.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5865 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/patch.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1800 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/readlineng.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28848 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/dump.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8414 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/threads.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13586 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/convert.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13936 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/enums.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2634 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/decorators.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6032 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/bigarray.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/gui.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/exception.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15220 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/testing.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7536 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/optiondict.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34190 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/target.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1980 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/session.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    59654 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/agent.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   106617 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/option.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    45517 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap/lib/core/settings.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8986 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/compat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/subprocessng.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1876 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/revision.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      885 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/profiling.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/defaults.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5489 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/log.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4956 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/shell.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17637 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/dicts.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3201 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/wordlist.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      988 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/unescaper.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7468 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/update.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5046 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/replication.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6646 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/datatype.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   193937 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/core/common.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/takeover/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8440 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/abstraction.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13903 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/udf.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28240 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/metasploit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11839 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/xp_cmdshell.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3838 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/registry.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18315 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/web.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4739 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/takeover/icmpsh.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/lib/parse/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    50151 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/cmdline.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2703 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/handler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3578 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/payloads.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3498 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/configfile.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1460 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/headers.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1805 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/sitemap.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3580 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/banner.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3022 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/lib/parse/html.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6215 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/sqlmapapi.yaml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/cloak/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2286 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/cloak/cloak.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      732 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/cloak/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/cloak/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/shutils/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      305 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/modernize.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      797 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/duplicates.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     1317 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/precommit-hook.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      332 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/pycodestyle.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      660 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/drei.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/blanks.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      235 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/pylint.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     5861 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/pypi.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      630 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/recloak.sh
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/newlines.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      869 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/strip.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      245 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/junk.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      311 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/autocompletion.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      313 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/pydiatra.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      875 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/postcommit-hook.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      320 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shutils/pyflakes.sh
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      193 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      883 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd.sln
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      271 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1348 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      516 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/stdafx.h
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4508 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      293 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/stdafx.cpp
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    37206 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/runcmd/runcmd.exe_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/beep/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2901 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/beep/beep.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/beep/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    46772 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/beep/beep.wav
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/linux/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1691 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1927 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/windows/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2758 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3965 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh-m.c
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7009 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh.exe_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9342 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh-s.c
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1641 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2136 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh-m.pl
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      872 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4809 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh_m.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/dbgtool/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2475 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/dbgtool/dbgtool.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      549 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/dbgtool/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/dbgtool/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap/extra/vulnserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9127 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/vulnserver/vulnserver.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/extra/vulnserver/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     4229 2024-03-01 10:22:19.000000 sqlmap-1.8.3/sqlmap/sqlmapapi.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       38 2024-03-01 10:22:25.000000 sqlmap-1.8.3/setup.cfg
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3193 2024-03-01 10:22:24.000000 sqlmap-1.8.3/README.rst
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap.egg-info/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24143 2024-03-01 10:22:25.000000 sqlmap-1.8.3/sqlmap.egg-info/SOURCES.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4952 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap.egg-info/PKG-INFO
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        7 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap.egg-info/top_level.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap.egg-info/not-zip-safe
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap.egg-info/entry_points.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-03-01 10:22:24.000000 sqlmap-1.8.3/sqlmap.egg-info/dependency_links.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1549 2024-03-01 10:22:22.000000 sqlmap-1.8.3/setup.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29017 2024-04-08 08:49:36.000000 sqlmap-1.8.4/MANIFEST.in
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4946 2024-04-08 08:49:45.000000 sqlmap-1.8.4/PKG-INFO
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5302 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/README.md
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      319 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2775 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/win_inet_pton.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/clientform/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   126727 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/clientform/clientform.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/clientform/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/multipart/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4513 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/multipart/multipartpost.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/multipart/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17437 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/socks.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1401 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10510 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/escsm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3749 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/eucjpprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2766 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/utf8prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11102 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langturkishmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5110 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3413 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcharsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13546 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/version.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1754 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/cp949prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9411 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/chardistribution.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1661 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/enums.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11345 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhebrewmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12688 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langgreekmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3950 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/escprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/codingstatemachine.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31621 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5370 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/latin1prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12839 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31254 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5freq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1748 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25777 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/jisfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1757 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25481 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcssm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12485 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/universaldetector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    20715 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312freq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3774 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/sjisprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1134 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/compat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3546 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1559 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3787 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19643 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/jpcntx.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17948 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langcyrillicmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12592 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhungarianmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1747 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcharsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2012 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11290 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langthaimodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13838 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/hebrewprober.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/odict/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4283 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/odict/ordereddict.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      156 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/odict/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/keepalive/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      730 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/keepalive/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22807 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/keepalive/keepalive.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/magic/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6723 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/magic/magic.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/magic/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5329 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/ansistrm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25913 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/identYwaf.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61564 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/data.json
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      270 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1078 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1357 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4215 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/prettyprint.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/bottle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   170898 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/bottle/bottle.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        5 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/bottle/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26757 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/fcrypt.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/pydes/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27500 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/pydes/pyDes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      720 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/pydes/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80038 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1673 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/six/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34581 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/six/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/termcolor/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/termcolor/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5246 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/termcolor/termcolor.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2524 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansi.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2065 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/initialise.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6356 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/winterm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      240 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10243 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansitowin32.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5365 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/win32.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    16703 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/.pylintrc
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      269 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/create_new_xp_cmdshell.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      246 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/configure_openrowset.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/disable_xp_cmdshell_2000.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       70 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/enable_xp_cmdshell_2000.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      163 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/activate_sp_oacreate.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      333 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/run_statement_as_user.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      197 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/dns_request.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      236 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/configure_xp_cmdshell.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      187 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/postgresql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      536 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/postgresql/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/mysql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       73 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mysql/write_file_limit.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       85 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mysql/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/oracle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2010 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/oracle/read_file_export_extension.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      397 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/oracle/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.1/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/12/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3257 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/11/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2563 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2561 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2562 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/10/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.6/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.1/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2729 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/11/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2020 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2018 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2016 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/10/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.6/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4231 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4773 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4755 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4766 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/64/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3200 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/32/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2512 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/64/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5267 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/32/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4549 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/shell/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      379 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.php_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.asp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      529 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.aspx_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1321 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.jsp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      686 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      243 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.asp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      469 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.php_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      417 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.aspx_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      359 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.jsp_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/txt/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68896 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/smalldict.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18539 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-outputs.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    44074 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-tables.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   399831 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/user-agents.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61005 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/sha256sums.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48329 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-files.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/keywords.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26013 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-columns.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)  6076425 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/wordlist.tx_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/html/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5763 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/html/index.html
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/xml/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/errors.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19304 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/union_query.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5482 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/inline_query.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68050 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/error_based.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    79693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/time_blind.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24754 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/stacked_queries.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    60087 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/boolean_blind.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   141162 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/queries.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/sharepoint.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1649 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/x-powered-by.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1448 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/set-cookie.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      233 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/x-aspnet-version.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   101453 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/mssql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      805 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/servlet-engine.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3897 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/generic.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      327 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/postgresql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31443 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/server.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      158 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/oracle.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2956 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/mysql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15092 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/boundaries.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/tamper/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1879 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/between.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/symboliclogical.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/misunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      753 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/schemasplit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      906 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/dunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1127 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/least.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1211 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/substring2leftright.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1007 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/concat2concatws.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3046 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/luanginx.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      944 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/apostrophemask.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2589 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mssqlblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      700 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/0eunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1197 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/randomcomments.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1802 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/plus2concat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      963 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/varnish.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1314 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/multiplespaces.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1597 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/versionedkeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mssqlhash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      639 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/informationschemacomment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/ord2ascii.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1737 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/versionedmorekeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      523 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/apostrophenullencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1413 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/percentage.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      825 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/sp_password.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      766 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/equaltorlike.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2250 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/plus2fnconcat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/halfversionedmorekeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2morecomment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/modsecurityzeroversioned.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1135 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/greatest.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1290 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/bluecoat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1065 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/uppercase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1584 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2hash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1455 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/overlongutf8more.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      680 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/decentities.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1264 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2dash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1292 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/modsecurityversioned.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      715 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/hexentities.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1388 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/charencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/equaltolike.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1218 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/chardoubleencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      985 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/scientific.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1351 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2comment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1306 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/unmagicquotes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1285 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/xforwardedfor.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1282 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2plus.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1215 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/charunicodeescape.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      511 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/unionalltounion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2218 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2morehash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1744 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/ifnull2casewhenisnull.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      468 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/escapequotes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/ifnull2ifisnull.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      758 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/commentbeforeparentheses.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      868 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/sleep2getlock.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1002 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/lowercase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1225 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/commalessmid.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/charunicodeencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1168 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mysqldash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1377 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/hex2char.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1736 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/randomcase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1000 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/appendnullbyte.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      519 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/base64encode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1663 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2randomblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/binary.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2113 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/if2case.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1444 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/overlongutf8.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1977 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mysqlblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      849 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/htmlencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      970 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/commalesslimit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      258 2024-04-08 08:49:36.000000 sqlmap-1.8.4/sqlmap/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25734 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmap.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/doc/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34109 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/CHANGELOG.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25122 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/THANKS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      190 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/AUTHORS
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/doc/translations/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3275 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-it-IT.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4221 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-uk-UA.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3289 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ko-KR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3143 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-rs-RS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4882 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-in-HI.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3786 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-fa-IR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4086 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-bg-BG.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4212 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ru-RU.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3132 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-id-ID.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3326 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-fr-FR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3169 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-pt-BR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3174 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-hr-HR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3161 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-nl-NL.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3234 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-sk-SK.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3555 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-vi-VN.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3220 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-pl-PL.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4242 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-gr-GR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2951 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-zh-CN.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3603 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ja-JP.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6020 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ka-GE.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3023 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-tr-TR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3178 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-de-DE.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-es-MX.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14763 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/THIRD-PARTY.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22364 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmap.conf
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18886 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/generic/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2654 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2484 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5055 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/custom.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    30708 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/entries.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27907 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/search.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1730 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18208 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29216 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/users.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1723 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6887 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/misc.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    54885 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/databases.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12371 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/filesystem.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1701 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2204 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5279 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1445 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2784 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5276 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2537 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18049 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2583 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      889 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6499 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6913 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      950 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17312 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2525 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2130 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      670 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1011 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5843 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      919 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      691 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2609 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      520 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1035 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      703 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1322 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1830 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      995 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2636 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      907 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2397 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3135 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      900 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      459 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      689 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2992 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1080 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1151 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4990 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1103 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1894 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2549 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9202 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3792 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1858 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      807 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2591 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      428 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1016 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5448 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1304 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3005 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      265 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2095 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1044 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5124 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12785 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1113 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7731 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1022 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1902 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1272 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3284 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/filesystem.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      589 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2657 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2427 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2673 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2371 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      503 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      669 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      615 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1935 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5871 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      880 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1835 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      726 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2541 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1580 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      500 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3324 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      869 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      663 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6002 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2817 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      886 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1101 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3880 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2301 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      632 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2538 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11670 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2558 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      638 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/enumeration.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/connector.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/syntax.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      987 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/takeover.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2627 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/fingerprint.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      950 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      679 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2054 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3083 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      644 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3176 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1541 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2517 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      923 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2613 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/controller/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8896 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/handler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7233 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/action.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    75900 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/checks.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    36817 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/controller.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/utils/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7984 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/search.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4686 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/httpd.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/hash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2325 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/getch.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5207 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/sqlalchemy.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8450 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/hashdb.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2935 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/xrange.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/versioncheck.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3337 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/progress.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2674 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/purge.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10977 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/crawler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8030 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/har.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15901 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/brute.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7369 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/pivotdumptable.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34389 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/api.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3190 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/safe2bin.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1111 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/timeout.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5564 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/deps.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18275 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/sgmllib.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/request/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/basic.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6017 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/dns.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3229 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/direct.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8399 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/redirecthandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      942 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/rangehandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/methodrequest.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5815 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/httpshandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/templates.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1384 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/basicauthhandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1566 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/chunkedhandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1158 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/pkihandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24808 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/inject.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80509 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/connect.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7788 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/comparison.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/error/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    21157 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/error/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/error/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5061 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1125 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/test.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/blind/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/blind/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34684 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/blind/inference.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    23147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18664 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/test.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/core/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      728 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/data.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5865 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/patch.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1800 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/readlineng.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28848 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/dump.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8414 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/threads.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13586 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/convert.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13936 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/enums.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2634 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/decorators.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6032 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/bigarray.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/gui.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/exception.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15220 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/testing.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7536 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/optiondict.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34190 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/target.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1980 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/session.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    59654 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/agent.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   106570 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/option.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    45400 2024-04-08 08:49:36.000000 sqlmap-1.8.4/sqlmap/lib/core/settings.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8986 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/compat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/subprocessng.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1876 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/revision.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      885 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/profiling.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/defaults.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5489 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/log.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4956 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/shell.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17637 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/dicts.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3201 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/wordlist.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      988 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/unescaper.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7468 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/update.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5046 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/replication.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/datatype.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   195050 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/common.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/takeover/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8440 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/abstraction.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13903 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/udf.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28240 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/metasploit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11839 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/xp_cmdshell.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3838 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/registry.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18315 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/web.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4739 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/icmpsh.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/parse/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    50151 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/cmdline.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2703 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/handler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3578 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/payloads.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3498 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/configfile.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1460 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/headers.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1805 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/sitemap.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3580 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/banner.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3022 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/html.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6215 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmapapi.yaml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/cloak/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2286 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/cloak/cloak.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      732 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/cloak/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/cloak/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shutils/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      305 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/modernize.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      797 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/duplicates.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     1368 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/precommit-hook.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      332 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pycodestyle.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      660 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/drei.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/blanks.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      235 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pylint.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     5855 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pypi.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      630 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/recloak.sh
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/newlines.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      869 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/strip.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      245 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/junk.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      311 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/autocompletion.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      313 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pydiatra.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      875 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/postcommit-hook.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      320 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pyflakes.sh
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      193 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      883 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd.sln
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      271 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1348 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      516 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/stdafx.h
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4508 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      293 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/stdafx.cpp
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    37206 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/runcmd.exe_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/beep/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2901 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/beep/beep.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/beep/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    46772 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/beep/beep.wav
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1691 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1927 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/windows/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2758 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3965 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.c
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7009 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh.exe_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9342 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-s.c
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1641 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2136 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.pl
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      872 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4809 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh_m.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2475 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/dbgtool.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      549 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/vulnserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9127 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/vulnserver/vulnserver.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/vulnserver/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     4229 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmapapi.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       38 2024-04-08 08:49:45.000000 sqlmap-1.8.4/setup.cfg
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3187 2024-04-08 08:49:36.000000 sqlmap-1.8.4/README.rst
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24174 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4946 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/PKG-INFO
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        7 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/top_level.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/not-zip-safe
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/entry_points.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1549 2024-04-08 08:49:34.000000 sqlmap-1.8.4/setup.py
```

### Comparing `sqlmap-1.8.3/MANIFEST.in` & `sqlmap-1.8.4/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 include sqlmap/data/shell/backdoors/backdoor.php_
 include sqlmap/data/shell/backdoors/backdoor.aspx_
 include sqlmap/data/shell/backdoors/backdoor.jsp_
 include sqlmap/data/txt/smalldict.txt
 include sqlmap/data/txt/common-outputs.txt
 include sqlmap/data/txt/common-tables.txt
 include sqlmap/data/txt/user-agents.txt
+include sqlmap/data/txt/sha256sums.txt
 include sqlmap/data/txt/common-files.txt
 include sqlmap/data/txt/keywords.txt
 include sqlmap/data/txt/common-columns.txt
 include sqlmap/data/txt/wordlist.tx_
 include sqlmap/data/html/index.html
 include sqlmap/data/xml/errors.xml
 include sqlmap/data/xml/payloads/union_query.xml
```

### Comparing `sqlmap-1.8.3/PKG-INFO` & `sqlmap-1.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlmap
-Version: 1.8.3
+Version: 1.8.4
 Summary: Automatic SQL injection and database takeover tool
 Home-page: https://sqlmap.org
 Author: Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar
 Author-email: bernardo@sqlmap.org, miroslav@sqlmap.org
 License: GNU General Public License v2 (GPLv2)
-Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.3.zip
+Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.4.zip
 Project-URL: Source, https://github.com/sqlmapproject/sqlmap/
 Project-URL: Documentation, https://github.com/sqlmapproject/sqlmap/wiki
 Project-URL: Tracker, https://github.com/sqlmapproject/sqlmap/issues
 Description: sqlmap
         ======
         
         |Python 2.6|2.7|3.x| |License| |Twitter|
@@ -87,15 +87,15 @@
            or `.zip <https://github.com/sqlmapproject/sqlmap/zipball/master>`__
         -  Commits RSS feed:
            https://github.com/sqlmapproject/sqlmap/commits/master.atom
         -  Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
         -  User's manual: https://github.com/sqlmapproject/sqlmap/wiki
         -  Frequently Asked Questions (FAQ):
            https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-        -  Twitter: https://twitter.com/sqlmap
+        -  X: https://twitter.com/sqlmap
         -  Demos: http://www.youtube.com/user/inquisb/videos
         -  Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
         
         .. |Python 2.6|2.7|3.x| image:: https://img.shields.io/badge/python-2.6|2.7|3.x-yellow.svg
            :target: https://www.python.org/
         .. |License| image:: https://img.shields.io/badge/license-GPLv2-red.svg
            :target: https://raw.githubusercontent.com/sqlmapproject/sqlmap/master/LICENSE
```

### Comparing `sqlmap-1.8.3/sqlmap/README.md` & `sqlmap-1.8.4/sqlmap/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 * Homepage: https://sqlmap.org
 * Download: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Commits RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
 * User's manual: https://github.com/sqlmapproject/sqlmap/wiki
 * Frequently Asked Questions (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demos: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
 
 Translations
 ----
 
 * [Bulgarian](https://github.com/sqlmapproject/sqlmap/blob/master/doc/translations/README-bg-BG.md)
```

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/wininetpton/win_inet_pton.py` & `sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/win_inet_pton.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/clientform/clientform.py` & `sqlmap-1.8.4/sqlmap/thirdparty/clientform/clientform.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/multipart/multipartpost.py` & `sqlmap-1.8.4/sqlmap/thirdparty/multipart/multipartpost.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/socks/socks.py` & `sqlmap-1.8.4/sqlmap/thirdparty/socks/socks.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/socks/LICENSE` & `sqlmap-1.8.4/sqlmap/thirdparty/socks/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/escsm.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/eucjpprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/utf8prober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langturkishmodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/charsetprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/mbcharsetprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/euckrfreq.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/gb2312prober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/cp949prober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/chardistribution.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/enums.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langhebrewmodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langgreekmodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/escprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/codingstatemachine.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/euctwfreq.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/latin1prober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langbulgarianmodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/big5freq.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/euckrprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/jisfreq.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/big5prober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/mbcssm.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/universaldetector.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/gb2312freq.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/sjisprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/compat.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/sbcsgroupprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/charsetgroupprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/jpcntx.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langcyrillicmodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langhungarianmodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/euctwprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/sbcharsetprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/mbcsgroupprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/langthaimodel.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/chardet/hebrewprober.py` & `sqlmap-1.8.4/sqlmap/thirdparty/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/odict/ordereddict.py` & `sqlmap-1.8.4/sqlmap/thirdparty/odict/ordereddict.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/keepalive/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/keepalive/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/keepalive/keepalive.py` & `sqlmap-1.8.4/sqlmap/thirdparty/keepalive/keepalive.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/magic/magic.py` & `sqlmap-1.8.4/sqlmap/thirdparty/magic/magic.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/ansistrm/ansistrm.py` & `sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/ansistrm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/identywaf/identYwaf.py` & `sqlmap-1.8.4/sqlmap/thirdparty/identywaf/identYwaf.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/identywaf/data.json` & `sqlmap-1.8.4/sqlmap/thirdparty/identywaf/data.json`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/identywaf/LICENSE` & `sqlmap-1.8.4/sqlmap/thirdparty/identywaf/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/prettyprint/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/prettyprint/prettyprint.py` & `sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/prettyprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/bottle/bottle.py` & `sqlmap-1.8.4/sqlmap/thirdparty/bottle/bottle.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/fcrypt/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/fcrypt/fcrypt.py` & `sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/fcrypt.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/pydes/pyDes.py` & `sqlmap-1.8.4/sqlmap/thirdparty/pydes/pyDes.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/pydes/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/pydes/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py` & `sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/beautifulsoup/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/six/__init__.py` & `sqlmap-1.8.4/sqlmap/thirdparty/six/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/termcolor/termcolor.py` & `sqlmap-1.8.4/sqlmap/thirdparty/termcolor/termcolor.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/colorama/ansi.py` & `sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/colorama/initialise.py` & `sqlmap-1.8.4/sqlmap/thirdparty/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/colorama/winterm.py` & `sqlmap-1.8.4/sqlmap/thirdparty/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/colorama/ansitowin32.py` & `sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/thirdparty/colorama/win32.py` & `sqlmap-1.8.4/sqlmap/thirdparty/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/.pylintrc` & `sqlmap-1.8.4/sqlmap/.pylintrc`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/procs/postgresql/dns_request.sql` & `sqlmap-1.8.4/sqlmap/data/procs/postgresql/dns_request.sql`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/procs/oracle/read_file_export_extension.sql` & `sqlmap-1.8.4/sqlmap/data/procs/oracle/read_file_export_extension.sql`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_` & `sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_` & `sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_` & `sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.asp_` & `sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.asp_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.aspx_` & `sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.aspx_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/shell/stagers/stager.jsp_` & `sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.jsp_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/shell/README.txt` & `sqlmap-1.8.4/sqlmap/data/shell/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/smalldict.txt` & `sqlmap-1.8.4/sqlmap/data/txt/smalldict.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/common-outputs.txt` & `sqlmap-1.8.4/sqlmap/data/txt/common-outputs.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/common-tables.txt` & `sqlmap-1.8.4/sqlmap/data/txt/common-tables.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/user-agents.txt` & `sqlmap-1.8.4/sqlmap/data/txt/user-agents.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/common-files.txt` & `sqlmap-1.8.4/sqlmap/data/txt/common-files.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/keywords.txt` & `sqlmap-1.8.4/sqlmap/data/txt/keywords.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/common-columns.txt` & `sqlmap-1.8.4/sqlmap/data/txt/common-columns.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/txt/wordlist.tx_` & `sqlmap-1.8.4/sqlmap/data/txt/wordlist.tx_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/html/index.html` & `sqlmap-1.8.4/sqlmap/data/html/index.html`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/errors.xml` & `sqlmap-1.8.4/sqlmap/data/xml/errors.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/payloads/union_query.xml` & `sqlmap-1.8.4/sqlmap/data/xml/payloads/union_query.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/payloads/inline_query.xml` & `sqlmap-1.8.4/sqlmap/data/xml/payloads/inline_query.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/payloads/error_based.xml` & `sqlmap-1.8.4/sqlmap/data/xml/payloads/error_based.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/payloads/time_blind.xml` & `sqlmap-1.8.4/sqlmap/data/xml/payloads/time_blind.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/payloads/stacked_queries.xml` & `sqlmap-1.8.4/sqlmap/data/xml/payloads/stacked_queries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/payloads/boolean_blind.xml` & `sqlmap-1.8.4/sqlmap/data/xml/payloads/boolean_blind.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/queries.xml` & `sqlmap-1.8.4/sqlmap/data/xml/queries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/x-powered-by.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/x-powered-by.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/set-cookie.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/set-cookie.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/mssql.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/mssql.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/servlet-engine.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/servlet-engine.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/generic.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/generic.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/server.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/server.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/banner/mysql.xml` & `sqlmap-1.8.4/sqlmap/data/xml/banner/mysql.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/data/xml/boundaries.xml` & `sqlmap-1.8.4/sqlmap/data/xml/boundaries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/between.py` & `sqlmap-1.8.4/sqlmap/tamper/between.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/symboliclogical.py` & `sqlmap-1.8.4/sqlmap/tamper/symboliclogical.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/misunion.py` & `sqlmap-1.8.4/sqlmap/tamper/misunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/schemasplit.py` & `sqlmap-1.8.4/sqlmap/tamper/schemasplit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/dunion.py` & `sqlmap-1.8.4/sqlmap/tamper/dunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/least.py` & `sqlmap-1.8.4/sqlmap/tamper/least.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/substring2leftright.py` & `sqlmap-1.8.4/sqlmap/tamper/substring2leftright.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/concat2concatws.py` & `sqlmap-1.8.4/sqlmap/tamper/concat2concatws.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/luanginx.py` & `sqlmap-1.8.4/sqlmap/tamper/luanginx.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/apostrophemask.py` & `sqlmap-1.8.4/sqlmap/tamper/apostrophemask.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2mssqlblank.py` & `sqlmap-1.8.4/sqlmap/tamper/space2mssqlblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/0eunion.py` & `sqlmap-1.8.4/sqlmap/tamper/0eunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/randomcomments.py` & `sqlmap-1.8.4/sqlmap/tamper/randomcomments.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/plus2concat.py` & `sqlmap-1.8.4/sqlmap/tamper/plus2concat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/varnish.py` & `sqlmap-1.8.4/sqlmap/tamper/varnish.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/multiplespaces.py` & `sqlmap-1.8.4/sqlmap/tamper/multiplespaces.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/versionedkeywords.py` & `sqlmap-1.8.4/sqlmap/tamper/versionedkeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2mssqlhash.py` & `sqlmap-1.8.4/sqlmap/tamper/space2mssqlhash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/informationschemacomment.py` & `sqlmap-1.8.4/sqlmap/tamper/informationschemacomment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/ord2ascii.py` & `sqlmap-1.8.4/sqlmap/tamper/ord2ascii.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/versionedmorekeywords.py` & `sqlmap-1.8.4/sqlmap/tamper/versionedmorekeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/apostrophenullencode.py` & `sqlmap-1.8.4/sqlmap/tamper/apostrophenullencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/percentage.py` & `sqlmap-1.8.4/sqlmap/tamper/percentage.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/sp_password.py` & `sqlmap-1.8.4/sqlmap/tamper/sp_password.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/equaltorlike.py` & `sqlmap-1.8.4/sqlmap/tamper/equaltorlike.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/plus2fnconcat.py` & `sqlmap-1.8.4/sqlmap/tamper/plus2fnconcat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/halfversionedmorekeywords.py` & `sqlmap-1.8.4/sqlmap/tamper/halfversionedmorekeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2morecomment.py` & `sqlmap-1.8.4/sqlmap/tamper/space2morecomment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/modsecurityzeroversioned.py` & `sqlmap-1.8.4/sqlmap/tamper/modsecurityzeroversioned.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/greatest.py` & `sqlmap-1.8.4/sqlmap/tamper/greatest.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/bluecoat.py` & `sqlmap-1.8.4/sqlmap/tamper/bluecoat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/uppercase.py` & `sqlmap-1.8.4/sqlmap/tamper/uppercase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2hash.py` & `sqlmap-1.8.4/sqlmap/tamper/space2hash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/overlongutf8more.py` & `sqlmap-1.8.4/sqlmap/tamper/overlongutf8more.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/decentities.py` & `sqlmap-1.8.4/sqlmap/tamper/decentities.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2dash.py` & `sqlmap-1.8.4/sqlmap/tamper/space2dash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/modsecurityversioned.py` & `sqlmap-1.8.4/sqlmap/tamper/modsecurityversioned.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/hexentities.py` & `sqlmap-1.8.4/sqlmap/tamper/hexentities.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/charencode.py` & `sqlmap-1.8.4/sqlmap/tamper/charencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/equaltolike.py` & `sqlmap-1.8.4/sqlmap/tamper/equaltolike.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/chardoubleencode.py` & `sqlmap-1.8.4/sqlmap/tamper/chardoubleencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/scientific.py` & `sqlmap-1.8.4/sqlmap/tamper/scientific.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2comment.py` & `sqlmap-1.8.4/sqlmap/tamper/space2comment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/unmagicquotes.py` & `sqlmap-1.8.4/sqlmap/tamper/unmagicquotes.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/xforwardedfor.py` & `sqlmap-1.8.4/sqlmap/tamper/xforwardedfor.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2plus.py` & `sqlmap-1.8.4/sqlmap/tamper/space2plus.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/charunicodeescape.py` & `sqlmap-1.8.4/sqlmap/tamper/charunicodeescape.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2morehash.py` & `sqlmap-1.8.4/sqlmap/tamper/space2morehash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/ifnull2casewhenisnull.py` & `sqlmap-1.8.4/sqlmap/tamper/ifnull2casewhenisnull.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/ifnull2ifisnull.py` & `sqlmap-1.8.4/sqlmap/tamper/ifnull2ifisnull.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/commentbeforeparentheses.py` & `sqlmap-1.8.4/sqlmap/tamper/commentbeforeparentheses.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/sleep2getlock.py` & `sqlmap-1.8.4/sqlmap/tamper/sleep2getlock.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/lowercase.py` & `sqlmap-1.8.4/sqlmap/tamper/lowercase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/commalessmid.py` & `sqlmap-1.8.4/sqlmap/tamper/commalessmid.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/charunicodeencode.py` & `sqlmap-1.8.4/sqlmap/tamper/charunicodeencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2mysqldash.py` & `sqlmap-1.8.4/sqlmap/tamper/space2mysqldash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/hex2char.py` & `sqlmap-1.8.4/sqlmap/tamper/hex2char.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/randomcase.py` & `sqlmap-1.8.4/sqlmap/tamper/randomcase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/appendnullbyte.py` & `sqlmap-1.8.4/sqlmap/tamper/appendnullbyte.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/base64encode.py` & `sqlmap-1.8.4/sqlmap/tamper/base64encode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2randomblank.py` & `sqlmap-1.8.4/sqlmap/tamper/space2randomblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/binary.py` & `sqlmap-1.8.4/sqlmap/tamper/binary.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/if2case.py` & `sqlmap-1.8.4/sqlmap/tamper/if2case.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/overlongutf8.py` & `sqlmap-1.8.4/sqlmap/tamper/overlongutf8.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/space2mysqlblank.py` & `sqlmap-1.8.4/sqlmap/tamper/space2mysqlblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/htmlencode.py` & `sqlmap-1.8.4/sqlmap/tamper/htmlencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/tamper/commalesslimit.py` & `sqlmap-1.8.4/sqlmap/tamper/commalesslimit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/sqlmap.py` & `sqlmap-1.8.4/sqlmap/sqlmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     warnings.filterwarnings(action="ignore", message=".*using a very old release", category=UserWarning)
     warnings.filterwarnings(action="ignore", message=".*default buffer size will be used", category=RuntimeWarning)
     warnings.filterwarnings(action="ignore", category=UserWarning, module="psycopg2")
 
     from lib.core.data import logger
 
     from lib.core.common import banner
-    from lib.core.common import checkIntegrity
     from lib.core.common import checkPipedInput
+    from lib.core.common import checkSums
     from lib.core.common import createGithubIssue
     from lib.core.common import dataToStdout
     from lib.core.common import extractRegexResult
     from lib.core.common import filterNone
     from lib.core.common import getDaysFromLastUpdate
     from lib.core.common import getFileItems
     from lib.core.common import getSafeExString
@@ -264,15 +264,15 @@
     except SystemExit as ex:
         os._exitcode = ex.code or 0
 
     except:
         print()
         errMsg = unhandledExceptionMessage()
         excMsg = traceback.format_exc()
-        valid = checkIntegrity()
+        valid = checkSums()
 
         os._exitcode = 255
 
         if any(_ in excMsg for _ in ("MemoryError", "Cannot allocate memory")):
             errMsg = "memory exhaustion detected"
             logger.critical(errMsg)
             raise SystemExit
@@ -444,15 +444,15 @@
         elif kb.get("dumpKeyboardInterrupt"):
             raise SystemExit
 
         elif any(_ in excMsg for _ in ("Broken pipe",)):
             raise SystemExit
 
         elif valid is False:
-            errMsg = "code integrity check failed (turning off automatic issue creation). "
+            errMsg = "code checksum failed (turning off automatic issue creation). "
             errMsg += "You should retrieve the latest development version from official GitHub "
             errMsg += "repository at '%s'" % GIT_PAGE
             logger.critical(errMsg)
             print()
             dataToStdout(excMsg)
             raise SystemExit
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/CHANGELOG.md` & `sqlmap-1.8.4/sqlmap/doc/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/doc/THANKS.md` & `sqlmap-1.8.4/sqlmap/doc/THANKS.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-it-IT.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-it-IT.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Sito: https://sqlmap.org
 * Download: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS feed dei commit: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
 * Manuale dell'utente: https://github.com/sqlmapproject/sqlmap/wiki
 * Domande più frequenti (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Dimostrazioni: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Screenshot: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-uk-UA.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-uk-UA.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Основний сайт: https://sqlmap.org
 * Завантаження: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) або [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Канал новин RSS: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Відстеження проблем: https://github.com/sqlmapproject/sqlmap/issues
 * Інструкція користувача: https://github.com/sqlmapproject/sqlmap/wiki
 * Поширенні питання (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Демо: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Скриншоти: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-ko-KR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-ko-KR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-rs-RS.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-rs-RS.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Početna stranica: https://sqlmap.org
 * Preuzimanje: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) ili [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS feed promena u kodu: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Prijava problema: https://github.com/sqlmapproject/sqlmap/issues
 * Korisnički priručnik: https://github.com/sqlmapproject/sqlmap/wiki
 * Najčešće postavljena pitanja (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demo: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Slike: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-in-HI.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-in-HI.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-fa-IR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-fa-IR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-bg-BG.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-bg-BG.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Начална страница: https://sqlmap.org
 * Изтегляне: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS емисия: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Проследяване на проблеми и въпроси: https://github.com/sqlmapproject/sqlmap/issues
 * Упътване: https://github.com/sqlmapproject/sqlmap/wiki
 * Често задавани въпроси (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Демо: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Снимки на екрана: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-ru-RU.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-ru-RU.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Основной сайт: https://sqlmap.org
 * Скачивание: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) или [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Канал новостей RSS: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Отслеживание проблем: https://github.com/sqlmapproject/sqlmap/issues
 * Пользовательский мануал: https://github.com/sqlmapproject/sqlmap/wiki
 * Часто задаваемые вопросы (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Демки: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Скриншоты: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-id-ID.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-id-ID.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
 
 * Situs: https://sqlmap.org
 * Unduh: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) atau [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS Feed Dari Commits: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Pelacak Masalah: https://github.com/sqlmapproject/sqlmap/issues
 * Wiki Manual Penggunaan: https://github.com/sqlmapproject/sqlmap/wiki
 * Pertanyaan Yang Sering Ditanyakan (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Video Demo [#1](https://www.youtube.com/user/inquisb/videos) dan [#2](https://www.youtube.com/user/stamparm/videos)
 * Tangkapan Layar: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-fr-FR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-fr-FR.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 
 * Page d'acceuil: https://sqlmap.org
 * Téléchargement: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) ou [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Commits RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Suivi des issues: https://github.com/sqlmapproject/sqlmap/issues
 * Manuel de l'utilisateur: https://github.com/sqlmapproject/sqlmap/wiki
 * Foire aux questions (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Démonstrations: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Les captures d'écran: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-pt-BR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-pt-BR.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Homepage: https://sqlmap.org
 * Download: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) ou [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Commits RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
 * Manual do Usuário: https://github.com/sqlmapproject/sqlmap/wiki
 * Perguntas frequentes (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demonstrações: [#1](https://www.youtube.com/user/inquisb/videos) e [#2](https://www.youtube.com/user/stamparm/videos)
 * Imagens: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-hr-HR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-hr-HR.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Početna stranica: https://sqlmap.org
 * Preuzimanje: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) ili [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS feed promjena u kodu: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Prijava problema: https://github.com/sqlmapproject/sqlmap/issues
 * Korisnički priručnik: https://github.com/sqlmapproject/sqlmap/wiki
 * Najčešće postavljena pitanja (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demo: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Slike zaslona: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-nl-NL.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-nl-NL.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Homepage: https://sqlmap.org
 * Download: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) of [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Probleem tracker: https://github.com/sqlmapproject/sqlmap/issues
 * Gebruikers handleiding: https://github.com/sqlmapproject/sqlmap/wiki
 * Vaak gestelde vragen (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demos: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-sk-SK.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-sk-SK.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Domovská stránka: https://sqlmap.org
 * Stiahnutia: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) alebo [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Zdroje RSS Commits: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Sledovač problémov: https://github.com/sqlmapproject/sqlmap/issues
 * Používateľská príručka: https://github.com/sqlmapproject/sqlmap/wiki
 * Často kladené otázky (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demá: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Snímky obrazovky: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-vi-VN.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-vi-VN.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,10 +43,10 @@
 
 * Trang chủ: https://sqlmap.org
 * Tải xuống: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) hoặc [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Nguồn cấp dữ liệu RSS về commits: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Theo dõi vấn đề: https://github.com/sqlmapproject/sqlmap/issues
 * Hướng dẫn sử dụng: https://github.com/sqlmapproject/sqlmap/wiki
 * Các câu hỏi thường gặp (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demo: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Ảnh chụp màn hình: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-pl-PL.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-pl-PL.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Strona projektu: https://sqlmap.org
 * Pobieranie: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) lub [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Zgłaszanie błędów: https://github.com/sqlmapproject/sqlmap/issues
 * Instrukcja użytkowania: https://github.com/sqlmapproject/sqlmap/wiki
 * Często zadawane pytania (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Dema: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Zrzuty ekranu: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-gr-GR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-gr-GR.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 * Αρχική σελίδα: https://sqlmap.org
 * Λήψεις: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) ή [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Commits RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Προβλήματα: https://github.com/sqlmapproject/sqlmap/issues
 * Εγχειρίδιο Χρήστη: https://github.com/sqlmapproject/sqlmap/wiki
 * Συχνές Ερωτήσεις (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demos: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Εικόνες: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-zh-CN.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-zh-CN.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # sqlmap ![](https://i.imgur.com/fe85aVR.png)
 
 [![.github/workflows/tests.yml](https://github.com/sqlmapproject/sqlmap/actions/workflows/tests.yml/badge.svg)](https://github.com/sqlmapproject/sqlmap/actions/workflows/tests.yml) [![Python 2.6|2.7|3.x](https://img.shields.io/badge/python-2.6|2.7|3.x-yellow.svg)](https://www.python.org/) [![License](https://img.shields.io/badge/license-GPLv2-red.svg)](https://raw.githubusercontent.com/sqlmapproject/sqlmap/master/LICENSE) [![Twitter](https://img.shields.io/badge/twitter-@sqlmap-blue.svg)](https://twitter.com/sqlmap)
 
-sqlmap 是一个开源的渗透测试工具，可以用来自动化的检测，利用SQL注入漏洞，获取数据库服务器的权限。它具有功能强大的检测引擎,针对各种不同类型数据库的渗透测试的功能选项，包括获取数据库中存储的数据，访问操作系统文件甚至可以通过带外数据连接的方式执行操作系统命令。
+sqlmap 是一款开源的渗透测试工具，可以自动化进行SQL注入的检测、利用，并能接管数据库服务器。它具有功能强大的检测引擎,为渗透测试人员提供了许多专业的功能并且可以进行组合，其中包括数据库指纹识别、数据读取和访问底层文件系统，甚至可以通过带外数据连接的方式执行系统命令。
 
 演示截图
 ----
 
 ![截图](https://raw.github.com/wiki/sqlmapproject/sqlmap/images/sqlmap_screenshot.png)
 
-你可以访问 wiki上的 [截图](https://github.com/sqlmapproject/sqlmap/wiki/Screenshots) 查看各种用法的演示
+你可以查看 wiki 上的 [截图](https://github.com/sqlmapproject/sqlmap/wiki/Screenshots) 了解各种用法的示例
 
 安装方法
 ----
 
-你可以点击 [这里](https://github.com/sqlmapproject/sqlmap/tarball/master) 下载最新的 `tar` 打包的源代码 或者点击 [这里](https://github.com/sqlmapproject/sqlmap/zipball/master)下载最新的 `zip` 打包的源代码.
+你可以点击 [这里](https://github.com/sqlmapproject/sqlmap/tarball/master) 下载最新的 `tar` 打包好的源代码，或者点击 [这里](https://github.com/sqlmapproject/sqlmap/zipball/master)下载最新的 `zip` 打包好的源代码.
 
-推荐你从 [Git](https://github.com/sqlmapproject/sqlmap) 仓库获取最新的源代码:
+推荐直接从 [Git](https://github.com/sqlmapproject/sqlmap) 仓库获取最新的源代码:
 
     git clone --depth 1 https://github.com/sqlmapproject/sqlmap.git sqlmap-dev
 
 sqlmap 可以运行在 [Python](https://www.python.org/download/)  **2.6**, **2.7**  和  **3.x** 版本的任何平台上
 
 使用方法
 ----
@@ -29,21 +29,21 @@
 
     python sqlmap.py -h
 
 通过如下的命令可以查看所有的用法及命令行参数:
 
     python sqlmap.py -hh
 
-你可以从 [这里](https://asciinema.org/a/46601) 看到一个sqlmap 的使用样例。除此以外，你还可以查看 [使用手册](https://github.com/sqlmapproject/sqlmap/wiki/Usage)。获取sqlmap所有支持的特性、参数、命令行选项开关及说明的使用帮助。
+你可以从 [这里](https://asciinema.org/a/46601) 看到一个 sqlmap 的使用样例。除此以外，你还可以查看 [使用手册](https://github.com/sqlmapproject/sqlmap/wiki/Usage)。获取 sqlmap 所有支持的特性、参数、命令行选项开关及详细的使用帮助。
 
 链接
 ----
 
 * 项目主页: https://sqlmap.org
 * 源代码下载: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
-* RSS 订阅: https://github.com/sqlmapproject/sqlmap/commits/master.atom
-* Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
+* Commit的 RSS 订阅: https://github.com/sqlmapproject/sqlmap/commits/master.atom
+* 问题跟踪器: https://github.com/sqlmapproject/sqlmap/issues
 * 使用手册: https://github.com/sqlmapproject/sqlmap/wiki
 * 常见问题 (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * 教程: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * 截图: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-ja-JP.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-ja-JP.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
 
 * ホームページ: https://sqlmap.org
 * ダウンロード: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * コミットのRSSフィード: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * 課題管理: https://github.com/sqlmapproject/sqlmap/issues
 * ユーザーマニュアル: https://github.com/sqlmapproject/sqlmap/wiki
 * よくある質問 (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * デモ: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * スクリーンショット: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-ka-GE.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-ka-GE.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 
 * საწყისი გვერდი: https://sqlmap.org
 * ჩამოტვირთვა: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) ან [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * RSS არხი: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * პრობლემებისათვის თვალყურის დევნება: https://github.com/sqlmapproject/sqlmap/issues
 * მომხმარებლის სახელმძღვანელო: https://github.com/sqlmapproject/sqlmap/wiki
 * ხშირად დასმული კითხვები (ხდკ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * დემონსტრაციები: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * ეკრანის ანაბეჭდები: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-tr-TR.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-tr-TR.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
 
 * Anasayfa: https://sqlmap.org
 * İndirme bağlantıları: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Commitlerin RSS beslemeleri: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Hata takip etme sistemi: https://github.com/sqlmapproject/sqlmap/issues
 * Kullanıcı Manueli: https://github.com/sqlmapproject/sqlmap/wiki
 * Sıkça Sorulan Sorular(SSS): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demolar: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Ekran görüntüleri: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-de-DE.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-de-DE.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 
 * Webseite: https://sqlmap.org
 * Download: [.tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) or [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Commits RSS feed: https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Problemverfolgung: https://github.com/sqlmapproject/sqlmap/issues
 * Benutzerhandbuch: https://github.com/sqlmapproject/sqlmap/wiki
 * Häufig gestellte Fragen (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demonstrationen: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/translations/README-es-MX.md` & `sqlmap-1.8.4/sqlmap/doc/translations/README-es-MX.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 
 * Página principal: https://sqlmap.org 
 * Descargar: [. tar.gz](https://github.com/sqlmapproject/sqlmap/tarball/master) o [.zip](https://github.com/sqlmapproject/sqlmap/zipball/master)
 * Fuente de Cambios "Commit RSS feed": https://github.com/sqlmapproject/sqlmap/commits/master.atom
 * Seguimiento de problemas "Issue tracker": https://github.com/sqlmapproject/sqlmap/issues
 * Manual de usuario: https://github.com/sqlmapproject/sqlmap/wiki
 * Preguntas frecuentes (FAQ): https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-* Twitter: [@sqlmap](https://twitter.com/sqlmap)
+* X: [@sqlmap](https://twitter.com/sqlmap)
 * Demostraciones: [https://www.youtube.com/user/inquisb/videos](https://www.youtube.com/user/inquisb/videos)
 * Imágenes: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
```

### Comparing `sqlmap-1.8.3/sqlmap/doc/THIRD-PARTY.md` & `sqlmap-1.8.4/sqlmap/doc/THIRD-PARTY.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/sqlmap.conf` & `sqlmap-1.8.4/sqlmap/sqlmap.conf`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/LICENSE` & `sqlmap-1.8.4/sqlmap/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/custom.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/custom.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/entries.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/entries.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/search.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/search.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/users.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/users.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/misc.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/misc.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/databases.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/databases.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/generic/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/presto/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/hsqldb/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mssqlserver/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/access/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/access/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/raima/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/derby/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/derby/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/derby/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/derby/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/derby/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cache/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cache/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cache/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cache/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cache/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cache/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/vertica/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/firebird/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/monetdb/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/maxdb/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mimersql/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/postgresql/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mysql/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/informix/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/informix/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/informix/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/informix/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/informix/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/altibase/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/extremedb/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/mckoi/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/db2/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/db2/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/db2/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/db2/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/db2/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cubrid/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/h2/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/h2/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/h2/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/h2/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/h2/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/h2/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/oracle/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/cratedb/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sybase/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/clickhouse/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/connector.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/sqlite/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/syntax.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/virtuoso/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/enumeration.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/takeover.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/fingerprint.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/__init__.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/plugins/dbms/frontbase/filesystem.py` & `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/controller/handler.py` & `sqlmap-1.8.4/sqlmap/lib/controller/handler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/controller/action.py` & `sqlmap-1.8.4/sqlmap/lib/controller/action.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/controller/checks.py` & `sqlmap-1.8.4/sqlmap/lib/controller/checks.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/controller/controller.py` & `sqlmap-1.8.4/sqlmap/lib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/search.py` & `sqlmap-1.8.4/sqlmap/lib/utils/search.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/httpd.py` & `sqlmap-1.8.4/sqlmap/lib/utils/httpd.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/hash.py` & `sqlmap-1.8.4/sqlmap/lib/utils/hash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/getch.py` & `sqlmap-1.8.4/sqlmap/lib/utils/getch.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/sqlalchemy.py` & `sqlmap-1.8.4/sqlmap/lib/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/hashdb.py` & `sqlmap-1.8.4/sqlmap/lib/utils/hashdb.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/xrange.py` & `sqlmap-1.8.4/sqlmap/lib/utils/xrange.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/versioncheck.py` & `sqlmap-1.8.4/sqlmap/lib/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/progress.py` & `sqlmap-1.8.4/sqlmap/lib/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/purge.py` & `sqlmap-1.8.4/sqlmap/lib/utils/purge.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/crawler.py` & `sqlmap-1.8.4/sqlmap/lib/utils/crawler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/har.py` & `sqlmap-1.8.4/sqlmap/lib/utils/har.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/brute.py` & `sqlmap-1.8.4/sqlmap/lib/utils/brute.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/pivotdumptable.py` & `sqlmap-1.8.4/sqlmap/lib/utils/pivotdumptable.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/api.py` & `sqlmap-1.8.4/sqlmap/lib/utils/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,17 @@
                 else:
                     break
 
         if statement.lstrip().upper().startswith("SELECT"):
             return self.cursor.fetchall()
 
     def init(self):
-        self.execute("CREATE TABLE logs(id INTEGER PRIMARY KEY AUTOINCREMENT, taskid INTEGER, time TEXT, level TEXT, message TEXT)")
-        self.execute("CREATE TABLE data(id INTEGER PRIMARY KEY AUTOINCREMENT, taskid INTEGER, status INTEGER, content_type INTEGER, value TEXT)")
-        self.execute("CREATE TABLE errors(id INTEGER PRIMARY KEY AUTOINCREMENT, taskid INTEGER, error TEXT)")
+        self.execute("CREATE TABLE IF NOT EXISTS logs(id INTEGER PRIMARY KEY AUTOINCREMENT, taskid INTEGER, time TEXT, level TEXT, message TEXT)")
+        self.execute("CREATE TABLE IF NOT EXISTS data(id INTEGER PRIMARY KEY AUTOINCREMENT, taskid INTEGER, status INTEGER, content_type INTEGER, value TEXT)")
+        self.execute("CREATE TABLE IF NOT EXISTS errors(id INTEGER PRIMARY KEY AUTOINCREMENT, taskid INTEGER, error TEXT)")
 
 class Task(object):
     def __init__(self, taskid, remote_addr):
         self.remote_addr = remote_addr
         self.process = None
         self.output_directory = None
         self.options = None
@@ -272,15 +272,15 @@
 
 class LogRecorder(logging.StreamHandler):
     def emit(self, record):
         """
         Record emitted events to IPC database for asynchronous I/O
         communication with the parent process
         """
-        conf.databaseCursor.execute("INSERT INTO logs VALUES(NULL, ?, ?, ?, ?)", (conf.taskid, time.strftime("%X"), record.levelname, record.msg % record.args if record.args else record.msg))
+        conf.databaseCursor.execute("INSERT INTO logs VALUES(NULL, ?, ?, ?, ?)", (conf.taskid, time.strftime("%X"), record.levelname, str(record.msg % record.args if record.args else record.msg)))
 
 def setRestAPILog():
     if conf.api:
         try:
             conf.databaseCursor = Database(conf.database)
             conf.databaseCursor.connect("client")
         except sqlite3.OperationalError as ex:
```

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/safe2bin.py` & `sqlmap-1.8.4/sqlmap/lib/utils/safe2bin.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/timeout.py` & `sqlmap-1.8.4/sqlmap/lib/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/deps.py` & `sqlmap-1.8.4/sqlmap/lib/utils/deps.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/utils/sgmllib.py` & `sqlmap-1.8.4/sqlmap/lib/utils/sgmllib.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/basic.py` & `sqlmap-1.8.4/sqlmap/lib/request/basic.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/dns.py` & `sqlmap-1.8.4/sqlmap/lib/request/dns.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/direct.py` & `sqlmap-1.8.4/sqlmap/lib/request/direct.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/redirecthandler.py` & `sqlmap-1.8.4/sqlmap/lib/request/redirecthandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/rangehandler.py` & `sqlmap-1.8.4/sqlmap/lib/request/rangehandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/methodrequest.py` & `sqlmap-1.8.4/sqlmap/lib/request/methodrequest.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/httpshandler.py` & `sqlmap-1.8.4/sqlmap/lib/request/httpshandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/templates.py` & `sqlmap-1.8.4/sqlmap/lib/request/templates.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/basicauthhandler.py` & `sqlmap-1.8.4/sqlmap/lib/request/basicauthhandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/chunkedhandler.py` & `sqlmap-1.8.4/sqlmap/lib/request/chunkedhandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/pkihandler.py` & `sqlmap-1.8.4/sqlmap/lib/request/pkihandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/inject.py` & `sqlmap-1.8.4/sqlmap/lib/request/inject.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/connect.py` & `sqlmap-1.8.4/sqlmap/lib/request/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
         url = kwargs.get("url", None) or conf.url
         get = kwargs.get("get", None)
         post = kwargs.get("post", None)
         method = kwargs.get("method", None)
         cookie = kwargs.get("cookie", None)
         ua = kwargs.get("ua", None) or conf.agent
         referer = kwargs.get("referer", None) or conf.referer
-        host = kwargs.get("host", None) or conf.host
         direct_ = kwargs.get("direct", False)
         multipart = kwargs.get("multipart", None)
         silent = kwargs.get("silent", False)
         raise404 = kwargs.get("raise404", True)
         timeout = kwargs.get("timeout", None) or conf.timeout
         auxHeaders = kwargs.get("auxHeaders", None)
         response = kwargs.get("response", False)
```

### Comparing `sqlmap-1.8.3/sqlmap/lib/request/comparison.py` & `sqlmap-1.8.4/sqlmap/lib/request/comparison.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/techniques/error/use.py` & `sqlmap-1.8.4/sqlmap/lib/techniques/error/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/techniques/dns/use.py` & `sqlmap-1.8.4/sqlmap/lib/techniques/dns/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/techniques/dns/test.py` & `sqlmap-1.8.4/sqlmap/lib/techniques/dns/test.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/techniques/blind/inference.py` & `sqlmap-1.8.4/sqlmap/lib/techniques/blind/inference.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/techniques/union/use.py` & `sqlmap-1.8.4/sqlmap/lib/techniques/union/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/techniques/union/test.py` & `sqlmap-1.8.4/sqlmap/lib/techniques/union/test.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/data.py` & `sqlmap-1.8.4/sqlmap/lib/core/data.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/patch.py` & `sqlmap-1.8.4/sqlmap/lib/core/patch.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/readlineng.py` & `sqlmap-1.8.4/sqlmap/lib/core/readlineng.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/dump.py` & `sqlmap-1.8.4/sqlmap/lib/core/dump.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/threads.py` & `sqlmap-1.8.4/sqlmap/lib/core/threads.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/convert.py` & `sqlmap-1.8.4/sqlmap/lib/core/convert.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/enums.py` & `sqlmap-1.8.4/sqlmap/lib/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/decorators.py` & `sqlmap-1.8.4/sqlmap/lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/bigarray.py` & `sqlmap-1.8.4/sqlmap/lib/core/bigarray.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/gui.py` & `sqlmap-1.8.4/sqlmap/lib/core/gui.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/exception.py` & `sqlmap-1.8.4/sqlmap/lib/core/exception.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/testing.py` & `sqlmap-1.8.4/sqlmap/lib/core/testing.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/optiondict.py` & `sqlmap-1.8.4/sqlmap/lib/core/optiondict.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/target.py` & `sqlmap-1.8.4/sqlmap/lib/core/target.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/session.py` & `sqlmap-1.8.4/sqlmap/lib/core/session.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/agent.py` & `sqlmap-1.8.4/sqlmap/lib/core/agent.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/option.py` & `sqlmap-1.8.4/sqlmap/lib/core/option.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
 from lib.core.settings import PRECONNECT_CANDIDATE_TIMEOUT
 from lib.core.settings import PROXY_ENVIRONMENT_VARIABLES
 from lib.core.settings import SOCKET_PRE_CONNECT_QUEUE_SIZE
 from lib.core.settings import SQLMAP_ENVIRONMENT_PREFIX
 from lib.core.settings import SUPPORTED_DBMS
 from lib.core.settings import SUPPORTED_OS
 from lib.core.settings import TIME_DELAY_CANDIDATES
-from lib.core.settings import UNION_CHAR_REGEX
 from lib.core.settings import UNKNOWN_DBMS_VERSION
 from lib.core.settings import URI_INJECTABLE_REGEX
 from lib.core.threads import getCurrentThreadData
 from lib.core.threads import setDaemon
 from lib.core.update import update
 from lib.parse.configfile import configFileParser
 from lib.parse.payloads import loadBoundaries
```

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/settings.py` & `sqlmap-1.8.4/sqlmap/lib/core/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lib.core.enums import DBMS
 from lib.core.enums import DBMS_DIRECTORY_NAME
 from lib.core.enums import OS
 from thirdparty import six
 from thirdparty.six import unichr as _unichr
 
 # sqlmap version (<major>.<minor>.<month>.<monthly commit>)
-VERSION = "1.8.3"
+VERSION = "1.8.4"
 TYPE = "pip"
 TYPE_COLORS = {"dev": 33, "stable": 90, "pip": 34}
 VERSION_STRING = "sqlmap/%s#%s" % ('.'.join(VERSION.split('.')[:-1]) if VERSION.count('.') > 2 and VERSION.split('.')[-1] == '0' else VERSION, TYPE)
 DESCRIPTION = "automatic SQL injection and database takeover tool"
 SITE = "https://sqlmap.org"
 DEFAULT_USER_AGENT = "%s (%s)" % (VERSION_STRING, SITE)
 DEV_EMAIL_ADDRESS = "dev@sqlmap.org"
@@ -679,17 +679,14 @@
 
 # Maximum number of times for revalidation of a character in inference (as required)
 MAX_REVALIDATION_STEPS = 5
 
 # Characters that can be used to split parameter values in provided command line (e.g. in --tamper)
 PARAMETER_SPLITTING_REGEX = r"[,|;]"
 
-# Regular expression describing possible union char value (e.g. used in --union-char)
-UNION_CHAR_REGEX = r"\A\w+\Z"
-
 # Attribute used for storing original parameter value in special cases (e.g. POST)
 UNENCODED_ORIGINAL_VALUE = "original"
 
 # Common column names containing usernames (used for hash cracking in some cases)
 COMMON_USER_COLUMNS = ("login", "user", "username", "user_name", "user_login", "benutzername", "benutzer", "utilisateur", "usager", "consommateur", "utente", "utilizzatore", "utilizator", "utilizador", "usufrutuario", "korisnik", "uporabnik", "usuario", "consumidor", "client", "cuser")
 
 # Default delimiter in GET/POST values
@@ -698,15 +695,15 @@
 # Default delimiter in cookie values
 DEFAULT_COOKIE_DELIMITER = ';'
 
 # Unix timestamp used for forcing cookie expiration when provided with --load-cookies
 FORCE_COOKIE_EXPIRATION_TIME = "9999999999"
 
 # Github OAuth token used for creating an automatic Issue for unhandled exceptions
-GITHUB_REPORT_OAUTH_TOKEN = "Z2hwX09GTWlsWUJVZWhiYWluS3I3T2hUbE9abHJ4cXNUTTFYeUxxTw"
+GITHUB_REPORT_OAUTH_TOKEN = "Z2hwX0pNd0I2U25kN2Q5QmxlWkhxZmkxVXZTSHZiTlRDWjE5NUNpNA"
 
 # Skip unforced HashDB flush requests below the threshold number of cached items
 HASHDB_FLUSH_THRESHOLD = 32
 
 # Number of retries for unsuccessful HashDB flush attempts
 HASHDB_FLUSH_RETRIES = 3
```

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/compat.py` & `sqlmap-1.8.4/sqlmap/lib/core/compat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/subprocessng.py` & `sqlmap-1.8.4/sqlmap/lib/core/subprocessng.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/revision.py` & `sqlmap-1.8.4/sqlmap/lib/core/revision.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/profiling.py` & `sqlmap-1.8.4/sqlmap/lib/core/profiling.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/defaults.py` & `sqlmap-1.8.4/sqlmap/lib/core/defaults.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/log.py` & `sqlmap-1.8.4/sqlmap/lib/core/log.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/shell.py` & `sqlmap-1.8.4/sqlmap/lib/core/shell.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/dicts.py` & `sqlmap-1.8.4/sqlmap/lib/core/dicts.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/wordlist.py` & `sqlmap-1.8.4/sqlmap/lib/core/wordlist.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/unescaper.py` & `sqlmap-1.8.4/sqlmap/lib/core/unescaper.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/update.py` & `sqlmap-1.8.4/sqlmap/lib/core/update.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/replication.py` & `sqlmap-1.8.4/sqlmap/lib/core/replication.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/datatype.py` & `sqlmap-1.8.4/sqlmap/lib/core/datatype.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/core/common.py` & `sqlmap-1.8.4/sqlmap/lib/core/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,18 @@
         @return: detected back-end DBMS based upon fingerprint techniques.
         @rtype: C{str}
         """
 
         if versions is None and Backend.getVersionList():
             versions = Backend.getVersionList()
 
+        # NOTE: preventing ugly (e.g.) "back-end DBMS: MySQL Unknown"
+        if isListLike(versions) and UNKNOWN_DBMS_VERSION in versions:
+            versions = None
+
         return Backend.getDbms() if versions is None else "%s %s" % (Backend.getDbms(), " and ".join(filterNone(versions)))
 
     @staticmethod
     def getErrorParsedDBMSes():
         """
         Parses the knowledge base htmlFp list and return its values
         formatted as a human readable string.
@@ -703,16 +707,24 @@
                                                     current[key] = "%s%s" % (value, BOUNDED_INJECTION_MARKER)
                                                 candidates["%s (%s)" % (parameter, key)] = re.sub(r"\b(%s\s*=\s*)%s" % (re.escape(parameter), re.escape(testableParameters[parameter])), r"\g<1>%s" % json.dumps(deserialized, separators=(',', ':') if ", " not in testableParameters[parameter] else None), parameters)
                                                 current[key] = original
                                             elif isinstance(value, (list, tuple, set, dict)):
                                                 if value:
                                                     walk(head, value)
 
-                                deserialized = json.loads(testableParameters[parameter])
-                                walk(deserialized)
+                                # NOTE: for cases with custom injection marker(s) inside (e.g. https://github.com/sqlmapproject/sqlmap/issues/4137#issuecomment-2013783111) - p.s. doesn't care too much about the structure (e.g. injection into the flat array values)
+                                if CUSTOM_INJECTION_MARK_CHAR in testableParameters[parameter]:
+                                    for match in re.finditer(r'(\w+)[^\w]*"\s*:[^\w]*\w*%s' % re.escape(CUSTOM_INJECTION_MARK_CHAR), testableParameters[parameter]):
+                                        key = match.group(1)
+                                        value = testableParameters[parameter].replace(match.group(0), match.group(0).replace(CUSTOM_INJECTION_MARK_CHAR, BOUNDED_INJECTION_MARKER))
+                                        candidates["%s (%s)" % (parameter, key)] = re.sub(r"\b(%s\s*=\s*)%s" % (re.escape(parameter), re.escape(testableParameters[parameter])), r"\g<1>%s" % value, parameters)
+
+                                if not candidates:
+                                    deserialized = json.loads(testableParameters[parameter])
+                                    walk(deserialized)
 
                                 if candidates:
                                     message = "it appears that provided value for %sparameter '%s' " % ("%s " % place if place != parameter else "", parameter)
                                     message += "is JSON deserializable. Do you want to inject inside? [y/N] "
 
                                     if readInput(message, default='N', boolean=True):
                                         del testableParameters[parameter]
@@ -1504,14 +1516,15 @@
     paths.SQLMAP_XML_PAYLOADS_PATH = os.path.join(paths.SQLMAP_XML_PATH, "payloads")
 
     # sqlmap files
     paths.COMMON_COLUMNS = os.path.join(paths.SQLMAP_TXT_PATH, "common-columns.txt")
     paths.COMMON_FILES = os.path.join(paths.SQLMAP_TXT_PATH, "common-files.txt")
     paths.COMMON_TABLES = os.path.join(paths.SQLMAP_TXT_PATH, "common-tables.txt")
     paths.COMMON_OUTPUTS = os.path.join(paths.SQLMAP_TXT_PATH, 'common-outputs.txt')
+    paths.DIGEST_FILE = os.path.join(paths.SQLMAP_TXT_PATH, "sha256sums.txt")
     paths.SQL_KEYWORDS = os.path.join(paths.SQLMAP_TXT_PATH, "keywords.txt")
     paths.SMALL_DICT = os.path.join(paths.SQLMAP_TXT_PATH, "smalldict.txt")
     paths.USER_AGENTS = os.path.join(paths.SQLMAP_TXT_PATH, "user-agents.txt")
     paths.WORDLIST = os.path.join(paths.SQLMAP_TXT_PATH, "wordlist.tx_")
     paths.ERRORS_XML = os.path.join(paths.SQLMAP_XML_PATH, "errors.xml")
     paths.BOUNDARIES_XML = os.path.join(paths.SQLMAP_XML_PATH, "boundaries.xml")
     paths.QUERIES_XML = os.path.join(paths.SQLMAP_XML_PATH, "queries.xml")
@@ -3843,41 +3856,14 @@
             else:
                 retVal = _unichr(value)
         except:
             retVal = INFERENCE_UNKNOWN_CHAR
 
     return retVal
 
-def checkIntegrity():
-    """
-    Checks integrity of code files during the unhandled exceptions
-    """
-
-    if not paths:
-        return
-
-    logger.debug("running code integrity check")
-
-    retVal = True
-
-    baseTime = os.path.getmtime(paths.SQLMAP_SETTINGS_PATH) + 3600  # First hour free parking :)
-    for root, _, filenames in os.walk(paths.SQLMAP_ROOT_PATH):
-        for filename in filenames:
-            if re.search(r"(\.py|\.xml|_)\Z", filename):
-                filepath = os.path.join(root, filename)
-                if os.path.getmtime(filepath) > baseTime:
-                    logger.error("wrong modification time of '%s'" % filepath)
-                    retVal = False
-
-    suffix = extractRegexResult(r"#(?P<result>\w+)", VERSION_STRING)
-    if suffix and suffix not in {"dev", "stable"}:
-        retVal = False
-
-    return retVal
-
 def getDaysFromLastUpdate():
     """
     Get total number of days from last update
 
     >>> getDaysFromLastUpdate() >= 0
     True
     """
@@ -5587,7 +5573,29 @@
         index += chunkSize
         retVal += "%x;%s\r\n" % (chunkSize, salt)
         retVal += "%s\r\n" % candidate
 
     retVal += "0\r\n\r\n"
 
     return retVal
+
+def checkSums():
+    """
+    Validate the content of the digest file (i.e. sha256sums.txt)
+    >>> checkSums()
+    True
+    """
+
+    retVal = True
+
+    if paths.get("DIGEST_FILE"):
+        for entry in getFileItems(paths.DIGEST_FILE):
+            match = re.search(r"([0-9a-f]+)\s+([^\s]+)", entry)
+            if match:
+                expected, filename = match.groups()
+                filepath = os.path.join(paths.SQLMAP_ROOT_PATH, filename).replace('/', os.path.sep)
+                checkFile(filepath)
+                if not hashlib.sha256(open(filepath, "rb").read()).hexdigest() == expected:
+                    retVal &= False
+                    break
+
+    return retVal
```

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/abstraction.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/abstraction.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/udf.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/udf.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/metasploit.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/metasploit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/xp_cmdshell.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/xp_cmdshell.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/registry.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/registry.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/web.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/web.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/takeover/icmpsh.py` & `sqlmap-1.8.4/sqlmap/lib/takeover/icmpsh.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/cmdline.py` & `sqlmap-1.8.4/sqlmap/lib/parse/cmdline.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/handler.py` & `sqlmap-1.8.4/sqlmap/lib/parse/handler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/payloads.py` & `sqlmap-1.8.4/sqlmap/lib/parse/payloads.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/configfile.py` & `sqlmap-1.8.4/sqlmap/lib/parse/configfile.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/headers.py` & `sqlmap-1.8.4/sqlmap/lib/parse/headers.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/sitemap.py` & `sqlmap-1.8.4/sqlmap/lib/parse/sitemap.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/banner.py` & `sqlmap-1.8.4/sqlmap/lib/parse/banner.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/lib/parse/html.py` & `sqlmap-1.8.4/sqlmap/lib/parse/html.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/sqlmapapi.yaml` & `sqlmap-1.8.4/sqlmap/sqlmapapi.yaml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/cloak/cloak.py` & `sqlmap-1.8.4/sqlmap/extra/cloak/cloak.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/cloak/README.txt` & `sqlmap-1.8.4/sqlmap/extra/cloak/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/duplicates.py` & `sqlmap-1.8.4/sqlmap/extra/shutils/duplicates.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/precommit-hook.sh` & `sqlmap-1.8.4/sqlmap/extra/shutils/precommit-hook.sh`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 EOF
 
 chmod +x .git/hooks/pre-commit
 '
 
 PROJECT="../../"
 SETTINGS="../../lib/core/settings.py"
-DIGEST="../../sha256sums.txt"
+DIGEST="../../data/txt/sha256sums.txt"
 
 declare -x SCRIPTPATH="${0}"
 
 PROJECT_FULLPATH=${SCRIPTPATH%/*}/$PROJECT
 SETTINGS_FULLPATH=${SCRIPTPATH%/*}/$SETTINGS
 DIGEST_FULLPATH=${SCRIPTPATH%/*}/$DIGEST
 
@@ -34,8 +34,9 @@
     else
         echo "Something went wrong in VERSION increment"
         exit 1
     fi
     git add "$SETTINGS_FULLPATH"
 fi
 
-cd $PROJECT_FULLPATH && git ls-files | sort | uniq | grep -v sha256 | xargs sha256sum > $DIGEST_FULLPATH
+cd $PROJECT_FULLPATH && git ls-files | sort | uniq | grep -Pv '^\.|sha256' | xargs sha256sum > $DIGEST_FULLPATH && cd -
+git add "$DIGEST_FULLPATH"
```

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/drei.sh` & `sqlmap-1.8.4/sqlmap/extra/shutils/drei.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/pypi.sh` & `sqlmap-1.8.4/sqlmap/extra/shutils/pypi.sh`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
    or `.zip <https://github.com/sqlmapproject/sqlmap/zipball/master>`__
 -  Commits RSS feed:
    https://github.com/sqlmapproject/sqlmap/commits/master.atom
 -  Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
 -  User's manual: https://github.com/sqlmapproject/sqlmap/wiki
 -  Frequently Asked Questions (FAQ):
    https://github.com/sqlmapproject/sqlmap/wiki/FAQ
--  Twitter: https://twitter.com/sqlmap
+-  X: https://twitter.com/sqlmap
 -  Demos: http://www.youtube.com/user/inquisb/videos
 -  Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
 
 .. |Python 2.6|2.7|3.x| image:: https://img.shields.io/badge/python-2.6|2.7|3.x-yellow.svg
    :target: https://www.python.org/
 .. |License| image:: https://img.shields.io/badge/license-GPLv2-red.svg
    :target: https://raw.githubusercontent.com/sqlmapproject/sqlmap/master/LICENSE
```

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/recloak.sh` & `sqlmap-1.8.4/sqlmap/extra/shutils/recloak.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/newlines.py` & `sqlmap-1.8.4/sqlmap/extra/shutils/newlines.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/strip.sh` & `sqlmap-1.8.4/sqlmap/extra/shutils/strip.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shutils/postcommit-hook.sh` & `sqlmap-1.8.4/sqlmap/extra/shutils/postcommit-hook.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd.sln` & `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd.sln`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp` & `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/stdafx.h` & `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/stdafx.h`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj` & `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/runcmd/runcmd.exe_` & `sqlmap-1.8.4/sqlmap/extra/runcmd/runcmd.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/beep/beep.py` & `sqlmap-1.8.4/sqlmap/extra/beep/beep.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/beep/beep.wav` & `sqlmap-1.8.4/sqlmap/extra/beep/beep.wav`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_` & `sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_` & `sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_` & `sqlmap-1.8.4/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh-m.c` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.c`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh.exe_` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh-s.c` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-s.c`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/README.txt` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh-m.pl` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.pl`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/__init__.py` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/icmpsh/icmpsh_m.py` & `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh_m.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/dbgtool/dbgtool.py` & `sqlmap-1.8.4/sqlmap/extra/dbgtool/dbgtool.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/dbgtool/README.txt` & `sqlmap-1.8.4/sqlmap/extra/dbgtool/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/extra/vulnserver/vulnserver.py` & `sqlmap-1.8.4/sqlmap/extra/vulnserver/vulnserver.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/sqlmap/sqlmapapi.py` & `sqlmap-1.8.4/sqlmap/sqlmapapi.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.3/README.rst` & `sqlmap-1.8.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
    or `.zip <https://github.com/sqlmapproject/sqlmap/zipball/master>`__
 -  Commits RSS feed:
    https://github.com/sqlmapproject/sqlmap/commits/master.atom
 -  Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
 -  User's manual: https://github.com/sqlmapproject/sqlmap/wiki
 -  Frequently Asked Questions (FAQ):
    https://github.com/sqlmapproject/sqlmap/wiki/FAQ
--  Twitter: https://twitter.com/sqlmap
+-  X: https://twitter.com/sqlmap
 -  Demos: http://www.youtube.com/user/inquisb/videos
 -  Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
 
 .. |Python 2.6|2.7|3.x| image:: https://img.shields.io/badge/python-2.6|2.7|3.x-yellow.svg
    :target: https://www.python.org/
 .. |License| image:: https://img.shields.io/badge/license-GPLv2-red.svg
    :target: https://raw.githubusercontent.com/sqlmapproject/sqlmap/master/LICENSE
```

### Comparing `sqlmap-1.8.3/sqlmap.egg-info/SOURCES.txt` & `sqlmap-1.8.4/sqlmap.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 sqlmap/data/shell/stagers/stager.jsp_
 sqlmap/data/shell/stagers/stager.php_
 sqlmap/data/txt/common-columns.txt
 sqlmap/data/txt/common-files.txt
 sqlmap/data/txt/common-outputs.txt
 sqlmap/data/txt/common-tables.txt
 sqlmap/data/txt/keywords.txt
+sqlmap/data/txt/sha256sums.txt
 sqlmap/data/txt/smalldict.txt
 sqlmap/data/txt/user-agents.txt
 sqlmap/data/txt/wordlist.tx_
 sqlmap/data/udf/README.txt
 sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
 sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
 sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
```

### Comparing `sqlmap-1.8.3/sqlmap.egg-info/PKG-INFO` & `sqlmap-1.8.4/sqlmap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlmap
-Version: 1.8.3
+Version: 1.8.4
 Summary: Automatic SQL injection and database takeover tool
 Home-page: https://sqlmap.org
 Author: Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar
 Author-email: bernardo@sqlmap.org, miroslav@sqlmap.org
 License: GNU General Public License v2 (GPLv2)
-Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.3.zip
+Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.4.zip
 Project-URL: Source, https://github.com/sqlmapproject/sqlmap/
 Project-URL: Documentation, https://github.com/sqlmapproject/sqlmap/wiki
 Project-URL: Tracker, https://github.com/sqlmapproject/sqlmap/issues
 Description: sqlmap
         ======
         
         |Python 2.6|2.7|3.x| |License| |Twitter|
@@ -87,15 +87,15 @@
            or `.zip <https://github.com/sqlmapproject/sqlmap/zipball/master>`__
         -  Commits RSS feed:
            https://github.com/sqlmapproject/sqlmap/commits/master.atom
         -  Issue tracker: https://github.com/sqlmapproject/sqlmap/issues
         -  User's manual: https://github.com/sqlmapproject/sqlmap/wiki
         -  Frequently Asked Questions (FAQ):
            https://github.com/sqlmapproject/sqlmap/wiki/FAQ
-        -  Twitter: https://twitter.com/sqlmap
+        -  X: https://twitter.com/sqlmap
         -  Demos: http://www.youtube.com/user/inquisb/videos
         -  Screenshots: https://github.com/sqlmapproject/sqlmap/wiki/Screenshots
         
         .. |Python 2.6|2.7|3.x| image:: https://img.shields.io/badge/python-2.6|2.7|3.x-yellow.svg
            :target: https://www.python.org/
         .. |License| image:: https://img.shields.io/badge/license-GPLv2-red.svg
            :target: https://raw.githubusercontent.com/sqlmapproject/sqlmap/master/LICENSE
```

### Comparing `sqlmap-1.8.3/setup.py` & `sqlmap-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 See the file 'LICENSE' for copying permission
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='sqlmap',
-    version='1.8.3',
+    version='1.8.4',
     description='Automatic SQL injection and database takeover tool',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author='Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar',
     author_email='bernardo@sqlmap.org, miroslav@sqlmap.org',
     url='https://sqlmap.org',
     project_urls={
         'Documentation': 'https://github.com/sqlmapproject/sqlmap/wiki',
         'Source': 'https://github.com/sqlmapproject/sqlmap/',
         'Tracker': 'https://github.com/sqlmapproject/sqlmap/issues',
     },
-    download_url='https://github.com/sqlmapproject/sqlmap/archive/1.8.3.zip',
+    download_url='https://github.com/sqlmapproject/sqlmap/archive/1.8.4.zip',
     license='GNU General Public License v2 (GPLv2)',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

