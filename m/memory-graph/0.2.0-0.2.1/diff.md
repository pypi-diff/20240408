# Comparing `tmp/memory_graph-0.2.0.tar.gz` & `tmp/memory_graph-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.2.0.tar", last modified: Sun Apr  7 18:29:12 2024, max compression
+gzip compressed data, was "memory_graph-0.2.1.tar", last modified: Mon Apr  8 21:14:46 2024, max compression
```

## Comparing `memory_graph-0.2.0.tar` & `memory_graph-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-07 18:29:12.275152 memory_graph-0.2.0/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-02-16 13:16:53.000000 memory_graph-0.2.0/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-02-16 13:16:53.000000 memory_graph-0.2.0/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21116 2024-04-07 18:29:12.275152 memory_graph-0.2.0/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20451 2024-04-07 18:24:52.000000 memory_graph-0.2.0/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-07 18:29:12.275152 memory_graph-0.2.0/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/HTML_Table.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Memory_Graph.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3428 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Memory_Visitor.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3168 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Hidden.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3968 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Key_Value.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2520 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Linear.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3287 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Table.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3949 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Sliced.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Slicer.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6542 2024-04-07 18:28:19.000000 memory_graph-0.2.0/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      331 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/config.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2947 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/config_default.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/config_helpers.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/extension_numpy.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/extension_pandas.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4903 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/test.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      537 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/test_memory_graph.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/test_memory_visitor.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/utils.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-07 18:29:12.275152 memory_graph-0.2.0/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21116 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      777 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-07 18:29:12.275152 memory_graph-0.2.0/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1055 2024-04-07 18:28:38.000000 memory_graph-0.2.0/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-08 21:14:46.607196 memory_graph-0.2.1/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-02-16 13:16:53.000000 memory_graph-0.2.1/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-02-16 13:16:53.000000 memory_graph-0.2.1/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21297 2024-04-08 21:14:46.607196 memory_graph-0.2.1/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20650 2024-04-08 21:11:27.000000 memory_graph-0.2.1/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-08 21:14:46.607196 memory_graph-0.2.1/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/HTML_Table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Memory_Graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-08 20:46:55.000000 memory_graph-0.2.1/memory_graph/Memory_Visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3168 2024-04-08 20:45:29.000000 memory_graph-0.2.1/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Node_Hidden.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3968 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Node_Key_Value.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2520 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Node_Linear.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3287 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Node_Table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3949 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Sliced.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/Slicer.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6542 2024-04-08 21:13:11.000000 memory_graph-0.2.1/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      327 2024-04-08 20:50:18.000000 memory_graph-0.2.1/memory_graph/config.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3231 2024-04-08 21:10:10.000000 memory_graph-0.2.1/memory_graph/config_default.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/config_helpers.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/extension_numpy.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/extension_pandas.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       24 2024-04-08 20:16:22.000000 memory_graph-0.2.1/memory_graph/special_types.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4909 2024-04-08 21:05:52.000000 memory_graph-0.2.1/memory_graph/test.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      536 2024-04-08 19:52:20.000000 memory_graph-0.2.1/memory_graph/test_memory_graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/test_memory_visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-07 17:46:45.000000 memory_graph-0.2.1/memory_graph/utils.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-08 21:14:46.607196 memory_graph-0.2.1/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21297 2024-04-08 21:14:46.000000 memory_graph-0.2.1/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      807 2024-04-08 21:14:46.000000 memory_graph-0.2.1/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-08 21:14:46.000000 memory_graph-0.2.1/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-08 21:14:46.000000 memory_graph-0.2.1/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-08 21:14:46.000000 memory_graph-0.2.1/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-08 21:14:46.607196 memory_graph-0.2.1/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1037 2024-04-08 21:14:16.000000 memory_graph-0.2.1/setup.py
```

### Comparing `memory_graph-0.2.0/LICENSE.txt` & `memory_graph-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/PKG-INFO` & `memory_graph-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.2.0
-Summary: Draws a graph of your data to analyze the structure of its references.
+Version: 0.2.1
+Summary: Draws a graph of your data to analyze its structure.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -34,24 +34,24 @@
 import memory_graph
 
 # create the lists 'a' and 'b'
 a = [4, 3, 2]
 b = a
 a.append(1) # changing 'a' changes 'b'
 
-# print the lists
+# print the 'a' and 'b' list
 print('a:', a)
 print('b:', b)
 
-# check if they share data
+# check if 'a' and 'b' share data
 print('ids:', id(a), id(b))
 print('identical?:', a is b)
 
-# show the lists in a graph
-memory_graph.show(locals()) 
+# show all local variables in a graph
+memory_graph.show( locals() )
 ```
 
 </td><td>
 
 ![mutable2.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/mutable2.png)
 
 a graph showing `a` and `b` share data
@@ -61,29 +61,34 @@
 The fact that `a` and `b` share data can not be verified by printing the lists. It can be verified by comparing the identity of both variables using the `id()` function or by using the `is` comparison operator as shown in the program output below, but this quickly becomes impractical for larger programs. 
 ```{verbatim}
 a: 4, 3, 2, 1
 b: 4, 3, 2, 1
 ids: 126432214913216 126432214913216
 identical?: True
 ```
-A better way to understand what data is shared is to draw a graph of the data using this [memory_graph](https://pypi.org/project/memory-graph/) package.
+A better way to understand what data is shared is to draw a graph of the data using the [memory_graph](https://pypi.org/project/memory-graph/) package.
 
 # Memory Graph Packge #
-The [memory_graph](https://pypi.org/project/memory-graph/) package can show a graph with many different data types.
+The [memory_graph](https://pypi.org/project/memory-graph/) package can graph many different data types.
 
 ```python
 import memory_graph
 
-data = [ (1, 2), [3, 4], {5, 6}, {7:'seven', 8:'eight'} ]
+class MyClass:
+
+    def __init__(self, x, y):
+        self.x = x
+        self.y = y
+
+data = [ range(1, 2), (3, 4), {5, 6}, {7:'seven', 8:'eight'},  MyClass(9, 10) ]
 memory_graph.show(data, block=True)
 ```
-
 ![many_types.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/many_types.png)
 
-By using `block=True` the program blocks until the ENTER key is pressed so you can view the graph before continuing program execution (and possibly viewing later graphs). Instead of showing the graph you can also render it to an output file of our choosing (see [Graphviz Output Formats](https://graphviz.org/docs/outputs/)) using for example:
+By using `block=True` the program blocks until the ENTER key is pressed so you can view the graph before continuing program execution (and possibly viewing later graphs). Instead of showing the graph you can also render it to an output file of your choosing (see [Graphviz Output Formats](https://graphviz.org/docs/outputs/)) using for example:
 
 ```python
 memory_graph.render(data, "my_graph.pdf")
 memory_graph.render(data, "my_graph.png")
 memory_graph.render(data, "my_graph.gv") # Graphviz DOT file
 ```
 
@@ -454,26 +459,26 @@
 ```
 ![hash_set.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/hash_set.png)
 
 
 ## 5. Configuration ##
 Different aspects of memory_graph can be configured. The default configuration is reset by importing 'memory_graph.config_default'.
 
+- ***memory_graph.config.max_number_nodes*** : int
+  - The maxium number of Nodes shown in the graph. When the graph gets too big set this to a smaller number. A `★` symbol indictes where the graph is cut short.
+
+- ***memory_graph.config.max_string_length*** : int
+  - The maximum length of strings shown in the graph. Longer strings will be truncated.
+
 - ***memory_graph.config.no_reference_types*** : dict
-  - Holds all types for which no seperate node it drawn but that are shown as elements in their parent Node. It maps each type to a function that determines how it is visualized.
+  - Holds all types for which no seperate node is drawn but that instead are shown as elements in their parent Node. It maps each type to a function that determines how it is visualized.
 
 - ***memory_graph.config.no_child_references_types*** : set
   - The set of key_value types that don't draw references to their direct childeren but have their children shown as elements of their node.
 
-- ***memory_graph.config.max_string_length*** : int
-  - The maximum length of strings shown in the graph.
-
-- ***memory_graph.config.max_number_nodes*** : int
-  - The maxium number of Nodes shows in the graph. When the graph gets to big set this to a small number to analyze the problem.
-
 - ***memory_graph.config.type_to_node*** : dict
   - Determines how a data types is converted to a Node (sub)class for visualization in the graph.
 
 - ***memory_graph.config.type_to_color*** : dict
   - Maps each type to the [graphviz color](https://graphviz.org/doc/info/colors.html) it gets in the graph. 
 
 - ***memory_graph.config.type_to_vertical_orientation*** : dict
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `memory_graph-0.2.0/README.md` & `memory_graph-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 import memory_graph
 
 # create the lists 'a' and 'b'
 a = [4, 3, 2]
 b = a
 a.append(1) # changing 'a' changes 'b'
 
-# print the lists
+# print the 'a' and 'b' list
 print('a:', a)
 print('b:', b)
 
-# check if they share data
+# check if 'a' and 'b' share data
 print('ids:', id(a), id(b))
 print('identical?:', a is b)
 
-# show the lists in a graph
-memory_graph.show(locals()) 
+# show all local variables in a graph
+memory_graph.show( locals() )
 ```
 
 </td><td>
 
 ![mutable2.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/mutable2.png)
 
 a graph showing `a` and `b` share data
@@ -42,29 +42,34 @@
 The fact that `a` and `b` share data can not be verified by printing the lists. It can be verified by comparing the identity of both variables using the `id()` function or by using the `is` comparison operator as shown in the program output below, but this quickly becomes impractical for larger programs. 
 ```{verbatim}
 a: 4, 3, 2, 1
 b: 4, 3, 2, 1
 ids: 126432214913216 126432214913216
 identical?: True
 ```
-A better way to understand what data is shared is to draw a graph of the data using this [memory_graph](https://pypi.org/project/memory-graph/) package.
+A better way to understand what data is shared is to draw a graph of the data using the [memory_graph](https://pypi.org/project/memory-graph/) package.
 
 # Memory Graph Packge #
-The [memory_graph](https://pypi.org/project/memory-graph/) package can show a graph with many different data types.
+The [memory_graph](https://pypi.org/project/memory-graph/) package can graph many different data types.
 
 ```python
 import memory_graph
 
-data = [ (1, 2), [3, 4], {5, 6}, {7:'seven', 8:'eight'} ]
+class MyClass:
+
+    def __init__(self, x, y):
+        self.x = x
+        self.y = y
+
+data = [ range(1, 2), (3, 4), {5, 6}, {7:'seven', 8:'eight'},  MyClass(9, 10) ]
 memory_graph.show(data, block=True)
 ```
-
 ![many_types.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/many_types.png)
 
-By using `block=True` the program blocks until the ENTER key is pressed so you can view the graph before continuing program execution (and possibly viewing later graphs). Instead of showing the graph you can also render it to an output file of our choosing (see [Graphviz Output Formats](https://graphviz.org/docs/outputs/)) using for example:
+By using `block=True` the program blocks until the ENTER key is pressed so you can view the graph before continuing program execution (and possibly viewing later graphs). Instead of showing the graph you can also render it to an output file of your choosing (see [Graphviz Output Formats](https://graphviz.org/docs/outputs/)) using for example:
 
 ```python
 memory_graph.render(data, "my_graph.pdf")
 memory_graph.render(data, "my_graph.png")
 memory_graph.render(data, "my_graph.gv") # Graphviz DOT file
 ```
 
@@ -435,26 +440,26 @@
 ```
 ![hash_set.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/hash_set.png)
 
 
 ## 5. Configuration ##
 Different aspects of memory_graph can be configured. The default configuration is reset by importing 'memory_graph.config_default'.
 
+- ***memory_graph.config.max_number_nodes*** : int
+  - The maxium number of Nodes shown in the graph. When the graph gets too big set this to a smaller number. A `★` symbol indictes where the graph is cut short.
+
+- ***memory_graph.config.max_string_length*** : int
+  - The maximum length of strings shown in the graph. Longer strings will be truncated.
+
 - ***memory_graph.config.no_reference_types*** : dict
-  - Holds all types for which no seperate node it drawn but that are shown as elements in their parent Node. It maps each type to a function that determines how it is visualized.
+  - Holds all types for which no seperate node is drawn but that instead are shown as elements in their parent Node. It maps each type to a function that determines how it is visualized.
 
 - ***memory_graph.config.no_child_references_types*** : set
   - The set of key_value types that don't draw references to their direct childeren but have their children shown as elements of their node.
 
-- ***memory_graph.config.max_string_length*** : int
-  - The maximum length of strings shown in the graph.
-
-- ***memory_graph.config.max_number_nodes*** : int
-  - The maxium number of Nodes shows in the graph. When the graph gets to big set this to a small number to analyze the problem.
-
 - ***memory_graph.config.type_to_node*** : dict
   - Determines how a data types is converted to a Node (sub)class for visualization in the graph.
 
 - ***memory_graph.config.type_to_color*** : dict
   - Maps each type to the [graphviz color](https://graphviz.org/doc/info/colors.html) it gets in the graph. 
 
 - ***memory_graph.config.type_to_vertical_orientation*** : dict
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `memory_graph-0.2.0/memory_graph/HTML_Table.py` & `memory_graph-0.2.1/memory_graph/HTML_Table.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Memory_Graph.py` & `memory_graph-0.2.1/memory_graph/Memory_Graph.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Memory_Visitor.py` & `memory_graph-0.2.1/memory_graph/Memory_Visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from memory_graph.Node_Linear import Node_Linear
 from memory_graph.Node_Key_Value import Node_Key_Value
 
 import memory_graph.utils as utils    
 import memory_graph.config as config
 import memory_graph.config_helpers as config_helpers
 
-
 def default_backtrack_callback(node):
     print('backtrack_callback:', node)
     #node.visit_with_depth(lambda child: print('-- child:', child))
 
 class Memory_Visitor:
     """
     Memory_Visitor visits the memory in a depth first manner starting from the 'data' root node.
@@ -45,20 +44,20 @@
         """
         #print('visit_recursive:', data, parent_node)
         if data is self:
             return None
         data_type = type(data)
         if (parent_node != None and data_type in config.no_reference_types):
             return config.no_reference_types[data_type](data)
-        if len(self.data_ids) > config.max_number_nodes:
-            print(f"Memory_Visitor max_number_nodes ({config.max_number_nodes}) reached, stopping recursion.")
-            return None
         data_id = id(data)
         if data_id in self.data_ids:
             return self.data_ids[data_id]
+        elif len(self.data_ids) > config.max_number_nodes:
+            print(f"Memory_Visitor max_number_nodes ({config.max_number_nodes}) reached, stopping recursion.")
+            return "★"
         else:
             node = self.data_to_node(data)
             self.data_ids[data_id] = node
             if node is not None:
                 node.set_parent(parent_node)
                 node.transform(lambda child: self.visit_recursive(child, node))
                 if node.do_backtrack_callback():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `memory_graph-0.2.0/memory_graph/Node.py` & `memory_graph-0.2.1/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Node_Hidden.py` & `memory_graph-0.2.1/memory_graph/Node_Hidden.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Node_Key_Value.py` & `memory_graph-0.2.1/memory_graph/Node_Key_Value.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Node_Linear.py` & `memory_graph-0.2.1/memory_graph/Node_Linear.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Node_Table.py` & `memory_graph-0.2.1/memory_graph/Node_Table.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Sliced.py` & `memory_graph-0.2.1/memory_graph/Sliced.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/Slicer.py` & `memory_graph-0.2.1/memory_graph/Slicer.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/__init__.py` & `memory_graph-0.2.1/memory_graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import memory_graph.config_default as config_default
 import memory_graph.utils as utils
 
 import inspect
 import sys
 
-__version__ = "0.2.00"
+__version__ = "0.2.01"
 __author__ = 'Bas Terwijn'
 
 log_file=sys.stdout
 press_enter_text="press <ENTER> to continue..."
 
 def get_source_location(stack_index):
     """ Helper function to get the source location of the stack with 'stack_index' of the call stack. """
```

### Comparing `memory_graph-0.2.0/memory_graph/config_default.py` & `memory_graph-0.2.1/memory_graph/config_default.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from memory_graph.Slicer import Slicer
 
 import memory_graph.config as config
 import memory_graph.utils as utils
 
 import types
 
+""" The maxium number of Nodes shown in the graph. When the graph gets too big set this to a smaller number to analyze the problem. A `★` symbol indictes where the gra[h is cut short.  """
+config.max_number_nodes = 1000
+
+""" The maximum length of strings shown in the graph. Longer strings will be truncated. """
+config.max_string_length = 42
+
 """ Types that by default will not have references pointing to them in the graph but instead will be visualized in the node of their parent. """
 config.no_reference_types = {
     type(None) : lambda d: "None",  # so None can be used to indicate no value
     bool : lambda d: d, 
     int : lambda d: d, 
     float : lambda d: d, 
     complex : lambda d: d, 
@@ -22,17 +28,14 @@
     types.FunctionType : lambda d: str(d.__qualname__),
     types.MethodType  : lambda d: str(d.__qualname__),
 }
 
 """ Types that will not have references pointing to their children in the graph but instead will have their children visualized in their node. """
 config.no_child_references_types = {dict, types.MappingProxyType}
 
-config.max_string_length = 42
-config.max_number_nodes = 1000
-
 """ Conversion from type to Node objects. """
 config.type_to_node = {
     str: lambda data: Node(data), # visit as whole string, don't iterate over characters
     range: lambda data: Node_Key_Value(data, {'start':data.start, 'stop':data.stop, 'step':data.step}.items()),
     types.FunctionType: lambda data: Node(data.__qualname__),
     types.MethodType: lambda data: Node(data.__qualname__),
     dict: lambda data: (
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `memory_graph-0.2.0/memory_graph/config_helpers.py` & `memory_graph-0.2.1/memory_graph/config_helpers.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/extension_numpy.py` & `memory_graph-0.2.1/memory_graph/extension_numpy.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/extension_pandas.py` & `memory_graph-0.2.1/memory_graph/extension_pandas.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph/test.py` & `memory_graph-0.2.1/memory_graph/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     config.no_reference_types = restore
 
 def test_empty_linear(fun):
     data = [tuple(), list(), set(), frozenset(), dict() , bytes(), bytearray()]
     fun(data)
 
 def test_nested_list(fun):
-    data = utils.nested_list([2,3,4,5])
+    data = utils.nested_list([2,2,2,2,2,2,2])
     fun(data)
 
 def test_key_value(fun):
     data1 = {1:'a', 2:'b', 3:'c', 4:'d'}
     data2 = {10:100, 20:200, 30:300, 40:400}
     data2[50] = ('c','c')
     data2[60] = data1
```

### Comparing `memory_graph-0.2.0/memory_graph/test_memory_graph.py` & `memory_graph-0.2.1/memory_graph/test_memory_graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,8 +7,7 @@
     test_fun_count = 0
     def test_fun(data):
         global test_fun_count
         graph = Memory_Graph(data) #, colors={id(data):'red'}, vertical_orientations={id(data):True, list:False}, slicers={id(data):(Slicer(0,0),Slicer(0,0))} )
         graph.get_graph().render(outfile=f'test_graph{test_fun_count}.png')
         test_fun_count += 1
     test.test_all(test_fun)
-
```

### Comparing `memory_graph-0.2.0/memory_graph/utils.py` & `memory_graph-0.2.1/memory_graph/utils.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.0/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.2.1/memory_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.2.0
-Summary: Draws a graph of your data to analyze the structure of its references.
+Version: 0.2.1
+Summary: Draws a graph of your data to analyze its structure.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -34,24 +34,24 @@
 import memory_graph
 
 # create the lists 'a' and 'b'
 a = [4, 3, 2]
 b = a
 a.append(1) # changing 'a' changes 'b'
 
-# print the lists
+# print the 'a' and 'b' list
 print('a:', a)
 print('b:', b)
 
-# check if they share data
+# check if 'a' and 'b' share data
 print('ids:', id(a), id(b))
 print('identical?:', a is b)
 
-# show the lists in a graph
-memory_graph.show(locals()) 
+# show all local variables in a graph
+memory_graph.show( locals() )
 ```
 
 </td><td>
 
 ![mutable2.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/mutable2.png)
 
 a graph showing `a` and `b` share data
@@ -61,29 +61,34 @@
 The fact that `a` and `b` share data can not be verified by printing the lists. It can be verified by comparing the identity of both variables using the `id()` function or by using the `is` comparison operator as shown in the program output below, but this quickly becomes impractical for larger programs. 
 ```{verbatim}
 a: 4, 3, 2, 1
 b: 4, 3, 2, 1
 ids: 126432214913216 126432214913216
 identical?: True
 ```
-A better way to understand what data is shared is to draw a graph of the data using this [memory_graph](https://pypi.org/project/memory-graph/) package.
+A better way to understand what data is shared is to draw a graph of the data using the [memory_graph](https://pypi.org/project/memory-graph/) package.
 
 # Memory Graph Packge #
-The [memory_graph](https://pypi.org/project/memory-graph/) package can show a graph with many different data types.
+The [memory_graph](https://pypi.org/project/memory-graph/) package can graph many different data types.
 
 ```python
 import memory_graph
 
-data = [ (1, 2), [3, 4], {5, 6}, {7:'seven', 8:'eight'} ]
+class MyClass:
+
+    def __init__(self, x, y):
+        self.x = x
+        self.y = y
+
+data = [ range(1, 2), (3, 4), {5, 6}, {7:'seven', 8:'eight'},  MyClass(9, 10) ]
 memory_graph.show(data, block=True)
 ```
-
 ![many_types.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/many_types.png)
 
-By using `block=True` the program blocks until the ENTER key is pressed so you can view the graph before continuing program execution (and possibly viewing later graphs). Instead of showing the graph you can also render it to an output file of our choosing (see [Graphviz Output Formats](https://graphviz.org/docs/outputs/)) using for example:
+By using `block=True` the program blocks until the ENTER key is pressed so you can view the graph before continuing program execution (and possibly viewing later graphs). Instead of showing the graph you can also render it to an output file of your choosing (see [Graphviz Output Formats](https://graphviz.org/docs/outputs/)) using for example:
 
 ```python
 memory_graph.render(data, "my_graph.pdf")
 memory_graph.render(data, "my_graph.png")
 memory_graph.render(data, "my_graph.gv") # Graphviz DOT file
 ```
 
@@ -454,26 +459,26 @@
 ```
 ![hash_set.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/hash_set.png)
 
 
 ## 5. Configuration ##
 Different aspects of memory_graph can be configured. The default configuration is reset by importing 'memory_graph.config_default'.
 
+- ***memory_graph.config.max_number_nodes*** : int
+  - The maxium number of Nodes shown in the graph. When the graph gets too big set this to a smaller number. A `★` symbol indictes where the graph is cut short.
+
+- ***memory_graph.config.max_string_length*** : int
+  - The maximum length of strings shown in the graph. Longer strings will be truncated.
+
 - ***memory_graph.config.no_reference_types*** : dict
-  - Holds all types for which no seperate node it drawn but that are shown as elements in their parent Node. It maps each type to a function that determines how it is visualized.
+  - Holds all types for which no seperate node is drawn but that instead are shown as elements in their parent Node. It maps each type to a function that determines how it is visualized.
 
 - ***memory_graph.config.no_child_references_types*** : set
   - The set of key_value types that don't draw references to their direct childeren but have their children shown as elements of their node.
 
-- ***memory_graph.config.max_string_length*** : int
-  - The maximum length of strings shown in the graph.
-
-- ***memory_graph.config.max_number_nodes*** : int
-  - The maxium number of Nodes shows in the graph. When the graph gets to big set this to a small number to analyze the problem.
-
 - ***memory_graph.config.type_to_node*** : dict
   - Determines how a data types is converted to a Node (sub)class for visualization in the graph.
 
 - ***memory_graph.config.type_to_color*** : dict
   - Maps each type to the [graphviz color](https://graphviz.org/doc/info/colors.html) it gets in the graph. 
 
 - ***memory_graph.config.type_to_vertical_orientation*** : dict
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `memory_graph-0.2.0/memory_graph.egg-info/SOURCES.txt` & `memory_graph-0.2.1/memory_graph.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 memory_graph/Slicer.py
 memory_graph/__init__.py
 memory_graph/config.py
 memory_graph/config_default.py
 memory_graph/config_helpers.py
 memory_graph/extension_numpy.py
 memory_graph/extension_pandas.py
+memory_graph/special_types.py
 memory_graph/test.py
 memory_graph/test_memory_graph.py
 memory_graph/test_memory_visitor.py
 memory_graph/utils.py
 memory_graph.egg-info/PKG-INFO
 memory_graph.egg-info/SOURCES.txt
 memory_graph.egg-info/dependency_links.txt
```

### Comparing `memory_graph-0.2.0/setup.py` & `memory_graph-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.2.00',
-    description = 'Draws a graph of your data to analyze the structure of its references.',
+    version = '0.2.01',
+    description = 'Draws a graph of your data to analyze its structure.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
     license = 'BSD 2-clause',
```

