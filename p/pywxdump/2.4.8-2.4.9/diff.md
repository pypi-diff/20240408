# Comparing `tmp/pywxdump-2.4.8.tar.gz` & `tmp/pywxdump-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywxdump-2.4.8.tar", last modified: Tue Jan  9 10:55:02 2024, max compression
+gzip compressed data, was "pywxdump-2.4.9.tar", last modified: Tue Jan  9 14:20:58 2024, max compression
```

## Comparing `pywxdump-2.4.8.tar` & `pywxdump-2.4.9.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.986455 pywxdump-2.4.8/
--rw-rw-rw-   0        0        0     1147 2024-01-09 10:53:59.000000 pywxdump-2.4.8/LICENSE
--rw-rw-rw-   0        0        0     9607 2024-01-09 10:55:01.986455 pywxdump-2.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     8862 2024-01-09 10:53:59.000000 pywxdump-2.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.923955 pywxdump-2.4.8/pywxdump/
--rw-rw-rw-   0        0        0     1010 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.939577 pywxdump-2.4.8/pywxdump/analyzer/
--rw-rw-rw-   0        0        0      547 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/analyzer/__init__.py
--rw-rw-rw-   0        0        0    16241 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/analyzer/chat_analysis.py
--rw-rw-rw-   0        0        0     9175 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/analyzer/db_parsing.py
--rw-rw-rw-   0        0        0    11633 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/analyzer/export_chat.py
--rw-rw-rw-   0        0        0     4909 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/analyzer/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.939577 pywxdump-2.4.8/pywxdump/api/
--rw-rw-rw-   0        0        0      354 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/api/__init__.py
--rw-rw-rw-   0        0        0     6499 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/api/api.py
--rw-rw-rw-   0        0        0     2830 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/api/rjson.py
--rw-rw-rw-   0        0        0    24138 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/cli.py
--rw-rw-rw-   0        0        0     1102 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/server.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.939577 pywxdump-2.4.8/pywxdump/ui/
--rw-rw-rw-   0        0        0      396 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.939577 pywxdump-2.4.8/pywxdump/ui/templates/
--rw-rw-rw-   0        0        0     2935 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/templates/chat.html
--rw-rw-rw-   0        0        0     8758 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/templates/index.html
--rw-rw-rw-   0        0        0    13425 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/view_chat.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.939577 pywxdump-2.4.8/pywxdump/ui/web/
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.986455 pywxdump-2.4.8/pywxdump/ui/web/assets/
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView--cnbKyym.js
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-CSBYkAXG.js
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-MhlltB0I.js
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-Sn48sdfK.js
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-_s3gT1Xp.js
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-kYVs5JEG.js
--rw-rw-rw-   0        0        0     9631 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-rPqWO3uF.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-9ehgf76d.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-GJ4usZ7i.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-JYvOIZ-h.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-NExRUHcN.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-S8cEni1P.js
--rw-rw-rw-   0        0        0      130 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-SGGZRxzN.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/BiasView-sTt7E6fn.js
--rw-rw-rw-   0        0        0     6216 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-15JuBujm.css
--rw-rw-rw-   0        0        0    39669 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-4ri3i3eq.js
--rw-rw-rw-   0        0        0     6216 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-Cq3nrHWr.css
--rw-rw-rw-   0        0        0    39279 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-FJ9S7qyN.js
--rw-rw-rw-   0        0        0    39279 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-HW_vdY-j.js
--rw-rw-rw-   0        0        0    39220 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-I97tceRE.js
--rw-rw-rw-   0        0        0    39247 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-f1frImBl.js
--rw-rw-rw-   0        0        0    39799 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-jPL_n3Jb.js
--rw-rw-rw-   0        0        0     6279 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-jmXHC3bo.css
--rw-rw-rw-   0        0        0     6279 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-m6EtLxOn.css
--rw-rw-rw-   0        0        0    39279 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-wPwc1zoU.js
--rw-rw-rw-   0        0        0     6279 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-z--hfQ3b.css
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-2Qa3Wr8S.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-P07bl4Jm.js
--rw-rw-rw-   0        0        0      130 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-Q00DOMTR.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-Rb9jr00x.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-WsqxZecE.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-oA-kfyeb.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/DecryptView-u74EqMxx.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-9KuJj0oa.js
--rw-rw-rw-   0        0        0      130 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-K6aMFPGo.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-LXLUt7GL.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-N1QRWJbS.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-ZWP2OetY.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-aBV0pbzt.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/ExportView-qGAsS75W.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView--AuXynPs.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-7mSirb0J.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-mICbfIET.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-qB-m2RRg.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-rRdILXH_.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-xsTynFSv.js
--rw-rw-rw-   0        0        0     9569 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-zAt3JwGe.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-2Qa3Wr8S.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-P07bl4Jm.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-Rb9jr00x.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-WsqxZecE.js
--rw-rw-rw-   0        0        0      130 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-Y01u0JPM.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-oA-kfyeb.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/MergeView-u74EqMxx.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView--ftkEmmU.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView-8rlx9JqU.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView-IVrFP57G.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView-Yth5IqVq.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView-v-n8Q3Re.js
--rw-rw-rw-   0        0        0      497 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView-wZ1Lzh9k.js
--rw-rw-rw-   0        0        0      130 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/StatisticsView-x7MZYcRO.js
--rw-rw-rw-   0        0        0      130 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-3m0pT8F6.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-7B-uuO4n.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-GheYIeQt.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-T1JKlNEu.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-ZqEAZdPk.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-k_BUJAJw.js
--rw-rw-rw-   0        0        0      502 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/WxinfoView-o23bX2UB.js
--rw-rw-rw-   0        0        0   890768 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-2HAW1XkK.js
--rw-rw-rw-   0        0        0   890760 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-37InGr6e.js
--rw-rw-rw-   0        0        0   327570 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-9ireuRE8.css
--rw-rw-rw-   0        0        0   890572 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-E8u1MHmX.js
--rw-rw-rw-   0        0        0   890760 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-PqvHLxTR.js
--rw-rw-rw-   0        0        0   890572 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-Z9WQipGJ.js
--rw-rw-rw-   0        0        0   890572 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-ct5HAHRh.js
--rw-rw-rw-   0        0        0   890768 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-jRSp3SF2.js
--rw-rw-rw-   0        0        0   327610 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/index-k5cZ60vP.css
--rw-rw-rw-   0        0        0    84108 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/qq-iQ8jIM6k.png
--rw-rw-rw-   0        0        0    27332 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/assets/qrcode_gh-wCDAugtE.jpg
--rw-rw-rw-   0        0        0    67646 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/favicon.ico
--rw-rw-rw-   0        0        0      575 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/ui/web/index.html
--rw-rw-rw-   0        0        0     4803 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/version_list.json
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.986455 pywxdump-2.4.8/pywxdump/wx_info/
--rw-rw-rw-   0        0        0      521 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/wx_info/__init__.py
--rw-rw-rw-   0        0        0     7956 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/wx_info/decryption.py
--rw-rw-rw-   0        0        0     8036 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/wx_info/get_bias_addr.py
--rw-rw-rw-   0        0        0    11475 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/wx_info/get_wx_info.py
--rw-rw-rw-   0        0        0    11862 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/wx_info/merge_db.py
--rw-rw-rw-   0        0        0     3606 2024-01-09 10:53:59.000000 pywxdump-2.4.8/pywxdump/wx_info/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.986455 pywxdump-2.4.8/pywxdump.egg-info/
--rw-rw-rw-   0        0        0     9607 2024-01-09 10:55:01.000000 pywxdump-2.4.8/pywxdump.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4521 2024-01-09 10:55:01.000000 pywxdump-2.4.8/pywxdump.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-09 10:55:01.000000 pywxdump-2.4.8/pywxdump.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-01-09 10:55:01.000000 pywxdump-2.4.8/pywxdump.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      128 2024-01-09 10:55:01.000000 pywxdump-2.4.8/pywxdump.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-09 10:55:01.000000 pywxdump-2.4.8/pywxdump.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-09 10:55:01.986455 pywxdump-2.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1919 2024-01-09 10:53:59.000000 pywxdump-2.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-09 10:55:01.986455 pywxdump-2.4.8/tests/
--rw-rw-rw-   0        0        0      700 2024-01-09 10:53:59.000000 pywxdump-2.4.8/tests/test_Bias.py
--rw-rw-rw-   0        0        0     1246 2024-01-09 10:53:59.000000 pywxdump-2.4.8/tests/test_dbshow.py
--rw-rw-rw-   0        0        0      590 2024-01-09 10:53:59.000000 pywxdump-2.4.8/tests/test_decrypt.py
--rw-rw-rw-   0        0        0      513 2024-01-09 10:53:59.000000 pywxdump-2.4.8/tests/test_read_info.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.111793 pywxdump-2.4.9/
+-rw-rw-rw-   0        0        0     1147 2024-01-09 14:19:48.000000 pywxdump-2.4.9/LICENSE
+-rw-rw-rw-   0        0        0     9748 2024-01-09 14:20:58.111793 pywxdump-2.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9003 2024-01-09 14:19:48.000000 pywxdump-2.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.049297 pywxdump-2.4.9/pywxdump/
+-rw-rw-rw-   0        0        0     1010 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.049297 pywxdump-2.4.9/pywxdump/analyzer/
+-rw-rw-rw-   0        0        0      547 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/analyzer/__init__.py
+-rw-rw-rw-   0        0        0    16241 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/analyzer/chat_analysis.py
+-rw-rw-rw-   0        0        0     9175 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/analyzer/db_parsing.py
+-rw-rw-rw-   0        0        0    11904 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/analyzer/export_chat.py
+-rw-rw-rw-   0        0        0     4909 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/analyzer/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.049297 pywxdump-2.4.9/pywxdump/api/
+-rw-rw-rw-   0        0        0      354 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/api/__init__.py
+-rw-rw-rw-   0        0        0     6499 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/api/api.py
+-rw-rw-rw-   0        0        0     2830 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/api/rjson.py
+-rw-rw-rw-   0        0        0    24310 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/cli.py
+-rw-rw-rw-   0        0        0     1102 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/server.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.049297 pywxdump-2.4.9/pywxdump/ui/
+-rw-rw-rw-   0        0        0      396 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.049297 pywxdump-2.4.9/pywxdump/ui/templates/
+-rw-rw-rw-   0        0        0     2935 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/templates/chat.html
+-rw-rw-rw-   0        0        0     8758 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/templates/index.html
+-rw-rw-rw-   0        0        0    13425 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/view_chat.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.064923 pywxdump-2.4.9/pywxdump/ui/web/
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.096169 pywxdump-2.4.9/pywxdump/ui/web/assets/
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView--cnbKyym.js
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-CSBYkAXG.js
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-MhlltB0I.js
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-Sn48sdfK.js
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-_s3gT1Xp.js
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-kYVs5JEG.js
+-rw-rw-rw-   0        0        0     9631 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-rPqWO3uF.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-9ehgf76d.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-GJ4usZ7i.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-JYvOIZ-h.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-NExRUHcN.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-S8cEni1P.js
+-rw-rw-rw-   0        0        0      130 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-SGGZRxzN.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/BiasView-sTt7E6fn.js
+-rw-rw-rw-   0        0        0     6216 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-15JuBujm.css
+-rw-rw-rw-   0        0        0    39669 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-4ri3i3eq.js
+-rw-rw-rw-   0        0        0     6216 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-Cq3nrHWr.css
+-rw-rw-rw-   0        0        0    39279 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-FJ9S7qyN.js
+-rw-rw-rw-   0        0        0    39279 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-HW_vdY-j.js
+-rw-rw-rw-   0        0        0    39220 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-I97tceRE.js
+-rw-rw-rw-   0        0        0    39247 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-f1frImBl.js
+-rw-rw-rw-   0        0        0    39799 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-jPL_n3Jb.js
+-rw-rw-rw-   0        0        0     6279 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-jmXHC3bo.css
+-rw-rw-rw-   0        0        0     6279 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-m6EtLxOn.css
+-rw-rw-rw-   0        0        0    39279 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-wPwc1zoU.js
+-rw-rw-rw-   0        0        0     6279 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-z--hfQ3b.css
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-2Qa3Wr8S.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-P07bl4Jm.js
+-rw-rw-rw-   0        0        0      130 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-Q00DOMTR.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-Rb9jr00x.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-WsqxZecE.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-oA-kfyeb.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/DecryptView-u74EqMxx.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-9KuJj0oa.js
+-rw-rw-rw-   0        0        0      130 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-K6aMFPGo.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-LXLUt7GL.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-N1QRWJbS.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-ZWP2OetY.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-aBV0pbzt.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/ExportView-qGAsS75W.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView--AuXynPs.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-7mSirb0J.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-mICbfIET.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-qB-m2RRg.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-rRdILXH_.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-xsTynFSv.js
+-rw-rw-rw-   0        0        0     9569 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-zAt3JwGe.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-2Qa3Wr8S.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-P07bl4Jm.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-Rb9jr00x.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-WsqxZecE.js
+-rw-rw-rw-   0        0        0      130 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-Y01u0JPM.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-oA-kfyeb.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/MergeView-u74EqMxx.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView--ftkEmmU.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView-8rlx9JqU.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView-IVrFP57G.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView-Yth5IqVq.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView-v-n8Q3Re.js
+-rw-rw-rw-   0        0        0      497 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView-wZ1Lzh9k.js
+-rw-rw-rw-   0        0        0      130 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/StatisticsView-x7MZYcRO.js
+-rw-rw-rw-   0        0        0      130 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-3m0pT8F6.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-7B-uuO4n.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-GheYIeQt.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-T1JKlNEu.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-ZqEAZdPk.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-k_BUJAJw.js
+-rw-rw-rw-   0        0        0      502 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/WxinfoView-o23bX2UB.js
+-rw-rw-rw-   0        0        0   890768 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-2HAW1XkK.js
+-rw-rw-rw-   0        0        0   890760 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-37InGr6e.js
+-rw-rw-rw-   0        0        0   327570 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-9ireuRE8.css
+-rw-rw-rw-   0        0        0   890572 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-E8u1MHmX.js
+-rw-rw-rw-   0        0        0   890760 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-PqvHLxTR.js
+-rw-rw-rw-   0        0        0   890572 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-Z9WQipGJ.js
+-rw-rw-rw-   0        0        0   890572 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-ct5HAHRh.js
+-rw-rw-rw-   0        0        0   890768 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-jRSp3SF2.js
+-rw-rw-rw-   0        0        0   327610 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/index-k5cZ60vP.css
+-rw-rw-rw-   0        0        0    84108 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/qq-iQ8jIM6k.png
+-rw-rw-rw-   0        0        0    27332 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/assets/qrcode_gh-wCDAugtE.jpg
+-rw-rw-rw-   0        0        0    67646 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/favicon.ico
+-rw-rw-rw-   0        0        0      575 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/ui/web/index.html
+-rw-rw-rw-   0        0        0     4803 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/version_list.json
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.111793 pywxdump-2.4.9/pywxdump/wx_info/
+-rw-rw-rw-   0        0        0      521 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/wx_info/__init__.py
+-rw-rw-rw-   0        0        0     7956 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/wx_info/decryption.py
+-rw-rw-rw-   0        0        0     8036 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/wx_info/get_bias_addr.py
+-rw-rw-rw-   0        0        0    11475 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/wx_info/get_wx_info.py
+-rw-rw-rw-   0        0        0    11862 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/wx_info/merge_db.py
+-rw-rw-rw-   0        0        0     3606 2024-01-09 14:19:48.000000 pywxdump-2.4.9/pywxdump/wx_info/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.111793 pywxdump-2.4.9/pywxdump.egg-info/
+-rw-rw-rw-   0        0        0     9748 2024-01-09 14:20:58.000000 pywxdump-2.4.9/pywxdump.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-01-09 14:20:58.000000 pywxdump-2.4.9/pywxdump.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-09 14:20:58.000000 pywxdump-2.4.9/pywxdump.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-01-09 14:20:58.000000 pywxdump-2.4.9/pywxdump.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      128 2024-01-09 14:20:58.000000 pywxdump-2.4.9/pywxdump.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-01-09 14:20:58.000000 pywxdump-2.4.9/pywxdump.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-09 14:20:58.111793 pywxdump-2.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1919 2024-01-09 14:19:48.000000 pywxdump-2.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-09 14:20:58.111793 pywxdump-2.4.9/tests/
+-rw-rw-rw-   0        0        0      700 2024-01-09 14:19:48.000000 pywxdump-2.4.9/tests/test_Bias.py
+-rw-rw-rw-   0        0        0     1246 2024-01-09 14:19:48.000000 pywxdump-2.4.9/tests/test_dbshow.py
+-rw-rw-rw-   0        0        0      590 2024-01-09 14:19:48.000000 pywxdump-2.4.9/tests/test_decrypt.py
+-rw-rw-rw-   0        0        0      513 2024-01-09 14:19:48.000000 pywxdump-2.4.9/tests/test_read_info.py
```

### Comparing `pywxdump-2.4.8/LICENSE` & `pywxdump-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/PKG-INFO` & `pywxdump-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdump
-Version: 2.4.8
+Version: 2.4.9
 Summary: 微信信息获取工具
 Home-page: https://github.com/xaoyaoo/PyWxDump
 Author: xaoyaoo
 Author-email: xaoyaoo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,17 @@
 [![GitHub license](https://img.shields.io/pypi/l/pywxdump)](https://github.com/xaoyaoo/PyWxDump/blob/master/LICENSE)
 [![Publish](https://github.com/xaoyaoo/PyWxDump/actions/workflows/publish.yml/badge.svg)](https://github.com/xaoyaoo/PyWxDump/actions/workflows/publish.yml)
 
 * 欢迎大家提供更多的想法，或者提供代码，一起完善这个项目。
 
 ### 如有问题，请先查看：[FAQ](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/FAQ.md) 是否有答案，或者关注公众号回复: `FAQ`。
 
-### 如果是小白，请关注公众号：`逍遥之芯` (右边二维码) ，回复：`PyWxDump` 获取图文教程。
+### 如果是小白，请关注公众号：`逍遥之芯`(右边二维码)，回复：`PyWxDump` 获取图文教程。
+
+### 如果对wxdump实现原理感兴趣，请关注公众号：`逍遥之芯`(右边二维码)，回复：`原理` 获取原理解析。
 
 qq交流群：577704006（左边二维码） or 点击链接加入群聊[pywxdump功能交流](https://s.xaoyo.top/gOLUDl)。
 
 （因为qq群将满，所以进群需要密码，密码请查看[UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)）
 
 <div>
 <a href="https://s.xaoyo.top/gOLUDl">
@@ -135,19 +137,19 @@
 
 [![Star History Chart](https://api.star-history.com/svg?repos=xaoyaoo/pywxdump&type=Date)](https://star-history.com/#xaoyaoo/pywxdump&Date)
 
 </details>
 
 # 二、使用说明
 
-* 详细使用说明见[UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)
+* 详细使用说明见 [UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)
 
-* 极简版使用说明[pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini)
+* 极简版使用说明 [pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini) 
 
-* 如果你想更改UI，请clone[wx_dump_web](https://github.com/xaoyaoo/wx_dump_web)项目，然后按需修改（该UI采用VUE+ElementUI开发）
+* 如果想修改UI，请clone [wx_dump_web](https://github.com/xaoyaoo/wx_dump_web) 项目，然后按需修改（该UI采用VUE+ElementUI开发）
 
 【注】:
 
 * 关于基址使用cheat engine获取，参考[CE获取基址.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/CE获取基址.md)
   （该方法可用`wxdump bias`命令代替，现仅用作学习原理）
 * 关于数据库解析，参考[wx数据库简述.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/wx数据库简述.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywxdump Version: 2.4.8 Summary:
+Metadata-Version: 2.1 Name: pywxdump Version: 2.4.9 Summary:
 å¾®ä¿¡ä¿¡æ¯è·åå·¥å· Home-page: https://github.com/xaoyaoo/PyWxDump Author:
 xaoyaoo Author-email: xaoyaoo@gmail.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: psutil Requires-Dist: pycryptodomex Requires-Dist:
 pywin32 Requires-Dist: pymem Requires-Dist: silk-python Requires-Dist: pyaudio
 Requires-Dist: requests Requires-Dist: pillow Requires-Dist: pyahocorasick
@@ -25,16 +25,18 @@
 [GitHub license](https://img.shields.io/pypi/l/pywxdump)](https://github.com/
 xaoyaoo/PyWxDump/blob/master/LICENSE) [![Publish](https://github.com/xaoyaoo/
 PyWxDump/actions/workflows/publish.yml/badge.svg)](https://github.com/xaoyaoo/
 PyWxDump/actions/workflows/publish.yml) *
 æ¬¢è¿å¤§å®¶æä¾æ´å¤çæ³æ³ï¼æèæä¾ä»£ç ï¼ä¸èµ·å®åè¿ä¸ªé¡¹ç®ã
 ### å¦æé®é¢ï¼è¯·åæ¥çï¼[FAQ](https://github.com/xaoyaoo/PyWxDump/
 tree/master/doc/FAQ.md) æ¯å¦æç­æ¡ï¼æèå³æ³¨å¬ä¼å·åå¤: `FAQ`ã
-### å¦ææ¯å°ç½ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯` (å³è¾¹äºç»´ç )
-ï¼åå¤ï¼`PyWxDump` è·åå¾ææç¨ã
+### å¦ææ¯å°ç½ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯`
+(å³è¾¹äºç»´ç )ï¼åå¤ï¼`PyWxDump` è·åå¾ææç¨ã ###
+å¦æå¯¹wxdumpå®ç°åçæå´è¶£ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯`
+(å³è¾¹äºç»´ç )ï¼åå¤ï¼`åç` è·ååçè§£æã
 qqäº¤æµç¾¤ï¼577704006ï¼å·¦è¾¹äºç»´ç ï¼ or ç¹å»é¾æ¥å å¥ç¾¤è
 [pywxdumpåè½äº¤æµ](https://s.xaoyo.top/gOLUDl)ã
 ï¼å ä¸ºqqç¾¤å°æ»¡ï¼æä»¥è¿ç¾¤éè¦å¯ç ï¼å¯ç è¯·æ¥ç[UserGuide.md]
 (https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)ï¼
 _[_Q_Q_ç_¾_¤_][å¬ä¼å·]
 # ä¸ãé¡¹ç®ä»ç» ## 1. é¡¹ç®ç®ä» [PyWxDump](https://github.com/xaoyaoo/
 PyWxDump)æ¯ä¸æ¬¾ç¨äºè·åè´¦å·ä¿¡æ¯(æµç§°/è´¦å·/ææº/é®ç®±/
@@ -84,19 +86,19 @@
 å¸¸è§é®é¢è¯·åè[FAQ](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/
 FAQ.md)ï¼æ´æ°æ¥å¿è¯·åè[CHANGELOG](https://github.com/xaoyaoo/PyWxDump/
 tree/master/doc/CHANGELOG.md) * Web UIçä»åºä½ç½® [wxdump_web](https://
 github.com/xaoyaoo/wxdump_web) * [:sparkling\_heart: Support Me](https://
 github.com/xaoyaoo/xaoyaoo/blob/main/donate.md) ## 5. Star History click to
 expand [![Star History Chart](https://api.star-history.com/svg?repos=xaoyaoo/
 pywxdump&type=Date)](https://star-history.com/#xaoyaoo/pywxdump&Date) #
-äºãä½¿ç¨è¯´æ * è¯¦ç»ä½¿ç¨è¯´æè§[UserGuide.md](https://github.com/
+äºãä½¿ç¨è¯´æ * è¯¦ç»ä½¿ç¨è¯´æè§ [UserGuide.md](https://github.com/
 xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md) * æç®çä½¿ç¨è¯´æ
 [pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini) *
-å¦æä½ æ³æ´æ¹UIï¼è¯·clone[wx_dump_web](https://github.com/xaoyaoo/
-wx_dump_web)é¡¹ç®ï¼ç¶åæéä¿®æ¹ï¼è¯¥UIéç¨VUE+ElementUIå¼åï¼
+å¦ææ³ä¿®æ¹UIï¼è¯·clone [wx_dump_web](https://github.com/xaoyaoo/
+wx_dump_web) é¡¹ç®ï¼ç¶åæéä¿®æ¹ï¼è¯¥UIéç¨VUE+ElementUIå¼åï¼
 ãæ³¨ã: * å³äºåºåä½¿ç¨cheat engineè·åï¼åè[CEè·ååºå.md]
 (https://github.com/xaoyaoo/PyWxDump/tree/master/doc/CEè·ååºå.md)
 ï¼è¯¥æ¹æ³å¯ç¨`wxdump bias`å½ä»¤ä»£æ¿ï¼ç°ä»ç¨ä½å­¦ä¹ åçï¼ *
 å³äºæ°æ®åºè§£æï¼åè[wxæ°æ®åºç®è¿°.md](https://github.com/
 xaoyaoo/PyWxDump/tree/master/doc/wxæ°æ®åºç®è¿°.md) #
 ä¸ãåè´£å£°æï¼éå¸¸éè¦ï¼ï¼ï¼ï¼ï¼ï¼ï¼ï¼
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·å¿ç¨äºéæ³ç¨éï¼å¦ååæèªè´ã
```

### Comparing `pywxdump-2.4.8/README.md` & `pywxdump-2.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 [![GitHub license](https://img.shields.io/pypi/l/pywxdump)](https://github.com/xaoyaoo/PyWxDump/blob/master/LICENSE)
 [![Publish](https://github.com/xaoyaoo/PyWxDump/actions/workflows/publish.yml/badge.svg)](https://github.com/xaoyaoo/PyWxDump/actions/workflows/publish.yml)
 
 * 欢迎大家提供更多的想法，或者提供代码，一起完善这个项目。
 
 ### 如有问题，请先查看：[FAQ](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/FAQ.md) 是否有答案，或者关注公众号回复: `FAQ`。
 
-### 如果是小白，请关注公众号：`逍遥之芯` (右边二维码) ，回复：`PyWxDump` 获取图文教程。
+### 如果是小白，请关注公众号：`逍遥之芯`(右边二维码)，回复：`PyWxDump` 获取图文教程。
+
+### 如果对wxdump实现原理感兴趣，请关注公众号：`逍遥之芯`(右边二维码)，回复：`原理` 获取原理解析。
 
 qq交流群：577704006（左边二维码） or 点击链接加入群聊[pywxdump功能交流](https://s.xaoyo.top/gOLUDl)。
 
 （因为qq群将满，所以进群需要密码，密码请查看[UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)）
 
 <div>
 <a href="https://s.xaoyo.top/gOLUDl">
@@ -107,19 +109,19 @@
 
 [![Star History Chart](https://api.star-history.com/svg?repos=xaoyaoo/pywxdump&type=Date)](https://star-history.com/#xaoyaoo/pywxdump&Date)
 
 </details>
 
 # 二、使用说明
 
-* 详细使用说明见[UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)
+* 详细使用说明见 [UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)
 
-* 极简版使用说明[pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini)
+* 极简版使用说明 [pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini) 
 
-* 如果你想更改UI，请clone[wx_dump_web](https://github.com/xaoyaoo/wx_dump_web)项目，然后按需修改（该UI采用VUE+ElementUI开发）
+* 如果想修改UI，请clone [wx_dump_web](https://github.com/xaoyaoo/wx_dump_web) 项目，然后按需修改（该UI采用VUE+ElementUI开发）
 
 【注】:
 
 * 关于基址使用cheat engine获取，参考[CE获取基址.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/CE获取基址.md)
   （该方法可用`wxdump bias`命令代替，现仅用作学习原理）
 * 关于数据库解析，参考[wx数据库简述.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/wx数据库简述.md)
```

#### html2text {}

```diff
@@ -16,16 +16,18 @@
 [GitHub license](https://img.shields.io/pypi/l/pywxdump)](https://github.com/
 xaoyaoo/PyWxDump/blob/master/LICENSE) [![Publish](https://github.com/xaoyaoo/
 PyWxDump/actions/workflows/publish.yml/badge.svg)](https://github.com/xaoyaoo/
 PyWxDump/actions/workflows/publish.yml) *
 æ¬¢è¿å¤§å®¶æä¾æ´å¤çæ³æ³ï¼æèæä¾ä»£ç ï¼ä¸èµ·å®åè¿ä¸ªé¡¹ç®ã
 ### å¦æé®é¢ï¼è¯·åæ¥çï¼[FAQ](https://github.com/xaoyaoo/PyWxDump/
 tree/master/doc/FAQ.md) æ¯å¦æç­æ¡ï¼æèå³æ³¨å¬ä¼å·åå¤: `FAQ`ã
-### å¦ææ¯å°ç½ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯` (å³è¾¹äºç»´ç )
-ï¼åå¤ï¼`PyWxDump` è·åå¾ææç¨ã
+### å¦ææ¯å°ç½ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯`
+(å³è¾¹äºç»´ç )ï¼åå¤ï¼`PyWxDump` è·åå¾ææç¨ã ###
+å¦æå¯¹wxdumpå®ç°åçæå´è¶£ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯`
+(å³è¾¹äºç»´ç )ï¼åå¤ï¼`åç` è·ååçè§£æã
 qqäº¤æµç¾¤ï¼577704006ï¼å·¦è¾¹äºç»´ç ï¼ or ç¹å»é¾æ¥å å¥ç¾¤è
 [pywxdumpåè½äº¤æµ](https://s.xaoyo.top/gOLUDl)ã
 ï¼å ä¸ºqqç¾¤å°æ»¡ï¼æä»¥è¿ç¾¤éè¦å¯ç ï¼å¯ç è¯·æ¥ç[UserGuide.md]
 (https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)ï¼
 _[_Q_Q_ç_¾_¤_][å¬ä¼å·]
 # ä¸ãé¡¹ç®ä»ç» ## 1. é¡¹ç®ç®ä» [PyWxDump](https://github.com/xaoyaoo/
 PyWxDump)æ¯ä¸æ¬¾ç¨äºè·åè´¦å·ä¿¡æ¯(æµç§°/è´¦å·/ææº/é®ç®±/
@@ -75,19 +77,19 @@
 å¸¸è§é®é¢è¯·åè[FAQ](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/
 FAQ.md)ï¼æ´æ°æ¥å¿è¯·åè[CHANGELOG](https://github.com/xaoyaoo/PyWxDump/
 tree/master/doc/CHANGELOG.md) * Web UIçä»åºä½ç½® [wxdump_web](https://
 github.com/xaoyaoo/wxdump_web) * [:sparkling\_heart: Support Me](https://
 github.com/xaoyaoo/xaoyaoo/blob/main/donate.md) ## 5. Star History click to
 expand [![Star History Chart](https://api.star-history.com/svg?repos=xaoyaoo/
 pywxdump&type=Date)](https://star-history.com/#xaoyaoo/pywxdump&Date) #
-äºãä½¿ç¨è¯´æ * è¯¦ç»ä½¿ç¨è¯´æè§[UserGuide.md](https://github.com/
+äºãä½¿ç¨è¯´æ * è¯¦ç»ä½¿ç¨è¯´æè§ [UserGuide.md](https://github.com/
 xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md) * æç®çä½¿ç¨è¯´æ
 [pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini) *
-å¦æä½ æ³æ´æ¹UIï¼è¯·clone[wx_dump_web](https://github.com/xaoyaoo/
-wx_dump_web)é¡¹ç®ï¼ç¶åæéä¿®æ¹ï¼è¯¥UIéç¨VUE+ElementUIå¼åï¼
+å¦ææ³ä¿®æ¹UIï¼è¯·clone [wx_dump_web](https://github.com/xaoyaoo/
+wx_dump_web) é¡¹ç®ï¼ç¶åæéä¿®æ¹ï¼è¯¥UIéç¨VUE+ElementUIå¼åï¼
 ãæ³¨ã: * å³äºåºåä½¿ç¨cheat engineè·åï¼åè[CEè·ååºå.md]
 (https://github.com/xaoyaoo/PyWxDump/tree/master/doc/CEè·ååºå.md)
 ï¼è¯¥æ¹æ³å¯ç¨`wxdump bias`å½ä»¤ä»£æ¿ï¼ç°ä»ç¨ä½å­¦ä¹ åçï¼ *
 å³äºæ°æ®åºè§£æï¼åè[wxæ°æ®åºç®è¿°.md](https://github.com/
 xaoyaoo/PyWxDump/tree/master/doc/wxæ°æ®åºç®è¿°.md) #
 ä¸ãåè´£å£°æï¼éå¸¸éè¦ï¼ï¼ï¼ï¼ï¼ï¼ï¼ï¼
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·å¿ç¨äºéæ³ç¨éï¼å¦ååæèªè´ã
```

### Comparing `pywxdump-2.4.8/pywxdump/__init__.py` & `pywxdump-2.4.9/pywxdump/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     VERSION_LIST_PATH = os.path.join(os.path.dirname(__file__), "version_list.json")
     with open(VERSION_LIST_PATH, "r", encoding="utf-8") as f:
         VERSION_LIST = json.load(f)
 except:
     VERSION_LIST = {}
     VERSION_LIST_PATH = None
 
-__version__ = "2.4.8"
+__version__ = "2.4.9"
```

### Comparing `pywxdump-2.4.8/pywxdump/analyzer/__init__.py` & `pywxdump-2.4.9/pywxdump/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/analyzer/chat_analysis.py` & `pywxdump-2.4.9/pywxdump/analyzer/chat_analysis.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/analyzer/db_parsing.py` & `pywxdump-2.4.9/pywxdump/analyzer/db_parsing.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/analyzer/export_chat.py` & `pywxdump-2.4.9/pywxdump/analyzer/export_chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # -*- coding: utf-8 -*-#
 # -------------------------------------------------------------------------------
 # Name:         GUI.py
 # Description:
 # Author:       xaoyaoo
 # Date:         2023/11/10
 # -------------------------------------------------------------------------------
+import csv
 import re
 import sqlite3
 import os
 import json
 import time
 from functools import wraps
 
@@ -221,35 +222,40 @@
         outpath = os.path.join(os.getcwd(), "export" + os.sep + username)
         if not os.path.exists(outpath):
             os.makedirs(outpath)
     count = get_chat_count(MSG_ALL_db_path, username)
     chatCount = count.get(username, 0)
     if chatCount == 0:
         return False, "没有聊天记录"
+    if page_size > chatCount:
+        page_size = chatCount + 1
     for i in range(0, chatCount, page_size):
         start_index = i
         data = get_msg_list(MSG_ALL_db_path, username, start_index, page_size)
         if len(data) == 0:
+            return False, "没有聊天记录"
             break
-        save_path = os.path.join(outpath, f"{username}_{int(i / page_size)}.csv")
-        with open(save_path, "w", encoding="utf-8") as f:
-            f.write("id,MsgSvrID,type_name,is_sender,talker,room_name,content,CreateTime\n")
+        save_path = os.path.join(outpath, f"{username}_{i}_{i + page_size}.csv")
+        with open(save_path, "w", encoding="utf-8", newline='') as f:
+            csv_writer = csv.writer(f, quoting=csv.QUOTE_MINIMAL)
+            csv_writer.writerow(["id", "MsgSvrID", "type_name", "is_sender", "talker", "room_name", "content",
+                                 "CreateTime"])
             for row in data:
                 id = row.get("id", "")
                 MsgSvrID = row.get("MsgSvrID", "")
                 type_name = row.get("type_name", "")
                 is_sender = row.get("is_sender", "")
                 talker = row.get("talker", "")
                 room_name = row.get("room_name", "")
                 content = row.get("content", "")
                 CreateTime = row.get("CreateTime", "")
 
                 content = json.dumps(content, ensure_ascii=False)
+                csv_writer.writerow([id, MsgSvrID, type_name, is_sender, talker, room_name, content, CreateTime])
 
-                f.write(f"{id},{MsgSvrID},{type_name},{is_sender},{talker},{room_name},{content},{CreateTime}\n")
     return True, f"导出成功: {outpath}"
 
 
 def export_html(user, outpath, MSG_ALL_db_path, MediaMSG_all_db_path, FileStorage_path, page_size=500):
     name_save = user.get("remark", user.get("nickname", user.get("username", "")))
     username = user.get("username", "")
```

### Comparing `pywxdump-2.4.8/pywxdump/analyzer/utils.py` & `pywxdump-2.4.9/pywxdump/analyzer/utils.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/api/api.py` & `pywxdump-2.4.9/pywxdump/api/api.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/api/rjson.py` & `pywxdump-2.4.9/pywxdump/api/rjson.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/cli.py` & `pywxdump-2.4.9/pywxdump/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,54 +283,59 @@
         sb_decrypt.add_argument("-msg", "--msg_path", type=str, help="解密后的 MSG.db 的路径", required=True,
                                 metavar="")
         sb_decrypt.add_argument("-micro", "--micro_path", type=str, help="解密后的 MicroMsg.db 的路径", required=True,
                                 metavar="")
         sb_decrypt.add_argument("-media", "--media_path", type=str, help="解密后的 MediaMSG.db 的路径", required=True,
                                 metavar="")
         sb_decrypt.add_argument("-fs", "--filestorage_path", type=str,
-                                help="(可选)文件夹FileStorage的路径（用于显示图片）", required=False,
-                                metavar="")
-        sb_decrypt.add_argument("-t", "--type", type=str, help="导出类型(可选:html,txt)", required=False,
-                                default="html",
-                                metavar="")
+                                help="(可选)文件夹FileStorage的路径（用于显示图片）", required=False, metavar="")
+        sb_decrypt.add_argument("-t", "--type", type=str, help="导出类型(可选:html,csv)", required=False,
+                                default="html", metavar="")
         return sb_decrypt
 
     def run(self, args):
         # 从命令行参数获取值
         t = args.type
-        if t not in ["html", "txt"]:
-            print("[-] 未知的导出类型")
-            return
-        if t == "txt":
+
+        if t == "csv":
             try:
-                export_csv(args.username, args.outpath, args.msg_path, page_size=1000000)
+                code, ret = export_csv(args.username, args.outpath, args.msg_path, page_size=10000000)
+                if not code:
+                    print(ret)
+                    return
+                print(f"[+] {ret}")
+                return
             except Exception as e:
                 print(e)
                 print("[-] 导出失败")
                 return
-        try:
-            from flask import Flask, request, jsonify, render_template, g
-            import logging
-        except Exception as e:
-            print(e)
-            print("[-] 请安装flask( pip install flask)")
-            return
-
-        if not os.path.exists(args.msg_path) or not os.path.exists(args.micro_path) or not os.path.exists(
-                args.media_path):
-            print(os.path.exists(args.msg_path), os.path.exists(args.micro_path), os.path.exists(args.media_path))
-            print("[-] 输入数据库路径不存在")
-            return
+        elif t == "html":
+            try:
+                from flask import Flask, request, jsonify, render_template, g
+                import logging
+            except Exception as e:
+                print(e)
+                print("[-] 请安装flask( pip install flask)")
+                return
 
-        if not os.path.exists(args.outpath):
-            os.makedirs(args.outpath)
-            print(f"[+] 创建输出文件夹：{args.outpath}")
+            if not os.path.exists(args.msg_path) or not os.path.exists(args.micro_path) or not os.path.exists(
+                    args.media_path):
+                print(os.path.exists(args.msg_path), os.path.exists(args.micro_path), os.path.exists(args.media_path))
+                print("[-] 输入数据库路径不存在")
+                return
 
-        export(args.username, args.outpath, args.msg_path, args.micro_path, args.media_path, args.filestorage_path)
-        print(f"[+] 导出成功{args.outpath}")
+            if not os.path.exists(args.outpath):
+                os.makedirs(args.outpath)
+                print(f"[+] 创建输出文件夹：{args.outpath}")
+
+            export(args.username, args.outpath, args.msg_path, args.micro_path, args.media_path, args.filestorage_path)
+            print(f"[+] 导出成功{args.outpath}")
+        else:
+            print("[-] 未知的导出类型")
+            return
 
 
 class MainAll():
     def init_parses(self, parser):
         self.mode = "all"
         # 添加 'all' 子命令解析器
         sb_all = parser.add_parser(self.mode, help="获取微信信息，解密微信数据库，查看聊天记录")
```

### Comparing `pywxdump-2.4.8/pywxdump/server.py` & `pywxdump-2.4.9/pywxdump/server.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/templates/chat.html` & `pywxdump-2.4.9/pywxdump/ui/templates/chat.html`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/templates/index.html` & `pywxdump-2.4.9/pywxdump/ui/templates/index.html`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/view_chat.py` & `pywxdump-2.4.9/pywxdump/ui/view_chat.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView--cnbKyym.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView--cnbKyym.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-CSBYkAXG.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-CSBYkAXG.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-MhlltB0I.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-MhlltB0I.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-Sn48sdfK.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-Sn48sdfK.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-_s3gT1Xp.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-_s3gT1Xp.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-kYVs5JEG.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-kYVs5JEG.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/AboutView-rPqWO3uF.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/AboutView-rPqWO3uF.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-15JuBujm.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-15JuBujm.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-4ri3i3eq.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-4ri3i3eq.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-Cq3nrHWr.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-Cq3nrHWr.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-FJ9S7qyN.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-FJ9S7qyN.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-HW_vdY-j.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-HW_vdY-j.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-I97tceRE.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-I97tceRE.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-f1frImBl.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-f1frImBl.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-jPL_n3Jb.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-jPL_n3Jb.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-jmXHC3bo.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-jmXHC3bo.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-m6EtLxOn.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-m6EtLxOn.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-wPwc1zoU.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-wPwc1zoU.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/ChatView-z--hfQ3b.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/ChatView-z--hfQ3b.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView--AuXynPs.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView--AuXynPs.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-7mSirb0J.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-7mSirb0J.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-mICbfIET.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-mICbfIET.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-qB-m2RRg.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-qB-m2RRg.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-rRdILXH_.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-rRdILXH_.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-xsTynFSv.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-xsTynFSv.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/HelpView-zAt3JwGe.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/HelpView-zAt3JwGe.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-2HAW1XkK.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-2HAW1XkK.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-37InGr6e.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-37InGr6e.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-9ireuRE8.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-9ireuRE8.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-E8u1MHmX.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-E8u1MHmX.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-PqvHLxTR.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-PqvHLxTR.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-Z9WQipGJ.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-Z9WQipGJ.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-ct5HAHRh.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-ct5HAHRh.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-jRSp3SF2.js` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-jRSp3SF2.js`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/index-k5cZ60vP.css` & `pywxdump-2.4.9/pywxdump/ui/web/assets/index-k5cZ60vP.css`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/qq-iQ8jIM6k.png` & `pywxdump-2.4.9/pywxdump/ui/web/assets/qq-iQ8jIM6k.png`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/assets/qrcode_gh-wCDAugtE.jpg` & `pywxdump-2.4.9/pywxdump/ui/web/assets/qrcode_gh-wCDAugtE.jpg`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/favicon.ico` & `pywxdump-2.4.9/pywxdump/ui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/ui/web/index.html` & `pywxdump-2.4.9/pywxdump/ui/web/index.html`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/version_list.json` & `pywxdump-2.4.9/pywxdump/version_list.json`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/wx_info/__init__.py` & `pywxdump-2.4.9/pywxdump/wx_info/__init__.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/wx_info/decryption.py` & `pywxdump-2.4.9/pywxdump/wx_info/decryption.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/wx_info/get_bias_addr.py` & `pywxdump-2.4.9/pywxdump/wx_info/get_bias_addr.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/wx_info/get_wx_info.py` & `pywxdump-2.4.9/pywxdump/wx_info/get_wx_info.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/wx_info/merge_db.py` & `pywxdump-2.4.9/pywxdump/wx_info/merge_db.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump/wx_info/utils.py` & `pywxdump-2.4.9/pywxdump/wx_info/utils.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/pywxdump.egg-info/PKG-INFO` & `pywxdump-2.4.9/pywxdump.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdump
-Version: 2.4.8
+Version: 2.4.9
 Summary: 微信信息获取工具
 Home-page: https://github.com/xaoyaoo/PyWxDump
 Author: xaoyaoo
 Author-email: xaoyaoo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,17 @@
 [![GitHub license](https://img.shields.io/pypi/l/pywxdump)](https://github.com/xaoyaoo/PyWxDump/blob/master/LICENSE)
 [![Publish](https://github.com/xaoyaoo/PyWxDump/actions/workflows/publish.yml/badge.svg)](https://github.com/xaoyaoo/PyWxDump/actions/workflows/publish.yml)
 
 * 欢迎大家提供更多的想法，或者提供代码，一起完善这个项目。
 
 ### 如有问题，请先查看：[FAQ](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/FAQ.md) 是否有答案，或者关注公众号回复: `FAQ`。
 
-### 如果是小白，请关注公众号：`逍遥之芯` (右边二维码) ，回复：`PyWxDump` 获取图文教程。
+### 如果是小白，请关注公众号：`逍遥之芯`(右边二维码)，回复：`PyWxDump` 获取图文教程。
+
+### 如果对wxdump实现原理感兴趣，请关注公众号：`逍遥之芯`(右边二维码)，回复：`原理` 获取原理解析。
 
 qq交流群：577704006（左边二维码） or 点击链接加入群聊[pywxdump功能交流](https://s.xaoyo.top/gOLUDl)。
 
 （因为qq群将满，所以进群需要密码，密码请查看[UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)）
 
 <div>
 <a href="https://s.xaoyo.top/gOLUDl">
@@ -135,19 +137,19 @@
 
 [![Star History Chart](https://api.star-history.com/svg?repos=xaoyaoo/pywxdump&type=Date)](https://star-history.com/#xaoyaoo/pywxdump&Date)
 
 </details>
 
 # 二、使用说明
 
-* 详细使用说明见[UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)
+* 详细使用说明见 [UserGuide.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)
 
-* 极简版使用说明[pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini)
+* 极简版使用说明 [pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini) 
 
-* 如果你想更改UI，请clone[wx_dump_web](https://github.com/xaoyaoo/wx_dump_web)项目，然后按需修改（该UI采用VUE+ElementUI开发）
+* 如果想修改UI，请clone [wx_dump_web](https://github.com/xaoyaoo/wx_dump_web) 项目，然后按需修改（该UI采用VUE+ElementUI开发）
 
 【注】:
 
 * 关于基址使用cheat engine获取，参考[CE获取基址.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/CE获取基址.md)
   （该方法可用`wxdump bias`命令代替，现仅用作学习原理）
 * 关于数据库解析，参考[wx数据库简述.md](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/wx数据库简述.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywxdump Version: 2.4.8 Summary:
+Metadata-Version: 2.1 Name: pywxdump Version: 2.4.9 Summary:
 å¾®ä¿¡ä¿¡æ¯è·åå·¥å· Home-page: https://github.com/xaoyaoo/PyWxDump Author:
 xaoyaoo Author-email: xaoyaoo@gmail.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: psutil Requires-Dist: pycryptodomex Requires-Dist:
 pywin32 Requires-Dist: pymem Requires-Dist: silk-python Requires-Dist: pyaudio
 Requires-Dist: requests Requires-Dist: pillow Requires-Dist: pyahocorasick
@@ -25,16 +25,18 @@
 [GitHub license](https://img.shields.io/pypi/l/pywxdump)](https://github.com/
 xaoyaoo/PyWxDump/blob/master/LICENSE) [![Publish](https://github.com/xaoyaoo/
 PyWxDump/actions/workflows/publish.yml/badge.svg)](https://github.com/xaoyaoo/
 PyWxDump/actions/workflows/publish.yml) *
 æ¬¢è¿å¤§å®¶æä¾æ´å¤çæ³æ³ï¼æèæä¾ä»£ç ï¼ä¸èµ·å®åè¿ä¸ªé¡¹ç®ã
 ### å¦æé®é¢ï¼è¯·åæ¥çï¼[FAQ](https://github.com/xaoyaoo/PyWxDump/
 tree/master/doc/FAQ.md) æ¯å¦æç­æ¡ï¼æèå³æ³¨å¬ä¼å·åå¤: `FAQ`ã
-### å¦ææ¯å°ç½ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯` (å³è¾¹äºç»´ç )
-ï¼åå¤ï¼`PyWxDump` è·åå¾ææç¨ã
+### å¦ææ¯å°ç½ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯`
+(å³è¾¹äºç»´ç )ï¼åå¤ï¼`PyWxDump` è·åå¾ææç¨ã ###
+å¦æå¯¹wxdumpå®ç°åçæå´è¶£ï¼è¯·å³æ³¨å¬ä¼å·ï¼`éé¥ä¹è¯`
+(å³è¾¹äºç»´ç )ï¼åå¤ï¼`åç` è·ååçè§£æã
 qqäº¤æµç¾¤ï¼577704006ï¼å·¦è¾¹äºç»´ç ï¼ or ç¹å»é¾æ¥å å¥ç¾¤è
 [pywxdumpåè½äº¤æµ](https://s.xaoyo.top/gOLUDl)ã
 ï¼å ä¸ºqqç¾¤å°æ»¡ï¼æä»¥è¿ç¾¤éè¦å¯ç ï¼å¯ç è¯·æ¥ç[UserGuide.md]
 (https://github.com/xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md)ï¼
 _[_Q_Q_ç_¾_¤_][å¬ä¼å·]
 # ä¸ãé¡¹ç®ä»ç» ## 1. é¡¹ç®ç®ä» [PyWxDump](https://github.com/xaoyaoo/
 PyWxDump)æ¯ä¸æ¬¾ç¨äºè·åè´¦å·ä¿¡æ¯(æµç§°/è´¦å·/ææº/é®ç®±/
@@ -84,19 +86,19 @@
 å¸¸è§é®é¢è¯·åè[FAQ](https://github.com/xaoyaoo/PyWxDump/tree/master/doc/
 FAQ.md)ï¼æ´æ°æ¥å¿è¯·åè[CHANGELOG](https://github.com/xaoyaoo/PyWxDump/
 tree/master/doc/CHANGELOG.md) * Web UIçä»åºä½ç½® [wxdump_web](https://
 github.com/xaoyaoo/wxdump_web) * [:sparkling\_heart: Support Me](https://
 github.com/xaoyaoo/xaoyaoo/blob/main/donate.md) ## 5. Star History click to
 expand [![Star History Chart](https://api.star-history.com/svg?repos=xaoyaoo/
 pywxdump&type=Date)](https://star-history.com/#xaoyaoo/pywxdump&Date) #
-äºãä½¿ç¨è¯´æ * è¯¦ç»ä½¿ç¨è¯´æè§[UserGuide.md](https://github.com/
+äºãä½¿ç¨è¯´æ * è¯¦ç»ä½¿ç¨è¯´æè§ [UserGuide.md](https://github.com/
 xaoyaoo/PyWxDump/tree/master/doc/UserGuide.md) * æç®çä½¿ç¨è¯´æ
 [pywxdumpmini](https://github.com/xaoyaoo/pywxdumpmini) *
-å¦æä½ æ³æ´æ¹UIï¼è¯·clone[wx_dump_web](https://github.com/xaoyaoo/
-wx_dump_web)é¡¹ç®ï¼ç¶åæéä¿®æ¹ï¼è¯¥UIéç¨VUE+ElementUIå¼åï¼
+å¦ææ³ä¿®æ¹UIï¼è¯·clone [wx_dump_web](https://github.com/xaoyaoo/
+wx_dump_web) é¡¹ç®ï¼ç¶åæéä¿®æ¹ï¼è¯¥UIéç¨VUE+ElementUIå¼åï¼
 ãæ³¨ã: * å³äºåºåä½¿ç¨cheat engineè·åï¼åè[CEè·ååºå.md]
 (https://github.com/xaoyaoo/PyWxDump/tree/master/doc/CEè·ååºå.md)
 ï¼è¯¥æ¹æ³å¯ç¨`wxdump bias`å½ä»¤ä»£æ¿ï¼ç°ä»ç¨ä½å­¦ä¹ åçï¼ *
 å³äºæ°æ®åºè§£æï¼åè[wxæ°æ®åºç®è¿°.md](https://github.com/
 xaoyaoo/PyWxDump/tree/master/doc/wxæ°æ®åºç®è¿°.md) #
 ä¸ãåè´£å£°æï¼éå¸¸éè¦ï¼ï¼ï¼ï¼ï¼ï¼ï¼ï¼
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·å¿ç¨äºéæ³ç¨éï¼å¦ååæèªè´ã
```

### Comparing `pywxdump-2.4.8/pywxdump.egg-info/SOURCES.txt` & `pywxdump-2.4.9/pywxdump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/setup.py` & `pywxdump-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/tests/test_Bias.py` & `pywxdump-2.4.9/tests/test_Bias.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/tests/test_dbshow.py` & `pywxdump-2.4.9/tests/test_dbshow.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/tests/test_decrypt.py` & `pywxdump-2.4.9/tests/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `pywxdump-2.4.8/tests/test_read_info.py` & `pywxdump-2.4.9/tests/test_read_info.py`

 * *Files identical despite different names*

