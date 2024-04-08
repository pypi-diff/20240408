# Comparing `tmp/Dramatist-0.0.5.tar.gz` & `tmp/Dramatist-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dramatist-0.0.5.tar", last modified: Fri Feb  9 15:53:47 2024, max compression
+gzip compressed data, was "Dramatist-0.0.6.tar", last modified: Mon Apr  8 11:17:06 2024, max compression
```

## Comparing `Dramatist-0.0.5.tar` & `Dramatist-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 15:53:46.995937 Dramatist-0.0.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 15:53:46.995937 Dramatist-0.0.5/Dramatist.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16794 2024-02-09 15:53:46.000000 Dramatist-0.0.5/Dramatist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      676 2024-02-09 15:53:46.000000 Dramatist-0.0.5/Dramatist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-09 15:53:46.000000 Dramatist-0.0.5/Dramatist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-02-09 15:53:46.000000 Dramatist-0.0.5/Dramatist.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-09 15:53:46.000000 Dramatist-0.0.5/Dramatist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-09 15:53:46.000000 Dramatist-0.0.5/Dramatist.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-01-29 09:51:05.000000 Dramatist-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16794 2024-02-09 15:53:46.995937 Dramatist-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2985 2024-02-09 15:51:44.000000 Dramatist-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 15:53:46.991937 Dramatist-0.0.5/dramatist/
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-01-29 09:51:05.000000 Dramatist-0.0.5/dramatist/TextBlock.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-09 15:53:23.000000 Dramatist-0.0.5/dramatist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 15:53:46.991937 Dramatist-0.0.5/dramatist/cli/
--rw-rw-rw-   0 root         (0) root         (0)     3842 2024-02-07 19:14:26.000000 Dramatist-0.0.5/dramatist/cli/DramatistCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-09 15:53:23.000000 Dramatist-0.0.5/dramatist/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 15:53:46.991937 Dramatist-0.0.5/dramatist/core/
--rw-rw-rw-   0 root         (0) root         (0)     9657 2024-02-07 19:14:26.000000 Dramatist-0.0.5/dramatist/core/Dramatist.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/core/DramatistParseException.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-09 15:53:23.000000 Dramatist-0.0.5/dramatist/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 15:53:46.995937 Dramatist-0.0.5/dramatist/drama/
--rw-rw-rw-   0 root         (0) root         (0)     3068 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/Act.py
--rw-rw-rw-   0 root         (0) root         (0)    10849 2024-02-09 15:51:44.000000 Dramatist-0.0.5/dramatist/drama/Drama.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/Markup.py
--rw-rw-rw-   0 root         (0) root         (0)     6316 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/Scene.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/ScenePart.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/Speech.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/SpeechPart.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-05 08:39:23.000000 Dramatist-0.0.5/dramatist/drama/StageDirection.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-09 15:53:23.000000 Dramatist-0.0.5/dramatist/drama/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2024-02-07 19:14:26.000000 Dramatist-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-09 15:53:46.995937 Dramatist-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:17:06.299018 Dramatist-0.0.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:17:06.299018 Dramatist-0.0.6/Dramatist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16794 2024-04-08 11:17:06.000000 Dramatist-0.0.6/Dramatist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-08 11:17:06.000000 Dramatist-0.0.6/Dramatist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 11:17:06.000000 Dramatist-0.0.6/Dramatist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-08 11:17:06.000000 Dramatist-0.0.6/Dramatist.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-08 11:17:06.000000 Dramatist-0.0.6/Dramatist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-08 11:17:06.000000 Dramatist-0.0.6/Dramatist.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-03-26 16:59:43.000000 Dramatist-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16794 2024-04-08 11:17:06.299018 Dramatist-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2024-03-26 16:59:43.000000 Dramatist-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:17:06.295018 Dramatist-0.0.6/dramatist/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/TextBlock.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:16:52.000000 Dramatist-0.0.6/dramatist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:17:06.295018 Dramatist-0.0.6/dramatist/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     3842 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/cli/DramatistCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:16:52.000000 Dramatist-0.0.6/dramatist/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:17:06.295018 Dramatist-0.0.6/dramatist/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9731 2024-04-08 11:15:43.000000 Dramatist-0.0.6/dramatist/core/Dramatist.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/core/DramatistParseException.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:16:52.000000 Dramatist-0.0.6/dramatist/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 11:17:06.295018 Dramatist-0.0.6/dramatist/drama/
+-rw-rw-rw-   0 root         (0) root         (0)     3083 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/drama/Act.py
+-rw-rw-rw-   0 root         (0) root         (0)    11369 2024-04-08 11:15:43.000000 Dramatist-0.0.6/dramatist/drama/Drama.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/drama/Markup.py
+-rw-rw-rw-   0 root         (0) root         (0)     6347 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/drama/Scene.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/drama/ScenePart.py
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2024-04-08 11:15:43.000000 Dramatist-0.0.6/dramatist/drama/Speech.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 11:15:43.000000 Dramatist-0.0.6/dramatist/drama/SpeechPart.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-03-26 16:59:43.000000 Dramatist-0.0.6/dramatist/drama/StageDirection.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:16:52.000000 Dramatist-0.0.6/dramatist/drama/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2024-03-26 16:59:43.000000 Dramatist-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 11:17:06.299018 Dramatist-0.0.6/setup.cfg
```

### Comparing `Dramatist-0.0.5/Dramatist.egg-info/PKG-INFO` & `Dramatist-0.0.6/Dramatist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dramatist
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dramatist is a project for parsing plays from DraCor (https://dracor.org/) into a data structure which allows to access the text of the play "character" perfect, that is, character start and end positions for various parts, for example, act or scenes, can be retrieved. This also allows for functionality like getting the act and scene number for a character position.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `Dramatist-0.0.5/Dramatist.egg-info/SOURCES.txt` & `Dramatist-0.0.6/Dramatist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Dramatist-0.0.5/LICENSE` & `Dramatist-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Dramatist-0.0.5/PKG-INFO` & `Dramatist-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dramatist
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dramatist is a project for parsing plays from DraCor (https://dracor.org/) into a data structure which allows to access the text of the play "character" perfect, that is, character start and end positions for various parts, for example, act or scenes, can be retrieved. This also allows for functionality like getting the act and scene number for a character position.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `Dramatist-0.0.5/README.md` & `Dramatist-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Dramatist-0.0.5/dramatist/cli/DramatistCLI.py` & `Dramatist-0.0.6/dramatist/cli/DramatistCLI.py`

 * *Files identical despite different names*

### Comparing `Dramatist-0.0.5/dramatist/core/Dramatist.py` & `Dramatist-0.0.6/dramatist/core/Dramatist.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,16 @@
         if 'speaker' in stack:
             drama.set_speaker(result)
             result = ''
 
         if 'stage' in stack and 'stage' == stack[-1]:
             if 'p' in stack:
                 if first_child:
-                    drama.add_speech(result.strip(), SpeechPart.TYPE_STAGE_DIRECTION, markups)
+                    # TODO: improve special case, see SpeechPart.py
+                    drama.add_speech(result.strip(), SpeechPart.TYPE_STAGE_DIRECTION_COUNT, markups)
                     markups = []
                 else:
                     drama.add_speech(result.strip(), SpeechPart.TYPE_STAGE_DIRECTION_INLINE, markups)
                     markups = []
                 result = ''
             elif 'sp' in stack:
                 if (sibling_tag == 'lg' or sibling_tag == 'l' or sibling_tag == 'head' or sibling_tag == 'stage' or
```

### Comparing `Dramatist-0.0.5/dramatist/drama/Act.py` & `Dramatist-0.0.6/dramatist/drama/Act.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     def get_text_for_scene(self, scene) -> str:
         return self.scenes[scene-1].get_text()
 
     def get_text_for_scene_in_blocks(self, scene: int, max_length: int) -> List[TextBlock]:
         return self.scenes[scene-1].get_text_in_blocks(max_length)
 
-    def get_text_for_scene_by_character(self, scene: int, max_length: int):
-        return self.scenes[scene-1].get_text_by_character(max_length)
+    def get_text_for_scene_by_speaker(self, scene: int, max_length: int) -> List[TextBlock]:
+        return self.scenes[scene-1].get_text_by_speaker(max_length)
 
     def get_range(self) -> Tuple[int, int]:
         return self.start, self.end
 
     def __len__(self):
         return len(self.scenes)
```

### Comparing `Dramatist-0.0.5/dramatist/drama/Drama.py` & `Dramatist-0.0.6/dramatist/drama/Drama.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass, field
 from typing import List, Tuple
 
+from dramatist.TextBlock import TextBlock
 from dramatist.drama.Act import Act
 from dramatist.core.DramatistParseException import DramatistParseException
 from dramatist.drama.Markup import Markup
 from dramatist.drama.Speech import Speech
 from dramatist.drama.SpeechPart import SpeechPart
 from dramatist.drama.StageDirection import StageDirection
 
@@ -112,42 +113,43 @@
         Get the text for the given scene in the given act.
         :param act: Number of the act
         :param scene: Number of the scene
         :return: The text of the scene
         """
         return self.acts[act-1].get_text_for_scene(scene)
 
-    def get_text_for_scene_in_blocks(self, act, scene, max_length):
+    def get_text_for_scene_in_blocks(self, act, scene, max_length) -> List[TextBlock]:
         """
         Get a list of text blocks for the given scene in the given act. Blocks that are longer than the given
         maximum length (in words) are split into multiple blocks.
         :param act: The act number
         :param scene: The scene number
         :param max_length: The maximum length in words of a returned text block. Longer blocks will be split.
         :return: A list of text blocks
         """
         return self.acts[act-1].get_text_for_scene_in_blocks(scene, max_length)
 
-    def get_text_for_scene_by_speaker(self, act, scene, max_length):
+    def get_text_for_scene_by_speaker(self, act, scene, max_length) -> List[TextBlock]:
         """
         Get a list of text blocks by speaker for the given scene in the given act. This means that for every speaker
         change a new text block is created. Blocks that are longer than the given maximum length (in words)
         are split into multiple blocks.
         :param act: The act number
         :param scene: The scene number
         :param max_length: The maximum length of a returned text block. Longer blocks will be split.
         :return: A list of text blocks
         """
-        return self.acts[act-1].get_text_for_scene_by_character(scene, max_length)
+        return self.acts[act-1].get_text_for_scene_by_speaker(scene, max_length)
 
     def get_scene_act_for_position(self, search_start: int) -> Tuple[int, int]:
         """
         Return a tuple of act and scene number for the given position.
         :param search_start: The character position for which to return the act and scene number
-        :return: A tuple of act and scene number
+        :return: A tuple of act and scene number. (-1, -1), if act and scene could not be found, or (act_nr, -1) if act
+        could be found but scene could not.
         """
         found_act_nr = -1
         for act_pos, act in enumerate(self.acts):
             act_start, act_end = act.get_range()
 
             if act_start <= search_start < act_end:
                 found_act_nr = act_pos + 1
@@ -159,29 +161,29 @@
 
         return found_act_nr, -1
 
     def get_scene_act_for_line(self, line_nr: int) -> Tuple[int, int]:
         """
         Return a tuple of act and scene number for the given line number.
         :param line_nr: A line number
-        :return: A tuple of act and scene number
+        :return: A tuple of act and scene number. (-1, -1), if act and scene could not be found
         """
         for act_pos, act in enumerate(self.acts):
             if act.scenes[-1].end_line >= line_nr:
                 for scene_pos, scene in enumerate(act.scenes):
                     if scene.start_line <= line_nr <= scene.end_line:
                         return act_pos + 1, scene_pos + 1
 
         return -1, -1
 
     def get_scene_act_for_text(self, text_to_search: str) -> Tuple[int, int]:
         """
         Return a tuple of act and scene number in which the given text appears.
         :param text_to_search: The text so search for
-        :return: A tuple of act and scene number
+        :return: A tuple of act and scene number. (-1, -1), if act and scene could not be found
         """
         search_string = text_to_search[0:100]
         search_string = (search_string.lower().replace('\n', '').replace('\t', '')
                          .replace(' ', ''))
 
         drama_text = (self.get_text().lower().replace('\n', '').replace('\t', '')
                       .replace(' ', ''))
@@ -256,17 +258,22 @@
                             markup.start = total_length + markup.start
                             markup.end = total_length + markup.end
 
                         if speech_part.type == SpeechPart.TYPE_SPEECH_LINE:
                             line_count += 1
                         elif speech_part.type == SpeechPart.TYPE_SPEECH_P_B:
                             line_count += 1
-                        elif speech_part.type == SpeechPart.TYPE_STAGE_DIRECTION:
+                        elif (speech_part.type == SpeechPart.TYPE_STAGE_DIRECTION or
+                              speech_part.type == SpeechPart.TYPE_STAGE_DIRECTION_COUNT):
                             speech_part.markups.append(Markup(total_length, total_length +
                                                               len(speech_part.text), 'stage'))
+
+                            if speech_part.type == SpeechPart.TYPE_STAGE_DIRECTION_COUNT:
+                                line_count += 1
+
                         elif speech_part.type == SpeechPart.TYPE_STAGE_DIRECTION_INLINE:
                             speech_part.markups.append(Markup(total_length, total_length +
                                                               len(speech_part.text), 'stage_inline'))
 
                         scene_part.end_line = total_lines + line_count
                         total_lines += line_count
                         total_length += len(speech_part.text) + 1
```

### Comparing `Dramatist-0.0.5/dramatist/drama/Scene.py` & `Dramatist-0.0.6/dramatist/drama/Scene.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,41 +118,40 @@
                             line_start += lines_per_part
 
         if current_length > 0:
             result.append(current)
 
         return result
 
-    # TODO: return text block
-    def get_text_by_character(self, max_length: int):
-        result = []
+    def get_text_by_speaker(self, max_length: int) -> List[TextBlock]:
+        result: List[TextBlock] = []
 
         for scene_block in self.scene_parts:
             if isinstance(scene_block, Speech):
                 speech = scene_block
 
                 if len(speech) < max_length:
-                    result.append((speech.start_line, speech.end_line, f'{speech.speaker}{speech.get_text()}'))
+                    result.append(TextBlock(speech.start_line, speech.end_line, f'{speech.speaker}{speech.get_text()}'))
                 else:
                     factor = (len(speech) // max_length) + 1
                     sub_length = math.ceil(len(speech) / factor)
                     parts = [speech.get_tokens()[i:i + sub_length] for i in range(0, len(speech), sub_length)]
 
                     # Line numbers are only estimations for now
                     line_count = speech.end_line - speech.start_line + 1
                     lines_per_part = line_count // factor
                     line_start = speech.start_line
 
                     for pos, p in enumerate(parts):
                         text = ' '.join(p)
 
                         if pos == 0:
-                            result.append((line_start, line_start + lines_per_part, f'{speech.speaker}{text}'))
+                            result.append(TextBlock(line_start, line_start + lines_per_part, f'{speech.speaker}{text}'))
                         else:
-                            result.append((line_start, line_start + lines_per_part, text))
+                            result.append(TextBlock(line_start, line_start + lines_per_part, text))
 
                         line_start += lines_per_part
 
         return result
 
     def get_range(self) -> Tuple[int, int]:
         return self.start, self.end
```

### Comparing `Dramatist-0.0.5/dramatist/drama/Speech.py` & `Dramatist-0.0.6/dramatist/drama/Speech.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         for pos, sb in enumerate(self.speech_parts):
             if sb.type == SpeechPart.TYPE_SPEECH_P_B:
                 result += '\n'
             elif sb.type == SpeechPart.TYPE_SPEECH_P:
                 result += ' '
             elif sb.type == SpeechPart.TYPE_SPEECH_LINE:
                 result += '\n'
-            elif sb.type == SpeechPart.TYPE_STAGE_DIRECTION:
+            elif sb.type == SpeechPart.TYPE_STAGE_DIRECTION or sb.type == SpeechPart.TYPE_STAGE_DIRECTION_COUNT:
                 result += '\n'
             elif sb.type == SpeechPart.TYPE_STAGE_DIRECTION_INLINE:
                 result += ' '
 
             result += f'{sb.text}'
 
         return result
```

### Comparing `Dramatist-0.0.5/dramatist/drama/StageDirection.py` & `Dramatist-0.0.6/dramatist/drama/StageDirection.py`

 * *Files identical despite different names*

### Comparing `Dramatist-0.0.5/pyproject.toml` & `Dramatist-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Dramatist"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Frederik Arnold", email = "frederik.arnold@hu-berlin.de"}
 ]
 description = "Dramatist is a project for parsing plays from DraCor (https://dracor.org/) into a data structure which allows to access the text of the play \"character\" perfect, that is, character start and end positions for various parts, for example, act or scenes, can be retrieved. This also allows for functionality like getting the act and scene number for a character position."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

