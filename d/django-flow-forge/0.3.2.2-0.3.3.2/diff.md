# Comparing `tmp/django_flow_forge-0.3.2.2.tar.gz` & `tmp/django_flow_forge-0.3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_flow_forge-0.3.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_flow_forge-0.3.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_flow_forge-0.3.2.2.tar` & `django_flow_forge-0.3.3.2.tar`

### file list

```diff
@@ -1,113 +1,114 @@
--rw-r--r--   0        0        0     6148 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/.gitattributes
--rw-r--r--   0        0        0      862 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/.github/workflows/deploy-mkdocs.yml
--rw-r--r--   0        0        0      620 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     2879 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/.gitignore
--rw-r--r--   0        0        0     1613 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/.vscode/launch.json
--rw-r--r--   0        0        0     1103 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/Dockerfile
--rw-r--r--   0        0        0     1061 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/LICENSE
--rw-r--r--   0        0        0      151 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/MANIFEST.in
--rw-r--r--   0        0        0      865 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/README.md
--rwxr-xr-x   0        0        0        0 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/__init__.py
--rwxr-xr-x   0        0        0     2599 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/admin.py
--rwxr-xr-x   0        0        0      160 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/apps.py
--rw-r--r--   0        0        0     2253 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/async_utils.py
--rw-r--r--   0        0        0     2950 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/authorization.py
--rw-r--r--   0        0        0    15409 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/flow_engine.py
--rw-r--r--   0        0        0     5435 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/0001_initial.py
--rw-r--r--   0        0        0      816 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
--rw-r--r--   0        0        0      449 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
--rw-r--r--   0        0        0      624 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
--rw-r--r--   0        0        0      428 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/0005_alter_flow_options.py
--rw-r--r--   0        0        0      564 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
--rwxr-xr-x   0        0        0        0 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/__init__.py
--rw-r--r--   0        0        0      778 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0001_initial.py
--rw-r--r--   0        0        0      392 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
--rw-r--r--   0        0        0     1236 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
--rw-r--r--   0        0        0      451 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
--rw-r--r--   0        0        0      400 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
--rw-r--r--   0        0        0      627 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
--rw-r--r--   0        0        0      448 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
--rw-r--r--   0        0        0      444 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
--rw-r--r--   0        0        0     1717 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
--rw-r--r--   0        0        0      414 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
--rw-r--r--   0        0        0      573 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
--rw-r--r--   0        0        0      980 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
--rw-r--r--   0        0        0      537 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
--rw-r--r--   0        0        0      732 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
--rw-r--r--   0        0        0      432 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
--rw-r--r--   0        0        0      467 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
--rw-r--r--   0        0        0      613 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
--rw-r--r--   0        0        0      740 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
--rw-r--r--   0        0        0      673 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      451 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
--rw-r--r--   0        0        0      841 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      554 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
--rw-r--r--   0        0        0     1295 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0023_mlresult.py
--rw-r--r--   0        0        0      550 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
--rw-r--r--   0        0        0      542 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
--rw-r--r--   0        0        0      647 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
--rw-r--r--   0        0        0      446 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
--rw-r--r--   0        0        0      639 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
--rw-r--r--   0        0        0      436 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
--rw-r--r--   0        0        0      771 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
--rwxr-xr-x   0        0        0     5380 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/models.py
--rw-r--r--   0        0        0      627 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
--rw-r--r--   0        0        0    47755 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/static/django_flow_forge/htmx.min.js
--rw-r--r--   0        0        0    10417 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/task_utils.py
--rw-r--r--   0        0        0      958 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
--rw-r--r--   0        0        0      570 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
--rw-r--r--   0        0        0     3526 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
--rw-r--r--   0        0        0      754 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
--rw-r--r--   0        0        0     2701 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
--rw-r--r--   0        0        0      826 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
--rw-r--r--   0        0        0     1422 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/ml_result.html
--rw-r--r--   0        0        0     1808 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0     2699 2024-03-27 22:13:53.541345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     3194 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
--rw-r--r--   0        0        0     3723 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
--rw-r--r--   0        0        0     5888 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
--rwxr-xr-x   0        0        0     2962 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/django_flow_forge/tests.py
--rw-r--r--   0        0        0      680 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/django_flow_forge/urls.py
--rwxr-xr-x   0        0        0     9518 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/django_flow_forge/views.py
--rw-r--r--   0        0        0      767 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docker-compose-local.yml
--rw-r--r--   0        0        0      846 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/authorization.md
--rw-r--r--   0        0        0     3996 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/considerations.md
--rw-r--r--   0        0        0      866 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/data_science_experiments.md
--rw-r--r--   0        0        0     1031 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/debugging.md
--rw-r--r--   0        0        0     1295 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/flows_dashboard.md
--rw-r--r--   0        0        0     4269 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/index.md
--rw-r--r--   0        0        0     3613 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/installation.md
--rw-r--r--   0        0        0      270 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/roadmap.md
--rw-r--r--   0        0        0     1037 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/docs/strategies.md
--rw-r--r--   0        0        0        0 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/example_project/conf/__init__.py
--rw-r--r--   0        0        0      396 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/example_project/conf/asgi.py
--rw-r--r--   0        0        0     4130 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/example_project/conf/settings.py
--rw-r--r--   0        0        0      898 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/example_project/conf/urls.py
--rw-r--r--   0        0        0      396 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/example_project/conf/wsgi.py
--rw-r--r--   0        0        0    32768 2024-03-27 22:13:53.545345 django_flow_forge-0.3.2.2/example_project/db.sqlite3-shm
--rw-r--r--   0        0        0  2904632 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/db.sqlite3-wal
--rw-r--r--   0        0        0      177 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/admin.py
--rw-r--r--   0        0        0      605 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/apps.py
--rw-r--r--   0        0        0      831 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/celery_app.py
--rw-r--r--   0        0        0     4720 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/flow__ml_grid_search.py
--rw-r--r--   0        0        0     1394 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/flow__parallel_celery.py
--rw-r--r--   0        0        0     1409 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/flow__simple.py
--rw-r--r--   0        0        0     2980 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/flow__simple_ml.py
--rw-r--r--   0        0        0     1555 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/flow__simple_with_celery.py
--rw-r--r--   0        0        0     2137 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/flow__with_nested_tasks.py
--rw-r--r--   0        0        0        0 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/models.py
--rw-r--r--   0        0        0     2134 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0      994 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     1922 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/templates/example_app/index.html
--rw-r--r--   0        0        0       60 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/tests.py
--rw-r--r--   0        0        0      962 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/urls.py
--rw-r--r--   0        0        0     2531 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/example_app/views.py
--rwxr-xr-x   0        0        0      660 2024-03-27 22:13:53.553345 django_flow_forge-0.3.2.2/example_project/manage.py
--rw-r--r--   0        0        0      522 2024-03-27 22:13:53.557345 django_flow_forge-0.3.2.2/example_project/run_tasks_no_server.py
--rw-r--r--   0        0        0      399 2024-03-27 22:13:53.557345 django_flow_forge-0.3.2.2/mkdocs.yml
--rw-r--r--   0        0        0      875 2024-03-27 22:13:53.557345 django_flow_forge-0.3.2.2/pyproject.toml
--rw-r--r--   0        0        0       45 2024-03-27 22:13:53.557345 django_flow_forge-0.3.2.2/requirements.txt
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 django_flow_forge-0.3.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.DS_Store
+-rw-r--r--   0        0        0       66 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.gitattributes
+-rw-r--r--   0        0        0      862 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.github/workflows/deploy-mkdocs.yml
+-rw-r--r--   0        0        0      620 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     2879 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.gitignore
+-rw-r--r--   0        0        0     1613 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.vscode/launch.json
+-rw-r--r--   0        0        0     1103 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/Dockerfile
+-rw-r--r--   0        0        0     1061 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/LICENSE
+-rw-r--r--   0        0        0      151 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/MANIFEST.in
+-rw-r--r--   0        0        0      865 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/README.md
+-rwxr-xr-x   0        0        0        0 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/__init__.py
+-rwxr-xr-x   0        0        0     2599 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/admin.py
+-rwxr-xr-x   0        0        0      160 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/apps.py
+-rw-r--r--   0        0        0     2253 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/async_utils.py
+-rw-r--r--   0        0        0     2950 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/authorization.py
+-rw-r--r--   0        0        0    15414 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/flow_engine.py
+-rw-r--r--   0        0        0     5435 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0001_initial.py
+-rw-r--r--   0        0        0      816 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
+-rw-r--r--   0        0        0      449 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
+-rw-r--r--   0        0        0      624 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
+-rw-r--r--   0        0        0      428 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0005_alter_flow_options.py
+-rw-r--r--   0        0        0      564 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
+-rw-r--r--   0        0        0      436 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0007_executedflow_params.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/__init__.py
+-rw-r--r--   0        0        0      778 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0001_initial.py
+-rw-r--r--   0        0        0      392 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
+-rw-r--r--   0        0        0     1236 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
+-rw-r--r--   0        0        0      451 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
+-rw-r--r--   0        0        0      400 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
+-rw-r--r--   0        0        0      627 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
+-rw-r--r--   0        0        0      448 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
+-rw-r--r--   0        0        0      444 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
+-rw-r--r--   0        0        0     1717 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
+-rw-r--r--   0        0        0      414 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
+-rw-r--r--   0        0        0      573 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
+-rw-r--r--   0        0        0      980 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
+-rw-r--r--   0        0        0      537 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      732 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
+-rw-r--r--   0        0        0      432 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
+-rw-r--r--   0        0        0      467 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
+-rw-r--r--   0        0        0      613 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      740 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
+-rw-r--r--   0        0        0      673 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      451 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
+-rw-r--r--   0        0        0      841 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      554 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
+-rw-r--r--   0        0        0     1295 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0023_mlresult.py
+-rw-r--r--   0        0        0      550 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
+-rw-r--r--   0        0        0      542 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
+-rw-r--r--   0        0        0      647 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
+-rw-r--r--   0        0        0      446 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
+-rw-r--r--   0        0        0      639 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
+-rw-r--r--   0        0        0      436 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
+-rw-r--r--   0        0        0      771 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
+-rwxr-xr-x   0        0        0     5447 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/models.py
+-rw-r--r--   0        0        0      627 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
+-rw-r--r--   0        0        0    47755 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/htmx.min.js
+-rw-r--r--   0        0        0    10490 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/task_utils.py
+-rw-r--r--   0        0        0      957 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
+-rw-r--r--   0        0        0      570 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
+-rw-r--r--   0        0        0     3526 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
+-rw-r--r--   0        0        0      754 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
+-rw-r--r--   0        0        0     2701 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
+-rw-r--r--   0        0        0      826 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
+-rw-r--r--   0        0        0     1422 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result.html
+-rw-r--r--   0        0        0     1808 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0     2699 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     3194 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
+-rw-r--r--   0        0        0     3723 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
+-rw-r--r--   0        0        0     5888 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
+-rwxr-xr-x   0        0        0     2962 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/tests.py
+-rw-r--r--   0        0        0      680 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/urls.py
+-rwxr-xr-x   0        0        0     9518 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/views.py
+-rw-r--r--   0        0        0      767 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docker-compose-local.yml
+-rw-r--r--   0        0        0      846 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/authorization.md
+-rw-r--r--   0        0        0     3996 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/considerations.md
+-rw-r--r--   0        0        0      866 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/data_science_experiments.md
+-rw-r--r--   0        0        0     1031 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/debugging.md
+-rw-r--r--   0        0        0     1295 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/flows_dashboard.md
+-rw-r--r--   0        0        0     4269 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/index.md
+-rw-r--r--   0        0        0     3613 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/installation.md
+-rw-r--r--   0        0        0      270 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/roadmap.md
+-rw-r--r--   0        0        0     1037 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/strategies.md
+-rw-r--r--   0        0        0        0 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/asgi.py
+-rw-r--r--   0        0        0     4130 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/settings.py
+-rw-r--r--   0        0        0      898 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/urls.py
+-rw-r--r--   0        0        0      396 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/wsgi.py
+-rw-r--r--   0        0        0    32768 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/db.sqlite3-shm
+-rw-r--r--   0        0        0  2904632 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/db.sqlite3-wal
+-rw-r--r--   0        0        0      177 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/admin.py
+-rw-r--r--   0        0        0      605 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/apps.py
+-rw-r--r--   0        0        0      831 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/celery_app.py
+-rw-r--r--   0        0        0     4720 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__ml_grid_search.py
+-rw-r--r--   0        0        0     1394 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__parallel_celery.py
+-rw-r--r--   0        0        0     1409 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__simple.py
+-rw-r--r--   0        0        0     2980 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_ml.py
+-rw-r--r--   0        0        0     1555 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_with_celery.py
+-rw-r--r--   0        0        0     2137 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__with_nested_tasks.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/models.py
+-rw-r--r--   0        0        0     2134 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0      994 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     1922 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/templates/example_app/index.html
+-rw-r--r--   0        0        0       60 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/tests.py
+-rw-r--r--   0        0        0      962 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/urls.py
+-rw-r--r--   0        0        0     2531 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/views.py
+-rwxr-xr-x   0        0        0      660 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/manage.py
+-rw-r--r--   0        0        0      522 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/run_tasks_no_server.py
+-rw-r--r--   0        0        0      399 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/mkdocs.yml
+-rw-r--r--   0        0        0      875 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/requirements.txt
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 django_flow_forge-0.3.3.2/PKG-INFO
```

### Comparing `django_flow_forge-0.3.2.2/.DS_Store` & `django_flow_forge-0.3.3.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/.github/workflows/deploy-mkdocs.yml` & `django_flow_forge-0.3.3.2/.github/workflows/deploy-mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/.github/workflows/publish-to-pypi.yml` & `django_flow_forge-0.3.3.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/.gitignore` & `django_flow_forge-0.3.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/.vscode/launch.json` & `django_flow_forge-0.3.3.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/Dockerfile` & `django_flow_forge-0.3.3.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/LICENSE` & `django_flow_forge-0.3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/README.md` & `django_flow_forge-0.3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/admin.py` & `django_flow_forge-0.3.3.2/django_flow_forge/admin.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/async_utils.py` & `django_flow_forge-0.3.3.2/django_flow_forge/async_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/authorization.py` & `django_flow_forge-0.3.3.2/django_flow_forge/authorization.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/flow_engine.py` & `django_flow_forge-0.3.3.2/django_flow_forge/flow_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
                         executor.collect_and_store_output()
 
                         executor.task_post_process()
                 
                 elif executor.task_run.status == 'in_progress':
                     
                     # Else if task is in progress then check status and collect data #
-                    if counter % 1000:
+                    if counter % 1000 == 0:
                         executor.create_checkpoint()
             
                     if executor.task_is_ready_for_close():
                         # collect output
                         executor.collect_and_store_output()
 
                         executor.task_post_process()
```

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/0001_initial.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0001_initial.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0023_mlresult.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0023_mlresult.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py` & `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/models.py` & `django_flow_forge-0.3.3.2/django_flow_forge/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     executed_tasks = models.ManyToManyField(FlowTask, related_name='executed_tasks', blank=True)
     executed_by = models.CharField(null=True, blank=True, max_length=255)
     flow_complete = models.BooleanField(default=False)  # Indicates if the flow run is complete
     status = models.CharField(max_length=20, choices=STATUS_CHOICES, default='pending')
     last_checkpoint_datetime = models.DateTimeField(blank=True, auto_now_add=True)
     flow_snapshot = models.JSONField(default=dict)  # Captures the output of the task for this run
     exceptions = models.JSONField(default=dict, null=True, blank=True)
+    params = models.JSONField(default=dict, null=True, blank=True)
 
     def __str__(self):
         if self.flow:
             return f"Run of {self.flow.flow_name} on {self.start_time}. Completed: {self.flow_complete}"
         else:
             return f"Run of an unknown flow on {self.start_time}. Completed: {self.flow_complete}"
```

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/static/django_flow_forge/cytoscape_setup.js` & `django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/cytoscape_setup.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/static/django_flow_forge/htmx.min.js` & `django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/task_utils.py` & `django_flow_forge-0.3.3.2/django_flow_forge/task_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.task_output_ready = False
         self.task_future = None
 
     def create_checkpoint(self,):
 
         # If the task is async, you might want to handle the result differently                
         self.flow_run.last_checkpoint_datetime = timezone.now()
-        self.flow_run.save()
+        self.flow_run.save(update_fields=['last_checkpoint_datetime'])
 
     def submit_task(self, **kwargs):
 
         """
         Executes a specific task as part of a flow run, handling logging, execution, and status updates.
 
         """
@@ -281,10 +281,10 @@
     for count, i in enumerate(nodes):
         index_map[i['data']['id']] = count
         etask = etasks.filter(task_snapshot_id=i['data']['id'])
         if len(etask) > 0:
             i['data']['status'] = etask[0].status
     snapshot['graph']['nodes'] = nodes
     flow_run.flow_snapshot = snapshot
-    flow_run.save()
+    flow_run.save(update_fields=['flow_snapshot'])
 
     return
```

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html`

 * *Files 0% similar despite different names*

```diff
@@ -21,9 +21,8 @@
         <div class="col-sm-1 text-light"><strong>Code:</strong></div>
         <div class="col-sm-11 text-light">
             <pre><code class="python">{{ task.code }}</code></pre>
         </div>
     </div>
 </div>
 
-
 <script>hljs.highlightAll();</script>
```

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/ml_result.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html` & `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/tests.py` & `django_flow_forge-0.3.3.2/django_flow_forge/tests.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/urls.py` & `django_flow_forge-0.3.3.2/django_flow_forge/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/django_flow_forge/views.py` & `django_flow_forge-0.3.3.2/django_flow_forge/views.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docker-compose-local.yml` & `django_flow_forge-0.3.3.2/docker-compose-local.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/authorization.md` & `django_flow_forge-0.3.3.2/docs/authorization.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/considerations.md` & `django_flow_forge-0.3.3.2/docs/considerations.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/data_science_experiments.md` & `django_flow_forge-0.3.3.2/docs/data_science_experiments.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/debugging.md` & `django_flow_forge-0.3.3.2/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/flows_dashboard.md` & `django_flow_forge-0.3.3.2/docs/flows_dashboard.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/index.md` & `django_flow_forge-0.3.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/installation.md` & `django_flow_forge-0.3.3.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/docs/strategies.md` & `django_flow_forge-0.3.3.2/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/conf/settings.py` & `django_flow_forge-0.3.3.2/example_project/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/conf/urls.py` & `django_flow_forge-0.3.3.2/example_project/conf/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/db.sqlite3-shm` & `django_flow_forge-0.3.3.2/example_project/db.sqlite3-shm`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/db.sqlite3-wal` & `django_flow_forge-0.3.3.2/example_project/db.sqlite3-wal`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/apps.py` & `django_flow_forge-0.3.3.2/example_project/example_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/celery_app.py` & `django_flow_forge-0.3.3.2/example_project/example_app/celery_app.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/flow__ml_grid_search.py` & `django_flow_forge-0.3.3.2/example_project/example_app/flow__ml_grid_search.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/flow__parallel_celery.py` & `django_flow_forge-0.3.3.2/example_project/example_app/flow__parallel_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/flow__simple.py` & `django_flow_forge-0.3.3.2/example_project/example_app/flow__simple.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/flow__simple_ml.py` & `django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_ml.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/flow__simple_with_celery.py` & `django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_with_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/flow__with_nested_tasks.py` & `django_flow_forge-0.3.3.2/example_project/example_app/flow__with_nested_tasks.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/templates/example_app/index.html` & `django_flow_forge-0.3.3.2/example_project/example_app/templates/example_app/index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/urls.py` & `django_flow_forge-0.3.3.2/example_project/example_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/example_app/views.py` & `django_flow_forge-0.3.3.2/example_project/example_app/views.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/manage.py` & `django_flow_forge-0.3.3.2/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/example_project/run_tasks_no_server.py` & `django_flow_forge-0.3.3.2/example_project/run_tasks_no_server.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.2.2/pyproject.toml` & `django_flow_forge-0.3.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-flow-forge"
-version = "0.3.2.2"
+version = "0.3.3.2"
 description = "Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows."
 authors = [{name = "Ed Burmicz", email = "eddyojb@gmail.com"}]
 readme = "README.md"
 license = {text = "MIT"} 
 keywords = ["django", "mlops", "data", "machine learning", "data science", "pipelines", "flow", "orchestration", "AI",]
 classifiers = [
     "Framework :: Django",
```

### Comparing `django_flow_forge-0.3.2.2/PKG-INFO` & `django_flow_forge-0.3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flow-forge
-Version: 0.3.2.2
+Version: 0.3.3.2
 Summary: Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows.
 Keywords: django,mlops,data,machine learning,data science,pipelines,flow,orchestration,AI
 Author-email: Ed Burmicz <eddyojb@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

