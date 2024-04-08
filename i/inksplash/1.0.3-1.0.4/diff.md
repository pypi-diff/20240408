# Comparing `tmp/inksplash-1.0.3.tar.gz` & `tmp/inksplash-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inksplash-1.0.3.tar", last modified: Thu Mar  7 12:54:22 2024, max compression
+gzip compressed data, was "inksplash-1.0.4.tar", last modified: Mon Apr  8 07:05:57 2024, max compression
```

## Comparing `inksplash-1.0.3.tar` & `inksplash-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:15.000000 inksplash-1.0.3/.github/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-07 12:54:15.000000 inksplash-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-07 12:54:15.000000 inksplash-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-07 12:54:15.000000 inksplash-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-07 12:54:15.000000 inksplash-1.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-07 12:54:15.000000 inksplash-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-03-07 12:54:22.755830 inksplash-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-03-07 12:54:15.000000 inksplash-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-07 12:54:15.000000 inksplash-1.0.3/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/images/
--rw-r--r--   0 runner    (1001) docker     (127)    24236 2024-03-07 12:54:15.000000 inksplash-1.0.3/images/demo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/inksplash/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-07 12:54:15.000000 inksplash-1.0.3/inksplash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-03-07 12:54:15.000000 inksplash-1.0.3/inksplash/chameleon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/inksplash/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-07 12:54:15.000000 inksplash-1.0.3/inksplash/tests/test_hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:22.755830 inksplash-1.0.3/inksplash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-03-07 12:54:22.000000 inksplash-1.0.3/inksplash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-07 12:54:22.000000 inksplash-1.0.3/inksplash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:54:22.000000 inksplash-1.0.3/inksplash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 12:54:22.000000 inksplash-1.0.3/inksplash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-03-07 12:54:15.000000 inksplash-1.0.3/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-07 12:54:15.000000 inksplash-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-07 12:54:15.000000 inksplash-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 12:54:22.755830 inksplash-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.575133 inksplash-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:49.000000 inksplash-1.0.4/.github/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-08 07:05:49.000000 inksplash-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 07:05:49.000000 inksplash-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-08 07:05:49.000000 inksplash-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-08 07:05:49.000000 inksplash-1.0.4/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 07:05:49.000000 inksplash-1.0.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 07:05:49.000000 inksplash-1.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 07:05:49.000000 inksplash-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-08 07:05:57.575133 inksplash-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-04-08 07:05:49.000000 inksplash-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/docs/source/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/github/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/github/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/images/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/docs/source/styles_and_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/styles_and_functions/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/styles_and_functions/bg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/styles_and_functions/bright_bg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/styles_and_functions/bright_tc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/styles_and_functions/text_styles.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 07:05:49.000000 inksplash-1.0.4/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 07:05:49.000000 inksplash-1.0.4/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    24236 2024-04-08 07:05:49.000000 inksplash-1.0.4/images/demo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.571133 inksplash-1.0.4/inksplash/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 07:05:49.000000 inksplash-1.0.4/inksplash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-08 07:05:49.000000 inksplash-1.0.4/inksplash/chameleon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.575133 inksplash-1.0.4/inksplash/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 07:05:49.000000 inksplash-1.0.4/inksplash/tests/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:05:57.575133 inksplash-1.0.4/inksplash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-08 07:05:57.000000 inksplash-1.0.4/inksplash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-08 07:05:57.000000 inksplash-1.0.4/inksplash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:05:57.000000 inksplash-1.0.4/inksplash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 07:05:57.000000 inksplash-1.0.4/inksplash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-04-08 07:05:49.000000 inksplash-1.0.4/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-08 07:05:49.000000 inksplash-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 07:05:49.000000 inksplash-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:05:57.575133 inksplash-1.0.4/setup.cfg
```

### Comparing `inksplash-1.0.3/.github/workflows/ci.yml` & `inksplash-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/.github/workflows/publish.yml` & `inksplash-1.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/.gitignore` & `inksplash-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/LICENSE` & `inksplash-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/PKG-INFO` & `inksplash-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inksplash
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is a Python package that provides a versatile set of utilities for colorizing and styling text output in terminal environments.
 Author-email: Crispen Gari <crispengari@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 crispengari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,15 +73,16 @@
 - [Usage](#usage)
 - [Features](#features)
 - [Available styles and functions](#available-styles-and-functions)
   - [1. Basics](#1-basics)
   - [2. Text Styles](#2-text-styles)
   - [3. Bright Text Colors](#3-bright-text-colors)
   - [4. Background Color](#4-background-color)
-  - [Bright background styles](#bright-background-styles)
+  - [5. Bright background styles](#5-bright-background-styles)
+  - [Docs](#docs)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Installation
 
 You can install `inksplash` via pip:
 
@@ -512,15 +513,15 @@
 
    **Returns:**
 
    - str: The input text with a white background color.
 
 ---
 
-#### Bright background styles
+#### 5. Bright background styles
 
 1. **`bg_bright_black`**
 
    Applies a bright black background color to the text.
 
    **Parameters:**
 
@@ -624,14 +625,18 @@
 
    - `value` (str): The input text.
 
    **Returns:**
 
    - str: The input text with a bright white background color.
 
+#### Docs
+
+You can read more in the [documentation](https://inksplash.readthedocs.io/en/latest/index.html).
+
 ### Contributing
 
 Contributions to `inksplash` are welcome! Feel free to submit bug reports, feature requests, or pull requests on [GitHub](https://github.com/CrispenGari/inksplash).
 
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inksplash Version: 1.0.3 Summary: This is a Python
+Metadata-Version: 2.1 Name: inksplash Version: 1.0.4 Summary: This is a Python
 package that provides a versatile set of utilities for colorizing and styling
 text output in terminal environments. Author-email: Crispen Gari
 gmail.com> License: MIT License Copyright (c) 2024 crispengari Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -41,20 +41,20 @@
   _i_n_k_s_p_l_a_s_h_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
    _l_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_i_n_k_s_p_l_a_s_h_._s_v_g_]
 ### Table of Contents - [inksplash](#inksplash) - [Table of Contents](#table-
 of-contents) - [Installation](#installation) - [Usage](#usage) - [Features]
 (#features) - [Available styles and functions](#available-styles-and-functions)
 - [1. Basics](#1-basics) - [2. Text Styles](#2-text-styles) - [3. Bright Text
 Colors](#3-bright-text-colors) - [4. Background Color](#4-background-color) -
-[Bright background styles](#bright-background-styles) - [Contributing]
-(#contributing) - [License](#license) ### Installation You can install
-`inksplash` via pip: ```bash pip install inksplash ``` ### Usage First, you
-need to import the `chameleon` module from the `inksplash` package: ```py from
-inksplash import chameleon print(chameleon.bg_bright_green(chameleon.italic
-(chameleon.black("Hello world")))) ``` Output:
+[5. Bright background styles](#5-bright-background-styles) - [Docs](#docs) -
+[Contributing](#contributing) - [License](#license) ### Installation You can
+install `inksplash` via pip: ```bash pip install inksplash ``` ### Usage First,
+you need to import the `chameleon` module from the `inksplash` package: ```py
+from inksplash import chameleon print(chameleon.bg_bright_green
+(chameleon.italic(chameleon.black("Hello world")))) ``` Output:
                                     [demo]
 This example demonstrates how to use `chameleon` functions from `inksplash` to
 colorize and style text output. In this case, it applies a bright green
 background, italic style, and black text color to the string "Hello world". ###
 Features - Easy-to-use API for applying various text styles and colors. -
 Supports a wide range of styling options, including bold, italic, underline,
 foreground and background colors, etc. - Compatible with ANSI terminal escape
@@ -119,15 +119,15 @@
 background color. --- 6. **`bg_purple`** Applies a purple background color to
 the text. **Parameters:** - `value` (str): The input text. **Returns:** - str:
 The input text with a purple background color. --- 7. **`bg_cyan`** Applies a
 cyan background color to the text. **Parameters:** - `value` (str): The input
 text. **Returns:** - str: The input text with a cyan background color. --- 8.
 **`bg_white`** Applies a white background color to the text. **Parameters:** -
 `value` (str): The input text. **Returns:** - str: The input text with a white
-background color. --- #### Bright background styles 1. **`bg_bright_black`**
+background color. --- #### 5. Bright background styles 1. **`bg_bright_black`**
 Applies a bright black background color to the text. **Parameters:** - `value`
 (str): The input text. **Returns:** - str: The input text with a bright black
 background color. --- 2. **`bg_bright_red`** Applies a bright red background
 color to the text. **Parameters:** - `value` (str): The input text. **Returns:
 ** - str: The input text with a bright red background color. --- 3.
 **`bg_bright_green`** Applies a bright green background color to the text.
 **Parameters:** - `value` (str): The input text. **Returns:** - str: The input
@@ -140,12 +140,13 @@
 **`bg_bright_purple`** Applies a bright purple background color to the text.
 **Parameters:** - `value` (str): The input text. **Returns:** - str: The input
 text with a bright purple background color. --- 7. **`bg_bright_cyan`** Applies
 a bright cyan background color to the text. **Parameters:** - `value` (str):
 The input text. **Returns:** - str: The input text with a bright cyan
 background color. --- 8. **`bg_bright_white`** Applies a bright white
 background color to the text. **Parameters:** - `value` (str): The input text.
-**Returns:** - str: The input text with a bright white background color. ###
-Contributing Contributions to `inksplash` are welcome! Feel free to submit bug
-reports, feature requests, or pull requests on [GitHub](https://github.com/
-CrispenGari/inksplash). ### License This project is licensed under the MIT
-License - see the [LICENSE](/LISENSE) file for details.
+**Returns:** - str: The input text with a bright white background color. ####
+Docs You can read more in the [documentation](https://inksplash.readthedocs.io/
+en/latest/index.html). ### Contributing Contributions to `inksplash` are
+welcome! Feel free to submit bug reports, feature requests, or pull requests on
+[GitHub](https://github.com/CrispenGari/inksplash). ### License This project is
+licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `inksplash-1.0.3/README.md` & `inksplash-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 - [Usage](#usage)
 - [Features](#features)
 - [Available styles and functions](#available-styles-and-functions)
   - [1. Basics](#1-basics)
   - [2. Text Styles](#2-text-styles)
   - [3. Bright Text Colors](#3-bright-text-colors)
   - [4. Background Color](#4-background-color)
-  - [Bright background styles](#bright-background-styles)
+  - [5. Bright background styles](#5-bright-background-styles)
+  - [Docs](#docs)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Installation
 
 You can install `inksplash` via pip:
 
@@ -460,15 +461,15 @@
 
    **Returns:**
 
    - str: The input text with a white background color.
 
 ---
 
-#### Bright background styles
+#### 5. Bright background styles
 
 1. **`bg_bright_black`**
 
    Applies a bright black background color to the text.
 
    **Parameters:**
 
@@ -572,14 +573,18 @@
 
    - `value` (str): The input text.
 
    **Returns:**
 
    - str: The input text with a bright white background color.
 
+#### Docs
+
+You can read more in the [documentation](https://inksplash.readthedocs.io/en/latest/index.html).
+
 ### Contributing
 
 Contributions to `inksplash` are welcome! Feel free to submit bug reports, feature requests, or pull requests on [GitHub](https://github.com/CrispenGari/inksplash).
 
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -6,20 +6,20 @@
   _i_n_k_s_p_l_a_s_h_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
    _l_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_i_n_k_s_p_l_a_s_h_._s_v_g_]
 ### Table of Contents - [inksplash](#inksplash) - [Table of Contents](#table-
 of-contents) - [Installation](#installation) - [Usage](#usage) - [Features]
 (#features) - [Available styles and functions](#available-styles-and-functions)
 - [1. Basics](#1-basics) - [2. Text Styles](#2-text-styles) - [3. Bright Text
 Colors](#3-bright-text-colors) - [4. Background Color](#4-background-color) -
-[Bright background styles](#bright-background-styles) - [Contributing]
-(#contributing) - [License](#license) ### Installation You can install
-`inksplash` via pip: ```bash pip install inksplash ``` ### Usage First, you
-need to import the `chameleon` module from the `inksplash` package: ```py from
-inksplash import chameleon print(chameleon.bg_bright_green(chameleon.italic
-(chameleon.black("Hello world")))) ``` Output:
+[5. Bright background styles](#5-bright-background-styles) - [Docs](#docs) -
+[Contributing](#contributing) - [License](#license) ### Installation You can
+install `inksplash` via pip: ```bash pip install inksplash ``` ### Usage First,
+you need to import the `chameleon` module from the `inksplash` package: ```py
+from inksplash import chameleon print(chameleon.bg_bright_green
+(chameleon.italic(chameleon.black("Hello world")))) ``` Output:
                                     [demo]
 This example demonstrates how to use `chameleon` functions from `inksplash` to
 colorize and style text output. In this case, it applies a bright green
 background, italic style, and black text color to the string "Hello world". ###
 Features - Easy-to-use API for applying various text styles and colors. -
 Supports a wide range of styling options, including bold, italic, underline,
 foreground and background colors, etc. - Compatible with ANSI terminal escape
@@ -84,15 +84,15 @@
 background color. --- 6. **`bg_purple`** Applies a purple background color to
 the text. **Parameters:** - `value` (str): The input text. **Returns:** - str:
 The input text with a purple background color. --- 7. **`bg_cyan`** Applies a
 cyan background color to the text. **Parameters:** - `value` (str): The input
 text. **Returns:** - str: The input text with a cyan background color. --- 8.
 **`bg_white`** Applies a white background color to the text. **Parameters:** -
 `value` (str): The input text. **Returns:** - str: The input text with a white
-background color. --- #### Bright background styles 1. **`bg_bright_black`**
+background color. --- #### 5. Bright background styles 1. **`bg_bright_black`**
 Applies a bright black background color to the text. **Parameters:** - `value`
 (str): The input text. **Returns:** - str: The input text with a bright black
 background color. --- 2. **`bg_bright_red`** Applies a bright red background
 color to the text. **Parameters:** - `value` (str): The input text. **Returns:
 ** - str: The input text with a bright red background color. --- 3.
 **`bg_bright_green`** Applies a bright green background color to the text.
 **Parameters:** - `value` (str): The input text. **Returns:** - str: The input
@@ -105,12 +105,13 @@
 **`bg_bright_purple`** Applies a bright purple background color to the text.
 **Parameters:** - `value` (str): The input text. **Returns:** - str: The input
 text with a bright purple background color. --- 7. **`bg_bright_cyan`** Applies
 a bright cyan background color to the text. **Parameters:** - `value` (str):
 The input text. **Returns:** - str: The input text with a bright cyan
 background color. --- 8. **`bg_bright_white`** Applies a bright white
 background color to the text. **Parameters:** - `value` (str): The input text.
-**Returns:** - str: The input text with a bright white background color. ###
-Contributing Contributions to `inksplash` are welcome! Feel free to submit bug
-reports, feature requests, or pull requests on [GitHub](https://github.com/
-CrispenGari/inksplash). ### License This project is licensed under the MIT
-License - see the [LICENSE](/LISENSE) file for details.
+**Returns:** - str: The input text with a bright white background color. ####
+Docs You can read more in the [documentation](https://inksplash.readthedocs.io/
+en/latest/index.html). ### Contributing Contributions to `inksplash` are
+welcome! Feel free to submit bug reports, feature requests, or pull requests on
+[GitHub](https://github.com/CrispenGari/inksplash). ### License This project is
+licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `inksplash-1.0.3/images/demo.jpg` & `inksplash-1.0.4/images/demo.jpg`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/inksplash/chameleon.py` & `inksplash-1.0.4/inksplash/chameleon.py`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/inksplash.egg-info/PKG-INFO` & `inksplash-1.0.4/inksplash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inksplash
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is a Python package that provides a versatile set of utilities for colorizing and styling text output in terminal environments.
 Author-email: Crispen Gari <crispengari@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 crispengari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,15 +73,16 @@
 - [Usage](#usage)
 - [Features](#features)
 - [Available styles and functions](#available-styles-and-functions)
   - [1. Basics](#1-basics)
   - [2. Text Styles](#2-text-styles)
   - [3. Bright Text Colors](#3-bright-text-colors)
   - [4. Background Color](#4-background-color)
-  - [Bright background styles](#bright-background-styles)
+  - [5. Bright background styles](#5-bright-background-styles)
+  - [Docs](#docs)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Installation
 
 You can install `inksplash` via pip:
 
@@ -512,15 +513,15 @@
 
    **Returns:**
 
    - str: The input text with a white background color.
 
 ---
 
-#### Bright background styles
+#### 5. Bright background styles
 
 1. **`bg_bright_black`**
 
    Applies a bright black background color to the text.
 
    **Parameters:**
 
@@ -624,14 +625,18 @@
 
    - `value` (str): The input text.
 
    **Returns:**
 
    - str: The input text with a bright white background color.
 
+#### Docs
+
+You can read more in the [documentation](https://inksplash.readthedocs.io/en/latest/index.html).
+
 ### Contributing
 
 Contributions to `inksplash` are welcome! Feel free to submit bug reports, feature requests, or pull requests on [GitHub](https://github.com/CrispenGari/inksplash).
 
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inksplash Version: 1.0.3 Summary: This is a Python
+Metadata-Version: 2.1 Name: inksplash Version: 1.0.4 Summary: This is a Python
 package that provides a versatile set of utilities for colorizing and styling
 text output in terminal environments. Author-email: Crispen Gari
 gmail.com> License: MIT License Copyright (c) 2024 crispengari Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -41,20 +41,20 @@
   _i_n_k_s_p_l_a_s_h_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
    _l_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_i_n_k_s_p_l_a_s_h_._s_v_g_]
 ### Table of Contents - [inksplash](#inksplash) - [Table of Contents](#table-
 of-contents) - [Installation](#installation) - [Usage](#usage) - [Features]
 (#features) - [Available styles and functions](#available-styles-and-functions)
 - [1. Basics](#1-basics) - [2. Text Styles](#2-text-styles) - [3. Bright Text
 Colors](#3-bright-text-colors) - [4. Background Color](#4-background-color) -
-[Bright background styles](#bright-background-styles) - [Contributing]
-(#contributing) - [License](#license) ### Installation You can install
-`inksplash` via pip: ```bash pip install inksplash ``` ### Usage First, you
-need to import the `chameleon` module from the `inksplash` package: ```py from
-inksplash import chameleon print(chameleon.bg_bright_green(chameleon.italic
-(chameleon.black("Hello world")))) ``` Output:
+[5. Bright background styles](#5-bright-background-styles) - [Docs](#docs) -
+[Contributing](#contributing) - [License](#license) ### Installation You can
+install `inksplash` via pip: ```bash pip install inksplash ``` ### Usage First,
+you need to import the `chameleon` module from the `inksplash` package: ```py
+from inksplash import chameleon print(chameleon.bg_bright_green
+(chameleon.italic(chameleon.black("Hello world")))) ``` Output:
                                     [demo]
 This example demonstrates how to use `chameleon` functions from `inksplash` to
 colorize and style text output. In this case, it applies a bright green
 background, italic style, and black text color to the string "Hello world". ###
 Features - Easy-to-use API for applying various text styles and colors. -
 Supports a wide range of styling options, including bold, italic, underline,
 foreground and background colors, etc. - Compatible with ANSI terminal escape
@@ -119,15 +119,15 @@
 background color. --- 6. **`bg_purple`** Applies a purple background color to
 the text. **Parameters:** - `value` (str): The input text. **Returns:** - str:
 The input text with a purple background color. --- 7. **`bg_cyan`** Applies a
 cyan background color to the text. **Parameters:** - `value` (str): The input
 text. **Returns:** - str: The input text with a cyan background color. --- 8.
 **`bg_white`** Applies a white background color to the text. **Parameters:** -
 `value` (str): The input text. **Returns:** - str: The input text with a white
-background color. --- #### Bright background styles 1. **`bg_bright_black`**
+background color. --- #### 5. Bright background styles 1. **`bg_bright_black`**
 Applies a bright black background color to the text. **Parameters:** - `value`
 (str): The input text. **Returns:** - str: The input text with a bright black
 background color. --- 2. **`bg_bright_red`** Applies a bright red background
 color to the text. **Parameters:** - `value` (str): The input text. **Returns:
 ** - str: The input text with a bright red background color. --- 3.
 **`bg_bright_green`** Applies a bright green background color to the text.
 **Parameters:** - `value` (str): The input text. **Returns:** - str: The input
@@ -140,12 +140,13 @@
 **`bg_bright_purple`** Applies a bright purple background color to the text.
 **Parameters:** - `value` (str): The input text. **Returns:** - str: The input
 text with a bright purple background color. --- 7. **`bg_bright_cyan`** Applies
 a bright cyan background color to the text. **Parameters:** - `value` (str):
 The input text. **Returns:** - str: The input text with a bright cyan
 background color. --- 8. **`bg_bright_white`** Applies a bright white
 background color to the text. **Parameters:** - `value` (str): The input text.
-**Returns:** - str: The input text with a bright white background color. ###
-Contributing Contributions to `inksplash` are welcome! Feel free to submit bug
-reports, feature requests, or pull requests on [GitHub](https://github.com/
-CrispenGari/inksplash). ### License This project is licensed under the MIT
-License - see the [LICENSE](/LISENSE) file for details.
+**Returns:** - str: The input text with a bright white background color. ####
+Docs You can read more in the [documentation](https://inksplash.readthedocs.io/
+en/latest/index.html). ### Contributing Contributions to `inksplash` are
+welcome! Feel free to submit bug reports, feature requests, or pull requests on
+[GitHub](https://github.com/CrispenGari/inksplash). ### License This project is
+licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `inksplash-1.0.3/logo.png` & `inksplash-1.0.4/docs/source/images/logo.png`

 * *Files identical despite different names*

### Comparing `inksplash-1.0.3/pyproject.toml` & `inksplash-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inksplash"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name = "Crispen Gari", email = "crispengari@gmail.com"},
 ]
 description = "This is a Python package that provides a versatile set of utilities for colorizing and styling text output in terminal environments."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
```

