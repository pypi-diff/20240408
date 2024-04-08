# Comparing `tmp/dbis-exc-manager-0.3.2.tar.gz` & `tmp/dbis-exc-manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-exc-manager-0.3.2.tar", last modified: Tue Mar 26 09:52:55 2024, max compression
+gzip compressed data, was "dbis-exc-manager-0.4.0.tar", last modified: Mon Apr  8 13:21:59 2024, max compression
```

## Comparing `dbis-exc-manager-0.3.2.tar` & `dbis-exc-manager-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:52:55.651091 dbis-exc-manager-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1315 2024-03-26 09:52:55.651091 dbis-exc-manager-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-06 09:26:04.000000 dbis-exc-manager-0.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-03-26 09:48:19.000000 dbis-exc-manager-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 09:52:55.651091 dbis-exc-manager-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:52:55.647091 dbis-exc-manager-0.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:52:55.651091 dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1315 2024-03-26 09:52:55.000000 dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      434 2024-03-26 09:52:55.000000 dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 09:52:55.000000 dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2024-03-26 09:52:55.000000 dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-26 09:52:55.000000 dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:52:55.647091 dbis-exc-manager-0.3.2/src/excmanager/
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/src/excmanager/Task.py
--rw-rw-rw-   0 root         (0) root         (0)    10359 2023-12-22 08:49:38.000000 dbis-exc-manager-0.3.2/src/excmanager/Util.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/src/excmanager/Version.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/src/excmanager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/src/excmanager/scorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 09:52:55.651091 dbis-exc-manager-0.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/tests/test_Task.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/tests/test_Util.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-12-22 08:44:56.000000 dbis-exc-manager-0.3.2/tests/test_scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-06 09:26:04.000000 dbis-exc-manager-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-08 13:12:08.000000 dbis-exc-manager-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.149930 dbis-exc-manager-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/src/excmanager/
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/src/excmanager/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)    10376 2024-04-08 13:03:55.000000 dbis-exc-manager-0.4.0/src/excmanager/Util.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/src/excmanager/Version.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/src/excmanager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2024-04-08 13:03:55.000000 dbis-exc-manager-0.4.0/src/excmanager/scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/tests/test_Task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/tests/test_Util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/tests/test_scorer.py
```

### Comparing `dbis-exc-manager-0.3.2/LICENSE` & `dbis-exc-manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.3.2/PKG-INFO` & `dbis-exc-manager-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-exc-manager
-Version: 0.3.2
+Version: 0.4.0
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-exercise-manager
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-exc-manager-0.3.2/README.md` & `dbis-exc-manager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.3.2/pyproject.toml` & `dbis-exc-manager-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-exc-manager"
-version = "0.3.2"
+version = "0.4.0"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "DBIS i5 RWTH Aachen", email = "dbis-vl@dbis.rwth-aachen.de " },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-exc-manager-0.3.2/src/dbis_exc_manager.egg-info/PKG-INFO` & `dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-exc-manager
-Version: 0.3.2
+Version: 0.4.0
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-exercise-manager
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-exc-manager-0.3.2/src/excmanager/Task.py` & `dbis-exc-manager-0.4.0/src/excmanager/Task.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.3.2/src/excmanager/Util.py` & `dbis-exc-manager-0.4.0/src/excmanager/Util.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         local_filename = url.split("/")[-1]
         full_path = os.path.join(folder, local_filename)
         with requests.get(url, stream=True) as r:
             r.raise_for_status()
             with open(full_path, "wb") as f:
                 for chunk in r.iter_content(chunk_size=8192):
                     f.write(chunk)
-        print(f"Downloaded and placed file at {full_path}")
+        print(f"Lade herunter und speichere unter {full_path}")
         return local_filename
 
     @staticmethod
     def evaluate_sql(path_to_db, query, display_table=True):
         if not os.path.exists(path_to_db):
             raise FileNotFoundError()
         conn = sqlite3.connect(path_to_db)
@@ -63,37 +63,37 @@
     ):
         score = 0
         try:
             solution = {Util.str_sanitize(k): v for k, v in solution.items()}
             student_dict = {Util.str_sanitize(k): v for k, v in student_dict.items()}
             # check for exact match
             for x in solution:
-                print("checking columns: ", x, " | ", solution[x])
+                print("Überprüfe Spalte: ", x, " | ", solution[x])
                 for y in range(len(solution[x])):
-                    print("   checking cell:", y, " | ", solution[x][y])
+                    print("   Überprüfe Zelle:", y, " | ", solution[x][y])
                     check = Util.levenshtein_str_callback(
                         solution[x][y], student_dict[x][y]
                     )
                     if 0.8 <= check:
                         score += partial_score_exact
                     print("    > ", check, ", score: ", round(score, 4))
         except Exception as e:
-            print("exception caught, aborting")
+            print("Exception festgestellt")
             print(f"  {type(e).__name__} {e} ")
             if type(e).__name__ == "KeyError":
                 print(
-                    "  ... this error message likely means that a column name is misspelled or that a column was not found."
+                    "  ... diese Errormeldung bedeutet wahrscheinlich, dass eine Spalte fehlerhaft benannt wurde oder nicht gefunden wurde."
                 )
             pass  # catch, return
         else:
             # if the solution isn't exact, apply other rules
             # = check for keywords in SQL.
             if round(score, 2) < no_of_points:
                 score = 0
-                print("partial score")
+                print("Teilpunkte")
                 for i in partial_score_keywords:
                     if i in query_text.upper():
                         score += partial_score_points
         return score
 
     # count solution cells in result array
     @staticmethod
@@ -173,27 +173,27 @@
                 if new_ratio >= best_ratio:
                     best_ratio = new_ratio
                     best = j
             if best_ratio >= levenshtein_threshold:
                 res.insert(i, best)
                 if best_ratio < 1 and not quiet:
                     print(
-                        f"Found {elem_name} '{a[i]}', did you mean '{b[best]}'? Using this instead."
+                        f"Gefunden wurde {elem_name} '{a[i]}', verwendet wird '{b[best]}'?"
                     )
                 b[best] = None  # Mark as matched
             else:
                 if not quiet:
-                    print(f"Wrong {elem_name} '{a[i]}'")
+                    print(f"Fehlerhaft: {elem_name} '{a[i]}'")
                 error = True
 
         # Check if all items have been used, if not, it was missing in student's solution
         for j in range(0, len(b)):
             if b[j] != None:
                 if not quiet:
-                    print(f"Missing {elem_name} '{b[j]}'")
+                    print(f"Fehlend: {elem_name} '{b[j]}'")
                 error = True
         if error:
             return None
         return res
 
     @staticmethod
     def str_sanitize(s: str) -> str:
```

### Comparing `dbis-exc-manager-0.3.2/src/excmanager/scorer.py` & `dbis-exc-manager-0.4.0/src/excmanager/scorer.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,23 +58,23 @@
         amountstr = (
             f"{frac.numerator}/{frac.denominator}"
             if frac.denominator > 1
             else f"{frac.numerator}"
         )
         if problem is not None:
             if negativeOnProblem:
-                msg = f"subtracting {amountstr}"
+                msg = f"Ziehe ab: {amountstr}"
                 self.score -= amount
             else:
-                msg = f"no score"
-            self.feedback(f"{msg} for {check} due to {problem}", positive=False)
+                msg = f"Keine Punkte"
+            self.feedback(f"{msg} für {check} wegen: {problem}", positive=False)
             return
         else:
             self.score += amount
-            self.feedback(f"adding {amountstr} to score for {check}", positive=True)
+            self.feedback(f"Füge {amountstr} Punkte hinzu für: {check}", positive=True)
 
 
 class MultipleChoiceScorer(Scorer):
     """
     scorer for multiple choice questions
 
     Für jede richtige Antwort gibt es 1/𝑛 Punkte.
@@ -86,17 +86,17 @@
     def evaluate_mctask(self, result, correct, max_points, toManyEquals0: bool):
         """
         evaluate the given multiple choice task results
         """
         amount = max_points / len(correct)
         for ans in result:
             problem = None
-            check = f"check {ans}"
+            check = f"Überprüfung Antwort {ans}"
             if not ans in correct:
-                problem = f" is incorrect"
+                problem = f" Ist falsch"
             self.addScore(amount, check, problem, negativeOnProblem=True)
         # Bei zu vielen angegebenen Antworten mehr falschen als richtigen Antworten: 0 Punkte
         if self.score < 0 or (len(result) > len(correct) and toManyEquals0 == True):
             self.score = 0
         return self.score
 
 
@@ -114,15 +114,15 @@
     Wenn Sie also mehr falsche als richtige Antworten auswählen, gibt es insgesamt keine Minuspunkte.
     """
 
     def evaluate_set(self, result, expected, max_points):
         amount = max_points / len(expected)
         for ans in result:
             problem = None
-            check = f"check {ans}"
+            check = f"Überprüfung {ans}"
             if not ans in expected:
-                problem = f" is incorrect"
+                problem = f"Ist fehlerhaft"
             self.addScore(amount, check, problem, negativeOnProblem=True)
         # Bei zu vielen angegebenen Antworten mehr falschen als richtigen Antworten: 0 Punkte
         if self.score < 0:
             self.score = 0
         return self.score
```

### Comparing `dbis-exc-manager-0.3.2/tests/test_Task.py` & `dbis-exc-manager-0.4.0/tests/test_Task.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.3.2/tests/test_Util.py` & `dbis-exc-manager-0.4.0/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.3.2/tests/test_scorer.py` & `dbis-exc-manager-0.4.0/tests/test_scorer.py`

 * *Files identical despite different names*

