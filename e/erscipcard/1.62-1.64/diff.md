# Comparing `tmp/erscipcard-1.62.tar.gz` & `tmp/erscipcard-1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.62.tar", last modified: Mon Apr  8 04:13:12 2024, max compression
+gzip compressed data, was "erscipcard-1.64.tar", last modified: Mon Apr  8 05:26:49 2024, max compression
```

## Comparing `erscipcard-1.62.tar` & `erscipcard-1.64.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.026160 erscipcard-1.62/
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-08 04:12:35.000000 erscipcard-1.62/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-08 04:12:35.000000 erscipcard-1.62/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-08 04:13:12.026160 erscipcard-1.62/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-08 04:12:35.000000 erscipcard-1.62/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.007159 erscipcard-1.62/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/epfsurls.py
--rw-r--r--   0 root         (0) root         (0)     6342 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/epfsviews.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/evtturls.py
--rw-r--r--   0 root         (0) root         (0)      821 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/evttviews.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/forms.py
--rw-r--r--   0 root         (0) root         (0)     2938 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/inst.py
--rw-r--r--   0 root         (0) root         (0)     2254 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/models.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/qrurls.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/qrviews.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.013159 erscipcard-1.62/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    11041 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    11792 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)     2648 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/back.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:11.999158 erscipcard-1.62/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.015159 erscipcard-1.62/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.016159 erscipcard-1.62/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.018159 erscipcard-1.62/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    58072 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/js/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.018159 erscipcard-1.62/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)     2344 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/doc.svg
--rw-r--r--   0 root         (0) root         (0)    37259 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/ersci_app.zip
--rw-r--r--   0 root         (0) root         (0)    12683 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/ersci_viddown_tab2-1.4.xpi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.019160 erscipcard-1.62/erscipcard/static/evtt/
--rw-r--r--   0 root         (0) root         (0)     5675 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/evtt/app.js
--rw-r--r--   0 root         (0) root         (0)    13027 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/evtt/recorder.js
--rw-r--r--   0 root         (0) root         (0)      950 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/evtt/style.css
--rw-r--r--   0 root         (0) root         (0)    29117 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/icon.png
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/inst
--rw-r--r--   0 root         (0) root         (0)    35195 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/main.css
--rw-r--r--   0 root         (0) root         (0)      525 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/manifest.json
--rw-r--r--   0 root         (0) root         (0)     2291 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/mic.svg
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/s
--rw-r--r--   0 root         (0) root         (0)      641 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.024160 erscipcard-1.62/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/spinners.css
--rw-r--r--   0 root         (0) root         (0)     1446 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/style.css
--rw-r--r--   0 root         (0) root         (0)        2 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/static/ytvid.mp4
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.025160 erscipcard-1.62/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.025160 erscipcard-1.62/erscipcard/templates/epfs/
--rw-r--r--   0 root         (0) root         (0)     5201 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templates/epfs/sharefile.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.025160 erscipcard-1.62/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    12224 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templates/erscipcard/ou.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.025160 erscipcard-1.62/erscipcard/templates/evtt/
--rw-r--r--   0 root         (0) root         (0)     2252 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templates/evtt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.026160 erscipcard-1.62/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1452 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    12726 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/widget.py
--rw-r--r--   0 root         (0) root         (0)      450 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/yturls.py
--rw-r--r--   0 root         (0) root         (0)    14884 2024-04-08 04:12:35.000000 erscipcard-1.62/erscipcard/ytviews.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:13:12.008159 erscipcard-1.62/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-08 04:13:11.000000 erscipcard-1.62/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3188 2024-04-08 04:13:11.000000 erscipcard-1.62/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 04:13:11.000000 erscipcard-1.62/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-08 04:13:11.000000 erscipcard-1.62/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-08 04:13:11.000000 erscipcard-1.62/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      777 2024-04-08 04:13:12.027160 erscipcard-1.62/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-08 04:12:35.000000 erscipcard-1.62/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-08 05:26:43.000000 erscipcard-1.64/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-08 05:26:43.000000 erscipcard-1.64/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-08 05:26:49.496103 erscipcard-1.64/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-08 05:26:43.000000 erscipcard-1.64/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.475101 erscipcard-1.64/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/epfsurls.py
+-rw-r--r--   0 root         (0) root         (0)     6342 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/epfsviews.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/evtturls.py
+-rw-r--r--   0 root         (0) root         (0)      821 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/evttviews.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/inst.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/models.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/qrurls.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/qrviews.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.482101 erscipcard-1.64/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    11041 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    11792 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/back.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.468100 erscipcard-1.64/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.483101 erscipcard-1.64/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.487102 erscipcard-1.64/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.488102 erscipcard-1.64/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    58072 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/js/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.489102 erscipcard-1.64/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/doc.svg
+-rw-r--r--   0 root         (0) root         (0)    37259 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/ersci_app.zip
+-rw-r--r--   0 root         (0) root         (0)    12683 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/ersci_viddown_tab2-1.4.xpi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.489102 erscipcard-1.64/erscipcard/static/evtt/
+-rw-r--r--   0 root         (0) root         (0)     5675 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/evtt/app.js
+-rw-r--r--   0 root         (0) root         (0)    13027 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/evtt/recorder.js
+-rw-r--r--   0 root         (0) root         (0)      950 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/evtt/style.css
+-rw-r--r--   0 root         (0) root         (0)    29117 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/icon.png
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/inst
+-rw-r--r--   0 root         (0) root         (0)    35195 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/main.css
+-rw-r--r--   0 root         (0) root         (0)      525 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/manifest.json
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/mic.svg
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/s
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/spinners.css
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/style.css
+-rw-r--r--   0 root         (0) root         (0)        2 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/static/ytvid.mp4
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/erscipcard/templates/epfs/
+-rw-r--r--   0 root         (0) root         (0)     5201 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templates/epfs/sharefile.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12224 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templates/erscipcard/ou.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/erscipcard/templates/evtt/
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templates/evtt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.494102 erscipcard-1.64/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12726 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/widget.py
+-rw-r--r--   0 root         (0) root         (0)      450 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/yturls.py
+-rw-r--r--   0 root         (0) root         (0)    14835 2024-04-08 05:26:43.000000 erscipcard-1.64/erscipcard/ytviews.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 05:26:49.476101 erscipcard-1.64/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-08 05:26:49.000000 erscipcard-1.64/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3188 2024-04-08 05:26:49.000000 erscipcard-1.64/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 05:26:49.000000 erscipcard-1.64/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-08 05:26:49.000000 erscipcard-1.64/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-08 05:26:49.000000 erscipcard-1.64/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      777 2024-04-08 05:26:49.496103 erscipcard-1.64/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-08 05:26:43.000000 erscipcard-1.64/setup.py
```

### Comparing `erscipcard-1.62/LICENSE` & `erscipcard-1.64/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/PKG-INFO` & `erscipcard-1.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.62
+Version: 1.64
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `erscipcard-1.62/README.md` & `erscipcard-1.64/README.md`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/epfsurls.py` & `erscipcard-1.64/erscipcard/epfsurls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/epfsviews.py` & `erscipcard-1.64/erscipcard/epfsviews.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/evtturls.py` & `erscipcard-1.64/erscipcard/evtturls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/evttviews.py` & `erscipcard-1.64/erscipcard/evttviews.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/forms.py` & `erscipcard-1.64/erscipcard/forms.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/inst.py` & `erscipcard-1.64/erscipcard/inst.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/models.py` & `erscipcard-1.64/erscipcard/models.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/qrviews.py` & `erscipcard-1.64/erscipcard/qrviews.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/1.docx` & `erscipcard-1.64/erscipcard/static/1.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/2.docx` & `erscipcard-1.64/erscipcard/static/2.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.64/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/BTITR.TTF` & `erscipcard-1.64/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/back.svg` & `erscipcard-1.64/erscipcard/static/back.svg`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.64/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.64/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.64/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.64/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/css/style.css` & `erscipcard-1.64/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/css/util.css` & `erscipcard-1.64/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.64/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.64/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.64/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.64/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.64/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/js/bootstrap.min.js` & `erscipcard-1.64/erscipcard/static/bt/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.64/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.64/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.64/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.64/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.64/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.64/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/doc.svg` & `erscipcard-1.64/erscipcard/static/doc.svg`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/ersci_app.zip` & `erscipcard-1.64/erscipcard/static/ersci_app.zip`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/ersci_viddown_tab2-1.4.xpi` & `erscipcard-1.64/erscipcard/static/ersci_viddown_tab2-1.4.xpi`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/evtt/app.js` & `erscipcard-1.64/erscipcard/static/evtt/app.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/evtt/recorder.js` & `erscipcard-1.64/erscipcard/static/evtt/recorder.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/evtt/style.css` & `erscipcard-1.64/erscipcard/static/evtt/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/favicon.ico` & `erscipcard-1.64/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/icon.png` & `erscipcard-1.64/erscipcard/static/icon.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/inst` & `erscipcard-1.64/erscipcard/static/inst`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/logo.png` & `erscipcard-1.64/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/main.css` & `erscipcard-1.64/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/manifest.json` & `erscipcard-1.64/erscipcard/static/manifest.json`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/mic.svg` & `erscipcard-1.64/erscipcard/static/mic.svg`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/service-worker.js` & `erscipcard-1.64/erscipcard/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/atebits.css` & `erscipcard-1.64/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/ball.css` & `erscipcard-1.64/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/circles.css` & `erscipcard-1.64/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/dots.css` & `erscipcard-1.64/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/echo.css` & `erscipcard-1.64/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/flower.css` & `erscipcard-1.64/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/gauge.css` & `erscipcard-1.64/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.64/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.64/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.64/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.64/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.64/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/plus.css` & `erscipcard-1.64/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/pong.css` & `erscipcard-1.64/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/pulse.css` & `erscipcard-1.64/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.64/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/spinner.css` & `erscipcard-1.64/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.64/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.64/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/throbber.css` & `erscipcard-1.64/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/timer.css` & `erscipcard-1.64/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/whirly.css` & `erscipcard-1.64/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.64/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/spinners.css` & `erscipcard-1.64/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/static/style.css` & `erscipcard-1.64/erscipcard/static/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/templates/epfs/sharefile.html` & `erscipcard-1.64/erscipcard/templates/epfs/sharefile.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.64/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.64/erscipcard/templates/erscipcard/ou.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/templates/evtt/index.html` & `erscipcard-1.64/erscipcard/templates/evtt/index.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/urls.py` & `erscipcard-1.64/erscipcard/urls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/views.py` & `erscipcard-1.64/erscipcard/views.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/widget.py` & `erscipcard-1.64/erscipcard/widget.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/erscipcard/ytviews.py` & `erscipcard-1.64/erscipcard/ytviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,17 +263,16 @@
         os.system('sudo service nginx restart')
         return redirect(f'https://{url}/a.mp4')
     except:
         return ('Youtube Url Is Mistake!')
     
 def ytv(request,url,link):
     try:
-        os.system('sudo yt-dlp  -f 18 -o /content/a.mp4 https://www.youtube.com/watch?v={}'.format(link))        
-        os.system('sudo service nginx restart')
-        return redirect(f'https://{url}/a.mp4')
+        os.system('sudo yt-dlp  -f 18 -o video.mp4 https://www.youtube.com/watch?v={}'.format(link))        
+        return redirect(f'https://{url}/video.mp4')
     except:
         return ('Youtube Url Is Mistake!')
 
 def ytp(request,link):
     try:
         os.system('sudo yt-dlp  -f 18 -o /content/a.mp4 https://www.youtube.com/watch?v={}'.format(link))        
         filename = '/content/a.mp4'
```

### Comparing `erscipcard-1.62/erscipcard.egg-info/PKG-INFO` & `erscipcard-1.64/erscipcard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.62
+Version: 1.64
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `erscipcard-1.62/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.64/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.62/setup.cfg` & `erscipcard-1.64/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.62
+version = 1.64
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

