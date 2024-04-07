# Comparing `tmp/dolphie-4.3.4.tar.gz` & `tmp/dolphie-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-4.3.4.tar", max compression
+gzip compressed data, was "dolphie-4.3.5.tar", max compression
```

## Comparing `dolphie-4.3.4.tar` & `dolphie-4.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-4.3.4/LICENSE
--rw-r--r--   0        0        0    10412 2024-03-02 09:52:23.105106 dolphie-4.3.4/README.md
--rw-r--r--   0        0        0     5425 2024-02-29 04:17:53.317177 dolphie-4.3.4/dolphie/DataTypes.py
--rw-r--r--   0        0        0     8108 2024-03-02 07:04:18.585838 dolphie-4.3.4/dolphie/Dolphie.css
--rw-r--r--   0        0        0    22016 2024-03-02 09:47:47.243202 dolphie-4.3.4/dolphie/Modules/ArgumentParser.py
--rw-r--r--   0        0        0     6770 2024-03-02 06:56:36.204962 dolphie-4.3.4/dolphie/Modules/Functions.py
--rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-4.3.4/dolphie/Modules/ManualException.py
--rw-r--r--   0        0        0    26287 2024-02-27 06:42:42.249716 dolphie-4.3.4/dolphie/Modules/MetricManager.py
--rw-r--r--   0        0        0     7438 2024-03-11 10:26:22.542650 dolphie-4.3.4/dolphie/Modules/MySQL.py
--rw-r--r--   0        0        0    17000 2024-03-02 10:44:31.780001 dolphie-4.3.4/dolphie/Modules/Queries.py
--rw-r--r--   0        0        0    23820 2024-03-02 06:25:14.219098 dolphie-4.3.4/dolphie/Modules/TabManager.py
--rw-r--r--   0        0        0     9270 2024-02-27 06:42:42.250655 dolphie-4.3.4/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-4.3.4/dolphie/Panels/ddl_panel.py
--rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-4.3.4/dolphie/Panels/innodb_trx_locks_panel.py
--rw-r--r--   0        0        0     6877 2024-03-02 10:45:55.398930 dolphie-4.3.4/dolphie/Panels/metadata_locks_panel.py
--rw-r--r--   0        0        0     9137 2024-02-29 04:18:16.735166 dolphie-4.3.4/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0    25774 2024-02-27 06:28:11.313610 dolphie-4.3.4/dolphie/Panels/replication_panel.py
--rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-4.3.4/dolphie/Widgets/command_screen.py
--rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-4.3.4/dolphie/Widgets/event_log_screen.py
--rw-r--r--   0        0        0    13757 2024-03-02 10:03:46.219361 dolphie-4.3.4/dolphie/Widgets/host_setup.py
--rw-r--r--   0        0        0    11260 2024-02-26 06:55:52.590875 dolphie-4.3.4/dolphie/Widgets/modal.py
--rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-4.3.4/dolphie/Widgets/spinner.py
--rw-r--r--   0        0        0     5926 2024-02-26 06:55:52.591850 dolphie-4.3.4/dolphie/Widgets/thread_screen.py
--rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-4.3.4/dolphie/Widgets/topbar.py
--rw-r--r--   0        0        0    11572 2024-02-27 06:42:42.251022 dolphie-4.3.4/dolphie/__init__.py
--rwxr-xr-x   0        0        0    66502 2024-02-29 09:42:26.387075 dolphie-4.3.4/dolphie/app.py
--rw-r--r--   0        0        0      645 2024-03-11 10:26:55.550248 dolphie-4.3.4/pyproject.toml
--rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 dolphie-4.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-4.3.5/LICENSE
+-rw-r--r--   0        0        0    10412 2024-03-02 09:52:23.105106 dolphie-4.3.5/README.md
+-rw-r--r--   0        0        0     5425 2024-02-29 04:17:53.317177 dolphie-4.3.5/dolphie/DataTypes.py
+-rw-r--r--   0        0        0     7998 2024-04-07 22:58:19.683385 dolphie-4.3.5/dolphie/Dolphie.css
+-rw-r--r--   0        0        0    22016 2024-03-02 09:47:47.243202 dolphie-4.3.5/dolphie/Modules/ArgumentParser.py
+-rw-r--r--   0        0        0     6770 2024-03-02 06:56:36.204962 dolphie-4.3.5/dolphie/Modules/Functions.py
+-rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-4.3.5/dolphie/Modules/ManualException.py
+-rw-r--r--   0        0        0    26287 2024-02-27 06:42:42.249716 dolphie-4.3.5/dolphie/Modules/MetricManager.py
+-rw-r--r--   0        0        0     7446 2024-03-11 10:37:06.615356 dolphie-4.3.5/dolphie/Modules/MySQL.py
+-rw-r--r--   0        0        0    17039 2024-03-12 05:51:44.344342 dolphie-4.3.5/dolphie/Modules/Queries.py
+-rw-r--r--   0        0        0    23820 2024-03-02 06:25:14.219098 dolphie-4.3.5/dolphie/Modules/TabManager.py
+-rw-r--r--   0        0        0     9270 2024-02-27 06:42:42.250655 dolphie-4.3.5/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-4.3.5/dolphie/Panels/ddl_panel.py
+-rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-4.3.5/dolphie/Panels/innodb_trx_locks_panel.py
+-rw-r--r--   0        0        0     6877 2024-03-02 10:45:55.398930 dolphie-4.3.5/dolphie/Panels/metadata_locks_panel.py
+-rw-r--r--   0        0        0     9179 2024-04-07 22:50:40.254587 dolphie-4.3.5/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0    25774 2024-02-27 06:28:11.313610 dolphie-4.3.5/dolphie/Panels/replication_panel.py
+-rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-4.3.5/dolphie/Widgets/command_screen.py
+-rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-4.3.5/dolphie/Widgets/event_log_screen.py
+-rw-r--r--   0        0        0    13960 2024-03-15 01:09:17.039272 dolphie-4.3.5/dolphie/Widgets/host_setup.py
+-rw-r--r--   0        0        0    11456 2024-03-28 20:01:57.993852 dolphie-4.3.5/dolphie/Widgets/modal.py
+-rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-4.3.5/dolphie/Widgets/spinner.py
+-rw-r--r--   0        0        0     5926 2024-03-12 06:05:29.747155 dolphie-4.3.5/dolphie/Widgets/thread_screen.py
+-rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-4.3.5/dolphie/Widgets/topbar.py
+-rw-r--r--   0        0        0    11982 2024-03-28 19:49:45.553457 dolphie-4.3.5/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    66820 2024-03-28 19:49:45.554130 dolphie-4.3.5/dolphie/app.py
+-rw-r--r--   0        0        0      645 2024-04-07 23:24:53.185954 dolphie-4.3.5/pyproject.toml
+-rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 dolphie-4.3.5/PKG-INFO
```

### Comparing `dolphie-4.3.4/LICENSE` & `dolphie-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/README.md` & `dolphie-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/DataTypes.py` & `dolphie-4.3.5/dolphie/DataTypes.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Dolphie.css` & `dolphie-4.3.5/dolphie/Dolphie.css`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 }
 Rule {
     color: #32416a;
     margin: 0;
 }
 DataTable {
     overflow-x: hidden;
+    max-height: 100vh;
 }
 DataTable > .datatable--odd-row {
     background: #131a2c;
 }
 DataTable > .datatable--even-row {
     background: #0f1525;
 }
@@ -401,22 +402,14 @@
 RadioSet:focus RadioButton.-selected .toggle--label {
     color: #a5b8e7;
 }
 RadioSet > RadioButton.-selected > .toggle--label {
     color: #9bb2eb;
 }
 
-
-Checkbox {
-    background: #131626;
-    border: none;
-    padding-left: 2;
-    padding-bottom: 1;
-    content-align: left middle;
-}
 Checkbox .toggle--button {
     background: #343d56;
 }
 RadioSet:focus > .toggle--label {
     text-style: underline;
 }
 ToggleButton:focus > .toggle--label {
```

### Comparing `dolphie-4.3.4/dolphie/Modules/ArgumentParser.py` & `dolphie-4.3.5/dolphie/Modules/ArgumentParser.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Modules/Functions.py` & `dolphie-4.3.5/dolphie/Modules/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Modules/ManualException.py` & `dolphie-4.3.5/dolphie/Modules/ManualException.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Modules/MetricManager.py` & `dolphie-4.3.5/dolphie/Modules/MetricManager.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Modules/MySQL.py` & `dolphie-4.3.5/dolphie/Modules/MySQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             if self.save_connection_id:
                 self.connection_id = self.fetch_value_from_field("SELECT CONNECTION_ID()")
 
             # Determine if SSL is being used
             self.using_ssl = "ON" if self.fetch_value_from_field("SHOW STATUS LIKE 'Ssl_cipher'", "Value") else "OFF"
         except pymysql.Error as e:
             if len(e.args) == 1:
-                raise ManualException(e)
+                raise ManualException(e.args[0])
             else:
                 raise ManualException(e.args[1])
         except FileNotFoundError:  # Catch SSL file path errors
             raise ManualException("SSL certificate file path isn't valid!")
         except SSLError as e:
             raise ManualException(f"SSL error: {e}")
```

### Comparing `dolphie-4.3.4/dolphie/Modules/Queries.py` & `dolphie-4.3.5/dolphie/Modules/Queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,16 @@
             ATTR_NAME,
             ATTR_VALUE
         FROM
             `performance_schema`.session_connect_attrs sca
             JOIN `performance_schema`.threads t ON sca.PROCESSLIST_ID = t.processlist_id
         WHERE
             t.processlist_id = $1
+        ORDER BY
+            ATTR_NAME
     """
     ddls: str = """
         SELECT
             t.processlist_id,
             ANY_VALUE(stmt.sql_text) AS sql_text,
             ANY_VALUE(stage.event_name) AS state,
             ANY_VALUE(CONCAT(ROUND(100 * stage.work_completed / stage.work_estimated, 2), "%")) AS percentage_completed,
```

### Comparing `dolphie-4.3.4/dolphie/Modules/TabManager.py` & `dolphie-4.3.5/dolphie/Modules/TabManager.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Panels/dashboard_panel.py` & `dolphie-4.3.5/dolphie/Panels/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Panels/ddl_panel.py` & `dolphie-4.3.5/dolphie/Panels/ddl_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Panels/innodb_trx_locks_panel.py` & `dolphie-4.3.5/dolphie/Panels/innodb_trx_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Panels/metadata_locks_panel.py` & `dolphie-4.3.5/dolphie/Panels/metadata_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Panels/processlist_panel.py` & `dolphie-4.3.5/dolphie/Panels/processlist_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from textual.widgets import DataTable
 
 
 def create_panel(tab: Tab) -> DataTable:
     dolphie = tab.dolphie
 
     if not dolphie.performance_schema_enabled and dolphie.use_performance_schema:
-        dolphie.notify("Performance Schema is not enabled on this host, using Information Schema instead")
+        dolphie.app.notify(
+            "Performance Schema is not enabled on this host, using Information Schema instead for processlist"
+        )
         dolphie.use_performance_schema = False
 
     columns = [
         {"name": "Process ID", "field": "id", "width": 11, "format_number": False},
         {"name": "Protocol", "field": "protocol", "width": 8, "format_number": False},
         {"name": "Username", "field": "user", "width": 20, "format_number": False},
     ]
```

### Comparing `dolphie-4.3.4/dolphie/Panels/replication_panel.py` & `dolphie-4.3.5/dolphie/Panels/replication_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Widgets/command_screen.py` & `dolphie-4.3.5/dolphie/Widgets/command_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Widgets/event_log_screen.py` & `dolphie-4.3.5/dolphie/Widgets/event_log_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Widgets/host_setup.py` & `dolphie-4.3.5/dolphie/Widgets/host_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,21 @@
         HostSetupModal #modal_footer {
             color: #d3565c;
             width: 100%;
             padding-bottom: 0;
             padding-top: 1;
             margin: 0 2;
         }
+        HostSetupModal Checkbox {
+            background: #131626;
+            border: none;
+            padding-left: 2;
+            padding-bottom: 1;
+            content-align: left middle;
+        }
         HostSetupModal Select {
             width: 100%;
             margin: 0 2;
             margin-bottom: 1;
         }
         HostSetupModal SelectCurrent Static#label {
             color: #606e88;
```

### Comparing `dolphie-4.3.4/dolphie/Widgets/modal.py` & `dolphie-4.3.5/dolphie/Widgets/modal.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,21 @@
         CommandModal #error_response {
             color: #fe5c5c;
             width: 100%;
             height: auto;
             content-align: center middle;
             padding-bottom: 1;
         }
+        CommandModal Checkbox {
+            background: #131626;
+            border: none;
+            content-align: center middle;
+            padding-top: 1;
+            width: 100%;
+        }
     """
     BINDINGS = [
         Binding("escape", "app.pop_screen", "", show=False),
     ]
 
     def __init__(self, command, message, processlist_data=None, host_cache_data=None):
         super().__init__()
```

### Comparing `dolphie-4.3.4/dolphie/Widgets/spinner.py` & `dolphie-4.3.5/dolphie/Widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Widgets/thread_screen.py` & `dolphie-4.3.5/dolphie/Widgets/thread_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/Widgets/topbar.py` & `dolphie-4.3.5/dolphie/Widgets/topbar.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.4/dolphie/__init__.py` & `dolphie-4.3.5/dolphie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         # Types of hosts
         self.galera_cluster: bool = False
         self.group_replication: bool = False
         self.innodb_cluster: bool = False
         self.innodb_cluster_read_replica: bool = False
         self.replicaset: bool = False
         self.aws_rds: bool = False
+        self.azure: bool = False
         self.mariadb: bool = False
 
         # These are for group replication in replication panel
         self.is_group_replication_primary: bool = False
         self.group_replication_members: dict = {}
         self.group_replication_data: dict = {}
 
@@ -172,20 +173,25 @@
             self.mariadb = True
         elif aurora_version:
             self.host_distro = "Amazon Aurora"
             self.aws_rds = True
         elif "rdsdb" in basedir:
             self.host_distro = "Amazon RDS"
             self.aws_rds = True
+        elif global_variables.get("aad_auth_only"):
+            self.host_distro = "Azure MySQL"
+            self.azure = True
         else:
             self.host_distro = "MySQL"
 
-        # For RDS, we will use the host specified to connect with since hostname isn't related to the endpoint
+        # For RDS and Azure, we will use the host specified to connect with since hostname isn't related to the endpoint
         if self.aws_rds:
             self.mysql_host = f"{self.host.split('.rds.amazonaws.com')[0]}:{self.port}"
+        elif self.azure:
+            self.mysql_host = f"{self.host.split('.mysql.database.azure.com')[0]}:{self.port}"
         else:
             self.mysql_host = f"{global_variables.get('hostname')}:{self.port}"
 
         major_version = int(version_split[0])
         self.server_uuid = global_variables.get("server_uuid")
         if "MariaDB" in self.host_distro and major_version >= 10:
             self.server_uuid = global_variables.get("server_id")
@@ -264,15 +270,16 @@
 
         return hostname
 
     def massage_metrics_data(self):
         if self.is_mysql_version_at_least("8.0"):
             # If we're using MySQL 8, we need to fetch the checkpoint age from the performance schema if it's not
             # available in global status
-            if not self.global_status.get("Innodb_checkpoint_age"):
+            # On Azure MySQL there is no BACKUP_ADMIN privilege so we can't fetch the checkpoint age
+            if not self.global_status.get("Innodb_checkpoint_age") and not self.azure:
                 self.global_status["Innodb_checkpoint_age"] = self.main_db_connection.fetch_value_from_field(
                     MySQLQueries.checkpoint_age, "checkpoint_age"
                 )
 
             if self.is_mysql_version_at_least("8.0.30"):
                 active_redo_logs_count = self.main_db_connection.fetch_value_from_field(
                     MySQLQueries.active_redo_logs, "count"
```

### Comparing `dolphie-4.3.4/dolphie/app.py` & `dolphie-4.3.5/dolphie/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1174,25 +1174,33 @@
                 self.call_from_thread(show_command_screen)
 
             if key == "k":
                 thread_id = additional_data
                 try:
                     if dolphie.aws_rds:
                         dolphie.secondary_db_connection.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                    elif dolphie.azure:
+                        dolphie.secondary_db_connection.execute("CALL mysql.az_kill(%s)" % thread_id)
                     else:
                         dolphie.secondary_db_connection.execute("KILL %s" % thread_id)
 
                     self.notify("Killed Thread ID [b highlight]%s[/b highlight]" % thread_id, severity="success")
                 except ManualException as e:
                     self.notify(e.reason, title="Error killing Thread ID", severity="error")
 
             if key == "K":
 
                 def execute_kill(thread_id):
-                    query = "CALL mysql.rds_kill(%s)" if dolphie.aws_rds else "KILL %s"
+                    if dolphie.aws_rds:
+                        query = "CALL mysql.rds_kill(%s)"
+                    elif dolphie.azure:
+                        query = "CALL mysql.az_kill(%s)"
+                    else:
+                        query = "KILL %s"
+
                     dolphie.secondary_db_connection.execute(query % thread_id)
 
                 kill_type, kill_value, include_sleeping_queries, lower_limit, upper_limit = additional_data
                 db_field = {"username": "user", "host": "host", "time_range": "time"}.get(kill_type)
 
                 commands_to_kill = ["Query", "Execute"]
```

### Comparing `dolphie-4.3.4/pyproject.toml` & `dolphie-4.3.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "dolphie"
-version = "4.3.4"
+version = "4.3.5"
 license = "GPL-3.0-or-later"
 description = "Echolocate your MySQL health with real-time monitoring in the terminal"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-rich = "^13.7.0"
+rich = "^13.7.1"
 pymysql = "^1.1.0"
 myloginpath = "^0.0.4"
-packaging = "^23.2"
+packaging = "^24.0"
 requests = "^2.31.0"
 sqlparse = "^0.4.4"
-textual = "^0.52.1"
+textual = "^0.56.2"
 textual-autocomplete = "^2.1.0b0"
-charset-normalizer = "^3.2.0"
+charset-normalizer = "^3.3.2"
 plotext = "^5.2.8"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `dolphie-4.3.4/PKG-INFO` & `dolphie-4.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 4.3.4
+Version: 4.3.5
 Summary: Echolocate your MySQL health with real-time monitoring in the terminal
 License: GPL-3.0-or-later
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: charset-normalizer (>=3.2.0,<4.0.0)
+Requires-Dist: charset-normalizer (>=3.3.2,<4.0.0)
 Requires-Dist: myloginpath (>=0.0.4,<0.0.5)
-Requires-Dist: packaging (>=23.2,<24.0)
+Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: textual (>=0.52.1,<0.53.0)
+Requires-Dist: textual (>=0.56.2,<0.57.0)
 Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Dolphie
 <p align="center">
   <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
   Echolocate your MySQL health with real-time monitoring in the terminal<br><br>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: dolphie Version: 4.3.4 Summary: Echolocate your
+Metadata-Version: 2.1 Name: dolphie Version: 4.3.5 Summary: Echolocate your
 MySQL health with real-time monitoring in the terminal License: GPL-3.0-or-
 later Author: Charles Thompson Author-email: 01charles.t@gmail.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: charset-
-normalizer (>=3.2.0,<4.0.0) Requires-Dist: myloginpath (>=0.0.4,<0.0.5)
-Requires-Dist: packaging (>=23.2,<24.0) Requires-Dist: plotext (>=5.2.8,<6.0.0)
+normalizer (>=3.3.2,<4.0.0) Requires-Dist: myloginpath (>=0.0.4,<0.0.5)
+Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.0,<14.0.0) Requires-Dist:
-sqlparse (>=0.4.4,<0.5.0) Requires-Dist: textual (>=0.52.1,<0.53.0) Requires-
+(>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist:
+sqlparse (>=0.4.4,<0.5.0) Requires-Dist: textual (>=0.56.2,<0.57.0) Requires-
 Dist: textual-autocomplete (>=2.1.0b0,<3.0.0) Description-Content-Type: text/
 markdown # Dolphie
  [https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-
                           4f9c-ada5-a153cdcf4070.png]
     Echolocate your MySQL health with real-time monitoring in the terminal
 
   [https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-
```

