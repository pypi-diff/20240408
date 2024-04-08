# Comparing `tmp/ghfetch-pip-1.5.3.tar.gz` & `tmp/ghfetch-pip-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfetch-pip-1.5.3.tar", last modified: Sun Mar 17 15:58:48 2024, max compression
+gzip compressed data, was "ghfetch-pip-1.5.4.tar", last modified: Mon Apr  8 20:46:50 2024, max compression
```

## Comparing `ghfetch-pip-1.5.3.tar` & `ghfetch-pip-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-03-17 15:58:48.418899 ghfetch-pip-1.5.3/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1071 2023-07-13 21:40:21.000000 ghfetch-pip-1.5.3/LICENSE
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      299 2024-03-17 15:58:48.418899 ghfetch-pip-1.5.3/PKG-INFO
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     3940 2024-03-17 15:38:44.000000 ghfetch-pip-1.5.3/README.md
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-03-17 15:58:48.415565 ghfetch-pip-1.5.3/ghfetch/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 21:40:21.000000 ghfetch-pip-1.5.3/ghfetch/__init__.py
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-03-17 15:58:48.415565 ghfetch-pip-1.5.3/ghfetch/data/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-17 22:53:55.000000 ghfetch-pip-1.5.3/ghfetch/data/__init__.py
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    26795 2023-07-17 22:53:55.000000 ghfetch-pip-1.5.3/ghfetch/data/language-colors.json
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    11912 2023-07-23 15:02:20.000000 ghfetch-pip-1.5.3/ghfetch/main.py
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-03-17 15:58:48.418899 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      299 2024-03-17 15:58:48.000000 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/PKG-INFO
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      343 2024-03-17 15:58:48.000000 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/SOURCES.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        1 2024-03-17 15:58:48.000000 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/dependency_links.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       46 2024-03-17 15:58:48.000000 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/entry_points.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       20 2024-03-17 15:58:48.000000 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/requires.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        8 2024-03-17 15:58:48.000000 ghfetch-pip-1.5.3/ghfetch_pip.egg-info/top_level.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      200 2024-03-17 15:58:48.418899 ghfetch-pip-1.5.3/setup.cfg
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      618 2024-03-17 15:43:24.000000 ghfetch-pip-1.5.3/setup.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-04-08 20:46:50.698199 ghfetch-pip-1.5.4/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1071 2023-07-13 21:40:21.000000 ghfetch-pip-1.5.4/LICENSE
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      299 2024-04-08 20:46:50.698199 ghfetch-pip-1.5.4/PKG-INFO
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     4029 2024-04-08 20:30:15.000000 ghfetch-pip-1.5.4/README.md
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-04-08 20:46:50.694866 ghfetch-pip-1.5.4/ghfetch/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 21:40:21.000000 ghfetch-pip-1.5.4/ghfetch/__init__.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-04-08 20:46:50.698199 ghfetch-pip-1.5.4/ghfetch/data/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-17 22:53:55.000000 ghfetch-pip-1.5.4/ghfetch/data/__init__.py
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    26795 2023-07-17 22:53:55.000000 ghfetch-pip-1.5.4/ghfetch/data/language-colors.json
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    12099 2024-04-08 20:30:15.000000 ghfetch-pip-1.5.4/ghfetch/main.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2024-04-08 20:46:50.698199 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      299 2024-04-08 20:46:50.000000 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/PKG-INFO
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      343 2024-04-08 20:46:50.000000 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        1 2024-04-08 20:46:50.000000 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       46 2024-04-08 20:46:50.000000 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/entry_points.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       20 2024-04-08 20:46:50.000000 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/requires.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        8 2024-04-08 20:46:50.000000 ghfetch-pip-1.5.4/ghfetch_pip.egg-info/top_level.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      200 2024-04-08 20:46:50.698199 ghfetch-pip-1.5.4/setup.cfg
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      618 2024-04-08 20:38:31.000000 ghfetch-pip-1.5.4/setup.py
```

### Comparing `ghfetch-pip-1.5.3/LICENSE` & `ghfetch-pip-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.5.3/README.md` & `ghfetch-pip-1.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 add-apt-repository "deb https://ppa.launchpadcontent.net/ghfetch/ghfetch/ubuntu/ mantic main"
 apt-get update
 ```
 If you don't have "add-apt-repository", you can install it with: 
 ```sh
 apt-get install software-properties-common python3-launchpadlib
 ```
+
+> For troubleshooting see [here](https://github.com/ghfetch/ghfetch#troubleshooting-%EF%B8%8F).
+
 And then you can install **ghfetch**
 ```sh
 apt-get install ghfetch
 ```
 
 **Arch Linux:**</br>
 Use your favorite AUR helper, i.e:
@@ -81,15 +84,15 @@
 
 **Organization:**
 ```sh
 ghfetch ghfetch
 ghfetch confugiradores
 ```
 
-**Repo:**README.md
+**Repo:**
 ```sh
 ghfetch torvalds/linux
 ghfetch ghfetch/ghfetch
 ```
 
 ## To-do's 📋
```

### Comparing `ghfetch-pip-1.5.3/ghfetch/data/language-colors.json` & `ghfetch-pip-1.5.4/ghfetch/data/language-colors.json`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.5.3/ghfetch/main.py` & `ghfetch-pip-1.5.4/ghfetch/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,17 @@
     user_img_location = Path(f'{HOME_PATH}/.ghfetch/tmp/{file_name}.png')
 
     img_data = get(url).content
 
     with open(user_img_location, 'wb') as file:
         file.write(img_data)
 
+    # Convert image to RGB in case the image is .gif
+    Image.open(user_img_location).convert('RGB').save(user_img_location)
+
     with Image.open(user_img_location) as image:
         MULTIPLIER = 0.45 # Used to fix the image height because the characters are taller
 
         # Get initial width and height
         width, height = image.size
         aspect_ratio = height / width
 
@@ -160,14 +163,15 @@
 
             if len(line) == COLORED_CHAR_LENGTH * IMAGE_WIDTH:
                 unicode_per_rows.append(f'{line}\t')
                 line = ''
 
         Path.unlink(user_img_location, missing_ok=True)
 
+        unicode_per_rows.append(f"{' ' * IMAGE_WIDTH}\t")
         return unicode_per_rows
 
 def print_output(fetched_info):
     COLOR_TITLE = '#068FFF'
     COLOR_TEXT = '#EDEDED'
     COLOR_ARCHIVED = '#F48024'
 
@@ -249,22 +253,22 @@
             if len(fetched_info["languages"].items()) > 2:
                 output[n + 13] += ', '.join([(f"{title(k, get_lang_color(languages, k))}: {text(v)}") for k, v in fetched_info["languages"].items()][:2]) + ' '
                 output[n + 14] += ', '.join([(f"{title(k, get_lang_color(languages, k))}: {text(v)}") for k, v in fetched_info["languages"].items()][2:])
             else:
                 output[n + 13] += ', '.join([(f"{title(k, get_lang_color(languages, k))}: {text(v)}") for k, v in fetched_info["languages"].items()])
 
 
-            LENTH_BAR_DIVIDER = 3
+            LENGTH_BAR_DIVIDER = 3
 
             for lang, percentage in fetched_info['languages'].items():
                 percentage = float(percentage[:-1])
                 color = get_lang_color(languages, lang)
 
 
-                cols = ceil(percentage / LENTH_BAR_DIVIDER)
+                cols = ceil(percentage / LENGTH_BAR_DIVIDER)
                 for _ in range(cols):
                     output[n + 12] += f'{language(color)}'
 
     for line in output:
         Console().print(line, overflow='crop', soft_wrap=True)
```

### Comparing `ghfetch-pip-1.5.3/setup.py` & `ghfetch-pip-1.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='ghfetch-pip',
-      version='1.5.3',
+      version='1.5.4',
       description='CLI tool to fetch GitHub information',
       author='Nullgaro, Icutum',
       author_email='ghfetch.contact@gmail.com',
       url='https://github.com/ghfetch/ghfetch',
       packages=['ghfetch', 'ghfetch.data'],
       install_requires=['pillow', 'aiohttp', 'rich'],
       package_data={'': ['./data/language-colors.json', './LICENSE', './README.md']},
```

