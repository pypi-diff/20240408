# Comparing `tmp/Stucent-0.1.6.tar.gz` & `tmp/Stucent-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Stucent-0.1.6.tar", last modified: Sun Feb 18 06:35:39 2024, max compression
+gzip compressed data, was "Stucent-0.1.7.tar", last modified: Mon Apr  8 05:52:31 2024, max compression
```

## Comparing `Stucent-0.1.6.tar` & `Stucent-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:35:39.668142 Stucent-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-18 06:35:26.000000 Stucent-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-18 06:35:39.668142 Stucent-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-18 06:35:26.000000 Stucent-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:35:39.668142 Stucent-0.1.6/Stucent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-18 06:35:39.000000 Stucent-0.1.6/Stucent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-18 06:35:39.000000 Stucent-0.1.6/Stucent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 06:35:39.000000 Stucent-0.1.6/Stucent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-18 06:35:39.000000 Stucent-0.1.6/Stucent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-18 06:35:39.000000 Stucent-0.1.6/Stucent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 06:35:39.668142 Stucent-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-18 06:35:26.000000 Stucent-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:35:39.668142 Stucent-0.1.6/stucent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 06:35:26.000000 Stucent-0.1.6/stucent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-18 06:35:26.000000 Stucent-0.1.6/stucent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-02-18 06:35:26.000000 Stucent-0.1.6/stucent/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-02-18 06:35:26.000000 Stucent-0.1.6/stucent/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:35:39.668142 Stucent-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 06:35:26.000000 Stucent-0.1.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:52:31.101839 Stucent-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-08 05:52:21.000000 Stucent-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 05:52:31.101839 Stucent-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 05:52:21.000000 Stucent-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:52:31.101839 Stucent-0.1.7/Stucent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 05:52:31.000000 Stucent-0.1.7/Stucent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 05:52:31.000000 Stucent-0.1.7/Stucent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:52:31.000000 Stucent-0.1.7/Stucent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 05:52:31.000000 Stucent-0.1.7/Stucent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 05:52:31.000000 Stucent-0.1.7/Stucent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:52:31.101839 Stucent-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 05:52:21.000000 Stucent-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:52:31.101839 Stucent-0.1.7/stucent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:52:21.000000 Stucent-0.1.7/stucent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-08 05:52:21.000000 Stucent-0.1.7/stucent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 05:52:21.000000 Stucent-0.1.7/stucent/content_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-08 05:52:21.000000 Stucent-0.1.7/stucent/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19797 2024-04-08 05:52:21.000000 Stucent-0.1.7/stucent/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:52:31.101839 Stucent-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:52:21.000000 Stucent-0.1.7/tests/test.py
```

### Comparing `Stucent-0.1.6/LICENSE` & `Stucent-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Stucent-0.1.6/stucent/client.py` & `Stucent-0.1.7/stucent/client.py`

 * *Files identical despite different names*

### Comparing `Stucent-0.1.6/stucent/models.py` & `Stucent-0.1.7/stucent/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     prompt_name: Optional[str] = "lesson.activities"
     schema_name: Optional[str] = "activities"
     activities_examples: Optional[str] = "lesson.activities"
     context: Optional[Union[Context, str]] = None
     request: Optional[str] = None
 
 # Model for agenerate_complete_course_content
-class CompleteCourseContentRequest(BaseModel):
+class CourseActivitiesRequest(BaseModel):
     course_title: str
     course_meta: CourseMeta
     course_outline: CourseTree
     lesson_layout: List[str]
     prompt_name: Optional[str] = "lesson.activities"
     schema_name: Optional[str] = "activities"
     activities_examples: Optional[str] = "lesson.activities"
```

### Comparing `Stucent-0.1.6/stucent/services.py` & `Stucent-0.1.7/stucent/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
                 with open(f"{stucent_dir}/meta_{output_name}.json", "w") as w:
                     w.write(meta.model_dump_json(indent=2, exclude_none=True))
             return meta
         except Exception as e:
             error_message = self._get_error_message(e)
             raise Exception(f"Failed to create meta: {error_message}")
 
-    def createOutline(self, request: CourseOutlineRequest,  output_name: str = None, load_exists=False) -> CourseTree:
+    def generateOutline(self, request: CourseOutlineRequest,  output_name: str = None, load_exists=False) -> CourseTree:
         """
         Creates a course outline.
 
         Args:
             request (CourseOutlineRequest): The request data for creating a course outline.
 
         Returns:
@@ -291,22 +291,25 @@
                     w.write(outline.model_dump_json(
                         indent=2, exclude_none=True))
             return outline
         except Exception as e:
             error_message = self._get_error_message(e)
             raise Exception(f"Failed to create outline: {error_message}")
 
-    def createActivity(self, request: ActivityRequest,  output_name: str = None, load_exists=False) -> Activities:
+    def generateActivity3(self, request, o):
+        print ("ddd")
+
+    def generateActivity1(self, request: ActivityRequest,  output_name: str = None, load_exists=False) -> Activities:
         """
         Creates course activities individually.
         """
         try:
             if os.path.exists(f"{stucent_dir}/activity_{output_name}.json"):
                 with open(f"{stucent_dir}/activity_{output_name}.json", "r") as r:
-                    return CourseTree.model_validate_json(r.read())
+                    return Activities.model_validate_json(r.read())
             response = self._post("/generate/activity", request.model_dump())
             usage = response.get('usage', {})
             self.last_usage['activity'] = usage
             activitis = Activities(**response['data'])
             if output_name:
                 with open(f"{stucent_dir}/activity_{output_name}.json", "w") as w:
                     w.write(activitis.model_dump_json(
@@ -333,20 +336,20 @@
             self.last_usage[response.get('id', 'last')] = usage
             return TaskStatusResponse(**response)
         except Exception as e:
             error_message = self._get_error_message(e)
             raise Exception(
                 f"Failed to generate lesson activities: {error_message}")
 
-    def generateCourseActivities(self, request: CompleteCourseContentRequest,  output_name: str = None, load_exists=False) -> TaskStatusResponse:
+    def generateCourseActivities(self, request: CourseActivitiesRequest,  output_name: str = None, load_exists=False) -> TaskStatusResponse:
         """
         Initiates the generation of course activities and returns the task status.
 
         Args:
-            request (CompleteCourseContentRequest): The request data for course activities generation.
+            request (CourseActivitiesRequest): The request data for course activities generation.
 
         Returns:
             TaskStatusResponse: The status of the course activities generation task.
         """
         try:
             if os.path.exists(f"{stucent_dir}/task_{output_name}.json"):
                 with open(f"{stucent_dir}/task_{output_name}.json", "r") as r:
@@ -359,20 +362,20 @@
             task = TaskStatusResponse(**response)
             return task
         except Exception as e:
             error_message = self._get_error_message(e)
             raise Exception(
                 f"Failed to generate course activities: {error_message}")
 
-    def generateDebugCourseActivities(self, request: CompleteCourseContentRequest) -> TaskStatusResponse:
+    def generateDebugCourseActivities(self, request: CourseActivitiesRequest) -> TaskStatusResponse:
         """
         Initiates the generation of course activities and returns the task status.
 
         Args:
-            request (CompleteCourseContentRequest): The request data for course activities generation.
+            request (CourseActivitiesRequest): The request data for course activities generation.
 
         Returns:
             TaskStatusResponse: The status of the course activities generation task.
         """
         try:
             response = self._post("/debug/course-activities", request.dict())
             return TaskStatusResponse(**response)
@@ -436,15 +439,15 @@
             raise Exception(f"Failed to get template content: {error_message}")
         # response = requests.get(
         #     url=f"{self.base_url}/templates/{target}/{template_name}", headers=self.headers
         # )
         # response.raise_for_status()
         # return response.text
 
-    def createOutlineSchema(self, request: SchemaRequest) -> dict:
+    def generateOutlineSchema(self, request: SchemaRequest) -> dict:
         """
         Creates a course outline schema.
 
         Args:
             request (SchemaRequest): The request data for creating an outline schema.
 
         Returns:
```

