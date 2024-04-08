# Comparing `tmp/jcci-0.1.0.tar.gz` & `tmp/jcci-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.1.0.tar", last modified: Wed Apr  3 09:29:42 2024, max compression
+gzip compressed data, was "jcci-0.1.1.tar", last modified: Sun Apr  7 05:17:55 2024, max compression
```

## Comparing `jcci-0.1.0.tar` & `jcci-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.948499 jcci-0.1.0/
--rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3087 2024-04-03 09:29:42.946500 jcci-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3412 2024-04-03 09:26:49.000000 jcci-0.1.0/README.md
--rw-rw-rw-   0        0        0     1186 2023-12-15 07:51:52.000000 jcci-0.1.0/README.pypi.md
--rw-rw-rw-   0        0        0      763 2024-04-03 09:18:17.000000 jcci-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 09:29:42.948499 jcci-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.912501 jcci-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.934500 jcci-0.1.0/src/jcci/
--rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.0/src/jcci/__init__.py
--rw-rw-rw-   0        0        0    38366 2024-04-03 09:21:22.000000 jcci-0.1.0/src/jcci/analyze.py
--rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.0/src/jcci/config.py
--rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.0/src/jcci/constant.py
--rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.0/src/jcci/database.py
--rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.0/src/jcci/diff_parse.py
--rw-rw-rw-   0        0        0     7847 2024-03-25 09:09:49.000000 jcci-0.1.0/src/jcci/graph.py
--rw-rw-rw-   0        0        0    38308 2024-04-03 09:15:40.000000 jcci-0.1.0/src/jcci/java_parse.py
--rw-rw-rw-   0        0        0     4117 2023-08-07 08:01:30.000000 jcci-0.1.0/src/jcci/mapper_parse.py
--rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.0/src/jcci/sql.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.945500 jcci-0.1.0/src/jcci.egg-info/
--rw-rw-rw-   0        0        0     3087 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.942499 jcci-0.1.0/test/
--rw-rw-rw-   0        0        0     2525 2024-01-18 02:12:50.000000 jcci-0.1.0/test/test_case.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.603564 jcci-0.1.1/
+-rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    15240 2024-04-07 05:17:55.602564 jcci-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3903 2024-04-03 10:11:39.000000 jcci-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1448 2024-04-07 05:17:43.000000 jcci-0.1.1/README.pypi.md
+-rw-rw-rw-   0        0        0      763 2024-04-07 05:17:03.000000 jcci-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 05:17:55.604564 jcci-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.556818 jcci-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.587564 jcci-0.1.1/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.1/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    39584 2024-04-07 05:01:16.000000 jcci-0.1.1/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.1/src/jcci/config.py
+-rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.1/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.1/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.1/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     7847 2024-03-25 09:09:49.000000 jcci-0.1.1/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    38308 2024-04-03 09:15:40.000000 jcci-0.1.1/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4117 2023-08-07 08:01:30.000000 jcci-0.1.1/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.1/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.600564 jcci-0.1.1/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0    15240 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-07 05:17:55.000000 jcci-0.1.1/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 05:17:55.597566 jcci-0.1.1/test/
+-rw-rw-rw-   0        0        0     2525 2024-01-18 02:12:50.000000 jcci-0.1.1/test/test_case.py
```

### Comparing `jcci-0.1.0/README.md` & `jcci-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 通过unidiff 解析git diff信息（diff file, added_line_num, removed_lin_num)
 
 然后根据文件增删的代码行去判断影响了哪些类和方法，不断遍历受影响的类和方法直至找到最上层的controller层
 
 通过传入项目git地址 分支 两次的commit id，即可分析出两次commit id之间代码改动所带来的影响，并生成树图数据方便展示影响链路。
 
 #### 安装教程
-
+要求python >= 3.9 , sqlite3 >= 3.38
 ##### 方式1：pypi安装（会落后github几个版本）
 ```
 $ pip install jcci
 ```
 
 ##### 方式2：克隆项目（推荐此种方式）
 ```
@@ -35,18 +35,23 @@
 ```
 
 #### 使用说明
 
 ##### 方式1：pypi安装（会落后github几个版本）
 新建python项目，新建python文件，代码如下：
 ```
-from jcci import jcci
+from jcci.analyze import JCCI
 
 # 同一分支不同commit比较
-jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+commit_analyze = JCCI('git@xxxx.git', 'username1')
+commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
+
+# 分析一个类的方法影响, analyze_class_method方法最后参数为方法所在行数，不同方法行数用逗号分割，不填则分析完整类影响
+class_analyze = JCCI('git@xxxx.git', 'username1')
+class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
 ```
 
 ##### 方式2：克隆项目（推荐此种方式）
 项目克隆下来后，新建python文件，引入jcci项目src目录下的jcci
 ```
 from path.to.jcci.src.jcci.analyze import JCCI
@@ -62,13 +67,14 @@
 ```
 ###### 参数说明：
 * project_git_url - 项目git地址，代码使用本机git配置clone代码，确保本机git权限或通过用户名密码/token的方式拼接url来clone代码。示例：https://userName:password@github.com/xxx.git 或 https://token@github.com/xxx.git
 * username1 - 随便输入，为了避免并发分析同一项目导致结果错误，用户1分析项目A时，用户B需要等待，所以设置了该参数
 
 运行时，会将项目克隆到目录中，然后进行分析，生成后缀格式为.cci的文件，其中包含分析结果生成的关系图数据，下载[jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) ，选择分析结果的.cci文件，即可可通过视图显示。
 
-#### 开源不易，如本工具对您有帮助，请点一下右上角 star ⭐ , 谢谢~~~
+#### 开源不易，如本工具对您有帮助，请点一下右上角 star ⭐ , 也可以请作者喝杯咖啡，谢谢~~~
+![请作者喝咖啡](./images/donation.png)
 
 #### 沟通交流
 扫码加微信，备注：JCCI微信群交流
 
 ![微信交流群](./images/wechat.jpg)
```

### Comparing `jcci-0.1.0/pyproject.toml` & `jcci-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `jcci-0.1.0/src/jcci/analyze.py` & `jcci-0.1.1/src/jcci/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def _parse_project(self, project_dir, new_commit_or_branch, old_commit_or_branch):
         # 解析最新的项目文件
         os.system(f'cd {project_dir} && git reset --hard {new_commit_or_branch}')
         time.sleep(2)
         file_path_list = self._get_project_files(project_dir)
         diff_xml_file_path = [key for key in file_path_list if key.endswith('.xml') and any(key.endswith(diff_path) for diff_path in self.diff_parse_map.keys())]
         java_parse = JavaParse(self.sqlite.db_path, self.project_id)
-        java_parse.parse_java_file_list(file_path_list, new_commit_or_branch)
+        # java_parse.parse_java_file_list(file_path_list, new_commit_or_branch)
         xml_parse_result_new = self._parse_xml_file(diff_xml_file_path)
         xml_parse_result_old = {}
         if not old_commit_or_branch:
             return xml_parse_result_new, xml_parse_result_old
         # 解析旧版本有差异的文件
         os.system(f'cd {project_dir} && git reset --hard {old_commit_or_branch}')
         time.sleep(2)
@@ -124,16 +124,15 @@
                 filepath = os.path.join(root, file)
                 for pattern in ignore_file:
                     if fnmatch.fnmatch(filepath, pattern):
                         ignore = True
                         break
                 if ignore:
                     continue
-                filepath.replace('\\', '/')
-                file_lists.append(filepath)
+                file_lists.append(filepath.replace('\\', '/'))
         return file_lists
 
     # Step 3.3
     def _parse_xml_file(self, file_path_list):
         xml_parse_results = {}
         for filepath in file_path_list:
             if filepath.endswith('.xml'):
@@ -147,15 +146,15 @@
         if is_xml_file:
             self._xml_diff_analyze(patch_filepath, diff_parse_obj)
         else:
             self._java_diff_analyze(patch_filepath, diff_parse_obj)
 
     # Step 4.1
     def _xml_diff_analyze(self, patch_filepath, diff_parse_obj: dict):
-        xml_file_path_list = [filepath for filepath in self.xml_parse_results_new.keys() if self.file_path.endswith(patch_filepath)]
+        xml_file_path_list = [filepath for filepath in self.xml_parse_results_new.keys() if filepath.endswith(patch_filepath)]
         if not xml_file_path_list:
             return
         xml_file_path = xml_file_path_list[0]
         xml_name = xml_file_path.split('/')[-1]
         xml_parse_result_new: mapper_parse.Mapper = self.xml_parse_results_new.get(xml_file_path)
         methods = xml_parse_result_new.result_maps + xml_parse_result_new.sqls + xml_parse_result_new.statements
         self._xml_method_diff_analyze(methods, diff_parse_obj['line_num_added'], diff_parse_obj['line_content_added'], xml_parse_result_new, xml_name, xml_file_path, self.commit_or_branch_new)
@@ -300,32 +299,41 @@
                 annotations: list = json.loads(class_entity['annotations'])
                 entity_impacted_methods = self._get_field_invocation_in_methods_table(package_class, need_analyze_obj, annotations, commit_or_branch)
                 source_node_id = need_analyze_obj.get('field_node_id')
             elif need_analyze_obj.get('method_param'):
                 method_param = need_analyze_obj.get('method_param')
                 method_name: str = method_param.split('(')[0]
                 method_node_id = need_analyze_obj.get('method_node_id')
+                source_node_id = method_node_id
                 entity_impacted_methods = self._get_method_invocation_in_methods_table(package_class, method_param, commit_or_branch)
                 method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE method_id = {need_analyze_obj.get("method_id")}')[0]
                 is_override_method = 'Override' in method_db['annotations']
-                if is_override_method and class_entity['extends_class']:
-                    abstract_package_class = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'True', commit_or_branch)
-                    if abstract_package_class:
-                        extends_methods = self._get_method_invocation_in_methods_table(abstract_package_class, method_param, commit_or_branch)
-                        for method in extends_methods:
-                            method['class_id'] = class_id
-                        entity_impacted_methods += extends_methods
+                if is_override_method:
+                    if class_entity['extends_class']:
+                        abstract_package_class = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'True', commit_or_branch)
+                        if abstract_package_class:
+                            extends_methods = self._get_method_invocation_in_methods_table(abstract_package_class, method_param, commit_or_branch)
+                            for method in extends_methods:
+                                method['class_id'] = class_id
+                            entity_impacted_methods += extends_methods
+                    if class_entity['implements']:
+                        class_implements = class_entity['implements'].split(',')
+                        class_implements_obj = self.sqlite.select_data(f'''select c.package_name , c.class_name from methods m left join class c on c.class_id = m.class_id 
+                                                where c.project_id = {self.project_id} and m.method_name = '{method_name}' and c.class_name in ("{'","'.join(class_implements)}")''')
+                        if class_implements_obj:
+                            implements_package_class = class_implements_obj[0].get('package_name') + '.' + class_implements_obj[0].get('class_name')
+                            implements_methods = self._get_method_invocation_in_methods_table(implements_package_class, method_param, commit_or_branch)
+                            entity_impacted_methods += implements_methods
                 else:
                     class_method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {class_id} and method_name = "{method_name}"')
                     if not class_method_db:
                         extends_package_class = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'False', commit_or_branch)
                         if extends_package_class:
                             extends_methods = self._get_method_invocation_in_methods_table(extends_package_class, method_param, commit_or_branch)
                             entity_impacted_methods += extends_methods
-                source_node_id = method_node_id
             if not entity_impacted_methods:
                 return
             self._handle_impacted_methods(entity_impacted_methods, source_node_id)
 
     def _is_method_param_in_extends_package_class(self, method_param, extends_package_class, is_abstract, commit_or_branch):
         method_name: str = method_param.split('(')[0]
         extends_package = '.'.join(extends_package_class.split('.')[0: -1])
@@ -520,18 +528,25 @@
         need_analyze_entity: dict = {
             'file_type': file_type,
             'package_class': package_class,
             'field_name': field_name,
             'method_param': method_param,
             'commit_or_branch': commit_or_branch
         }
-        if need_analyze_entity not in self.need_analyze_obj_list:
+        is_exist = [obj for obj in self.need_analyze_obj_list if self.check_dict_keys_equal_values(need_analyze_entity, obj)]
+        if not is_exist:
             need_analyze_entity.update(mapper_extend_dict)
             self.need_analyze_obj_list.append(need_analyze_entity)
 
+    def check_dict_keys_equal_values(self, dict1, dict2):
+        for key in dict1:
+            if key in dict2 and dict1[key] != dict2[key]:
+                return False
+        return True
+
     def _draw_and_write_result(self):
         if self.view.nodes:
             self.view.draw_graph(1200, 600)
         logging.info(f'Analyze success, generating cci result file......')
         result = {
             'nodes': self.view.nodes,
             'links': self.view.links,
```

### Comparing `jcci-0.1.0/src/jcci/constant.py` & `jcci-0.1.1/src/jcci/constant.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/src/jcci/database.py` & `jcci-0.1.1/src/jcci/database.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/src/jcci/diff_parse.py` & `jcci-0.1.1/src/jcci/diff_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/src/jcci/graph.py` & `jcci-0.1.1/src/jcci/graph.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/src/jcci/java_parse.py` & `jcci-0.1.1/src/jcci/java_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/src/jcci/mapper_parse.py` & `jcci-0.1.1/src/jcci/mapper_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/src/jcci/sql.py` & `jcci-0.1.1/src/jcci/sql.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.0/test/test_case.py` & `jcci-0.1.1/test/test_case.py`

 * *Files identical despite different names*

