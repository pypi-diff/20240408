# Comparing `tmp/autoanki-1.1.6.tar.gz` & `tmp/autoanki-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.1.6.tar", last modified: Fri Apr  5 18:21:02 2024, max compression
+gzip compressed data, was "autoanki-1.1.7.tar", last modified: Sun Apr  7 23:12:41 2024, max compression
```

## Comparing `autoanki-1.1.6.tar` & `autoanki-1.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.805143 autoanki-1.1.6/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.6/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.6/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     4826 2024-04-05 18:21:02.805055 autoanki-1.1.6/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     4293 2024-04-05 17:17:58.000000 autoanki-1.1.6/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.6/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-05 18:21:02.805456 autoanki-1.1.6/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.798447 autoanki-1.1.6/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.799871 autoanki-1.1.6/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     5486 2024-04-05 18:12:11.000000 autoanki-1.1.6/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.802452 autoanki-1.1.6/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7294 2024-04-05 15:59:59.000000 autoanki-1.1.6/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.6/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.803470 autoanki-1.1.6/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13046 2024-04-05 16:28:43.000000 autoanki-1.1.6/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.6/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.6/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.6/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.6/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.803932 autoanki-1.1.6/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     3362 2024-04-05 18:08:57.000000 autoanki-1.1.6/src/autoanki/DeckManager/DeckManager.py
--rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.6/src/autoanki/DeckManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)     2676 2024-04-05 16:28:54.000000 autoanki-1.1.6/src/autoanki/DeckManager/template_decks.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.804559 autoanki-1.1.6/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     3221 2024-04-05 18:18:47.000000 autoanki-1.1.6/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-05 16:04:00.000000 autoanki-1.1.6/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5561 2024-03-31 20:00:33.000000 autoanki-1.1.6/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.6/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.6/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:21:02.804777 autoanki-1.1.6/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     4826 2024-04-05 18:21:02.000000 autoanki-1.1.6/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      878 2024-04-05 18:21:02.000000 autoanki-1.1.6/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-05 18:21:02.000000 autoanki-1.1.6/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.6/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-05 18:21:02.000000 autoanki-1.1.6/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.601729 autoanki-1.1.7/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.7/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.7/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     4836 2024-04-07 23:12:41.601662 autoanki-1.1.7/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     4303 2024-04-05 18:36:02.000000 autoanki-1.1.7/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.7/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-07 23:12:41.602012 autoanki-1.1.7/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.593366 autoanki-1.1.7/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.594681 autoanki-1.1.7/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     6488 2024-04-07 23:12:30.000000 autoanki-1.1.7/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.597349 autoanki-1.1.7/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     7249 2024-04-07 18:35:54.000000 autoanki-1.1.7/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.598800 autoanki-1.1.7/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13764 2024-04-07 20:46:36.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.599676 autoanki-1.1.7/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     4175 2024-04-07 18:11:20.000000 autoanki-1.1.7/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.7/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     2676 2024-04-06 21:14:34.000000 autoanki-1.1.7/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.600967 autoanki-1.1.7/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     4390 2024-04-07 20:47:34.000000 autoanki-1.1.7/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-05 16:04:00.000000 autoanki-1.1.7/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5320 2024-04-07 04:26:04.000000 autoanki-1.1.7/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.7/src/autoanki/Dictionary/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.7/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.601398 autoanki-1.1.7/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     4836 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      878 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.7/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.1.6/LICENSE.txt` & `autoanki-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.6/PKG-INFO` & `autoanki-1.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.6
+Version: 1.1.7
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,36 +19,36 @@
 # autoanki
 Tool for generating Anki flashcards to learn Chinese.
 
 <img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
 
 ## Motivation
 
-When learning Chinese, advice is to learn the top X most common words.
+When learning Chinese, some common advice is to learn the top X most common words.
 This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
 For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
-With autoanki, you selectivley add words to an Anki file to continue progressing with your lanuage learning skills.
+With autoanki, you selectively add words to an Anki file to continue progressing with your lanuage learning skills.
 
 ## Usage
 
 autoanki is both a library and a command-line tool.
 
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
 
 To get started, first, create a database for autoanki to use 
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
-    AutoAnki.create_autoanki_db(db_path)
+    AutoAnki.create_database(db_path)
 ```
 Then create an instance of autoanki using the database
 ```
 aa = AutoAnki(db_path)
 ```
 Add whatever books you want in your deck. These can be a single file, or a folder
 ```
@@ -118,7 +118,8 @@
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
 To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence. 
+
```

### Comparing `autoanki-1.1.6/README.md` & `autoanki-1.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 # autoanki
 Tool for generating Anki flashcards to learn Chinese.
 
 <img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
 
 ## Motivation
 
-When learning Chinese, advice is to learn the top X most common words.
+When learning Chinese, some common advice is to learn the top X most common words.
 This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
 For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
-With autoanki, you selectivley add words to an Anki file to continue progressing with your lanuage learning skills.
+With autoanki, you selectively add words to an Anki file to continue progressing with your lanuage learning skills.
 
 ## Usage
 
 autoanki is both a library and a command-line tool.
 
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
 
 To get started, first, create a database for autoanki to use 
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
-    AutoAnki.create_autoanki_db(db_path)
+    AutoAnki.create_database(db_path)
 ```
 Then create an instance of autoanki using the database
 ```
 aa = AutoAnki(db_path)
 ```
 Add whatever books you want in your deck. These can be a single file, or a folder
 ```
@@ -103,7 +103,8 @@
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
 To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence. 
+
```

### Comparing `autoanki-1.1.6/setup.cfg` & `autoanki-1.1.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.1.6
+version = 1.1.7
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls =
```

### Comparing `autoanki-1.1.6/src/autoanki/AutoAnki.py` & `autoanki-1.1.7/src/autoanki/AutoAnki.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from autoanki.Dictionary.YellowBridgeDictionary import YellowBridgeDictionary
+
 from .BookCleaner import BookCleaner
 from .DatabaseManager import DatabaseManager
 from .Dictionary import CEDictionary
 from .DeckManager import DeckManager
 
 BLACK = "\u001b[30m"
 RED = "\u001b[31m"
@@ -13,15 +15,15 @@
 MAGENTA = "\u001b[35m"
 CYAN = "\u001b[36m"
 WHITE = "\u001b[37m"
 RESET = "\u001b[0m"
 logging.basicConfig(
     # filename='HISTORY.log',
     level=logging.WARNING,
-    format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)18s{RESET}: %(message)s',
+    format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)16s{RESET}: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 
 class AutoAnki:
 
     def __init__(self, database_filepath='autoanki.db', debug_level=20):
         """
@@ -33,34 +35,35 @@
         self.logger = logging.getLogger('autoanki')
         self.logger.setLevel(debug_level)
         self.logger.debug(f"logger active")
         self.logger.info("Connecting to database...")
 
         self.book_cleaner = BookCleaner(debug_level)
 
+        self.dictionary = CEDictionary(debug_level)
+        self.online_dictionary = YellowBridgeDictionary(debug_level)
+
         self.database_filepath = database_filepath
         if not DatabaseManager.is_database(database_filepath):
             self.logger.info("Creating database...")
-            DatabaseManager.create_autoanki_db(database_filepath)
+            DatabaseManager.create_database(database_filepath)
             self.logger.info("Done creating database.")
         self.database_manager = DatabaseManager(database_filepath, debug_level)
 
-        self.dictionary = CEDictionary(debug_level)
         self.deck_manager = DeckManager(debug_level)
 
         self.logger.info("Connected!")
 
     def add_book(self, book_path: str, book_name: str = 'New Book'):
         """
         Add a directory full of files to the database
         :param book_path: The filepath to the directory that contains the files to add. e.g. lost_prince.txt
         :param book_name: The name of the book being added e.g. "Lost Prince"
         :return:
         """
-
         self.logger.debug(f"autoanki: Adding book from [{book_path}]")
 
         # Clean the book
         if not self.book_cleaner.clean(book_path):
             # logger.warning("autoanki: Unable to clean book [" + book_name + "].")
             return
 
@@ -70,56 +73,82 @@
             return
 
         self.logger.info("autoanki: Added [" + book_path + "].")
 
     def complete_unfinished_definitions(self):
         """
         autoanki contains an internal definitions table that is scraped from the internet. As words are added to
-        autoanki, their definitions must be found. This function passively finds definitions and adds them to the table
+        autoanki, their definitions must be found.
+        This function passively finds definitions and adds them to the table
         :return: None
         """
 
         # TODO Make progress bar for unfinished records
         self.logger.info("Checking for records...")
         self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         response_rows = self.database_manager.cursor.fetchall()
-        #while len(response_rows) > 0:
-        self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
-        response_rows = self.database_manager.cursor.fetchall()
         if len(response_rows) > 0:
             self.logger.info("Adding " + str(len(response_rows)) + " rows to dictionary table")
             for row in response_rows:
                 word = row[0]
 
-                self.logger.debug(f"Finding: [{word}]...")
+                # self.logger.debug(f"Finding: [{word}]...")
+
+                # self.logger.debug("Trying local dictionary...")
                 params = self.dictionary.find_word(word)
-                if not params:
-                    self.logger.debug(f"❌Could not find: [{word}]")
-                else:
-                    self.logger.debug(f"✅Found: [{word}]")
+                if params:
+                    # self.logger.debug(f"✅Found: [{params[8]}]")
                     self.database_manager.update_definition(params)
+                    continue
+
+                # self.logger.debug("Trying YellowBridge...")
+                # params = self.online_dictionary.find_word(word)
+                # if params:
+                    # self.logger.debug(f"✅Found: [{word}]")
+                    # self.database_manager.update_definition(params)
+                    # continue
+
+                self.logger.info(f"❌Could not find: [{word}]")
 
         else:
             self.logger.info("No new rows to complete in dictionary table")
-            # time.sleep(2)
+
+    def deck_settings(self,
+                      inclue_traditional = True, 
+                      inclue_part_of_speech = True, 
+                      ):
+        """
+        Configures settings for what's in the deck, and how it looks
+        """
+
+
+        self.deck_manager.settings(
+            inclue_traditional,
+            inclue_part_of_speech, 
+        )
+
+
+        pass
 
     def print_database_info(self):
         self.database_manager.print_info()
 
     @staticmethod
     def is_database(db_path):
         return DatabaseManager.is_database(db_path)
 
     @staticmethod
-    def create_autoanki_db(db_path: str):
-        DatabaseManager.create_autoanki_db(db_path)
+    def create_database(db_path: str):
+        DatabaseManager.create_database(db_path)
 
     def create_deck(self, deck_name: str, filepath: str):
         """
         Creates a deck file in the directory of the main file.
+        `deck_name` The name that will show up in Anki
+        `filepath` Path to the file
         :return:
         """
 
         self.logger.info("Generating deck file [" + deck_name + ".apk]")
         words = self.database_manager.get_all_completed_definitions()
 
         deck_path = self.deck_manager.generate_deck_file(words, deck_name, filepath)
@@ -147,9 +176,17 @@
     @unfinished_entries.setter
     def unfinished_entries(self, _):
         pass
 
 
 if __name__ == '__main__':
 
+    # This is where the command line tool will be put
+    # Parse args
+    # parser = argparse.ArgumentParser(description='This is a new command-line tool')
+
+    # Input files
     aa = AutoAnki()
+
+    # Output deck
+    # aa.create_deck()
     print(aa.book_list)
```

### Comparing `autoanki-1.1.6/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.1.7/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,9 @@
 import logging
 import os
-# import shutil
-# import glob
-# from pathlib import Path
-#
-# from selenium.webdriver import ActionChains
-# from selenium.webdriver.common.by import By
-#
-# from selenium import webdriver
-# from os.path import isfile, join
-# import time
-# MAX_TXT_TO_PINYIN_SIZE = 270000
 
 CLEANED_FILES_DIRECTORY = 'cleaned_files'
 CLEANED_FILES_SUFFIX = '_cleaned'
 # Sentences That should not be added to the completed file.
 GARBAGE_SENTENCES = ['',
                      "",
                      "。",
@@ -75,33 +64,35 @@
 
         for file in dirty_files:
             cleaned_filepath = self._clean_file(file, cleaned_files_root=cleaned_files_root)
             cleaned_files.append(cleaned_filepath)
 
         return cleaned_files
 
-    @staticmethod
-    def _clean_file(filepath, cleaned_files_root):
+    def _clean_file(self, filepath, cleaned_files_root):
         """
         Takes a txt file and cleans it up, putting every sentence on a new line
         :param filepath: The txt file to clean
         :param cleaned_files_root: The root
         :return:
         """
-
         # Set the directory where the cleaned file will go
         if not cleaned_files_root:
             # root/test1.txt -> root/hello_cleaned.txt
             new_filepath = os.path.splitext(filepath)[0] + CLEANED_FILES_SUFFIX + os.path.splitext(filepath)[1]
         else:
-            new_filepath = os.path.join(cleaned_files_root, '/'.join(filepath.split('/')[1:]))
+            # TODO I'm suspicious that this works every time
+            new_filepath = os.path.join(cleaned_files_root, '/'.join(filepath.split('/')[2:]))
+        # self.logger.debug(f"Old filepath: [{filepath}]")
+        # self.logger.debug(f"New filepath: [{new_filepath}]")
 
         # Clean page file of characters that may cause issues.
         page_file = open(filepath, encoding='utf-8')
         page_sentences = page_file.read().split("。")
+        # f = open("test.txt", "w", encoding='utf-8')
         cleaned_file = open(new_filepath, "w", encoding='utf-8')
 
         for page_sentence in page_sentences:
             # Clean string
             page_sentence = page_sentence\
                 .lstrip()\
                 .rstrip()\
```

### Comparing `autoanki-1.1.6/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.1.7/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import os
-import pprint
+from string import punctuation
 import re
 import sqlite3
 import logging
 import unicodedata
+from glob import glob
 
 from pathlib import Path
 import jieba
+import chinese_converter
 
-FILTERED_WORDS = [
-    '\n',
-    ' ',
-    '。',
-    '"',
-    "‘",
-    "’",
-    "“",
-    "”",
-    "，",
-    "、",
-    "·",
-]
+from autoanki.BookCleaner.BookCleaner import CLEANED_FILES_DIRECTORY
+
+CHINESE_PUNC = "！？｡。＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏."
+PUNC = "™∞•◎ "
 
 class DatabaseManager:
 
     def __init__(self, database_path, debug_level):
         self.logger = logging.getLogger('autoanki.dbmngr')
         self.logger.setLevel(debug_level)
         if not os.path.exists(database_path):
@@ -62,15 +55,15 @@
             cursor.execute("SELECT word FROM dictionary")
             connection.close()
         except sqlite3.OperationalError:
             return False
         return True
 
     @staticmethod
-    def create_autoanki_db(database_path):
+    def create_database(database_path):
         """
         Creates an autoanki database file, including all tables needed for autoanki
         `database_path` The path to the database to create
         """
         logger = logging.getLogger('autoanki.dbmngr')
         logger.info("Creating database [" + database_path + "]")
         path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
@@ -119,49 +112,54 @@
         Adds every word in a file to both the dictionary table and the book's table
         `filepath` The path to the file
         `table_name` The name of the table to add the words to.
             This should be the same for every wile in a given book
         """
         self.logger.info(f"Adding file {filepath} to database...")
 
-        # Get number of appearances for each word in the file, and put it into a dictionary
+
         word_appearances = {}
-        # As we add words to the definitions table, get the id. This is for the book table
-        word_ids = {}
         with open(filepath,'r',encoding='utf-8') as f:
             line = " "
             while line:
                 line = f.readline()
-                if line:
-                    # print("Line: ", line)
-                    tokenized_line = jieba.lcut(line)
-                    # print("Tokenized line: ", tokenized_line)
-                    for word in tokenized_line:
-
-                        is_ascii = len(word) == len(word.encode())
-                        if word not in FILTERED_WORDS and not is_ascii:
-                            # print("Word: ",word)
-                            if word_appearances.get(word) == None:
-                                word_appearances[word] = 1
-                            else:
-                                word_appearances[word] += 1
+                if not line:
+                    continue
+                words = jieba.lcut(line)
+                for word in words:
+
+                    # Remove puncuation
+                    word = word.translate(str.maketrans('', '', punctuation))
+
+                    is_ascii = len(word) == len(word.encode())
+
+                    is_ascii_special = False
+                    if len(word) == 1:
+                        is_ascii_special = ord(word[0]) > 128 and ord(word[0]) < 255 
+
+                    if word in PUNC or word in CHINESE_PUNC or is_ascii or is_ascii_special or word is None:
+                        continue
+                    if word_appearances.get(word) == None:
+                        # Convert the word to simplified if needed
+                        word = chinese_converter.to_simplified(word)
+                        word_appearances[word] = 1
+                    else:
+                        word_appearances[word] += 1
+
 
-        self.logger.info(f"Found {str(len(word_appearances.items()))} words in file.")
 
         # Add the words to the dictionary if they are not already there
         self.cursor.execute(f"SELECT word FROM dictionary")
         self.connection.commit()
         dictionary_words = self.cursor.fetchall()
-
-        self.logger.info(f"Found {str(len(dictionary_words))} words in dictionary.")
+        self.logger.info(f"{len(word_appearances.items())} words in file. {len(dictionary_words)} in dictionary.")
 
         for word, appearances in word_appearances.items():
             if (word,) not in dictionary_words:
                 # self.logger.debug("Adding word...")
-
                 self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
                 self.connection.commit()
 
         # Make a dictionary of word ids from dictionary
         self.cursor.execute(f"SELECT word_id, word FROM dictionary")
         result = self.cursor.fetchall()
         word_id_dict = {}
@@ -182,27 +180,27 @@
 
             dictionary_word_id = word_id_dict[word]
 
             # If the word is already in the dictionary, add the number of appearances to it
             if dictionary_word_id in book_table_appearances:
                 file_appearances = word_appearances[word]
                 db_appearances = book_table_appearances[dictionary_word_id]
-                print("File app:", file_appearances)
-                print("Book app:", book_table_appearances[dictionary_word_id])
+                # print("File app:", file_appearances)
+                # print("Book app:", book_table_appearances[dictionary_word_id])
                 sum = file_appearances + db_appearances
                 self.cursor.execute(f"UPDATE {table_name} SET number_of_appearances = ? "
                                     f"WHERE dictionary_word_id = ?", [sum, dictionary_word_id])
                 self.connection.commit()
 
             else:
                 self.cursor.execute(f"INSERT INTO {table_name} (dictionary_word_id, number_of_appearances) "
                                     f"VALUES (?,?)", [dictionary_word_id, word_appearances[word]])
                 self.connection.commit()
 
-        self.logger.info("Done adding file to database")
+        # self.logger.debug("Done adding file to database")
 
     def add_book(self, bookpath: str, book_name: str):
         """
         Adds a file to the autoanki database. This involves the following steps:\n
         1 - Add book to the book_list table
         2 - Add all the files in "bookpath" to the definitions table and book table
         3 - Add book to book_list property
@@ -210,32 +208,41 @@
         If given a directory, it will recursively search for all files in the directory and add them.
 
         if not already there, adding the
         :param bookpath: The filepath to the book. This is file, or a directory of files
         :param book_name: The name of the book. This will show up in the Anki deck
         :return: None
         """
-        # TODO Make this work for multiple files. Right now only works for one filepath
         self.logger.info("Adding book...")
+
         # Gets a 'table name' clean version of the book name
         book_tablename = self.convert_to_tablename(book_name)
 
         # Add the name of the book to the book_list table
         success = self._create_book_table(book_name, book_tablename)
         if not success:
             self.logger.error("Failed to create book table")
             return
 
-        # Add all the words in the book to the 'definitions' table
-        self.add_file_to_database(bookpath, book_tablename)
+        self.logger.debug(bookpath)
+        if os.path.isdir(bookpath):
+            self.logger.debug("Directory found:")
+            result = [y for x in os.walk(bookpath + '/' + CLEANED_FILES_DIRECTORY) for y in glob(os.path.join(x[0], '*.txt'))]
+            for path in result:
+                self.logger.debug(path)
+                self.add_file_to_database(path, book_tablename)
+
+        elif os.path.isfile(bookpath):
+            self.logger.debug("File found:")
+            # Add all the words in the book to the `definitions` table
+            self.add_file_to_database(bookpath, book_tablename)
 
-        # # Add all the words in the bookpath to a new table with the name of the book.
-        # success = self.add_book_table_to_db(bookpath, table_book_name)
-        # if success is False:
-        #     return
+        else:
+            self.logger.warning(f"Incorrect bookpath: [{bookpath}]")
+            return False
 
         self.logger.info("Done adding book.")
         return True
 
     def print_info(self):
         """
         Print basic information about the database
@@ -267,15 +274,16 @@
         hsk_level = params[5]\n
         top_level = params[6]\n
         definition = params[7]\n
         word = params[8]
         :param params: A list of params for the database:
         :return:
         """
-
+        # TODO Some sanatization here might be a good idea
+        #   Make sure junk data can't crash this function
         self.cursor.execute("UPDATE dictionary "
                             "SET word_traditional = ?, "
                             "word_type = ?,"
                             "pinyin = ?, "
                             "pinyin_numbers = ?,"
                             "sub_components = ?,"
                             "hsk_level = ?,"
```

### Comparing `autoanki-1.1.6/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.1.7/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.6/src/autoanki/DeckManager/DeckManager.py` & `autoanki-1.1.7/src/autoanki/DeckManager/DeckManager.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,41 @@
     The class to make anki decks. Create the file using generate_deck_file()
     One of the most important concepts is the id. No matter what deck the word is in, it should have the same id so the
     same card in different decks can be remembered.
     This class makes extensive use of genanki, so understanding how genanki works
         is pretty significant for understanding this.
     """
 
-    def __init__(self, debug_level):
+    def __init__(self, debug_level,
+                include_traditional=True,
+                 include_part_of_speech=True
+                 ):
         self.logger = logging.getLogger('autoanki.dckmngr')
         self.logger.setLevel(debug_level)
         self.deck = genanki.Deck(
             2020000110,
             "autoankiTesting"
         )
         self.include_pinyin_numbers = False
         self.include_number_of_strokes = False
+        self.include_traditional = include_traditional 
+        self.include_part_of_speech = include_part_of_speech
 
         self.book_list = []
 
+    def settings(self,
+                 include_traditional,
+                 include_part_of_speech
+                 ):
+        """
+        Configures settings for what's in the deck, and how it looks
+        """
+        self.include_traditional = include_traditional
+        self.include_part_of_speech = include_part_of_speech 
+
     def generate_deck_file(self, words, deck_name: str, filename: str):
         """
         Generates a deck file from the database
         :param deck_name: The name of the deck to be created
         :param definitions_filename: The name of the file containing the definitions.
         :return:
         """
@@ -43,17 +58,24 @@
         self.deck = genanki.Deck(
             2020000110,
             deck_name
         )
 
         for row in words:
             word = row["word"]
-            word_traditional = row["word_traditional"]
+
+            if self.include_traditional:
+                word_traditional = row["word_traditional"]
+            else:
+                word_traditional = ""
+
+            if len(word) != len(word_traditional):
+                self.logger.error(f"{word} and {word_traditional} should be the same length")
             if word_traditional == word:
-                word_traditional = "-"
+                word_traditional = "-"*len(word)
             if row["pinyin"]:
                 pinyin = row["pinyin"]
             else:
                 pinyin = row["pinyin_numbers"]
             definition = "<br>" + row["definition"]
             # word["word_id"]
             # word["word"]
```

### Comparing `autoanki-1.1.6/src/autoanki/DeckManager/template_decks.py` & `autoanki-1.1.7/src/autoanki/DeckManager/template_decks.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.6/src/autoanki/Dictionary/CEDictionary.py` & `autoanki-1.1.7/src/autoanki/Dictionary/CEDictionary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,145 @@
 from .Dictionary import Dictionary
 from os import path
-import re
 import logging
-from pprint import pprint
+import pinyin
+
+import jieba
+import jieba.posseg as pseg
+import chinese_converter
 
 PATH_TO_FILE = path.join(path.dirname(__file__), 'cedict_ts.u8')
 
+#   Use the lookup table here: https://github.com/fxsjy/jieba
+POS_LUT = {
+    'n':'noun',
+    'nt':'noun',
+    'nrt':'noun',
+    'ORG':'noun',
+    'nr':'noun',
+    'PER':'noun',
+    'ns':'noun',
+    'nw':'noun',
+    'nz':'noun',
+    'f':'noun',
+    's':'noun',
+    'an':'noun',
+    't':'time',
+    'TIME':'time',
+    'p':'adposition',
+    'r':'pronoun',
+    'q':'quantifier',
+    'm':'quantifier',
+    'v':'verb',
+    'vd':'verb',
+    'vn':'verb',
+    'a':'adjective',
+    'ad':'adverb',
+    'd':'adverb',
+    'c':'conjunction',
+    'u':'particle',
+    'vn':'other',
+    'xc':'other',
+    'x':'other',
+    'w':'puncuation',
+}
+
 class CEDictionary(Dictionary):
 
     def __init__(self, debug_level):
         """Chinese to English Dictionary
 
         """
         self.logger = logging.getLogger('autoanki.cedict')
         self.logger.setLevel(debug_level)
+        self.logger.info("Loading Chinese Dictionary")
         self.dict = self._parse_file()
+        self.logger.info("Done!")
         
         pass
 
     def _parse_file(self) -> dict[str, dict]:
-        self.logger.info("Parsing dict file...")
+        self.logger.info("Parsing file...")
         if not path.isfile(PATH_TO_FILE):
             self.logger.critical("Could not open dictionary file")
 
         # TODO Some entries use a dot in the midde
         #   e.g. 哈利·波特
         #   this does not currently match
         definitions = {}
-        last_word = "~~"
+        last_word = "~"
         current_word = ""
 
         with open(PATH_TO_FILE, "r") as dict_file:
             for line in dict_file:
                 if line[0] == '#':
                     continue
                 parts = line.split(" ")
                 trad_word = parts[0]
                 current_word = parts[1]
-                
-                m = re.compile(r"\[[^]]*\]")
-                match = m.findall(line)
-                # self.logger.debug(match)
-                pinyin_numbers = match[0]
 
                 definition = line[line.find("]")+2:]
 
                 if current_word != last_word:
                     # self.logger.debug(f"Creating entry: {current_word}")
-                    definitions[current_word] = {'trad_word': "", 'pinyin_numbers':"", 'definition':""}
+                    definitions[current_word] = {
+                        'trad_word': "", 
+                        'pinyin_numbers':"", 
+                        'definition':"", 
+                        'pinyin':""
+                    }
                 
-                # self.logger.debug(f"Word: {current_word}")
-                # self.logger.debug(f"Trad: {trad_word}")
-                # self.logger.debug(f"PinYin: {pinyin_numbers}")
-                # self.logger.debug(f"DEF: {definition}")
-                definitions[current_word]['trad_word'] = trad_word
-                definitions[current_word]['pinyin_numbers'] += '<br>' + pinyin_numbers 
-                definitions[current_word]['definition'] += '<br>' + definition 
+                # These only need to be done the first time the word is seen
+                if last_word != current_word:
+                    definitions[current_word]['trad_word'] = trad_word
+                    definitions[current_word]['pinyin'] = pinyin.get(current_word)
+                    definitions[current_word]['pinyin_numbers'] = pinyin.get(current_word, format="numerical")
+
 
+                definitions[current_word]['definition'] += '<br>' + definition 
                 last_word = current_word
 
-        self.logger.info("Done!")
-        for key, value in definitions.items():
+        for key, _ in definitions.items():
             definitions[key]['definition'].strip('\n')
-            # print(key, '->', value)
         return definitions
 
 
     def find_word(self, word: str) -> None | list[str]:
+        """
+        Find a word in the dictionary. This can be simplified, or traditional
+        `return` Paramaters that get passed to the database
+        """
+        
+        # Convert the word to simplified if needed
+        word = chinese_converter.to_simplified(word)
 
         if word in self.dict:
             """
             traditional_script = params[0]\n
             word_type = params[1]\n
             pinyin = params[2]\n
             pinyin_numbers = params[3]\n
             sub_components = params[4]\n
             hsk_level = params[5]\n
             top_level = params[6]\n
             definition = params[7]\n
             word = params[8]
             """
             params = ["", "", "", "", "", "", "", "", ""]
+
+            slice = next(pseg.cut(word))
+            part_of_speech = POS_LUT.get(slice.flag)
+            if part_of_speech != None:
+                params[1] = part_of_speech
+
             params[0] = self.dict[word]['trad_word'] 
+            params[2] = self.dict[word]['pinyin'] 
             params[3] = self.dict[word]['pinyin_numbers'] 
             params[7] = self.dict[word]['definition'] 
+            self.logger.debug(f"Word: {word}")
             params[8] = word
             return params
         else:
             return None 
 
 
     def size(self):
```

### Comparing `autoanki-1.1.6/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.1.7/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,125 @@
 import logging
 import time
 import urllib
 
 import requests
+import selenium
+from selenium import webdriver
 from bs4 import BeautifulSoup
 import urllib.parse
 import pinyin as pin_to_num
 
 from .Dictionary import Dictionary
 
-logger = logging.getLogger('autoanki')
-# logger.setLevel()
-
-
 class YellowBridgeDictionary(Dictionary):
 
-    def __init__(self):
-        pass
+    def __init__(self, debug_level):
+        self.logger = logging.getLogger('autoanki.ybdict')
+        self.logger.setLevel(debug_level)
+        self.logger.debug(f"logger active")
+        self.logger.info("Loading Yellowbridge...")
 
     def find_word(self, word, cache_number=None):
         '''
         Helper function for complete_unfinished_dictionary_records() Takes a word (one or more characters),
         finds them on YellowBridge, and adds them to the dictionary
         :param word: The word to find on YellowBridge.
         :param cache_number: The secondary page number for a word with multiple definitions. (See comments in body of
         function)
         :return:
         '''
-        print(repr(word))
         if word == None or word == '':
-            print("There is no page on Yellowbridge page for null")
             return
 
+        self.logger.debug("Finding: " + repr(word))
+
         urlx = "http://www.yellowbridge.com/chinese/dictionary.php?word="
         url = urlx + urllib.parse.quote(word)
         if cache_number is not None:
             url += "&cache=" + cache_number
 
-        response = requests.get(url, headers={
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36'})
-        yellowbridge_soup = BeautifulSoup(response.content, "html.parser")
-
-        body = yellowbridge_soup.find(id='tabbody')
+        driver = webdriver.Chrome()
+        response = driver.get(url)
+        html = driver.page_source
+        # response = requests.get(url, headers={ 'user-agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36'})
+        yellowbridge_soup = BeautifulSoup(html, "html.parser")
         main_data = yellowbridge_soup.find(id='mainData')
+        self.logger.debug(yellowbridge_soup)
+
         # Some definitions will show up on the page differently because they have multiple meanings/pronunciations
-        # e.g 了 could be le or liao.
-        # These pages actually link to other pages with a different 'cache' number
+        # These pages link to other pages with a different 'cache' number
         # Default 了 page:
         # https://www.yellowbridge.com/chinese/dictionary.php?word=%E4%BA%86
         # Page for le:
         # https://www.yellowbridge.com/chinese/dictionary.php?word=%E4%BA%86&cache=5114
         # Page for laio:
         # https://www.yellowbridge.com/chinese/dictionary.php?word=%E4%BA%86&cache=5115
-        # This means that it would have to be possible to have multiple rows in the dictionary with the same word column,
-        # which breaks other parts of the code.
-        # For now, we just grab the first cache number and use that one. Maybe a v2 FEATURE will be able to have multiple
-        # definitions for the same character, but that is not a priority currently
-        if main_data:
-            yellowbridge_contains_exact_definition = True
-        else:
-            yellowbridge_contains_exact_definition = False
-        if yellowbridge_contains_exact_definition:
-            definition = simplified_script = traditional_script = pinyin = pinyin_num = part_of_speech = hsk_level = top_level = composing_words = None
-            main_data = main_data.find_all('tr')
-            # Collect all necessary information from the page:
-            for row in main_data:
-                row_info_type = row.find('td').getText()
-                row_info = row.find_all('td')[1].getText()
-                # print(row_info_type + ":")
-                # print(row_info)
-                if row_info_type == "English Definition":
-                    definition = row_info
-                elif row_info_type == "Simplified Script":
-                    simplified_script = row_info
-                elif row_info_type == "Traditional Script":
-                    traditional_script = row_info.split("P")[0]
-                elif row_info_type == "Pinyin":
-                    pinyin = row_info
-                    pinyin_num = pin_to_num.get(word, format="numerical")
-                elif row_info_type == "Part of Speech":
-                    part_of_speech = row_info
-                elif row_info_type == "Proficiency Test Level":
-                    proficiency_level = row_info
-                    if "HSK=" in proficiency_level:
-                        hsk_level = proficiency_level.split("HSK=")[1].split(";")[0]
-                    if "TOP=" in proficiency_level:
-                        top_level = proficiency_level.split("TOP=")[1].split(";")[0]
-
-            word_decomposition_soup = yellowbridge_soup.find(id='wordDecomp')
-            if len(word) > 1:
-                composing_words_list = word_decomposition_soup.find_all('tr')
-                composing_words = ""
-                for composing_word in composing_words_list:
-                    composing_words += str(composing_word.find_all('td')[0].find('a').getText()) + ";"
-
-            # This is all of the information that has been collected
-            # print([definition, simplified_script, traditional_script,pinyin,pinyin_num, part_of_speech,hsk_level,top_level,composing_words])
-            params = [traditional_script, part_of_speech, pinyin, pinyin_num,
-                      composing_words, hsk_level, top_level, definition, word]
-            # Add the information for this word to the database
-
-            return params
-        else:
+        # To solve this, return `find_word()` with the first cache number
+        if not main_data:
+            self.logger.debug("Main data not found. Multiple definitions")
             # print("This is not a definition page. getting all sub-pages")
             matching_results = yellowbridge_soup.find(id='multiRow')
             # Grab first row. This is usually the most common definition
-            row = matching_results.find_all('tr')[0]
+            rows = matching_results.find_all('tr')
+            if not rows:
+                self.logger.error("No rows found ")
+                return None
             # print(row.find('a'))
             href = str(row.find('a')['href'])
             # print(href)
             cache_number_from_href = href.split("word=")[1].split("&")[1].replace("cache=", "")
 
             return self.find_word(word, cache_number_from_href)
 
+        definition = \
+        traditional_script = \
+        pinyin = \
+        pinyin_num = \
+        part_of_speech = \
+        hsk_level = \
+        top_level = \
+        composing_words = None
+
+        main_data = main_data.find_all('tr')
+
+        # Collect all necessary information from the page:
+        for row in main_data:
+            row_info_type = row.find('td').getText()
+            row_info = row.find_all('td')[1].getText()
+            # print(row_info_type + ":")
+            # print(row_info)
+            if row_info_type == "English Definition":
+                definition = row_info
+            elif row_info_type == "Simplified Script":
+                simplified_script = row_info
+            elif row_info_type == "Traditional Script":
+                traditional_script = row_info.split("P")[0]
+            elif row_info_type == "Pinyin":
+                pinyin = row_info
+                pinyin_num = pin_to_num.get(word, format="numerical")
+            elif row_info_type == "Part of Speech":
+                part_of_speech = row_info
+            elif row_info_type == "Proficiency Test Level":
+                proficiency_level = row_info
+                if "HSK=" in proficiency_level:
+                    hsk_level = proficiency_level.split("HSK=")[1].split(";")[0]
+                if "TOP=" in proficiency_level:
+                    top_level = proficiency_level.split("TOP=")[1].split(";")[0]
+
+        word_decomposition_soup = yellowbridge_soup.find(id='wordDecomp')
+        if len(word) > 1:
+            composing_words_list = word_decomposition_soup.find_all('tr')
+            composing_words = ""
+            for composing_word in composing_words_list:
+                composing_words += str(composing_word.find_all('td')[0].find('a').getText()) + ";"
+
+        # This is all of the information that has been collected
+        # print([definition, simplified_script, traditional_script,pinyin,pinyin_num, part_of_speech,hsk_level,top_level,composing_words])
+        params = [traditional_script, part_of_speech, pinyin, pinyin_num,
+                  composing_words, hsk_level, top_level, definition, word]
+        # Add the information for this word to the database
+        return params
+
     def size(self):
         return 0
```

### Comparing `autoanki-1.1.6/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.1.7/src/autoanki.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.6
+Version: 1.1.7
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,36 +19,36 @@
 # autoanki
 Tool for generating Anki flashcards to learn Chinese.
 
 <img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
 
 ## Motivation
 
-When learning Chinese, advice is to learn the top X most common words.
+When learning Chinese, some common advice is to learn the top X most common words.
 This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
 For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
-With autoanki, you selectivley add words to an Anki file to continue progressing with your lanuage learning skills.
+With autoanki, you selectively add words to an Anki file to continue progressing with your lanuage learning skills.
 
 ## Usage
 
 autoanki is both a library and a command-line tool.
 
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
 
 To get started, first, create a database for autoanki to use 
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
-    AutoAnki.create_autoanki_db(db_path)
+    AutoAnki.create_database(db_path)
 ```
 Then create an instance of autoanki using the database
 ```
 aa = AutoAnki(db_path)
 ```
 Add whatever books you want in your deck. These can be a single file, or a folder
 ```
@@ -118,7 +118,8 @@
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
 To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence. 
+
```

### Comparing `autoanki-1.1.6/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.1.7/src/autoanki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

