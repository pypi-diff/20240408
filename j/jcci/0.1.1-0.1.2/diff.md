# Comparing `tmp/jcci-0.1.1.tar.gz` & `tmp/jcci-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.1.1.tar", last modified: Sun Apr  7 05:17:55 2024, max compression
+gzip compressed data, was "jcci-0.1.2.tar", last modified: Mon Apr  8 04:32:48 2024, max compression
```

## Comparing `jcci-0.1.1.tar` & `jcci-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.603564 jcci-0.1.1/
--rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    15240 2024-04-07 05:17:55.602564 jcci-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3903 2024-04-03 10:11:39.000000 jcci-0.1.1/README.md
--rw-rw-rw-   0        0        0     1448 2024-04-07 05:17:43.000000 jcci-0.1.1/README.pypi.md
--rw-rw-rw-   0        0        0      763 2024-04-07 05:17:03.000000 jcci-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 05:17:55.604564 jcci-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.556818 jcci-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.587564 jcci-0.1.1/src/jcci/
--rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.1/src/jcci/__init__.py
--rw-rw-rw-   0        0        0    39584 2024-04-07 05:01:16.000000 jcci-0.1.1/src/jcci/analyze.py
--rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.1/src/jcci/config.py
--rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.1/src/jcci/constant.py
--rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.1/src/jcci/database.py
--rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.1/src/jcci/diff_parse.py
--rw-rw-rw-   0        0        0     7847 2024-03-25 09:09:49.000000 jcci-0.1.1/src/jcci/graph.py
--rw-rw-rw-   0        0        0    38308 2024-04-03 09:15:40.000000 jcci-0.1.1/src/jcci/java_parse.py
--rw-rw-rw-   0        0        0     4117 2023-08-07 08:01:30.000000 jcci-0.1.1/src/jcci/mapper_parse.py
--rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.1/src/jcci/sql.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.600564 jcci-0.1.1/src/jcci.egg-info/
--rw-rw-rw-   0        0        0    15240 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.597566 jcci-0.1.1/test/
--rw-rw-rw-   0        0        0     2525 2024-01-18 02:12:50.000000 jcci-0.1.1/test/test_case.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.967731 jcci-0.1.2/
+-rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    15384 2024-04-08 04:32:48.965735 jcci-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4471 2024-04-08 04:32:29.000000 jcci-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1592 2024-04-08 04:32:29.000000 jcci-0.1.2/README.pypi.md
+-rw-rw-rw-   0        0        0      763 2024-04-08 04:32:29.000000 jcci-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 04:32:48.968731 jcci-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.921731 jcci-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.950732 jcci-0.1.2/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.2/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    45109 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.2/src/jcci/config.py
+-rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.2/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.2/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.2/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     7935 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    38345 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4371 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.2/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.962733 jcci-0.1.2/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0    15384 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.960731 jcci-0.1.2/test/
+-rw-rw-rw-   0        0        0     2525 2024-01-18 02:12:50.000000 jcci-0.1.2/test/test_case.py
```

### Comparing `jcci-0.1.1/LICENSE` & `jcci-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.1.1/PKG-INFO` & `jcci-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.1
+Version: 0.1.2
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -234,13 +234,16 @@
 commit_analyze = JCCI('git@xxxx.git', 'username1')
 commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
 
 # To analyze the impact of methods in a class, use the analyze_class_method method. The last parameter is the line number(s) of the method(s) you want to analyze. If multiple methods are specified, separate their line numbers with commas. If left blank, it will analyze the impact of the entire class.
 class_analyze = JCCI('git@xxxx.git', 'username1')
 class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
+# Compare different branches
+branch_analyze = JCCI('git@xxxx.git', 'username1')
+branch_analyze.analyze_two_branch('branch_new','branch_old')
 ```
 
 At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format xxxx.cci, 
 which contains the tree diagram data generated by the analysis results, download [jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) , 
 upload analyze result file end with .cci, then can be displayed through the view.
```

### Comparing `jcci-0.1.1/README.md` & `jcci-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbaikaishuipp%2Fjcci&countColor=%23263759)
+
 #### [中文简体](https://github.com/baikaishuipp/jcci/blob/main/README.md) OR [English](https://github.com/baikaishuipp/jcci/blob/main/README.en.md)
 # jcci
 
 #### 介绍
 Java代码提交影响分析，是一个纯python库，分析Java项目的两次git提交差异对项目的影响，并生成树形图数据。
 
 PYPI: [jcci](https://pypi.org/project/jcci/) （会落后github几个版本）
@@ -45,14 +47,17 @@
 commit_analyze = JCCI('git@xxxx.git', 'username1')
 commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
 
 # 分析一个类的方法影响, analyze_class_method方法最后参数为方法所在行数，不同方法行数用逗号分割，不填则分析完整类影响
 class_analyze = JCCI('git@xxxx.git', 'username1')
 class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
+# 不同分支比较
+branch_analyze = JCCI('git@xxxx.git', 'username1')
+branch_analyze.analyze_two_branch('branch_new','branch_old')
 ```
 
 ##### 方式2：克隆项目（推荐此种方式）
 项目克隆下来后，新建python文件，引入jcci项目src目录下的jcci
 ```
 from path.to.jcci.src.jcci.analyze import JCCI
 
@@ -60,21 +65,28 @@
 commit_analyze = JCCI('git@xxxx.git', 'username1')
 commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
 
 # 分析一个类的方法影响, analyze_class_method方法最后参数为方法所在行数，不同方法行数用逗号分割，不填则分析完整类影响
 class_analyze = JCCI('git@xxxx.git', 'username1')
 class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
+# 不同分支比较
+branch_analyze = JCCI('git@xxxx.git', 'username1')
+branch_analyze.analyze_two_branch('branch_new','branch_old')
 ```
 ###### 参数说明：
 * project_git_url - 项目git地址，代码使用本机git配置clone代码，确保本机git权限或通过用户名密码/token的方式拼接url来clone代码。示例：https://userName:password@github.com/xxx.git 或 https://token@github.com/xxx.git
 * username1 - 随便输入，为了避免并发分析同一项目导致结果错误，用户1分析项目A时，用户B需要等待，所以设置了该参数
 
 运行时，会将项目克隆到目录中，然后进行分析，生成后缀格式为.cci的文件，其中包含分析结果生成的关系图数据，下载[jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) ，选择分析结果的.cci文件，即可可通过视图显示。
 
 #### 开源不易，如本工具对您有帮助，请点一下右上角 star ⭐ , 也可以请作者喝杯咖啡，谢谢~~~
 ![请作者喝咖啡](./images/donation.png)
 
 #### 沟通交流
 扫码加微信，备注：JCCI微信群交流
 
 ![微信交流群](./images/wechat.jpg) 
+
+#### Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=baikaishuipp/jcci&type=Date)](https://star-history.com/#baikaishuipp/jcci&Date)
```

### Comparing `jcci-0.1.1/README.pypi.md` & `jcci-0.1.2/README.pypi.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,13 +17,16 @@
 commit_analyze = JCCI('git@xxxx.git', 'username1')
 commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
 
 # To analyze the impact of methods in a class, use the analyze_class_method method. The last parameter is the line number(s) of the method(s) you want to analyze. If multiple methods are specified, separate their line numbers with commas. If left blank, it will analyze the impact of the entire class.
 class_analyze = JCCI('git@xxxx.git', 'username1')
 class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
+# Compare different branches
+branch_analyze = JCCI('git@xxxx.git', 'username1')
+branch_analyze.analyze_two_branch('branch_new','branch_old')
 ```
 
 At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format xxxx.cci, 
 which contains the tree diagram data generated by the analysis results, download [jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) , 
 upload analyze result file end with .cci, then can be displayed through the view.
```

### Comparing `jcci-0.1.1/pyproject.toml` & `jcci-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `jcci-0.1.1/src/jcci/analyze.py` & `jcci-0.1.2/src/jcci/analyze.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,23 +84,37 @@
         logging.info(f'Git diff between {commit_first} and {commit_second}')
         diff_base = f'cd {self.file_path} && git diff {commit_second}..{commit_first} > diff_{commit_second}..{commit_first}.txt'
         os.system(diff_base)
         diff_txt = os.path.join(self.file_path, f'diff_{commit_second}..{commit_first}.txt')
         logging.info(f'Analyzing diff file, location: {diff_txt}')
         return diff_parse.get_diff_info(diff_txt)
 
+    # Step 2
+    def _get_branch_diff_parse_map(self, filepath, branch_first, branch_second):
+        logging.info('Git pull project to HEAD')
+        os.system(f'cd {filepath} && git fetch --all && git checkout -b {branch_second} origin/{branch_second} && git checkout {branch_second} && git pull')
+        time.sleep(1)
+        os.system(f'cd {filepath} && git fetch --all && git checkout -b {branch_first} origin/{branch_first} && git checkout {branch_first} && git pull')
+        time.sleep(1)
+        logging.info(f'Git diff between {branch_first} and {branch_second}')
+        diff_base = f'cd {self.file_path} && git diff {branch_second}..{branch_first} > diff_{branch_second.replace("/", "#")}..{branch_first.replace("/", "#")}.txt'
+        os.system(diff_base)
+        diff_txt = os.path.join(self.file_path, f'diff_{branch_second.replace("/", "#")}..{branch_first.replace("/", "#")}.txt')
+        logging.info(f'Analyzing diff file, location: {diff_txt}')
+        return diff_parse.get_diff_info(diff_txt)
+
     # Step 3
     def _parse_project(self, project_dir, new_commit_or_branch, old_commit_or_branch):
         # 解析最新的项目文件
         os.system(f'cd {project_dir} && git reset --hard {new_commit_or_branch}')
         time.sleep(2)
         file_path_list = self._get_project_files(project_dir)
         diff_xml_file_path = [key for key in file_path_list if key.endswith('.xml') and any(key.endswith(diff_path) for diff_path in self.diff_parse_map.keys())]
         java_parse = JavaParse(self.sqlite.db_path, self.project_id)
-        # java_parse.parse_java_file_list(file_path_list, new_commit_or_branch)
+        java_parse.parse_java_file_list(file_path_list, new_commit_or_branch)
         xml_parse_result_new = self._parse_xml_file(diff_xml_file_path)
         xml_parse_result_old = {}
         if not old_commit_or_branch:
             return xml_parse_result_new, xml_parse_result_old
         # 解析旧版本有差异的文件
         os.system(f'cd {project_dir} && git reset --hard {old_commit_or_branch}')
         time.sleep(2)
@@ -109,14 +123,36 @@
             matched_file_path_list = [filepath for filepath in file_path_list if filepath.endswith(key)]
             if not matched_file_path_list:
                 continue
             matched_file_path = matched_file_path_list[0]
             java_parse.parse_java_file(matched_file_path, old_commit_or_branch)
         return xml_parse_result_new, xml_parse_result_old
 
+    # Step 3
+    def _parse_branch_project(self, project_dir, new_branch, old_branch):
+        # 解析最新的项目文件
+        os.system(f'cd {project_dir} && git checkout {new_branch}')
+        time.sleep(2)
+        file_path_list = self._get_project_files(project_dir)
+        diff_xml_file_path = [key for key in file_path_list if key.endswith('.xml') and any(key.endswith(diff_path) for diff_path in self.diff_parse_map.keys())]
+        java_parse = JavaParse(self.sqlite.db_path, self.project_id)
+        java_parse.parse_java_file_list(file_path_list, new_branch)
+        xml_parse_result_new = self._parse_xml_file(diff_xml_file_path)
+        # 解析旧版本有差异的文件
+        os.system(f'cd {project_dir} && git checkout {old_branch}')
+        time.sleep(2)
+        xml_parse_result_old = self._parse_xml_file(diff_xml_file_path)
+        for key in self.diff_parse_map.keys():
+            matched_file_path_list = [filepath for filepath in file_path_list if filepath.endswith(key)]
+            if not matched_file_path_list:
+                continue
+            matched_file_path = matched_file_path_list[0]
+            java_parse.parse_java_file(matched_file_path, old_branch)
+        return xml_parse_result_new, xml_parse_result_old
+
     # Step 3.1 get all java files
     def _get_project_files(self, project_dir):
         file_lists = []
         for root, dirs, files in os.walk(project_dir):
             if '.git' in root or os.path.join('src', 'test') in root:
                 continue
             for file in files:
@@ -133,15 +169,16 @@
 
     # Step 3.3
     def _parse_xml_file(self, file_path_list):
         xml_parse_results = {}
         for filepath in file_path_list:
             if filepath.endswith('.xml'):
                 xml_parse_result = mapper_parse.parse(filepath)
-                xml_parse_results[filepath] = xml_parse_result
+                if xml_parse_result:
+                    xml_parse_results[filepath] = xml_parse_result
         return xml_parse_results
 
     # Step 4
     def _diff_analyze(self, patch_filepath: str, diff_parse_obj: dict):
         is_xml_file = patch_filepath.endswith('.xml')
         if is_xml_file:
             self._xml_diff_analyze(patch_filepath, diff_parse_obj)
@@ -255,14 +292,16 @@
         file_type = need_analyze_obj['file_type']
         package_class = need_analyze_obj['package_class']
         commit_or_branch = need_analyze_obj['commit_or_branch']
         package_name = '.'.join(package_class.split('.')[0: -1])
         class_name = package_class.split('.')[-1]
         class_db_list = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id = {self.project_id} and class_name="{class_name}" and package_name="{package_name}"')
         class_entity = self._get_right_class_entity(class_db_list, commit_or_branch)
+        if not class_entity:
+            return
         class_filepath = class_entity['filepath']
         class_id = class_entity["class_id"]
         # gengxin
         commit_or_branch = class_entity['commit_or_branch']
         is_controller = class_entity['is_controller']
         # todo 粗查，待细化
         if file_type == 'xml':
@@ -304,21 +343,23 @@
                 method_name: str = method_param.split('(')[0]
                 method_node_id = need_analyze_obj.get('method_node_id')
                 source_node_id = method_node_id
                 entity_impacted_methods = self._get_method_invocation_in_methods_table(package_class, method_param, commit_or_branch)
                 method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE method_id = {need_analyze_obj.get("method_id")}')[0]
                 is_override_method = 'Override' in method_db['annotations']
                 if is_override_method:
+
                     if class_entity['extends_class']:
                         abstract_package_class = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'True', commit_or_branch)
                         if abstract_package_class:
                             extends_methods = self._get_method_invocation_in_methods_table(abstract_package_class, method_param, commit_or_branch)
                             for method in extends_methods:
                                 method['class_id'] = class_id
                             entity_impacted_methods += extends_methods
+
                     if class_entity['implements']:
                         class_implements = class_entity['implements'].split(',')
                         class_implements_obj = self.sqlite.select_data(f'''select c.package_name , c.class_name from methods m left join class c on c.class_id = m.class_id 
                                                 where c.project_id = {self.project_id} and m.method_name = '{method_name}' and c.class_name in ("{'","'.join(class_implements)}")''')
                         if class_implements_obj:
                             implements_package_class = class_implements_obj[0].get('package_name') + '.' + class_implements_obj[0].get('class_name')
                             implements_methods = self._get_method_invocation_in_methods_table(implements_package_class, method_param, commit_or_branch)
@@ -430,73 +471,107 @@
     def _gen_all_possible_method_param_list(self, method_param):
         method_param_list = []
         method_name = method_param.split('(')[0]
         param_type_str = method_param.split('(')[1].split(')')[0]
         param_type_list = param_type_str.split(',')
         if not param_type_list:
             return method_param_list
-        all_possible_method_param_list = self._replace_with_null(param_type_list)
-        for param_type_list in all_possible_method_param_list:
+        all_possible_method_param_list = []
+        self._replace_with_unknown(param_type_list, all_possible_method_param_list, 0)
+        lst = list(set(tuple(sub_list) for sub_list in all_possible_method_param_list))
+        for param_type_list in lst:
             method_param_list.append(f'{method_name}({",".join(param_type_list)})')
         return method_param_list
 
     def _replace_with_null(self, lst):
         # lst = [item.split('<')[0].replace('<', '').replace('>', '') for item in lst]
         results = []
         lowercase_indices = [i for i, s in enumerate(lst) if s and s[0].islower()]  # 首字母小写的元素索引
 
         for num_replacements in range(len(lst) + 1):  # 遍历替换0到所有元素的情况
             replaceable_indices = [i for i in range(len(lst)) if i not in lowercase_indices]  # 可替换的元素索引
             for replace_indices in combinations(replaceable_indices, num_replacements):  # 所有可能的替换索引组合
                 new_lst = lst[:]  # 创建原始列表的副本
                 for idx in replace_indices:
                     if new_lst[idx].lower() not in constant.JAVA_BASIC_TYPE:
+                        if new_lst[idx].startswith('List'):
+                            new_lst2 = new_lst[:]
+                            new_lst2[idx] = 'ArrayList'
+                            results.append(new_lst2)
+                        elif new_lst[idx].startswith('Map'):
+                            new_lst2 = new_lst[:]
+                            new_lst2[idx] = 'HashMap'
+                            results.append(new_lst2)
+                        elif new_lst[idx].startswith('Set'):
+                            new_lst2 = new_lst[:]
+                            new_lst2[idx] = 'HashSet'
+                            results.append(new_lst2)
                         new_lst[idx] = constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
                     else:
-                        new_lst[idx] = 'null'
                         new_lst2 = new_lst[:]
                         new_lst2[idx] = constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
                         results.append(new_lst2)
+                        new_lst[idx] = 'null'
                         self._replace_extends_class(new_lst2, results)
                 results.append(new_lst)
                 self._replace_extends_class(new_lst, results)
+        results.append([constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN for _ in lst])
         return results
 
     def _replace_extends_class(self, new_lst, results):
         for i in range(0, len(new_lst)):
             if new_lst[i].lower() in constant.JAVA_BASIC_TYPE \
                     or new_lst[i] == constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN \
                     or new_lst[i] == 'null':
                 continue
             extends_package_class_list = self._get_extends_package_class(new_lst[i])
             for extends_package_class in extends_package_class_list:
                 result_item = [item for item in new_lst]
                 result_item[i] = extends_package_class
                 results.append(result_item)
 
+    def _is_duplicate_item(self, new_lst, lst):
+        is_duplicate = False
+        for item in lst:
+            if item == new_lst:
+                is_duplicate = True
+                break
+        return is_duplicate
+
     # Step 5.4.1.1
-    def _replace_with_unknown(self, data: list):
+    def _replace_with_unknown(self, lst: list, results: list, idx: int):
         # data = [item.split('<')[0].replace('<', '').replace('>', '') for item in data]
-        results = [data]
-        for i in range(0, len(data)):
-            result_item = [item for item in data]
-            if data[i].lower() not in constant.JAVA_BASIC_TYPE:
-                result_item[i] = constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
-            elif data[i][0].isupper():
-                result_item[i] = 'null'
-            results.append(result_item)
-        for i in range(0, len(data)):
-            if data[i].lower() in constant.JAVA_BASIC_TYPE:
-                continue
-            extends_package_class_list = self._get_extends_package_class(data[i])
-            for extends_package_class in extends_package_class_list:
-                result_item = [item for item in data]
-                result_item[i] = extends_package_class
-                results.append(result_item)
-        return results
+        for i in range(idx, len(lst)):
+            new_lst = lst[:]
+            if not self._is_duplicate_item(new_lst, results):
+                results.append(new_lst)
+            if new_lst[i].lower() not in constant.JAVA_BASIC_TYPE:
+                new_lst2 = new_lst[:]
+                if new_lst[i].startswith('List'):
+                    new_lst2[i] = 'ArrayList'
+                elif new_lst[i].startswith('Map'):
+                    new_lst2[i] = 'HashMap'
+                elif new_lst[i].startswith('Set'):
+                    new_lst2[i] = 'HashSet'
+                if not self._is_duplicate_item(new_lst2, results):
+                    results.append(new_lst2)
+                    self._replace_with_unknown(new_lst2, results, idx)
+            else:
+                if new_lst[i][0].isupper() and new_lst[i] != 'String':
+                    new_lst2 = new_lst[:]
+                    new_lst2[i] = new_lst[i][0].lower() + new_lst[i][1:]
+                    if not self._is_duplicate_item(new_lst2, results):
+                        results.append(new_lst2)
+                        self._replace_with_unknown(new_lst2, results, idx)
+            for el in ['null', 'unknown']:
+                new_lst_tmp = new_lst[:]
+                new_lst_tmp[i] = el
+                if not self._is_duplicate_item(new_lst_tmp, results):
+                    results.append(new_lst_tmp)
+                    self._replace_with_unknown(new_lst_tmp, results, min(idx, len(new_lst) - 1))
 
     # Step 5.5
     def _get_method_param_string(self, method_db: dict):
         method_name: str = method_db['method_name']
         params: list = json.loads(method_db['parameters'])
         params_type_list = [param['parameter_type'] for param in params]
         return f'{method_name}({",".join(params_type_list)})'
@@ -574,14 +649,34 @@
         try:
             logging.info(f'Analyze done, remove occupy, others can analyze now')
             os.remove(os.path.join(self.file_path, 'Occupy.ing'))
         finally:
             pass
         logging.info(f'Analyze done, spend: {t2 - self.t1}')
 
+    def analyze_two_branch(self, branch_first, branch_second):
+        logging.info('*' * 10 + 'Analyze start' + '*' * 10)
+        self.commit_or_branch_new = branch_first
+        self.commit_or_branch_old = branch_second
+        self.branch_name = branch_first
+        self.project_name = self.git_url.split('/')[-1].split('.git')[0]
+        self.file_path = os.path.join(project_path, self.project_name)
+        self.project_id = self.sqlite.add_project(self.project_name, self.git_url, self.branch_name, branch_first, branch_second)
+        # 已有分析结果
+        self.cci_filepath = os.path.join(self.file_path, f'{branch_second.replace("/", "#")}..{branch_first.replace("/", "#")}.cci')
+        self._can_analyze(self.file_path, self.cci_filepath)
+        # 无此项目, 先clone项目
+        if not os.path.exists(self.file_path):
+            logging.info(f'Cloning project: {self.git_url}')
+            os.system(f'git clone -b {branch_first} {self.git_url} {self.file_path}')
+        self._occupy_project()
+        self.diff_parse_map = self._get_branch_diff_parse_map(self.file_path, branch_first, branch_second)
+        self.xml_parse_results_new, self.xml_parse_results_old = self._parse_branch_project(self.file_path, branch_first, branch_second)
+        self._start_analysis_diff_and_impact()
+
     def analyze_two_commit(self, branch, commit_first, commit_second):
         logging.info('*' * 10 + 'Analyze start' + '*' * 10)
         self.branch_name = branch
         self.commit_or_branch_new = commit_first[0: 7] if len(commit_first) > 7 else commit_first
         self.commit_or_branch_old = commit_second[0: 7] if len(commit_second) > 7 else commit_second
 
         self.project_name = self.git_url.split('/')[-1].split('.git')[0]
```

### Comparing `jcci-0.1.1/src/jcci/constant.py` & `jcci-0.1.2/src/jcci/constant.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.1/src/jcci/database.py` & `jcci-0.1.2/src/jcci/database.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.1/src/jcci/diff_parse.py` & `jcci-0.1.2/src/jcci/diff_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.1/src/jcci/graph.py` & `jcci-0.1.2/src/jcci/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import src.jcci.constant as constant
 from collections import deque
 
 def max_relationship_length(relationships):
+    if not relationships:
+        return {}
     # 构建邻接列表
     graph = {}
     for relationship in relationships:
         source = relationship['source']
         target = relationship['target']
         if source not in graph:
             graph[source] = []
@@ -98,42 +100,42 @@
             changed_node['x'] = 100
             changed_node['y'] = (changed_nodes.index(changed_node) + 1) * (canvas_height / len(changed_nodes))
             changed_node['symbolSize'] = 20
             changed_node['label'] = {
                 'show': True,
                 'formatter': changed_node["name"].split("(")[0]
             }
-            tooltip = f'{changed_node["name"].split("(")[0]}<br>[Changed]{changed_node["diff_content"]}'
+            tooltip = f'{changed_node["name"].split("(")[0]}<br>[Changed]{changed_node.get("diff_content", "")}'
             if changed_node.get('is_api'):
-                tooltip = tooltip + f'<br>[API]{changed_node["api_path"]}'
+                tooltip = tooltip + f'<br>[API]{changed_node.get("api_path")}'
             changed_node['tooltip'] = {
                 'show': True,
                 'position': 'right',
                 'formatter': tooltip
             }
             all_node.append(changed_node)
-        max_link_count = max([value for key, value in result.items()])
+        max_link_count = max([value for key, value in result.items()]) if result else 1
         count_node_result = {}
         for key, value in result.items():
             value = str(value)
             if value not in count_node_result:
                 count_node_result[value] = []
             count_node_result[value].append(key)
         for impacted_node in impacted_nodes:
             path_level = result.get(impacted_node['id'], 0)
             level_node_list = count_node_result.get(str(path_level), [impacted_node['id']])
             level_node_index = level_node_list.index(impacted_node['id']) if impacted_node['id'] in level_node_list else 1
             impacted_node['x'] = 100 + ((canvas_width - 100) / max_link_count) * (path_level + 1)
-            impacted_node['y'] = (canvas_height / len(count_node_result[str(path_level)])) * level_node_index
+            impacted_node['y'] = (canvas_height / len(count_node_result.get(str(path_level), [1]))) * level_node_index
             impacted_node['label'] = {
                 'show': True,
                 'formatter': impacted_node["name"].split("(")[0]
             }
             if impacted_node.get('is_api'):
-                tooltip = f'{impacted_node["name"].split("(")[0]}<br>[API]{impacted_node["api_path"]}'
+                tooltip = f'{impacted_node["name"].split("(")[0]}<br>[API]{impacted_node.get("api_path")}'
                 impacted_node['tooltip'] = {
                     'show': True,
                     'position': 'right',
                     'formatter': tooltip
                 }
             all_node.append(impacted_node)
         self.nodes = all_node
```

### Comparing `jcci-0.1.1/src/jcci/java_parse.py` & `jcci-0.1.2/src/jcci/java_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,15 +571,15 @@
             start_line = field_map.get(var)['start_line']
             self._add_field_used_to_method_invocation(method_invocation, package_class, var, [start_line])
             return field_type
         if var in import_map.keys():
             var_type = import_map.get(var)
             self._add_entity_used_to_method_invocation(method_invocation, var_type, section)
             return var_type
-        return var
+        return PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
 
     def _get_extends_class_fields_map(self, class_id: int):
         class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
         extend_package_class = class_db['extends_class']
         if not extend_package_class:
             return {}
         extend_package = '.'.join(extend_package_class.split('.')[0: -1])
```

### Comparing `jcci-0.1.1/src/jcci/mapper_parse.py` & `jcci-0.1.2/src/jcci/mapper_parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 import xml.etree.ElementTree as ET
-
+import re
 
 class Mapper(object):
     def __init__(self, namespace, result_maps, sqls, statements):
         self.namespace = namespace
         self.result_maps = result_maps
         self.sqls = sqls
         self.statements = statements
@@ -24,19 +24,30 @@
 class MapperStatement(MapperElement):
     def __init__(self, id, type, start_line, end_line, content, statement_tag, result_map, include_sql):
         super(MapperStatement, self).__init__(id, type, start_line, end_line, content)
         self.statement_tag = statement_tag
         self.result_map = result_map
         self.include_sql = include_sql
 
+def extract_value(string, tag):
+    pattern = tag + r'\s*=\s*"(\w+)"'
+    match = re.search(pattern, string)
+    if match:
+        value = match.group(1)
+        return value
+    else:
+        return None
 
 def parse(filepath):
     # 读取XML文件内容
-    with open(filepath, "r", encoding="utf-8") as file:
-        xml_content = file.read()
+    try:
+        with open(filepath, "r", encoding="utf-8") as file:
+            xml_content = file.read()
+    except:
+        return None
 
     # 解析XML文件
     tree = ET.ElementTree(ET.fromstring(xml_content))
     root = tree.getroot()
 
     # 获取namespace
     try:
@@ -86,17 +97,17 @@
         end_line = 0
         result_map = None
         include_sql = None
         for i, line in enumerate(xml_content.splitlines(), start=1):
             if f'<{statement_element.tag} id="{statement_id}"' in line:
                 start_line = i
             if f'resultMap="' in line and start_line != 0:
-                result_map = line.split('resultMap="')[1].split('"')[0]
+                result_map = extract_value(line, 'resultMap')
             if line.strip().startswith('<include') and start_line != 0:
-                include_sql = line.split('refid="')[1].split('"')[0]
+                include_sql = extract_value(line, 'refid')
             if f'</{statement_element.tag}>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         statement_info.append(MapperStatement(statement_id, 'statement', start_line, end_line, content, statement_element.tag, result_map, include_sql))
 
     return Mapper(namespace, result_map_info, sql_info, statement_info)
```

### Comparing `jcci-0.1.1/src/jcci/sql.py` & `jcci-0.1.2/src/jcci/sql.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.1/src/jcci.egg-info/PKG-INFO` & `jcci-0.1.2/src/jcci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.1
+Version: 0.1.2
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -234,13 +234,16 @@
 commit_analyze = JCCI('git@xxxx.git', 'username1')
 commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
 
 # To analyze the impact of methods in a class, use the analyze_class_method method. The last parameter is the line number(s) of the method(s) you want to analyze. If multiple methods are specified, separate their line numbers with commas. If left blank, it will analyze the impact of the entire class.
 class_analyze = JCCI('git@xxxx.git', 'username1')
 class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
+# Compare different branches
+branch_analyze = JCCI('git@xxxx.git', 'username1')
+branch_analyze.analyze_two_branch('branch_new','branch_old')
 ```
 
 At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format xxxx.cci, 
 which contains the tree diagram data generated by the analysis results, download [jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) , 
 upload analyze result file end with .cci, then can be displayed through the view.
```

### Comparing `jcci-0.1.1/test/test_case.py` & `jcci-0.1.2/test/test_case.py`

 * *Files identical despite different names*

