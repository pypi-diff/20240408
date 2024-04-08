# Comparing `tmp/asosoft-0.1.2.tar.gz` & `tmp/asosoft-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asosoft-0.1.2.tar", last modified: Mon Jan 15 13:27:07 2024, max compression
+gzip compressed data, was "asosoft-0.1.3.tar", last modified: Mon Apr  8 11:17:52 2024, max compression
```

## Comparing `asosoft-0.1.2.tar` & `asosoft-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-01-15 13:27:07.499376 asosoft-0.1.2/
--rw-rw-rw-   0        0        0     1085 2024-01-08 06:48:08.000000 asosoft-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    11650 2024-01-15 13:27:07.498376 asosoft-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    11028 2024-01-14 08:11:19.000000 asosoft-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-01-15 13:27:07.500377 asosoft-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-01-15 13:26:56.000000 asosoft-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-15 13:27:07.393117 asosoft-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-01-15 13:27:07.429329 asosoft-0.1.2/src/asosoft/
--rw-rw-rw-   0        0        0    15068 2024-01-14 05:48:09.000000 asosoft-0.1.2/src/asosoft/G2P.py
--rw-rw-rw-   0        0        0    11748 2024-01-14 06:37:45.000000 asosoft-0.1.2/src/asosoft/Normalize.py
--rw-rw-rw-   0        0        0     3618 2024-01-14 01:32:03.000000 asosoft-0.1.2/src/asosoft/Number2Word.py
--rw-rw-rw-   0        0        0     8385 2024-01-13 23:01:33.000000 asosoft-0.1.2/src/asosoft/PoemClassifier.py
--rw-rw-rw-   0        0        0      660 2024-01-13 22:56:07.000000 asosoft-0.1.2/src/asosoft/Sort.py
--rw-rw-rw-   0        0        0     4681 2024-01-14 06:35:57.000000 asosoft-0.1.2/src/asosoft/Transliteration.py
--rw-rw-rw-   0        0        0      657 2024-01-14 06:38:24.000000 asosoft-0.1.2/src/asosoft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-15 13:27:07.494378 asosoft-0.1.2/src/asosoft/resources/
--rw-rw-rw-   0        0        0      535 2024-01-15 13:25:57.000000 asosoft-0.1.2/src/asosoft/resources/G2PCertain.csv
--rw-rw-rw-   0        0        0      122 2023-10-17 19:30:29.000000 asosoft-0.1.2/src/asosoft/resources/G2PExceptions.csv
--rw-rw-rw-   0        0        0     1216 2023-10-17 19:30:51.000000 asosoft-0.1.2/src/asosoft/resources/NormalizeUnicodeAdditional.csv
--rw-rw-rw-   0        0        0    14694 2023-10-17 19:30:58.000000 asosoft-0.1.2/src/asosoft/resources/NormalizeUnicodeDeep.csv
--rw-rw-rw-   0        0        0      185 2023-10-17 19:31:04.000000 asosoft-0.1.2/src/asosoft/resources/Phoneme2Ascii.csv
--rw-rw-rw-   0        0        0      233 2023-10-17 19:31:12.000000 asosoft-0.1.2/src/asosoft/resources/Phoneme2IPA.csv
--rw-rw-rw-   0        0        0     2603 2023-10-17 19:31:18.000000 asosoft-0.1.2/src/asosoft/resources/PoemPatterns.csv
-drwxrwxrwx   0        0        0        0 2024-01-15 13:27:07.465802 asosoft-0.1.2/src/asosoft.egg-info/
--rw-rw-rw-   0        0        0    11650 2024-01-15 13:27:06.000000 asosoft-0.1.2/src/asosoft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-01-15 13:27:06.000000 asosoft-0.1.2/src/asosoft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-15 13:27:06.000000 asosoft-0.1.2/src/asosoft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-01-15 13:27:06.000000 asosoft-0.1.2/src/asosoft.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-15 13:27:06.000000 asosoft-0.1.2/src/asosoft.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 11:17:52.558072 asosoft-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2024-01-18 00:42:54.000000 asosoft-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    11648 2024-04-08 11:17:52.552308 asosoft-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11028 2024-01-18 00:42:54.000000 asosoft-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 11:17:52.558072 asosoft-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2024-04-08 11:09:41.000000 asosoft-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:17:52.402301 asosoft-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:17:52.472543 asosoft-0.1.3/src/asosoft/
+-rw-rw-rw-   0        0        0    15068 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/G2P.py
+-rw-rw-rw-   0        0        0    11686 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/Normalize.py
+-rw-rw-rw-   0        0        0     3618 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/Number2Word.py
+-rw-rw-rw-   0        0        0     8385 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/PoemClassifier.py
+-rw-rw-rw-   0        0        0      658 2024-04-08 11:09:08.000000 asosoft-0.1.3/src/asosoft/Sort.py
+-rw-rw-rw-   0        0        0     4681 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/Transliteration.py
+-rw-rw-rw-   0        0        0      695 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:17:52.538795 asosoft-0.1.3/src/asosoft/resources/
+-rw-rw-rw-   0        0        0      579 2024-01-18 00:44:04.000000 asosoft-0.1.3/src/asosoft/resources/G2PCertain.csv
+-rw-rw-rw-   0        0        0      128 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/resources/G2PExceptions.csv
+-rw-rw-rw-   0        0        0     1300 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/resources/NormalizeUnicodeAdditional.csv
+-rw-rw-rw-   0        0        0    15687 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/resources/NormalizeUnicodeDeep.csv
+-rw-rw-rw-   0        0        0      221 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/resources/Phoneme2Ascii.csv
+-rw-rw-rw-   0        0        0      276 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/resources/Phoneme2IPA.csv
+-rw-rw-rw-   0        0        0     2630 2024-01-18 00:42:54.000000 asosoft-0.1.3/src/asosoft/resources/PoemPatterns.csv
+drwxrwxrwx   0        0        0        0 2024-04-08 11:17:52.505401 asosoft-0.1.3/src/asosoft.egg-info/
+-rw-rw-rw-   0        0        0    11648 2024-04-08 11:17:52.000000 asosoft-0.1.3/src/asosoft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-08 11:17:52.000000 asosoft-0.1.3/src/asosoft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 11:17:52.000000 asosoft-0.1.3/src/asosoft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-08 11:17:52.000000 asosoft-0.1.3/src/asosoft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 11:17:52.000000 asosoft-0.1.3/src/asosoft.egg-info/top_level.txt
```

### Comparing `asosoft-0.1.2/LICENSE` & `asosoft-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asosoft-0.1.2/PKG-INFO` & `asosoft-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: asosoft
-Version: 0.1.2
+Version: 0.1.3
 Summary: AsoSoft's Library for Kurdish language processing tasks
 Home-page: https://github.com/AsoSoft/AsoSoft-Library-py
 Author: Aso Mahmudi
 Author-email: aso.mehmudi@gmail.com
 License: MIT
 Keywords: natural-language-processing,normalization,unicode-normalization,central-kurdish,kurdish,sorani
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # AsoSoft Library (Python)
 AsoSoft Library offers basic natural language processing (NLP) algorithms for the Kurdish Language (ckb: Central branch of Kurdish).
 AsoSoft Library is originally written in C# and this library is the Python port.
```

### Comparing `asosoft-0.1.2/README.md` & `asosoft-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `asosoft-0.1.2/src/asosoft/G2P.py` & `asosoft-0.1.3/src/asosoft/G2P.py`

 * *Files identical despite different names*

### Comparing `asosoft-0.1.2/src/asosoft/Normalize.py` & `asosoft-0.1.3/src/asosoft/Normalize.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,64 +11,64 @@
 #    booktitle={The Second International Conference on Kurdish and Persian Languages and Literature},
 #    year={2019}
 #  }
 
 import regex as re
 import html
 
-def _replaceByList(text, replaceList):
-    for i in range(0, len(replaceList), 2):
-        text = re.sub(replaceList[i], replaceList[i + 1], text)
+def replace_by_list(text, replace_list):
+    for pattern, replacement in replace_list:
+        text = re.sub(pattern, replacement, text)
     return text
 
-_Ku = "ئابپتجچحخدرڕزژسشعغفڤقکگلڵمنوۆەهھیێأإآثذصضطظكيىةڎۊؤ" + "\u064B-\u065F"
-_joiners = "ئبپتثجچحخسشصضطظعغفڤقکكگلڵمنیيهھێ"
+KU = "ئابپتجچحخدرڕزژسشعغفڤقکگلڵمنوۆەهھیێأإآثذصضطظكيىةڎۊؤ" + "\u064B-\u065F"
+JOINERS = "ئبپتثجچحخسشصضطظعغفڤقکكگلڵمنیيهھێ"
 
-_normalizationReplaces = {
+normalization_replaces = {
     "NormalizeKurdish1": [
         #========= Tatweels (U+0640)
         "\u0640{2,}", "\u0640", # merge
-        rf"(?<=[{_joiners}])\u0640(?=[{_Ku}])", "", # delete unnecessary tatweel e.g. هـا to ها
+        rf"(?<=[{JOINERS}])\u0640(?=[{KU}])", "", # delete unnecessary tatweel e.g. هـا to ها
         # replace tatweel nonadjacent to Kurdish letters with dash
-        rf"(?<=[{_joiners}])\u0640", "\uF640", # temporal preserve
-        rf"\u0640(?=[{_Ku}])", "\uF640", # temporal preserve
+        rf"(?<=[{JOINERS}])\u0640", "\uF640", # temporal preserve
+        rf"\u0640(?=[{KU}])", "\uF640", # temporal preserve
         "\u0640", "-",
         "\uF640", "\u0640",
 
         #========= Zero-Width Non-Joiner
         "[\uFEFF\u200C]+", "\u200C", #Standardize and remove dublicated ZWNJ
         # remove unnecessary ZWNJ
         r"‌(?=(\s|\p{P}|$))", "",    # ZWNJ + white spaces
-        rf"(?<![{_joiners}])\u200C", "", # rmove after non-joiner letter: سەرzwnjزل                    
+        rf"(?<![{JOINERS}])\u200C", "", # rmove after non-joiner letter: سەرzwnjزل
 
         #========= Zero-Width Joiner (U+200D)
         "\u200D{2,}", "\u200D", # merge
-        "ه" + "\u200D", "هـ",   # final Heh, e.g. ماه‍  => ماهـ 
-        f"(?<![{_joiners}])\u200D(?![{_joiners}])", "", #remove unnecessary ZW-J
+        "ه" + "\u200D", "هـ",   # final Heh, e.g. ماه‍  => ماهـ
+        f"(?<![{JOINERS}])\u200D(?![{JOINERS}])", "", #remove unnecessary ZW-J
     ],
     "NormalizeKurdish2": [
-        #========= standard H, E, Y, K				    
+        #========= standard H, E, Y, K
         "ه" + "\u200C", "ە",    # Heh+ZWNJ =>  kurdish AE
-        "ه" + f"(?=([^{_Ku}ـ]|$))", "ە",   #final Heh looks like Ae
-        "ھ" + f"(?=([^{_Ku}]|$))", "هـ",   # final Heh Doachashmee
+        "ه" + f"(?=([^{KU}ـ]|$))", "ە",   #final Heh looks like Ae
+        "ھ" + f"(?=([^{KU}]|$))", "هـ",   # final Heh Doachashmee
         "ھ" , "ه",  # non-final Heh Doachashmee
         "ى|ي", "ی",  # Alef maksura | Arabic Ye => Farsi ye
         "ك", "ک",  # Arabic Kaf => Farsi Ke
         "\u200C" + "و ", " و ", # شوێن‌و جێ => شوێن و جێ
 
         #========= errors from font conversion
         "لاَ|لاً|لأ", "ڵا",
         "(ی|ێ)" + "[\u064E\u064B]+", "ێ",  #FATHA & FATHATAN
         "(و|ۆ)" + "[\u064E\u064B]+", "ۆ",
         "(ل|ڵ)" + "[\u064E\u064B]+", "ڵ",
         "(ر|ڕ)" + "\u0650+", "ڕ", #KASRA
     ],
     "NormalizeKurdish3": [
-            f"(?<![{_Ku}])" + "ر" + f"(?=[{_Ku}])", "ڕ", # initial R
-            f"(?<![{_Ku}])" + "وو" + "(?=[ئبپتجچحخدرڕزژسشعغفڤقکگلڵمنهھی])", "و", # inintial WU
+            f"(?<![{KU}])" + "ر" + f"(?=[{KU}])", "ڕ", # initial R
+            f"(?<![{KU}])" + "وو" + "(?=[ئبپتجچحخدرڕزژسشعغفڤقکگلڵمنهھی])", "و", # inintial WU
     ],
     "AliK2Unicode": [
             "لاَ|لآ|لاً", "ڵا",
             "لً|لَ|لأ", "ڵ",
             "ة", "ە",
             "ه" + "(?!([ئابپتجچحخدرڕزژسشعغفڤقکگلڵمنوۆەهھیێأإآثذصضطظكيىةڎۊؤ]|$))", "هـ",
             "ض", "چ",
@@ -156,85 +156,85 @@
             r"(?<![ \t\p{P}])(\uF8FD)", r" \1",   # A" B  => A " B
             r"(\uF8FD)(?![ \t\p{P}])", r"\1 ",   # A "B  => A " B
     ]
 }
 
 
 # ================= Normalization =================
-def _LoadNormalizerReplaces(file):
+def load_normalizer_replaces(file):
     output = {}
 
     items = file.strip().split('\n')
     for i in range(1, len(items)):
         item = items[i].split(',')
         ch_old = chr(int(item[0], 16))
         ch_new = ''.join(chr(int(ch, 16)) for ch in item[1].split() if ch != "")
         if ch_old not in output:
             output[ch_old] = ch_new
 
     return output
 
-_DeepReplacements = _LoadNormalizerReplaces("resources/NormalizeUnicodeDeep.csv")
-_additionalReplacements = _LoadNormalizerReplaces("resources/NormalizeUnicodeAdditional.csv")
+deep_replacements = load_normalizer_replaces("resources/NormalizeUnicodeDeep.csv")
+additional_replacements = load_normalizer_replaces("resources/NormalizeUnicodeAdditional.csv")
 
 # Unicode Normalization for Central Kurdish
 def Normalize(text, isOnlyKurdish=True, changeInitialR=True, deepUnicodeCorrectios=True, additionalUnicodeCorrections=True, usersReplaceList=None):
     if usersReplaceList is None:
         usersReplaceList = {}
 
     replaces = {}
-    
+
     # Character-based replacement (ReplaceList and Private Use Area)
     char_list = list(set(text))
 
     if deepUnicodeCorrectios:
-        for item in _DeepReplacements:
+        for item in deep_replacements:
             if item[0] in char_list:
                 replaces[item[0]] = item[1]
 
     if additionalUnicodeCorrections:
-        for item in _additionalReplacements:
+        for item in additional_replacements:
             if item[0] in char_list and item[0] not in replaces:
                 replaces[item[0]] = item[1]
 
     for item in usersReplaceList.items():
         if item[0] in char_list and item[0] not in replaces:
             replaces[item[0]] = item[1]
 
     for ch in char_list:
         if ch in replaces:  # ReplaceList
             text = text.replace(ch, replaces[ch])
         elif 57343 < ord(ch) < 63744:  # Private Use Area
             text = text.replace(ch, '□')  # u25A1 White Square
 
-    text = _replaceByList(text, _normalizationReplaces["NormalizeKurdish1"])
+    text = _replaceByList(text, normalization_replaces["NormalizeKurdish1"])
 
     # if the text is Monolingual (only Central Kurdish)
     if isOnlyKurdish:
-        text = _replaceByList(text, _normalizationReplaces["NormalizeKurdish2"])
-        
+        text = _replaceByList(text, normalization_replaces["NormalizeKurdish2"])
+
         # Initial r
         if changeInitialR:
-            text = _replaceByList(text, _normalizationReplaces["NormalizeKurdish3"])
+            text = _replaceByList(text, normalization_replaces["NormalizeKurdish3"])
 
     return text
 
 
 # Seperate digits from words (e.g. replacing "12a" with "12 a")
 def SeperateDigits(text):
-    return _replaceByList(text, _normalizationReplaces["SeperateDigits"])
+    return _replaceByList(text, normalization_replaces["SeperateDigits"])
 
 # Normalize Punctuations
 def NormalizePunctuations(text, seprateAllPunctuations):
     text = text.replace('"', "\uF8FD")  # temp replacement
-    text = _replaceByList(text, _normalizationReplaces["NormalizePunctuations1"])
+    text = _replaceByList(text, normalization_replaces["NormalizePunctuations1"])
     if not seprateAllPunctuations:
-        text = _replaceByList(text, _normalizationReplaces["NormalizePunctuations2"])
+        text = _replaceByList(text, normalization_replaces["NormalizePunctuations2"])
     else:
-        text = _replaceByList(text, _normalizationReplaces["NormalizePunctuations3"])
+        text = _replaceByList(text, normalization_replaces["NormalizePunctuations3"])
     text = text.replace("\uF8FD", '"')  # undo temp replacement
     return text
 
 # Trim white spaces of a line
 def TrimLine(line):
     line = re.sub("[\u200B\u200C\uFEFF]+$", "", line.strip())
     line = re.sub("^[\u200B\u200C\uFEFF]+", "", line.strip())
@@ -282,20 +282,20 @@
         elif NumeralType == "ar":
             text = re.sub(_digits[i] + "|" + _digits[i + 2], _digits[i + 1], text)
     return text
 
 # ================= Converting Non-Standard Fonts  =================
 # Converts Kurdish text written in AliK fonts into Unicode standard
 def AliK2Unicode(text):
-    return _replaceByList(text, _normalizationReplaces["AliK2Unicode"])
+    return _replaceByList(text, normalization_replaces["AliK2Unicode"])
 
 # Converts Kurdish text written in AliWeb fonts into Unicode standard
 def AliWeb2Unicode(text):
-    return _replaceByList(text, _normalizationReplaces["AliWeb2Unicode"])
+    return _replaceByList(text, normalization_replaces["AliWeb2Unicode"])
 
 # Converts Kurdish text written in KDylan fonts into Unicode standard
 def Dylan2Unicode(text):
-    return _replaceByList(text, _normalizationReplaces["Dylan2Unicode"])
+    return _replaceByList(text, normalization_replaces["Dylan2Unicode"])
 
 # Converts Kurdish text written in Zarnegar fonts into Unicode standard
 def Zarnegar2Unicode(text):
-    return _replaceByList(text, _normalizationReplaces["Zarnegar2Unicode"])
+    return _replaceByList(text, normalization_replaces["Zarnegar2Unicode"])
```

### Comparing `asosoft-0.1.2/src/asosoft/Number2Word.py` & `asosoft-0.1.3/src/asosoft/Number2Word.py`

 * *Files identical despite different names*

### Comparing `asosoft-0.1.2/src/asosoft/PoemClassifier.py` & `asosoft-0.1.3/src/asosoft/PoemClassifier.py`

 * *Files identical despite different names*

### Comparing `asosoft-0.1.2/src/asosoft/Sort.py` & `asosoft-0.1.3/src/asosoft/Sort.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 def kurdish_sort(inputList):
-    ku = list(["ئءاآأإبپتثجچحخدڎڊذرڕزژسشصضطظعغفڤقكکگڴلڵمنوۆۊۉۋهھەیێ"])
+    ku = list("ئءاآأإبپتثجچحخدڎڊذرڕزژسشصضطظعغفڤقكکگڴلڵمنوۆۊۉۋهھەیێ")
     return CustomSort(inputList, ku)
 
 def CustomSort(inputList, inputOrder):
     base_char = 62000
     order = [chr(base_char + i) for i in range(len(inputOrder))]
     for i in range(len(inputList)):
         for j in range(len(order)):
```

### Comparing `asosoft-0.1.2/src/asosoft/Transliteration.py` & `asosoft-0.1.3/src/asosoft/Transliteration.py`

 * *Files identical despite different names*

### Comparing `asosoft-0.1.2/src/asosoft/resources/NormalizeUnicodeAdditional.csv` & `asosoft-0.1.3/src/asosoft/resources/NormalizeUnicodeAdditional.csv`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-﻿From,To,Desc
-00AC,200C,Wrong ZWNJ by MS Word
-066A,0025,Arabic PERCENT SIGN
-066B,002E,Arabic DECIMAL SEPARATOR
-066C,002C,Arabic THOUSANDS SEPARATOR
-066D,002A,Arabic FIVE POINTED STAR
-0751,062B,ݑ
-0752,067E,ݒ
-0750,067E,ݐ
-0753,062A,ݓ
-067F,062A,ٿ
-0679,062A,ٹ
-0758,0686,ݘ
-0689,062F,ډ
-068A,062F,ڊ
-068B,062F,ڋ
-068C,062F,ڌ
-068D,062F,ڍ
-068F,062F,ڏ
-0690,062F,ڐ
-0759,062F,ݙ
-075A,062F,ݚ
-076C,0695,ݬ
-0691,0695,ڑ
-0692,0695,ڒ
-0693,0695,ړ
-0694,0695,ڔ
-0696,0695,ږ
-0697,0698,ڗ
-0699,0698,ڙ
-076B,0698,ݫ
-069A,0633,ښ
-069B,0633,ڛ
-069C,0634,ڜ
-06FA,0634,ۺ
-069D,0635,ڝ
-069E,0636,ڞ
-06FB,0636,ۻ
-069F,0638,ڟ
-06A0,063A,ڠ
-06FC,063A,ۼ
-06A1,0641,ڡ
-06A2,0641,ڢ
-06A3,0641,ڣ
-06A5,06A4,ڥ
-06A4,06A4,ڤ
-06A7,0642,ڧ
-06A8,0642,ڨ
-06A8,0642,ڨ
-06AA,06A9,ڪ
-06AB,06A9,ګ
-06AC,06A9,ڬ
-06AD,06A9,ڭ
-06AE,06A9,ڮ
-063B,06A9,ػ
-063C,06A9,ؼ
-06B0,06AF,ڰ
-06B1,06AF,ڱ
-06B2,06AF,ڲ
-06B3,06AF,ڳ
-06B4,06AF,ڴ
-06D2,06CC,ے
-06CD,06CC,ۍ
-06B6,06B5,ڶ
-06B7,06B5,ڷ
-06B8,06B5,ڸ
-076A,06B5,ݪ
-0765,0645,ݥ
-0766,0645,ݦ
-06B9,0646,ڹ
-06BA,0646,ں
-06BB,0646,ڻ
-06BC,0646,ڼ
-06BD,0646,ڽ
-0767,0646,ݧ
-0768,0646,ݨ
-0769,0646,ݩ
-06C4,06C6,ۄ
-06C5,06C6,ۅ
-06C8,06C6,ۈ
-06C9,06C6,ۉ
-06CB,06C6,ۋ
-0676,06C6,ٶ
-06C9,06C6,ۉ
+﻿From,To,Desc
+00AC,200C,Wrong ZWNJ by MS Word
+066A,0025,Arabic PERCENT SIGN
+066B,002E,Arabic DECIMAL SEPARATOR
+066C,002C,Arabic THOUSANDS SEPARATOR
+066D,002A,Arabic FIVE POINTED STAR
+0751,062B,ݑ
+0752,067E,ݒ
+0750,067E,ݐ
+0753,062A,ݓ
+067F,062A,ٿ
+0679,062A,ٹ
+0758,0686,ݘ
+0689,062F,ډ
+068A,062F,ڊ
+068B,062F,ڋ
+068C,062F,ڌ
+068D,062F,ڍ
+068F,062F,ڏ
+0690,062F,ڐ
+0759,062F,ݙ
+075A,062F,ݚ
+076C,0695,ݬ
+0691,0695,ڑ
+0692,0695,ڒ
+0693,0695,ړ
+0694,0695,ڔ
+0696,0695,ږ
+0697,0698,ڗ
+0699,0698,ڙ
+076B,0698,ݫ
+069A,0633,ښ
+069B,0633,ڛ
+069C,0634,ڜ
+06FA,0634,ۺ
+069D,0635,ڝ
+069E,0636,ڞ
+06FB,0636,ۻ
+069F,0638,ڟ
+06A0,063A,ڠ
+06FC,063A,ۼ
+06A1,0641,ڡ
+06A2,0641,ڢ
+06A3,0641,ڣ
+06A5,06A4,ڥ
+06A4,06A4,ڤ
+06A7,0642,ڧ
+06A8,0642,ڨ
+06A8,0642,ڨ
+06AA,06A9,ڪ
+06AB,06A9,ګ
+06AC,06A9,ڬ
+06AD,06A9,ڭ
+06AE,06A9,ڮ
+063B,06A9,ػ
+063C,06A9,ؼ
+06B0,06AF,ڰ
+06B1,06AF,ڱ
+06B2,06AF,ڲ
+06B3,06AF,ڳ
+06B4,06AF,ڴ
+06D2,06CC,ے
+06CD,06CC,ۍ
+06B6,06B5,ڶ
+06B7,06B5,ڷ
+06B8,06B5,ڸ
+076A,06B5,ݪ
+0765,0645,ݥ
+0766,0645,ݦ
+06B9,0646,ڹ
+06BA,0646,ں
+06BB,0646,ڻ
+06BC,0646,ڼ
+06BD,0646,ڽ
+0767,0646,ݧ
+0768,0646,ݨ
+0769,0646,ݩ
+06C4,06C6,ۄ
+06C5,06C6,ۅ
+06C8,06C6,ۈ
+06C9,06C6,ۉ
+06CB,06C6,ۋ
+0676,06C6,ٶ
+06C9,06C6,ۉ
 06C7,0648 0648,ۇ
```

### Comparing `asosoft-0.1.2/src/asosoft/resources/NormalizeUnicodeDeep.csv` & `asosoft-0.1.3/src/asosoft/resources/NormalizeUnicodeDeep.csv`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,994 +1,994 @@
-From,To,Desc
-A78C,0027,Latin Small Letter Saltillo ꞌ
-FEFF,200C,ZERO WIDTH NO-BREAK SPACE
-200B,200C,ZERO WIDTH SPACE
-2010,002D,HYPHEN
-2011,002D,NON-BREAKING HYPHEN
-2012,002D,FIGURE DASH
-2013,002D,EN DASH
-2014,002D,EM DASH
-2015,002D,HORIZONTAL BAR
-2212,002D,Minus
-00AD,002D,Soft Hyphen
-FE58,002D,SMALL EM DASH
-FE63,002D,MALL HYPHEN-MINUS
-FF0D,002D,FULLWIDTH HYPHEN-MINUS
-1680,0020,OGHAM SPACE MARK
-2000,0020,EN QUAD
-2001,0020,EM QUAD
-2002,0020,EN SPACE
-2003,0020,EM SPACE
-2004,0020,THREE-PER-EM SPACE
-2005,0020,FOUR-PER-EM SPACE
-2006,0020,SIX-PER-EM SPACE
-205F,0020,MEDIUM MATHEMATICAL SPACE
-3000,0020,IDEOGRAPHIC SPACE
-2007,0020,FIGURE SPACE
-2008,0020,PUNCTUATION SPACE
-2009,0020,THIN SPACE
-200A,0020,HAIR SPACE
-00A0,0020,NO-BREAK SPACE
-202F,0020,NARROW NO-BREAK SPACE
-200E,0020,LEFT-TO-RIGHT MARK
-200F,0020,RIGHT-TO-LEFT MARK
-202A,0020,LEFT-TO-RIGHT EMBEDDING
-202B,0020,RIGHT-TO-LEFT EMBEDDING
-202C,0020,POP DIRECTIONAL FORMATTING
-202D,0020,LEFT-TO-RIGHT OVERRIDE
-202E,0020,RIGHT-TO-LEFT OVERRIDE
-0000,0020,Control
-0001,0020,
-0002,0020,
-0003,0020,
-0004,0020,
-0005,0020,
-0006,0020,
-0007,0020,
-0008,0020,
-000B,0020,
-000C,0020,
-000E,0020,
-000F,0020,
-0010,0020,
-0011,0020,
-0012,0020,
-0013,0020,
-0014,0020,
-0015,0020,
-0016,0020,
-0017,0020,
-0018,0020,
-0019,0020,
-001A,0020,
-001B,0020,
-001C,0020,
-001D,0020,
-001E,0020,
-001F,0020,
-007F,0020,
-0080,0020,
-0081,0020,
-0082,0020,
-0083,0020,
-0084,0020,
-0085,0020,
-0086,0020,
-0087,0020,
-0088,0020,
-0089,0020,
-008A,0020,
-008B,0020,
-008C,0020,
-008D,0020,
-008E,0020,
-008F,0020,
-0090,0020,
-0091,0020,
-0092,0020,
-0093,0020,
-0094,0020,
-0095,0020,
-0096,0020,
-0097,0020,
-0098,0020,
-0099,0020,
-009A,0020,
-009B,0020,
-009C,0020,
-009D,0020,
-009E,0020,
-009F,0020,
-0610,,Arabic Nonspacing Marks
-0611,,
-0612,,
-0613,,
-0614,,
-0615,,
-0616,,
-0617,,
-0618,,
-0619,,
-061A,,
-0653,,
-0654,,
-0655,,
-0656,,
-0657,,
-0658,,
-0659,,
-065A,,
-065B,,
-065C,,
-065D,,
-065E,,
-065F,,
-0670,,
-06D6,,
-06D7,,
-06D8,,
-06D9,,
-06DA,,
-06DB,,
-06DC,,
-06DF,,
-06E0,,
-06E1,,
-06E2,,
-06E3,,
-06E4,,
-06E7,,
-06E8,,
-06EA,,
-06EB,,
-06EC,,
-06ED,,
-FB50,0671,Arabic Presentation Forms
-FB51,0671,
-FB52,067B,
-FB53,067B,
-FB54,067B,
-FB55,067B,
-FB56,067E,
-FB57,067E,
-FB58,067E,
-FB59,067E,
-FB5A,0680,
-FB5B,0680,
-FB5C,0680,
-FB5D,0680,
-FB5E,067A,
-FB5F,067A,
-FB60,067A,
-FB61,067A,
-FB62,067F,
-FB63,067F,
-FB64,067F,
-FB65,067F,
-FB66,0679,
-FB67,0679,
-FB68,0679,
-FB69,0679,
-FB6A,06A4,
-FB6B,06A4,
-FB6C,06A4,
-FB6D,06A4,
-FB6E,06A6,
-FB6F,06A6,
-FB70,06A6,
-FB71,06A6,
-FB72,0684,
-FB73,0684,
-FB74,0684,
-FB75,0684,
-FB76,0683,
-FB77,0683,
-FB78,0683,
-FB79,0683,
-FB7A,0686,
-FB7B,0686,
-FB7C,0686,
-FB7D,0686,
-FB7E,0687,
-FB7F,0687,
-FB80,0687,
-FB81,0687,
-FB82,068D,
-FB83,068D,
-FB84,068C,
-FB85,068C,
-FB86,068E,
-FB87,068E,
-FB88,0688,
-FB89,0688,
-FB8A,0698,
-FB8B,0698,
-FB8C,0691,
-FB8D,0691,
-FB8E,06A9,
-FB8F,06A9,
-FB90,06A9,
-FB91,06A9,
-FB92,06AF,
-FB93,06AF,
-FB94,06AF,
-FB95,06AF,
-FB96,06B3,
-FB97,06B3,
-FB98,06B3,
-FB99,06B3,
-FB9A,06B1,
-FB9B,06B1,
-FB9C,06B1,
-FB9D,06B1,
-FB9E,06BA,
-FB9F,06BA,
-FBA0,06BB,
-FBA1,06BB,
-FBA2,06BB,
-FBA3,06BB,
-FBA4,06C0,
-FBA5,06C0,
-FBA6,06C1,
-FBA7,06C1,
-FBA8,06C1,
-FBA9,06C1,
-FBAA,06BE,
-FBAB,06BE,
-FBAC,06BE,
-FBAD,06BE,
-FBAE,06D2,
-FBAF,06D2,
-FBB0,06D3,
-FBB1,06D3,
-FBD3,06AD,
-FBD4,06AD,
-FBD5,06AD,
-FBD6,06AD,
-FBD7,06C7,
-FBD8,06C7,
-FBD9,06C6,
-FBDA,06C6,
-FBDB,06C8,
-FBDC,06C8,
-FBDD,0677,
-FBDE,06CB,
-FBDF,06CB,
-FBE0,06C5,
-FBE1,06C5,
-FBE2,06C9,
-FBE3,06C9,
-FBE4,06D0,
-FBE5,06D0,
-FBE6,06D0,
-FBE7,06D0,
-FBE8,0649,
-FBE9,0649,
-FBEA,0626 0627,
-FBEB,0626 0627,
-FBEC,0626 06D5,
-FBED,0626 06D5,
-FBEE,0626 0648,
-FBEF,0626 0648,
-FBF0,0626 06C7,
-FBF1,0626 06C7,
-FBF2,0626 06C6,
-FBF3,0626 06C6,
-FBF4,0626 06C8,
-FBF5,0626 06C8,
-FBF6,0626 06D0,
-FBF7,0626 06D0,
-FBF8,0626 06D0,
-FBF9,0626 0649,
-FBFA,0626 0649,
-FBFB,0626 0649,
-FBFC,06CC,
-FBFD,06CC,
-FBFE,06CC,
-FBFF,06CC,
-FC00,0626 062C,
-FC01,0626 062D,
-FC02,0626 0645,
-FC03,0626 0649,
-FC04,0626 064A,
-FC05,0628 062C,
-FC06,0628 062D,
-FC07,0628 062E,
-FC08,0628 0645,
-FC09,0628 0649,
-FC0A,0628 064A,
-FC0B,062A 062C,
-FC0C,062A 062D,
-FC0D,062A 062E,
-FC0E,062A 0645,
-FC0F,062A 0649,
-FC10,062A 064A,
-FC11,062B 062C,
-FC12,062B 0645,
-FC13,062B 0649,
-FC14,062B 064A,
-FC15,062C 062D,
-FC16,062C 0645,
-FC17,062D 062C,
-FC18,062D 0645,
-FC19,062E 062C,
-FC1A,062E 062D,
-FC1B,062E 0645,
-FC1C,0633 062C,
-FC1D,0633 062D,
-FC1E,0633 062E,
-FC1F,0633 0645,
-FC20,0635 062D,
-FC21,0635 0645,
-FC22,0636 062C,
-FC23,0636 062D,
-FC24,0636 062E,
-FC25,0636 0645,
-FC26,0637 062D,
-FC27,0637 0645,
-FC28,0638 0645,
-FC29,0639 062C,
-FC2A,0639 0645,
-FC2B,063A 062C,
-FC2C,063A 0645,
-FC2D,0641 062C,
-FC2E,0641 062D,
-FC2F,0641 062E,
-FC30,0641 0645,
-FC31,0641 0649,
-FC32,0641 064A,
-FC33,0642 062D,
-FC34,0642 0645,
-FC35,0642 0649,
-FC36,0642 064A,
-FC37,0643 0627,
-FC38,0643 062C,
-FC39,0643 062D,
-FC3A,0643 062E,
-FC3B,0643 0644,
-FC3C,0643 0645,
-FC3D,0643 0649,
-FC3E,0643 064A,
-FC3F,0644 062C,
-FC40,0644 062D,
-FC41,0644 062E,
-FC42,0644 0645,
-FC43,0644 0649,
-FC44,0644 064A,
-FC45,0645 062C,
-FC46,0645 062D,
-FC47,0645 062E,
-FC48,0645 0645,
-FC49,0645 0649,
-FC4A,0645 064A,
-FC4B,0646 062C,
-FC4C,0646 062D,
-FC4D,0646 062E,
-FC4E,0646 0645,
-FC4F,0646 0649,
-FC50,0646 064A,
-FC51,0647 062C,
-FC52,0647 0645,
-FC53,0647 0649,
-FC54,0647 064A,
-FC55,064A 062C,
-FC56,064A 062D,
-FC57,064A 062E,
-FC58,064A 0645,
-FC59,064A 0649,
-FC5A,064A 064A,
-FC5B,0630 0670,
-FC5C,0631 0670,
-FC5D,0649 0670,
-FC5E,0020 064C 0651,
-FC5F,0020 064D 0651,
-FC60,0020 064E 0651,
-FC61,0020 064F 0651,
-FC62,0020 0650 0651,
-FC63,0020 0651 0670,
-FC64,0626 0631,
-FC65,0626 0632,
-FC66,0626 0645,
-FC67,0626 0646,
-FC68,0626 0649,
-FC69,0626 064A,
-FC6A,0628 0631,
-FC6B,0628 0632,
-FC6C,0628 0645,
-FC6D,0628 0646,
-FC6E,0628 0649,
-FC6F,0628 064A,
-FC70,062A 0631,
-FC71,062A 0632,
-FC72,062A 0645,
-FC73,062A 0646,
-FC74,062A 0649,
-FC75,062A 064A,
-FC76,062B 0631,
-FC77,062B 0632,
-FC78,062B 0645,
-FC79,062B 0646,
-FC7A,062B 0649,
-FC7B,062B 064A,
-FC7C,0641 0649,
-FC7D,0641 064A,
-FC7E,0642 0649,
-FC7F,0642 064A,
-FC80,0643 0627,
-FC81,0643 0644,
-FC82,0643 0645,
-FC83,0643 0649,
-FC84,0643 064A,
-FC85,0644 0645,
-FC86,0644 0649,
-FC87,0644 064A,
-FC88,0645 0627,
-FC89,0645 0645,
-FC8A,0646 0631,
-FC8B,0646 0632,
-FC8C,0646 0645,
-FC8D,0646 0646,
-FC8E,0646 0649,
-FC8F,0646 064A,
-FC90,0649 0670,
-FC91,064A 0631,
-FC92,064A 0632,
-FC93,064A 0645,
-FC94,064A 0646,
-FC95,064A 0649,
-FC96,064A 064A,
-FC97,0626 062C,
-FC98,0626 062D,
-FC99,0626 062E,
-FC9A,0626 0645,
-FC9B,0626 0647,
-FC9C,0628 062C,
-FC9D,0628 062D,
-FC9E,0628 062E,
-FC9F,0628 0645,
-FCA0,0628 0647,
-FCA1,062A 062C,
-FCA2,062A 062D,
-FCA3,062A 062E,
-FCA4,062A 0645,
-FCA5,062A 0647,
-FCA6,062B 0645,
-FCA7,062C 062D,
-FCA8,062C 0645,
-FCA9,062D 062C,
-FCAA,062D 0645,
-FCAB,062E 062C,
-FCAC,062E 0645,
-FCAD,0633 062C,
-FCAE,0633 062D,
-FCAF,0633 062E,
-FCB0,0633 0645,
-FCB1,0635 062D,
-FCB2,0635 062E,
-FCB3,0635 0645,
-FCB4,0636 062C,
-FCB5,0636 062D,
-FCB6,0636 062E,
-FCB7,0636 0645,
-FCB8,0637 062D,
-FCB9,0638 0645,
-FCBA,0639 062C,
-FCBB,0639 0645,
-FCBC,063A 062C,
-FCBD,063A 0645,
-FCBE,0641 062C,
-FCBF,0641 062D,
-FCC0,0641 062E,
-FCC1,0641 0645,
-FCC2,0642 062D,
-FCC3,0642 0645,
-FCC4,0643 062C,
-FCC5,0643 062D,
-FCC6,0643 062E,
-FCC7,0643 0644,
-FCC8,0643 0645,
-FCC9,0644 062C,
-FCCA,0644 062D,
-FCCB,0644 062E,
-FCCC,0644 0645,
-FCCD,0644 0647,
-FCCE,0645 062C,
-FCCF,0645 062D,
-FCD0,0645 062E,
-FCD1,0645 0645,
-FCD2,0646 062C,
-FCD3,0646 062D,
-FCD4,0646 062E,
-FCD5,0646 0645,
-FCD6,0646 0647,
-FCD7,0647 062C,
-FCD8,0647 0645,
-FCD9,0647 0670,
-FCDA,064A 062C,
-FCDB,064A 062D,
-FCDC,064A 062E,
-FCDD,064A 0645,
-FCDE,064A 0647,
-FCDF,0626 0645,
-FCE0,0626 0647,
-FCE1,0628 0645,
-FCE2,0628 0647,
-FCE3,062A 0645,
-FCE4,062A 0647,
-FCE5,062B 0645,
-FCE6,062B 0647,
-FCE7,0633 0645,
-FCE8,0633 0647,
-FCE9,0634 0645,
-FCEA,0634 0647,
-FCEB,0643 0644,
-FCEC,0643 0645,
-FCED,0644 0645,
-FCEE,0646 0645,
-FCEF,0646 0647,
-FCF0,064A 0645,
-FCF1,064A 0647,
-FCF2,0640 064E 0651,
-FCF3,0640 064F 0651,
-FCF4,0640 0650 0651,
-FCF5,0637 0649,
-FCF6,0637 064A,
-FCF7,0639 0649,
-FCF8,0639 064A,
-FCF9,063A 0649,
-FCFA,063A 064A,
-FCFB,0633 0649,
-FCFC,0633 064A,
-FCFD,0634 0649,
-FCFE,0634 064A,
-FCFF,062D 0649,
-FD00,062D 064A,
-FD01,062C 0649,
-FD02,062C 064A,
-FD03,062E 0649,
-FD04,062E 064A,
-FD05,0635 0649,
-FD06,0635 064A,
-FD07,0636 0649,
-FD08,0636 064A,
-FD09,0634 062C,
-FD0A,0634 062D,
-FD0B,0634 062E,
-FD0C,0634 0645,
-FD0D,0634 0631,
-FD0E,0633 0631,
-FD0F,0635 0631,
-FD10,0636 0631,
-FD11,0637 0649,
-FD12,0637 064A,
-FD13,0639 0649,
-FD14,0639 064A,
-FD15,063A 0649,
-FD16,063A 064A,
-FD17,0633 0649,
-FD18,0633 064A,
-FD19,0634 0649,
-FD1A,0634 064A,
-FD1B,062D 0649,
-FD1C,062D 064A,
-FD1D,062C 0649,
-FD1E,062C 064A,
-FD1F,062E 0649,
-FD20,062E 064A,
-FD21,0635 0649,
-FD22,0635 064A,
-FD23,0636 0649,
-FD24,0636 064A,
-FD25,0634 062C,
-FD26,0634 062D,
-FD27,0634 062E,
-FD28,0634 0645,
-FD29,0634 0631,
-FD2A,0633 0631,
-FD2B,0635 0631,
-FD2C,0636 0631,
-FD2D,0634 062C,
-FD2E,0634 062D,
-FD2F,0634 062E,
-FD30,0634 0645,
-FD31,0633 0647,
-FD32,0634 0647,
-FD33,0637 0645,
-FD34,0633 062C,
-FD35,0633 062D,
-FD36,0633 062E,
-FD37,0634 062C,
-FD38,0634 062D,
-FD39,0634 062E,
-FD3A,0637 0645,
-FD3B,0638 0645,
-FD3C,0627 064B,
-FD3D,0627 064B,
-FD50,062A 062C 0645,
-FD51,062A 062D 062C,
-FD52,062A 062D 062C,
-FD53,062A 062D 0645,
-FD54,062A 062E 0645,
-FD55,062A 0645 062C,
-FD56,062A 0645 062D,
-FD57,062A 0645 062E,
-FD58,062C 0645 062D,
-FD59,062C 0645 062D,
-FD5A,062D 0645 064A,
-FD5B,062D 0645 0649,
-FD5C,0633 062D 062C,
-FD5D,0633 062C 062D,
-FD5E,0633 062C 0649,
-FD5F,0633 0645 062D,
-FD60,0633 0645 062D,
-FD61,0633 0645 062C,
-FD62,0633 0645 0645,
-FD63,0633 0645 0645,
-FD64,0635 062D 062D,
-FD65,0635 062D 062D,
-FD66,0635 0645 0645,
-FD67,0634 062D 0645,
-FD68,0634 062D 0645,
-FD69,0634 062C 064A,
-FD6A,0634 0645 062E,
-FD6B,0634 0645 062E,
-FD6C,0634 0645 0645,
-FD6D,0634 0645 0645,
-FD6E,0636 062D 0649,
-FD6F,0636 062E 0645,
-FD70,0636 062E 0645,
-FD71,0637 0645 062D,
-FD72,0637 0645 062D,
-FD73,0637 0645 0645,
-FD74,0637 0645 064A,
-FD75,0639 062C 0645,
-FD76,0639 0645 0645,
-FD77,0639 0645 0645,
-FD78,0639 0645 0649,
-FD79,063A 0645 0645,
-FD7A,063A 0645 064A,
-FD7B,063A 0645 0649,
-FD7C,0641 062E 0645,
-FD7D,0641 062E 0645,
-FD7E,0642 0645 062D,
-FD7F,0642 0645 0645,
-FD80,0644 062D 0645,
-FD81,0644 062D 064A,
-FD82,0644 062D 0649,
-FD83,0644 062C 062C,
-FD84,0644 062C 062C,
-FD85,0644 062E 0645,
-FD86,0644 062E 0645,
-FD87,0644 0645 062D,
-FD88,0644 0645 062D,
-FD89,0645 062D 062C,
-FD8A,0645 062D 0645,
-FD8B,0645 062D 064A,
-FD8C,0645 062C 062D,
-FD8D,0645 062C 0645,
-FD8E,0645 062E 062C,
-FD8F,0645 062E 0645,
-FD92,0645 062C 062E,
-FD93,0647 0645 062C,
-FD94,0647 0645 0645,
-FD95,0646 062D 0645,
-FD96,0646 062D 0649,
-FD97,0646 062C 0645,
-FD98,0646 062C 0645,
-FD99,0646 062C 0649,
-FD9A,0646 0645 064A,
-FD9B,0646 0645 0649,
-FD9C,064A 0645 0645,
-FD9D,064A 0645 0645,
-FD9E,0628 062E 064A,
-FD9F,062A 062C 064A,
-FDA0,062A 062C 0649,
-FDA1,062A 062E 064A,
-FDA2,062A 062E 0649,
-FDA3,062A 0645 064A,
-FDA4,062A 0645 0649,
-FDA5,062C 0645 064A,
-FDA6,062C 062D 0649,
-FDA7,062C 0645 0649,
-FDA8,0633 062E 0649,
-FDA9,0635 062D 064A,
-FDAA,0634 062D 064A,
-FDAB,0636 062D 064A,
-FDAC,0644 062C 064A,
-FDAD,0644 0645 064A,
-FDAE,064A 062D 064A,
-FDAF,064A 062C 064A,
-FDB0,064A 0645 064A,
-FDB1,0645 0645 064A,
-FDB2,0642 0645 064A,
-FDB3,0646 062D 064A,
-FDB4,0642 0645 062D,
-FDB5,0644 062D 0645,
-FDB6,0639 0645 064A,
-FDB7,0643 0645 064A,
-FDB8,0646 062C 062D,
-FDB9,0645 062E 064A,
-FDBA,0644 062C 0645,
-FDBB,0643 0645 0645,
-FDBC,0644 062C 0645,
-FDBD,0646 062C 062D,
-FDBE,062C 062D 064A,
-FDBF,062D 062C 064A,
-FDC0,0645 062C 064A,
-FDC1,0641 0645 064A,
-FDC2,0628 062D 064A,
-FDC3,0643 0645 0645,
-FDC4,0639 062C 0645,
-FDC5,0635 0645 0645,
-FDC6,0633 062E 064A,
-FDC7,0646 062C 064A,
-FDF0,0635 0644 06D2,
-FDF1,0642 0644 06D2,
-FDF2,0627 0644 0644 0647,
-FDF3,0627 0643 0628 0631,
-FDF4,0645 062D 0645 062F,
-FDF5,0635 0644 0639 0645,
-FDF6,0631 0633 0648 0644,
-FDF7,0639 0644 064A 0647,
-FDF8,0648 0633 0644 0645,
-FDF9,0635 0644 0649,
-FDFA,0635 0644 0649 0020 0627 0644 0644 0647 0020 0639 0644 064A 0647 0020 0648 0633 0644 0645,
-FDFB,062C 0644 0020 062C 0644 0627 0644 0647,
-FDFC,0631 06CC 0627 0644,
-FE70,0020 064B,
-FE71,0640 064B,
-FE72,0020 064C,
-FE74,0020 064D,
-FE76,0020 064E,
-FE77,0640 064E,
-FE78,0020 064F,
-FE79,0640 064F,
-FE7A,0020 0650,
-FE7B,0640 0650,
-FE7C,0020 0651,
-FE7D,0640 0651,
-FE7E,0020 0652,
-FE7F,0640 0652,
-FE80,0621,
-FE81,0622,
-FE82,0622,
-FE83,0623,
-FE84,0623,
-FE85,0624,
-FE86,0624,
-FE87,0625,
-FE88,0625,
-FE89,0626,
-FE8A,0626,
-FE8B,0626,
-FE8C,0626,
-FE8D,0627,
-FE8E,0627,
-FE8F,0628,
-FE90,0628,
-FE91,0628,
-FE92,0628,
-FE93,0629,
-FE94,0629,
-FE95,062A,
-FE96,062A,
-FE97,062A,
-FE98,062A,
-FE99,062B,
-FE9A,062B,
-FE9B,062B,
-FE9C,062B,
-FE9D,062C,
-FE9E,062C,
-FE9F,062C,
-FEA0,062C,
-FEA1,062D,
-FEA2,062D,
-FEA3,062D,
-FEA4,062D,
-FEA5,062E,
-FEA6,062E,
-FEA7,062E,
-FEA8,062E,
-FEA9,062F,
-FEAA,062F,
-FEAB,0630,
-FEAC,0630,
-FEAD,0631,
-FEAE,0631,
-FEAF,0632,
-FEB0,0632,
-FEB1,0633,
-FEB2,0633,
-FEB3,0633,
-FEB4,0633,
-FEB5,0634,
-FEB6,0634,
-FEB7,0634,
-FEB8,0634,
-FEB9,0635,
-FEBA,0635,
-FEBB,0635,
-FEBC,0635,
-FEBD,0636,
-FEBE,0636,
-FEBF,0636,
-FEC0,0636,
-FEC1,0637,
-FEC2,0637,
-FEC3,0637,
-FEC4,0637,
-FEC5,0638,
-FEC6,0638,
-FEC7,0638,
-FEC8,0638,
-FEC9,0639,
-FECA,0639,
-FECB,0639,
-FECC,0639,
-FECD,063A,
-FECE,063A,
-FECF,063A,
-FED0,063A,
-FED1,0641,
-FED2,0641,
-FED3,0641,
-FED4,0641,
-FED5,0642,
-FED6,0642,
-FED7,0642,
-FED8,0642,
-FED9,0643,
-FEDA,0643,
-FEDB,0643,
-FEDC,0643,
-FEDD,0644,
-FEDE,0644,
-FEDF,0644,
-FEE0,0644,
-FEE1,0645,
-FEE2,0645,
-FEE3,0645,
-FEE4,0645,
-FEE5,0646,
-FEE6,0646,
-FEE7,0646,
-FEE8,0646,
-FEE9,0647,
-FEEA,0647,
-FEEB,0647,
-FEEC,0647,
-FEED,0648,
-FEEE,0648,
-FEEF,0649,
-FEF0,0649,
-FEF1,064A,
-FEF2,064A,
-FEF3,064A,
-FEF4,064A,
-FEF5,0644 0622,
-FEF6,0644 0622,
-FEF7,0644 0623,
-FEF8,0644 0623,
-FEF9,0644 0625,
-FEFA,0644 0625,
-FEFB,0644 0627,
-FEFC,0644 0627,
-FF01,0021,FullWidth
-FF02,0022,
-FF03,0023,
-FF04,0024,
-FF05,0025,
-FF06,0026,
-FF07,0027,
-FF08,0028,
-FF09,0029,
-FF0A,002A,
-FF0B,002B,
-FF0C,002C,
-FF0D,002D,
-FF0E,002E,
-FF0F,002F,
-FF10,0030,
-FF11,0031,
-FF12,0032,
-FF13,0033,
-FF14,0034,
-FF15,0035,
-FF16,0036,
-FF17,0037,
-FF18,0038,
-FF19,0039,
-FF1A,003A,
-FF1B,003B,
-FF1C,003C,
-FF1D,003D,
-FF1E,003E,
-FF1F,003F,
-FF20,0040,
-FF21,0041,
-FF22,0042,
-FF23,0043,
-FF24,0044,
-FF25,0045,
-FF26,0046,
-FF27,0047,
-FF28,0048,
-FF29,0049,
-FF2A,004A,
-FF2B,004B,
-FF2C,004C,
-FF2D,004D,
-FF2E,004E,
-FF2F,004F,
-FF30,0050,
-FF31,0051,
-FF32,0052,
-FF33,0053,
-FF34,0054,
-FF35,0055,
-FF36,0056,
-FF37,0057,
-FF38,0058,
-FF39,0059,
-FF3A,005A,
-FF3B,005B,
-FF3C,005C,
-FF3D,005D,
-FF3E,005E,
-FF3F,005F,
-FF40,0060,
-FF41,0061,
-FF42,0062,
-FF43,0063,
-FF44,0064,
-FF45,0065,
-FF46,0066,
-FF47,0067,
-FF48,0068,
-FF49,0069,
-FF4A,006A,
-FF4B,006B,
-FF4C,006C,
-FF4D,006D,
-FF4E,006E,
-FF4F,006F,
-FF50,0070,
-FF51,0071,
-FF52,0072,
-FF53,0073,
-FF54,0074,
-FF55,0075,
-FF56,0076,
-FF57,0077,
-FF58,0078,
-FF59,0079,
-FF5A,007A,
-FF5B,007B,
-FF5C,007C,
-FF5D,007D,
-FF5E,007E,
-FF5F,2985,
-FF60,2986,
-FFE0,00A2,
-FFE1,00A3,
-FFE2,00AC,
-FFE3,00AF,
-FFE4,00A6,
-FFE5,00A5,
-FFE6,20A9,
-FFF0,0020,Specials
-FFF1,0020,
-FFF2,0020,
-FFF3,0020,
-FFF4,0020,
-FFF5,0020,
-FFF6,0020,
-FFF7,0020,
-FFF8,0020,
-FFF9,0020,
-FFFA,0020,
-FFFB,0020,
-FFFC,0020,
-FFFD,0020,
-FFFE,0020,
+From,To,Desc
+A78C,0027,Latin Small Letter Saltillo ꞌ
+FEFF,200C,ZERO WIDTH NO-BREAK SPACE
+200B,200C,ZERO WIDTH SPACE
+2010,002D,HYPHEN
+2011,002D,NON-BREAKING HYPHEN
+2012,002D,FIGURE DASH
+2013,002D,EN DASH
+2014,002D,EM DASH
+2015,002D,HORIZONTAL BAR
+2212,002D,Minus
+00AD,002D,Soft Hyphen
+FE58,002D,SMALL EM DASH
+FE63,002D,MALL HYPHEN-MINUS
+FF0D,002D,FULLWIDTH HYPHEN-MINUS
+1680,0020,OGHAM SPACE MARK
+2000,0020,EN QUAD
+2001,0020,EM QUAD
+2002,0020,EN SPACE
+2003,0020,EM SPACE
+2004,0020,THREE-PER-EM SPACE
+2005,0020,FOUR-PER-EM SPACE
+2006,0020,SIX-PER-EM SPACE
+205F,0020,MEDIUM MATHEMATICAL SPACE
+3000,0020,IDEOGRAPHIC SPACE
+2007,0020,FIGURE SPACE
+2008,0020,PUNCTUATION SPACE
+2009,0020,THIN SPACE
+200A,0020,HAIR SPACE
+00A0,0020,NO-BREAK SPACE
+202F,0020,NARROW NO-BREAK SPACE
+200E,0020,LEFT-TO-RIGHT MARK
+200F,0020,RIGHT-TO-LEFT MARK
+202A,0020,LEFT-TO-RIGHT EMBEDDING
+202B,0020,RIGHT-TO-LEFT EMBEDDING
+202C,0020,POP DIRECTIONAL FORMATTING
+202D,0020,LEFT-TO-RIGHT OVERRIDE
+202E,0020,RIGHT-TO-LEFT OVERRIDE
+0000,0020,Control
+0001,0020,
+0002,0020,
+0003,0020,
+0004,0020,
+0005,0020,
+0006,0020,
+0007,0020,
+0008,0020,
+000B,0020,
+000C,0020,
+000E,0020,
+000F,0020,
+0010,0020,
+0011,0020,
+0012,0020,
+0013,0020,
+0014,0020,
+0015,0020,
+0016,0020,
+0017,0020,
+0018,0020,
+0019,0020,
+001A,0020,
+001B,0020,
+001C,0020,
+001D,0020,
+001E,0020,
+001F,0020,
+007F,0020,
+0080,0020,
+0081,0020,
+0082,0020,
+0083,0020,
+0084,0020,
+0085,0020,
+0086,0020,
+0087,0020,
+0088,0020,
+0089,0020,
+008A,0020,
+008B,0020,
+008C,0020,
+008D,0020,
+008E,0020,
+008F,0020,
+0090,0020,
+0091,0020,
+0092,0020,
+0093,0020,
+0094,0020,
+0095,0020,
+0096,0020,
+0097,0020,
+0098,0020,
+0099,0020,
+009A,0020,
+009B,0020,
+009C,0020,
+009D,0020,
+009E,0020,
+009F,0020,
+0610,,Arabic Nonspacing Marks
+0611,,
+0612,,
+0613,,
+0614,,
+0615,,
+0616,,
+0617,,
+0618,,
+0619,,
+061A,,
+0653,,
+0654,,
+0655,,
+0656,,
+0657,,
+0658,,
+0659,,
+065A,,
+065B,,
+065C,,
+065D,,
+065E,,
+065F,,
+0670,,
+06D6,,
+06D7,,
+06D8,,
+06D9,,
+06DA,,
+06DB,,
+06DC,,
+06DF,,
+06E0,,
+06E1,,
+06E2,,
+06E3,,
+06E4,,
+06E7,,
+06E8,,
+06EA,,
+06EB,,
+06EC,,
+06ED,,
+FB50,0671,Arabic Presentation Forms
+FB51,0671,
+FB52,067B,
+FB53,067B,
+FB54,067B,
+FB55,067B,
+FB56,067E,
+FB57,067E,
+FB58,067E,
+FB59,067E,
+FB5A,0680,
+FB5B,0680,
+FB5C,0680,
+FB5D,0680,
+FB5E,067A,
+FB5F,067A,
+FB60,067A,
+FB61,067A,
+FB62,067F,
+FB63,067F,
+FB64,067F,
+FB65,067F,
+FB66,0679,
+FB67,0679,
+FB68,0679,
+FB69,0679,
+FB6A,06A4,
+FB6B,06A4,
+FB6C,06A4,
+FB6D,06A4,
+FB6E,06A6,
+FB6F,06A6,
+FB70,06A6,
+FB71,06A6,
+FB72,0684,
+FB73,0684,
+FB74,0684,
+FB75,0684,
+FB76,0683,
+FB77,0683,
+FB78,0683,
+FB79,0683,
+FB7A,0686,
+FB7B,0686,
+FB7C,0686,
+FB7D,0686,
+FB7E,0687,
+FB7F,0687,
+FB80,0687,
+FB81,0687,
+FB82,068D,
+FB83,068D,
+FB84,068C,
+FB85,068C,
+FB86,068E,
+FB87,068E,
+FB88,0688,
+FB89,0688,
+FB8A,0698,
+FB8B,0698,
+FB8C,0691,
+FB8D,0691,
+FB8E,06A9,
+FB8F,06A9,
+FB90,06A9,
+FB91,06A9,
+FB92,06AF,
+FB93,06AF,
+FB94,06AF,
+FB95,06AF,
+FB96,06B3,
+FB97,06B3,
+FB98,06B3,
+FB99,06B3,
+FB9A,06B1,
+FB9B,06B1,
+FB9C,06B1,
+FB9D,06B1,
+FB9E,06BA,
+FB9F,06BA,
+FBA0,06BB,
+FBA1,06BB,
+FBA2,06BB,
+FBA3,06BB,
+FBA4,06C0,
+FBA5,06C0,
+FBA6,06C1,
+FBA7,06C1,
+FBA8,06C1,
+FBA9,06C1,
+FBAA,06BE,
+FBAB,06BE,
+FBAC,06BE,
+FBAD,06BE,
+FBAE,06D2,
+FBAF,06D2,
+FBB0,06D3,
+FBB1,06D3,
+FBD3,06AD,
+FBD4,06AD,
+FBD5,06AD,
+FBD6,06AD,
+FBD7,06C7,
+FBD8,06C7,
+FBD9,06C6,
+FBDA,06C6,
+FBDB,06C8,
+FBDC,06C8,
+FBDD,0677,
+FBDE,06CB,
+FBDF,06CB,
+FBE0,06C5,
+FBE1,06C5,
+FBE2,06C9,
+FBE3,06C9,
+FBE4,06D0,
+FBE5,06D0,
+FBE6,06D0,
+FBE7,06D0,
+FBE8,0649,
+FBE9,0649,
+FBEA,0626 0627,
+FBEB,0626 0627,
+FBEC,0626 06D5,
+FBED,0626 06D5,
+FBEE,0626 0648,
+FBEF,0626 0648,
+FBF0,0626 06C7,
+FBF1,0626 06C7,
+FBF2,0626 06C6,
+FBF3,0626 06C6,
+FBF4,0626 06C8,
+FBF5,0626 06C8,
+FBF6,0626 06D0,
+FBF7,0626 06D0,
+FBF8,0626 06D0,
+FBF9,0626 0649,
+FBFA,0626 0649,
+FBFB,0626 0649,
+FBFC,06CC,
+FBFD,06CC,
+FBFE,06CC,
+FBFF,06CC,
+FC00,0626 062C,
+FC01,0626 062D,
+FC02,0626 0645,
+FC03,0626 0649,
+FC04,0626 064A,
+FC05,0628 062C,
+FC06,0628 062D,
+FC07,0628 062E,
+FC08,0628 0645,
+FC09,0628 0649,
+FC0A,0628 064A,
+FC0B,062A 062C,
+FC0C,062A 062D,
+FC0D,062A 062E,
+FC0E,062A 0645,
+FC0F,062A 0649,
+FC10,062A 064A,
+FC11,062B 062C,
+FC12,062B 0645,
+FC13,062B 0649,
+FC14,062B 064A,
+FC15,062C 062D,
+FC16,062C 0645,
+FC17,062D 062C,
+FC18,062D 0645,
+FC19,062E 062C,
+FC1A,062E 062D,
+FC1B,062E 0645,
+FC1C,0633 062C,
+FC1D,0633 062D,
+FC1E,0633 062E,
+FC1F,0633 0645,
+FC20,0635 062D,
+FC21,0635 0645,
+FC22,0636 062C,
+FC23,0636 062D,
+FC24,0636 062E,
+FC25,0636 0645,
+FC26,0637 062D,
+FC27,0637 0645,
+FC28,0638 0645,
+FC29,0639 062C,
+FC2A,0639 0645,
+FC2B,063A 062C,
+FC2C,063A 0645,
+FC2D,0641 062C,
+FC2E,0641 062D,
+FC2F,0641 062E,
+FC30,0641 0645,
+FC31,0641 0649,
+FC32,0641 064A,
+FC33,0642 062D,
+FC34,0642 0645,
+FC35,0642 0649,
+FC36,0642 064A,
+FC37,0643 0627,
+FC38,0643 062C,
+FC39,0643 062D,
+FC3A,0643 062E,
+FC3B,0643 0644,
+FC3C,0643 0645,
+FC3D,0643 0649,
+FC3E,0643 064A,
+FC3F,0644 062C,
+FC40,0644 062D,
+FC41,0644 062E,
+FC42,0644 0645,
+FC43,0644 0649,
+FC44,0644 064A,
+FC45,0645 062C,
+FC46,0645 062D,
+FC47,0645 062E,
+FC48,0645 0645,
+FC49,0645 0649,
+FC4A,0645 064A,
+FC4B,0646 062C,
+FC4C,0646 062D,
+FC4D,0646 062E,
+FC4E,0646 0645,
+FC4F,0646 0649,
+FC50,0646 064A,
+FC51,0647 062C,
+FC52,0647 0645,
+FC53,0647 0649,
+FC54,0647 064A,
+FC55,064A 062C,
+FC56,064A 062D,
+FC57,064A 062E,
+FC58,064A 0645,
+FC59,064A 0649,
+FC5A,064A 064A,
+FC5B,0630 0670,
+FC5C,0631 0670,
+FC5D,0649 0670,
+FC5E,0020 064C 0651,
+FC5F,0020 064D 0651,
+FC60,0020 064E 0651,
+FC61,0020 064F 0651,
+FC62,0020 0650 0651,
+FC63,0020 0651 0670,
+FC64,0626 0631,
+FC65,0626 0632,
+FC66,0626 0645,
+FC67,0626 0646,
+FC68,0626 0649,
+FC69,0626 064A,
+FC6A,0628 0631,
+FC6B,0628 0632,
+FC6C,0628 0645,
+FC6D,0628 0646,
+FC6E,0628 0649,
+FC6F,0628 064A,
+FC70,062A 0631,
+FC71,062A 0632,
+FC72,062A 0645,
+FC73,062A 0646,
+FC74,062A 0649,
+FC75,062A 064A,
+FC76,062B 0631,
+FC77,062B 0632,
+FC78,062B 0645,
+FC79,062B 0646,
+FC7A,062B 0649,
+FC7B,062B 064A,
+FC7C,0641 0649,
+FC7D,0641 064A,
+FC7E,0642 0649,
+FC7F,0642 064A,
+FC80,0643 0627,
+FC81,0643 0644,
+FC82,0643 0645,
+FC83,0643 0649,
+FC84,0643 064A,
+FC85,0644 0645,
+FC86,0644 0649,
+FC87,0644 064A,
+FC88,0645 0627,
+FC89,0645 0645,
+FC8A,0646 0631,
+FC8B,0646 0632,
+FC8C,0646 0645,
+FC8D,0646 0646,
+FC8E,0646 0649,
+FC8F,0646 064A,
+FC90,0649 0670,
+FC91,064A 0631,
+FC92,064A 0632,
+FC93,064A 0645,
+FC94,064A 0646,
+FC95,064A 0649,
+FC96,064A 064A,
+FC97,0626 062C,
+FC98,0626 062D,
+FC99,0626 062E,
+FC9A,0626 0645,
+FC9B,0626 0647,
+FC9C,0628 062C,
+FC9D,0628 062D,
+FC9E,0628 062E,
+FC9F,0628 0645,
+FCA0,0628 0647,
+FCA1,062A 062C,
+FCA2,062A 062D,
+FCA3,062A 062E,
+FCA4,062A 0645,
+FCA5,062A 0647,
+FCA6,062B 0645,
+FCA7,062C 062D,
+FCA8,062C 0645,
+FCA9,062D 062C,
+FCAA,062D 0645,
+FCAB,062E 062C,
+FCAC,062E 0645,
+FCAD,0633 062C,
+FCAE,0633 062D,
+FCAF,0633 062E,
+FCB0,0633 0645,
+FCB1,0635 062D,
+FCB2,0635 062E,
+FCB3,0635 0645,
+FCB4,0636 062C,
+FCB5,0636 062D,
+FCB6,0636 062E,
+FCB7,0636 0645,
+FCB8,0637 062D,
+FCB9,0638 0645,
+FCBA,0639 062C,
+FCBB,0639 0645,
+FCBC,063A 062C,
+FCBD,063A 0645,
+FCBE,0641 062C,
+FCBF,0641 062D,
+FCC0,0641 062E,
+FCC1,0641 0645,
+FCC2,0642 062D,
+FCC3,0642 0645,
+FCC4,0643 062C,
+FCC5,0643 062D,
+FCC6,0643 062E,
+FCC7,0643 0644,
+FCC8,0643 0645,
+FCC9,0644 062C,
+FCCA,0644 062D,
+FCCB,0644 062E,
+FCCC,0644 0645,
+FCCD,0644 0647,
+FCCE,0645 062C,
+FCCF,0645 062D,
+FCD0,0645 062E,
+FCD1,0645 0645,
+FCD2,0646 062C,
+FCD3,0646 062D,
+FCD4,0646 062E,
+FCD5,0646 0645,
+FCD6,0646 0647,
+FCD7,0647 062C,
+FCD8,0647 0645,
+FCD9,0647 0670,
+FCDA,064A 062C,
+FCDB,064A 062D,
+FCDC,064A 062E,
+FCDD,064A 0645,
+FCDE,064A 0647,
+FCDF,0626 0645,
+FCE0,0626 0647,
+FCE1,0628 0645,
+FCE2,0628 0647,
+FCE3,062A 0645,
+FCE4,062A 0647,
+FCE5,062B 0645,
+FCE6,062B 0647,
+FCE7,0633 0645,
+FCE8,0633 0647,
+FCE9,0634 0645,
+FCEA,0634 0647,
+FCEB,0643 0644,
+FCEC,0643 0645,
+FCED,0644 0645,
+FCEE,0646 0645,
+FCEF,0646 0647,
+FCF0,064A 0645,
+FCF1,064A 0647,
+FCF2,0640 064E 0651,
+FCF3,0640 064F 0651,
+FCF4,0640 0650 0651,
+FCF5,0637 0649,
+FCF6,0637 064A,
+FCF7,0639 0649,
+FCF8,0639 064A,
+FCF9,063A 0649,
+FCFA,063A 064A,
+FCFB,0633 0649,
+FCFC,0633 064A,
+FCFD,0634 0649,
+FCFE,0634 064A,
+FCFF,062D 0649,
+FD00,062D 064A,
+FD01,062C 0649,
+FD02,062C 064A,
+FD03,062E 0649,
+FD04,062E 064A,
+FD05,0635 0649,
+FD06,0635 064A,
+FD07,0636 0649,
+FD08,0636 064A,
+FD09,0634 062C,
+FD0A,0634 062D,
+FD0B,0634 062E,
+FD0C,0634 0645,
+FD0D,0634 0631,
+FD0E,0633 0631,
+FD0F,0635 0631,
+FD10,0636 0631,
+FD11,0637 0649,
+FD12,0637 064A,
+FD13,0639 0649,
+FD14,0639 064A,
+FD15,063A 0649,
+FD16,063A 064A,
+FD17,0633 0649,
+FD18,0633 064A,
+FD19,0634 0649,
+FD1A,0634 064A,
+FD1B,062D 0649,
+FD1C,062D 064A,
+FD1D,062C 0649,
+FD1E,062C 064A,
+FD1F,062E 0649,
+FD20,062E 064A,
+FD21,0635 0649,
+FD22,0635 064A,
+FD23,0636 0649,
+FD24,0636 064A,
+FD25,0634 062C,
+FD26,0634 062D,
+FD27,0634 062E,
+FD28,0634 0645,
+FD29,0634 0631,
+FD2A,0633 0631,
+FD2B,0635 0631,
+FD2C,0636 0631,
+FD2D,0634 062C,
+FD2E,0634 062D,
+FD2F,0634 062E,
+FD30,0634 0645,
+FD31,0633 0647,
+FD32,0634 0647,
+FD33,0637 0645,
+FD34,0633 062C,
+FD35,0633 062D,
+FD36,0633 062E,
+FD37,0634 062C,
+FD38,0634 062D,
+FD39,0634 062E,
+FD3A,0637 0645,
+FD3B,0638 0645,
+FD3C,0627 064B,
+FD3D,0627 064B,
+FD50,062A 062C 0645,
+FD51,062A 062D 062C,
+FD52,062A 062D 062C,
+FD53,062A 062D 0645,
+FD54,062A 062E 0645,
+FD55,062A 0645 062C,
+FD56,062A 0645 062D,
+FD57,062A 0645 062E,
+FD58,062C 0645 062D,
+FD59,062C 0645 062D,
+FD5A,062D 0645 064A,
+FD5B,062D 0645 0649,
+FD5C,0633 062D 062C,
+FD5D,0633 062C 062D,
+FD5E,0633 062C 0649,
+FD5F,0633 0645 062D,
+FD60,0633 0645 062D,
+FD61,0633 0645 062C,
+FD62,0633 0645 0645,
+FD63,0633 0645 0645,
+FD64,0635 062D 062D,
+FD65,0635 062D 062D,
+FD66,0635 0645 0645,
+FD67,0634 062D 0645,
+FD68,0634 062D 0645,
+FD69,0634 062C 064A,
+FD6A,0634 0645 062E,
+FD6B,0634 0645 062E,
+FD6C,0634 0645 0645,
+FD6D,0634 0645 0645,
+FD6E,0636 062D 0649,
+FD6F,0636 062E 0645,
+FD70,0636 062E 0645,
+FD71,0637 0645 062D,
+FD72,0637 0645 062D,
+FD73,0637 0645 0645,
+FD74,0637 0645 064A,
+FD75,0639 062C 0645,
+FD76,0639 0645 0645,
+FD77,0639 0645 0645,
+FD78,0639 0645 0649,
+FD79,063A 0645 0645,
+FD7A,063A 0645 064A,
+FD7B,063A 0645 0649,
+FD7C,0641 062E 0645,
+FD7D,0641 062E 0645,
+FD7E,0642 0645 062D,
+FD7F,0642 0645 0645,
+FD80,0644 062D 0645,
+FD81,0644 062D 064A,
+FD82,0644 062D 0649,
+FD83,0644 062C 062C,
+FD84,0644 062C 062C,
+FD85,0644 062E 0645,
+FD86,0644 062E 0645,
+FD87,0644 0645 062D,
+FD88,0644 0645 062D,
+FD89,0645 062D 062C,
+FD8A,0645 062D 0645,
+FD8B,0645 062D 064A,
+FD8C,0645 062C 062D,
+FD8D,0645 062C 0645,
+FD8E,0645 062E 062C,
+FD8F,0645 062E 0645,
+FD92,0645 062C 062E,
+FD93,0647 0645 062C,
+FD94,0647 0645 0645,
+FD95,0646 062D 0645,
+FD96,0646 062D 0649,
+FD97,0646 062C 0645,
+FD98,0646 062C 0645,
+FD99,0646 062C 0649,
+FD9A,0646 0645 064A,
+FD9B,0646 0645 0649,
+FD9C,064A 0645 0645,
+FD9D,064A 0645 0645,
+FD9E,0628 062E 064A,
+FD9F,062A 062C 064A,
+FDA0,062A 062C 0649,
+FDA1,062A 062E 064A,
+FDA2,062A 062E 0649,
+FDA3,062A 0645 064A,
+FDA4,062A 0645 0649,
+FDA5,062C 0645 064A,
+FDA6,062C 062D 0649,
+FDA7,062C 0645 0649,
+FDA8,0633 062E 0649,
+FDA9,0635 062D 064A,
+FDAA,0634 062D 064A,
+FDAB,0636 062D 064A,
+FDAC,0644 062C 064A,
+FDAD,0644 0645 064A,
+FDAE,064A 062D 064A,
+FDAF,064A 062C 064A,
+FDB0,064A 0645 064A,
+FDB1,0645 0645 064A,
+FDB2,0642 0645 064A,
+FDB3,0646 062D 064A,
+FDB4,0642 0645 062D,
+FDB5,0644 062D 0645,
+FDB6,0639 0645 064A,
+FDB7,0643 0645 064A,
+FDB8,0646 062C 062D,
+FDB9,0645 062E 064A,
+FDBA,0644 062C 0645,
+FDBB,0643 0645 0645,
+FDBC,0644 062C 0645,
+FDBD,0646 062C 062D,
+FDBE,062C 062D 064A,
+FDBF,062D 062C 064A,
+FDC0,0645 062C 064A,
+FDC1,0641 0645 064A,
+FDC2,0628 062D 064A,
+FDC3,0643 0645 0645,
+FDC4,0639 062C 0645,
+FDC5,0635 0645 0645,
+FDC6,0633 062E 064A,
+FDC7,0646 062C 064A,
+FDF0,0635 0644 06D2,
+FDF1,0642 0644 06D2,
+FDF2,0627 0644 0644 0647,
+FDF3,0627 0643 0628 0631,
+FDF4,0645 062D 0645 062F,
+FDF5,0635 0644 0639 0645,
+FDF6,0631 0633 0648 0644,
+FDF7,0639 0644 064A 0647,
+FDF8,0648 0633 0644 0645,
+FDF9,0635 0644 0649,
+FDFA,0635 0644 0649 0020 0627 0644 0644 0647 0020 0639 0644 064A 0647 0020 0648 0633 0644 0645,
+FDFB,062C 0644 0020 062C 0644 0627 0644 0647,
+FDFC,0631 06CC 0627 0644,
+FE70,0020 064B,
+FE71,0640 064B,
+FE72,0020 064C,
+FE74,0020 064D,
+FE76,0020 064E,
+FE77,0640 064E,
+FE78,0020 064F,
+FE79,0640 064F,
+FE7A,0020 0650,
+FE7B,0640 0650,
+FE7C,0020 0651,
+FE7D,0640 0651,
+FE7E,0020 0652,
+FE7F,0640 0652,
+FE80,0621,
+FE81,0622,
+FE82,0622,
+FE83,0623,
+FE84,0623,
+FE85,0624,
+FE86,0624,
+FE87,0625,
+FE88,0625,
+FE89,0626,
+FE8A,0626,
+FE8B,0626,
+FE8C,0626,
+FE8D,0627,
+FE8E,0627,
+FE8F,0628,
+FE90,0628,
+FE91,0628,
+FE92,0628,
+FE93,0629,
+FE94,0629,
+FE95,062A,
+FE96,062A,
+FE97,062A,
+FE98,062A,
+FE99,062B,
+FE9A,062B,
+FE9B,062B,
+FE9C,062B,
+FE9D,062C,
+FE9E,062C,
+FE9F,062C,
+FEA0,062C,
+FEA1,062D,
+FEA2,062D,
+FEA3,062D,
+FEA4,062D,
+FEA5,062E,
+FEA6,062E,
+FEA7,062E,
+FEA8,062E,
+FEA9,062F,
+FEAA,062F,
+FEAB,0630,
+FEAC,0630,
+FEAD,0631,
+FEAE,0631,
+FEAF,0632,
+FEB0,0632,
+FEB1,0633,
+FEB2,0633,
+FEB3,0633,
+FEB4,0633,
+FEB5,0634,
+FEB6,0634,
+FEB7,0634,
+FEB8,0634,
+FEB9,0635,
+FEBA,0635,
+FEBB,0635,
+FEBC,0635,
+FEBD,0636,
+FEBE,0636,
+FEBF,0636,
+FEC0,0636,
+FEC1,0637,
+FEC2,0637,
+FEC3,0637,
+FEC4,0637,
+FEC5,0638,
+FEC6,0638,
+FEC7,0638,
+FEC8,0638,
+FEC9,0639,
+FECA,0639,
+FECB,0639,
+FECC,0639,
+FECD,063A,
+FECE,063A,
+FECF,063A,
+FED0,063A,
+FED1,0641,
+FED2,0641,
+FED3,0641,
+FED4,0641,
+FED5,0642,
+FED6,0642,
+FED7,0642,
+FED8,0642,
+FED9,0643,
+FEDA,0643,
+FEDB,0643,
+FEDC,0643,
+FEDD,0644,
+FEDE,0644,
+FEDF,0644,
+FEE0,0644,
+FEE1,0645,
+FEE2,0645,
+FEE3,0645,
+FEE4,0645,
+FEE5,0646,
+FEE6,0646,
+FEE7,0646,
+FEE8,0646,
+FEE9,0647,
+FEEA,0647,
+FEEB,0647,
+FEEC,0647,
+FEED,0648,
+FEEE,0648,
+FEEF,0649,
+FEF0,0649,
+FEF1,064A,
+FEF2,064A,
+FEF3,064A,
+FEF4,064A,
+FEF5,0644 0622,
+FEF6,0644 0622,
+FEF7,0644 0623,
+FEF8,0644 0623,
+FEF9,0644 0625,
+FEFA,0644 0625,
+FEFB,0644 0627,
+FEFC,0644 0627,
+FF01,0021,FullWidth
+FF02,0022,
+FF03,0023,
+FF04,0024,
+FF05,0025,
+FF06,0026,
+FF07,0027,
+FF08,0028,
+FF09,0029,
+FF0A,002A,
+FF0B,002B,
+FF0C,002C,
+FF0D,002D,
+FF0E,002E,
+FF0F,002F,
+FF10,0030,
+FF11,0031,
+FF12,0032,
+FF13,0033,
+FF14,0034,
+FF15,0035,
+FF16,0036,
+FF17,0037,
+FF18,0038,
+FF19,0039,
+FF1A,003A,
+FF1B,003B,
+FF1C,003C,
+FF1D,003D,
+FF1E,003E,
+FF1F,003F,
+FF20,0040,
+FF21,0041,
+FF22,0042,
+FF23,0043,
+FF24,0044,
+FF25,0045,
+FF26,0046,
+FF27,0047,
+FF28,0048,
+FF29,0049,
+FF2A,004A,
+FF2B,004B,
+FF2C,004C,
+FF2D,004D,
+FF2E,004E,
+FF2F,004F,
+FF30,0050,
+FF31,0051,
+FF32,0052,
+FF33,0053,
+FF34,0054,
+FF35,0055,
+FF36,0056,
+FF37,0057,
+FF38,0058,
+FF39,0059,
+FF3A,005A,
+FF3B,005B,
+FF3C,005C,
+FF3D,005D,
+FF3E,005E,
+FF3F,005F,
+FF40,0060,
+FF41,0061,
+FF42,0062,
+FF43,0063,
+FF44,0064,
+FF45,0065,
+FF46,0066,
+FF47,0067,
+FF48,0068,
+FF49,0069,
+FF4A,006A,
+FF4B,006B,
+FF4C,006C,
+FF4D,006D,
+FF4E,006E,
+FF4F,006F,
+FF50,0070,
+FF51,0071,
+FF52,0072,
+FF53,0073,
+FF54,0074,
+FF55,0075,
+FF56,0076,
+FF57,0077,
+FF58,0078,
+FF59,0079,
+FF5A,007A,
+FF5B,007B,
+FF5C,007C,
+FF5D,007D,
+FF5E,007E,
+FF5F,2985,
+FF60,2986,
+FFE0,00A2,
+FFE1,00A3,
+FFE2,00AC,
+FFE3,00AF,
+FFE4,00A6,
+FFE5,00A5,
+FFE6,20A9,
+FFF0,0020,Specials
+FFF1,0020,
+FFF2,0020,
+FFF3,0020,
+FFF4,0020,
+FFF5,0020,
+FFF6,0020,
+FFF7,0020,
+FFF8,0020,
+FFF9,0020,
+FFFA,0020,
+FFFB,0020,
+FFFC,0020,
+FFFD,0020,
+FFFE,0020,
 FFFF,0020
```

### Comparing `asosoft-0.1.2/src/asosoft/resources/PoemPatterns.csv` & `asosoft-0.1.3/src/asosoft/resources/PoemPatterns.csv`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Frequency,WeightPattern,Title
-1044,–∪–––∪–––∪–––∪–,فاعلاتن فاعلاتن فاعلاتن فاعلن
-999,∪–––∪–––∪–––∪–––,مفاعیلن مفاعیلن مفاعیلن مفاعیلن
-386,∪–––∪–––∪––,مفاعیلن مفاعیلن فعولن
-334,––∪∪––∪∪––∪∪––,مفعولُ مفاعیلُ مفاعیلُ فعولن
-272,––∪∪––∪∪––∪∪–,مفعولُ مفاعیلُ مفاعیلُ فعل
-213,––∪–∪–∪∪––∪–∪–,مفعولُ فاعلاتُ مفاعیلُ فاعلن
-138,∪∪––∪∪––∪∪––∪∪–,فعلاتن فعلاتن فعلاتن فعلن
-131,––∪∪–∪–∪––,مفعولُ مفاعلن فعولن
-62,–∪–––∪–––∪–,فاعلاتن فاعلاتن فاعلن
-45,∪∪––∪–∪–∪∪–,فعلاتن مفاعلن فعلن
-40,∪–∪–∪∪––∪–∪–∪∪–,مفاعلن فعلاتن مفاعلن فعلن
-31,––∪∪–––––∪∪–––,مفعولُ مفاعیلن مفعولُ مفاعیلن
-28,––∪–∪––––∪–∪––,مفعولُ فاعلاتن مفعولُ فاعلاتن
-20,∪∪––∪∪––∪∪–,فعلاتن فعلاتن فعلن
-19,––∪–––∪–––∪–––∪–,مستفعلن مستفعلن مستفعلن مستفعلن
-14,∪––∪––∪––∪–,فعولن فعولن فعولن فعل
-13,∪–∪–∪––∪–∪–∪––,مفاعلن فعولن مفاعلن فعولن
-9,–∪∪––∪––∪∪––∪–,مفتعلن فاعلن مفتعلن فاعلن
-8,–∪∪––∪∪––∪–,مفتعلن مفتعلن فاعلن
-8,–∪–––∪–––∪–––∪––,فاعلاتن فاعلاتن فاعلاتن فاعلاتن
-7,∪–∪–∪–∪–∪–∪–∪–∪–,مفاعلن مفاعلن مفاعلن مفاعلن
-7,–∪∪–∪–∪––∪∪–∪–∪–,مفتعلن مفاعلن مفتعلن مفاعلن
-6,∪––∪––∪––∪––,فعولن فعولن فعولن فعولن
-5,∪––∪∪––∪∪––∪∪––,مفاعیلُ مفاعیلُ مفاعیلُ فعولن
-3,∪∪–∪–∪∪–∪–∪∪–∪–∪∪–∪–,متفاعلن متفاعلن متفاعلن متفاعلن
-2,∪∪–∪–∪––∪∪–∪–∪––,فعلاتُ فاعلاتن فعلاتُ فاعلاتن
+Frequency,WeightPattern,Title
+1044,–∪–––∪–––∪–––∪–,فاعلاتن فاعلاتن فاعلاتن فاعلن
+999,∪–––∪–––∪–––∪–––,مفاعیلن مفاعیلن مفاعیلن مفاعیلن
+386,∪–––∪–––∪––,مفاعیلن مفاعیلن فعولن
+334,––∪∪––∪∪––∪∪––,مفعولُ مفاعیلُ مفاعیلُ فعولن
+272,––∪∪––∪∪––∪∪–,مفعولُ مفاعیلُ مفاعیلُ فعل
+213,––∪–∪–∪∪––∪–∪–,مفعولُ فاعلاتُ مفاعیلُ فاعلن
+138,∪∪––∪∪––∪∪––∪∪–,فعلاتن فعلاتن فعلاتن فعلن
+131,––∪∪–∪–∪––,مفعولُ مفاعلن فعولن
+62,–∪–––∪–––∪–,فاعلاتن فاعلاتن فاعلن
+45,∪∪––∪–∪–∪∪–,فعلاتن مفاعلن فعلن
+40,∪–∪–∪∪––∪–∪–∪∪–,مفاعلن فعلاتن مفاعلن فعلن
+31,––∪∪–––––∪∪–––,مفعولُ مفاعیلن مفعولُ مفاعیلن
+28,––∪–∪––––∪–∪––,مفعولُ فاعلاتن مفعولُ فاعلاتن
+20,∪∪––∪∪––∪∪–,فعلاتن فعلاتن فعلن
+19,––∪–––∪–––∪–––∪–,مستفعلن مستفعلن مستفعلن مستفعلن
+14,∪––∪––∪––∪–,فعولن فعولن فعولن فعل
+13,∪–∪–∪––∪–∪–∪––,مفاعلن فعولن مفاعلن فعولن
+9,–∪∪––∪––∪∪––∪–,مفتعلن فاعلن مفتعلن فاعلن
+8,–∪∪––∪∪––∪–,مفتعلن مفتعلن فاعلن
+8,–∪–––∪–––∪–––∪––,فاعلاتن فاعلاتن فاعلاتن فاعلاتن
+7,∪–∪–∪–∪–∪–∪–∪–∪–,مفاعلن مفاعلن مفاعلن مفاعلن
+7,–∪∪–∪–∪––∪∪–∪–∪–,مفتعلن مفاعلن مفتعلن مفاعلن
+6,∪––∪––∪––∪––,فعولن فعولن فعولن فعولن
+5,∪––∪∪––∪∪––∪∪––,مفاعیلُ مفاعیلُ مفاعیلُ فعولن
+3,∪∪–∪–∪∪–∪–∪∪–∪–∪∪–∪–,متفاعلن متفاعلن متفاعلن متفاعلن
+2,∪∪–∪–∪––∪∪–∪–∪––,فعلاتُ فاعلاتن فعلاتُ فاعلاتن
 2,∪–∪–∪∪––∪–∪–∪∪––,مفاعلن فعلاتن مفاعلن فعلاتن
```

### Comparing `asosoft-0.1.2/src/asosoft.egg-info/PKG-INFO` & `asosoft-0.1.3/src/asosoft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: asosoft
-Version: 0.1.2
+Version: 0.1.3
 Summary: AsoSoft's Library for Kurdish language processing tasks
 Home-page: https://github.com/AsoSoft/AsoSoft-Library-py
 Author: Aso Mahmudi
 Author-email: aso.mehmudi@gmail.com
 License: MIT
 Keywords: natural-language-processing,normalization,unicode-normalization,central-kurdish,kurdish,sorani
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # AsoSoft Library (Python)
 AsoSoft Library offers basic natural language processing (NLP) algorithms for the Kurdish Language (ckb: Central branch of Kurdish).
 AsoSoft Library is originally written in C# and this library is the Python port.
```

### Comparing `asosoft-0.1.2/src/asosoft.egg-info/SOURCES.txt` & `asosoft-0.1.3/src/asosoft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

