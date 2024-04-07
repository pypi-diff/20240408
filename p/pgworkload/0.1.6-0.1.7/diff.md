# Comparing `tmp/pgworkload-0.1.6.tar.gz` & `tmp/pgworkload-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgworkload-0.1.6.tar", max compression
+gzip compressed data, was "pgworkload-0.1.7.tar", max compression
```

## Comparing `pgworkload-0.1.6.tar` & `pgworkload-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-01-28 22:12:07.442794 pgworkload-0.1.6/LICENSE
--rw-r--r--   0        0        0     9028 2023-08-09 14:49:03.166934 pgworkload-0.1.6/README.md
--rw-r--r--   0        0        0      497 2023-08-09 14:49:46.732843 pgworkload-0.1.6/pgworkload/__init__.py
--rw-r--r--   0        0        0    10991 2024-03-15 17:34:54.705230 pgworkload-0.1.6/pgworkload/cli/main.py
--rw-r--r--   0        0        0    10688 2023-08-09 14:49:46.851360 pgworkload-0.1.6/pgworkload/models/init.py
--rw-r--r--   0        0        0    10451 2024-03-15 18:25:26.356768 pgworkload-0.1.6/pgworkload/models/run.py
--rw-r--r--   0        0        0     2308 2023-08-09 14:49:46.773195 pgworkload-0.1.6/pgworkload/models/util.py
--rw-r--r--   0        0        0     2208 2023-08-09 14:49:46.761340 pgworkload-0.1.6/pgworkload/utils/builtin_workloads.py
--rw-r--r--   0        0        0    21707 2024-03-14 14:45:20.907952 pgworkload-0.1.6/pgworkload/utils/simplefaker.py
--rw-r--r--   0        0        0    17469 2024-03-15 16:58:47.985432 pgworkload-0.1.6/pgworkload/utils/util.py
--rw-r--r--   0        0        0      867 2024-03-15 18:01:29.068031 pgworkload-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10186 1970-01-01 00:00:00.000000 pgworkload-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-01-28 22:12:07.442794 pgworkload-0.1.7/LICENSE
+-rw-r--r--   0        0        0     9028 2023-08-09 14:49:03.166934 pgworkload-0.1.7/README.md
+-rw-r--r--   0        0        0      495 2024-04-05 23:08:50.306315 pgworkload-0.1.7/pgworkload/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-07 22:27:57.373962 pgworkload-0.1.7/pgworkload/cli/dep.py
+-rw-r--r--   0        0        0     6915 2024-04-07 22:27:57.444521 pgworkload-0.1.7/pgworkload/cli/main.py
+-rw-r--r--   0        0        0     3863 2024-04-07 22:29:46.279410 pgworkload-0.1.7/pgworkload/cli/util.py
+-rw-r--r--   0        0        0    10746 2024-04-07 22:27:57.469736 pgworkload-0.1.7/pgworkload/models/init.py
+-rw-r--r--   0        0        0    10448 2024-04-07 22:20:28.798413 pgworkload-0.1.7/pgworkload/models/run.py
+-rw-r--r--   0        0        0     7610 2024-04-07 22:20:28.798521 pgworkload-0.1.7/pgworkload/models/util.py
+-rw-r--r--   0        0        0     2208 2023-08-09 14:49:46.761340 pgworkload-0.1.7/pgworkload/utils/builtin_workloads.py
+-rw-r--r--   0        0        0    17469 2024-03-15 16:58:47.985432 pgworkload-0.1.7/pgworkload/utils/common.py
+-rw-r--r--   0        0        0    21871 2024-04-05 19:40:38.128860 pgworkload-0.1.7/pgworkload/utils/simplefaker.py
+-rw-r--r--   0        0        0      867 2024-04-07 22:30:31.092928 pgworkload-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10186 1970-01-01 00:00:00.000000 pgworkload-0.1.7/PKG-INFO
```

### Comparing `pgworkload-0.1.6/LICENSE` & `pgworkload-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.6/README.md` & `pgworkload-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.6/pgworkload/cli/main.py` & `pgworkload-0.1.7/pgworkload/models/run.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,399 +1,362 @@
 #!/usr/bin/python
 
-from .. import __version__
-from enum import Enum
-from pathlib import Path
-from typing import Optional
-import json
 import logging
-import os
-import pgworkload.models.init
-import pgworkload.models.run
-import pgworkload.models.util
-import pgworkload.utils.util
-import platform
-import re
+import multiprocessing as mp
+import pgworkload.utils.common
+import psycopg
+import queue
+import random
+import signal
 import sys
-import typer
-import yaml
+import threading
+import time
+import traceback
+import logging.handlers
+import tabulate
 
-
-EPILOG = "GitHub: <https://github.com/fabiog1901/pgworkload>"
+DEFAULT_SLEEP = 3
 
 logger = logging.getLogger(__name__)
 
-app = typer.Typer(
-    epilog=EPILOG,
-    no_args_is_help=True,
-    help=f"pgworkload v{__version__}: Workload utility for the PostgreSQL protocol.",
-)
-
-util_app = typer.Typer(
-    epilog=EPILOG,
-    no_args_is_help=True,
-    help="Generate YAML data generation files and CSV datasets.",
-)
-app.add_typer(util_app, name="util")
-
-
-version: bool = typer.Option(True)
-
-
-class LogLevel(str, Enum):
-    debug = "debug"
-    info = "info"
-    warning = "warning"
-    error = "error"
+HEADERS: list = [
+    "id",
+    "elapsed",
+    "tot_ops",
+    "tot_ops/s",
+    "period_ops",
+    "period_ops/s",
+    "mean(ms)",
+    "p50(ms)",
+    "p90(ms)",
+    "p95(ms)",
+    "p99(ms)",
+    "pMax(ms)",
+]
+
+
+def signal_handler(sig, frame):
+    """Handles Ctrl+C events gracefully,
+    ensuring all running processes are closed rather than killed.
 
-
-class Param:
-    LogLevel = typer.Option(
-        "info", "--log-level", "-l", show_choices=True, help="Set the logging level."
-    )
-
-    WorkloadPath = typer.Option(
-        None,
-        "--workload",
-        "-w",
-        help="Filepath to the workload module.",
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-        writable=False,
-        readable=True,
-        resolve_path=True,
-    )
-
-    Procs = typer.Option(
-        None,
-        "--procs",
-        "-x",
-        help="Number of processes to spawn. Defaults to <system-cpu-count>.",
-        show_default=False,
-    )
-
-    DBUrl = typer.Option(
-        "postgres://root@localhost:26257/postgres?sslmode=disable",
-        "--url",
-        help="The connection string to the database.",
-    )
-
-    Args = typer.Option(
-        None, help="JSON string, or filepath to a JSON/YAML file, to pass to Workload."
-    )
-
-    HTTPServerPort = typer.Option(
-        3000,
-        "-p",
-        "--port",
-        help="The port of the http server that servers the CSV files.",
-    )
-
-    HTTPServerHostName = typer.Option(
-        None,
-        "-n",
-        "--hostname",
-        show_default=False,
-        help="The hostname of the http server that serves the CSV files.",
-    )
-
-    CSVMaxRows = typer.Option(100000, help="Max count of rows per resulting CSV file.")
+    Args:
+        sig (_type_):
+        frame (_type_):
+    """
+    global stats
+    global concurrency
+    logger.info("KeyboardInterrupt signal detected. Stopping processes...")
+
+    # send the poison pill to each worker
+    for _ in range(concurrency):
+        kill_q.put(None)
+
+    # wait until all workers return
+    start = time.time()
+    c = 0
+    timeout = True
+    while c < concurrency and timeout:
+        try:
+            kill_q2.get(block=False)
+            c += 1
+        except:
+            pass
+
+        time.sleep(0.01)
+        timeout = time.time() < start + 5
+
+    if not timeout:
+        logger.info("Timeout reached - forcing processes to stop")
+
+    logger.info("Printing final stats")
+    __print_stats()
+    sys.exit(0)
+
+
+def __ramp_up(processes: list, ramp_interval: int):
+    for p in processes:
+        logger.info("Starting a new Process...")
+        p.start()
+        time.sleep(ramp_interval)
 
 
-@app.command(help="Run the workload.", epilog=EPILOG, no_args_is_help=True)
 def run(
-    workload_path: Optional[Path] = Param.WorkloadPath,
-    builtin_workload: str = typer.Option(None, help="Built-in workload"),
-    dburl: str = Param.DBUrl,
-    procs: int = Param.Procs,
-    args: str = Param.Args,
-    concurrency: int = typer.Option(
-        1, "-c", "--concurrency", help="Number of concurrent workers."
-    ),
-    ramp: int = typer.Option(0, "-r", "--ramp", help="Ramp up time in seconds."),
-    iterations: int = typer.Option(
-        None,
-        "-i",
-        "--iterations",
-        help="Total number of iterations. Defaults to <ad infinitum>.",
-        show_default=False,
-    ),
-    duration: int = typer.Option(
-        None,
-        "-d",
-        "--duration",
-        help="Duration in seconds. Defaults to <ad infinitum>.",
-        show_default=False,
-    ),
-    conn_duration: int = typer.Option(
-        None,
-        "-k",
-        "--conn-duration",
-        show_default=False,
-        help="The number of seconds to keep database connection alive before restarting. Defaults to <ad infinitum>.",
-    ),
-    app_name: Optional[str] = typer.Option(
-        None,
-        "--app-name",
-        "-a",
-        help="The application name specified by the client. Defaults to <db-name>.",
-        show_default=False,
-    ),
-    autocommit: bool = typer.Option(
-        True,
-        "--no-autocommit",
-        show_default=False,
-        help="Unset autocommit in the connections.",
-    ),
-    frequency: int = typer.Option(
-        10, "-s", "--stats-frequency", help="How often to display the stats in seconds. Set 0 to disable"
-    ),
-    prom_port: int = typer.Option(
-        26260, "-p", "--port", help="The port of the Prometheus server."
-    ),
-    log_level: LogLevel = Param.LogLevel,
+    conc: int,
+    workload_path: str,
+    builtin_workload: str,
+    frequency: int,
+    prom_port: int,
+    iterations: int,
+    procs: int,
+    ramp: int,
+    dburl: str,
+    autocommit: bool,
+    duration: int,
+    conn_duration: int,
+    args: dict,
+    log_level: str,
 ):
-    logger.setLevel(log_level.upper())
-
-    logger.debug("Executing run()")
-
-    if workload_path:
-        procs, dburl, args = __validate(procs, dburl, app_name, args, workload_path)
-
-    else:
-        procs, dburl, args = __validate(procs, dburl, app_name, args, builtin_workload)
-
-    pgworkload.models.run.run(
-        conc=concurrency,
-        workload_path=workload_path,
-        builtin_workload=builtin_workload,
-        frequency=frequency,
-        prom_port=prom_port,
-        iterations=iterations,
-        procs=procs,
-        ramp=ramp,
-        dburl=dburl,
-        autocommit=autocommit,
-        duration=duration,
-        conn_duration=conn_duration,
-        args=args,
-        log_level=log_level.upper(),
-    )
-
-
-@app.command(help="Init the workload.", epilog=EPILOG, no_args_is_help=True)
-def init(
-    workload_path: Optional[Path] = Param.WorkloadPath,
-    procs: int = Param.Procs,
-    dburl: str = Param.DBUrl,
-    drop: bool = typer.Option(False, "--drop", help="Drop the database if it exists."),
-    csv_max_rows: int = Param.CSVMaxRows,
-    skip_schema: bool = typer.Option(
-        False, "-s", "--skip-schema", help="Don't run the schema creation script."
-    ),
-    skip_gen: bool = typer.Option(
-        False, "-g", "--skip-gen", help="Don't generate the CSV data files."
-    ),
-    skip_import: bool = typer.Option(
-        False, "-i", "--skip-import", help="Don't import the CSV data files."
-    ),
-    db: str = typer.Option(
-        None, show_default=False, help="Override the default DB name."
-    ),
-    http_server_hostname: str = Param.HTTPServerHostName,
-    http_server_port: int = Param.HTTPServerPort,
-    args: str = Param.Args,
-    log_level: LogLevel = Param.LogLevel,
-):
-    logging.getLogger(__package__).setLevel(log_level.upper())
-
-    logger.debug("Executing run()")
-
-    procs, dburl, args = __validate(procs, dburl, None, args, workload_path)
-
-    pgworkload.models.init.init(
-        db=db,
-        workload_path=workload_path,
-        dburl=dburl,
-        skip_schema=skip_schema,
-        drop=drop,
-        skip_gen=skip_gen,
-        procs=procs,
-        csv_max_rows=csv_max_rows,
-        skip_import=skip_import,
-        http_server_hostname=http_server_hostname,
-        http_server_port=http_server_port,
-        args=args,
-        log_level=log_level.upper(),
-    )
-
-
-@util_app.command(
-    "csv",
-    epilog=EPILOG,
-    no_args_is_help=True,
-    help="Generate CSV files from a YAML data generation file.",
-)
-def util_csv(
-    input: Optional[Path] = typer.Option(
-        ...,
-        "--input",
-        "-i",
-        help="Filepath to the YAML data generation file.",
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-        writable=False,
-        readable=True,
-        resolve_path=True,
-    ),
-    output: Optional[Path] = typer.Option(
-        None,
-        "--output",
-        "-o",
-        show_default=False,
-        help="Output directory for the CSV files. Defaults to <input-basename>.",
-        exists=False,
-        file_okay=False,
-        dir_okay=True,
-        writable=False,
-        readable=True,
-        resolve_path=True,
-    ),
-    procs: int = Param.Procs,
-    csv_max_rows: int = Param.CSVMaxRows,
-    http_server_hostname: str = Param.HTTPServerHostName,
-    http_server_port: int = Param.HTTPServerPort,
-    table_name: str = typer.Option(
-        "table_name",
-        "--table-name",
-        "-t",
-        help="The table name used in the import statement.",
-    ),
-    compression: str = typer.Option(
-        None, "-c", "--compression", help="The compression format."
-    ),
-    delimiter: str = typer.Option(
-        "\t",
-        "-d",
-        "--delimiter",
-        help='The delimeter char to use for the CSV files. Defaults to "tab".',
-        show_default=False,
-    ),
-):
-    pgworkload.models.util.util_csv(
-        input=input,
-        output=output,
-        compression=compression,
-        procs=procs,
-        csv_max_rows=csv_max_rows,
-        delimiter=delimiter,
-        http_server_hostname=http_server_hostname,
-        http_server_port=http_server_port,
-        table_name=table_name,
-    )
+    logger.setLevel(log_level)
 
+    global stats
+    global concurrency
+    global kill_q
+    global kill_q2
+
+    concurrency = conc
+
+    workload = pgworkload.utils.common.import_class_at_runtime(
+        workload_path if workload_path else builtin_workload
+    )
+
+    signal.signal(signal.SIGINT, signal_handler)
+
+    disable_stats = False
+
+    if frequency == 0:
+        disable_stats = True
+        frequency = 10
+
+    stats = pgworkload.utils.common.Stats(frequency, prom_port)
+
+    if iterations:
+        iterations = iterations // concurrency
+
+    q = mp.Queue(maxsize=1000)
+    kill_q = mp.Queue()
+    kill_q2 = mp.Queue()
+
+    c = 0
+
+    threads_per_proc = pgworkload.utils.common.get_threads_per_proc(procs, conc)
+    ramp_interval = int(ramp / len(threads_per_proc))
+
+    processes: list[mp.Process] = []
+
+    for x in threads_per_proc:
+        processes.append(
+            mp.Process(
+                target=worker,
+                args=(
+                    x - 1,
+                    q,
+                    kill_q,
+                    kill_q2,
+                    log_level,
+                    dburl,
+                    autocommit,
+                    workload,
+                    args,
+                    iterations,
+                    duration,
+                    conn_duration,
+                    disable_stats,
+                ),
+            )
+        )
 
-@util_app.command(
-    "yaml",
-    epilog=EPILOG,
-    no_args_is_help=True,
-    help="Generate YAML data generation file from a DDL SQL file.",
-)
-def util_yaml(
-    input: Optional[Path] = typer.Option(
-        ...,
-        "--input",
-        "-i",
-        help="Filepath to the DDL SQL file.",
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-        writable=False,
-        readable=True,
-        resolve_path=True,
-    ),
-    output: Optional[Path] = typer.Option(
-        None,
-        "--output",
-        "-o",
-        show_default=False,
-        help="Output filepath. Defaults to <input-basename>.yaml.",
-        exists=False,
-        file_okay=True,
-        dir_okay=True,
-        writable=False,
-        readable=True,
-        resolve_path=True,
-    ),
+    threading.Thread(
+        target=__ramp_up, daemon=True, args=(processes, ramp_interval)
+    ).start()
+
+    try:
+        stat_time = time.time() + frequency
+        while True:
+            try:
+                # read from the queue for stats or completion messages
+                tup = q.get(block=False)
+                if isinstance(tup, tuple):
+                    stats.add_latency_measurement(*tup)
+                else:
+                    c += 1
+            except queue.Empty:
+                pass
+
+            if c >= concurrency:
+                if isinstance(tup, psycopg.errors.UndefinedTable):
+                    logger.error(tup)
+                    logger.error(
+                        "The schema is not present. Did you initialize the workload?"
+                    )
+                    sys.exit(1)
+                elif isinstance(tup, Exception):
+                    logger.error("Exception raised: %s" % tup)
+                    sys.exit(1)
+                else:
+                    logger.info(
+                        "Requested iteration/duration limit reached. Printing final stats"
+                    )
+                    __print_stats()
+
+                    sys.exit(0)
+
+            if time.time() >= stat_time:
+                __print_stats()
+                stats.new_window()
+                stat_time = time.time() + frequency
+
+    except Exception as e:
+        logger.error(traceback.format_exc())
+
+
+def worker(
+    thread_count: int,
+    q: mp.Queue,
+    kill_q: mp.Queue,
+    kill_q2: mp.Queue,
+    log_level: str,
+    dburl: str,
+    autocommit: bool,
+    workload: object,
+    args: dict,
+    iterations: int,
+    duration: int,
+    conn_duration: int,
+    disable_stats: bool,
 ):
-    pgworkload.models.util.util_yaml(input=input, output=output)
-
-
-def __validate(procs: int, dburl: str, app_name: str, args: str, workload_path: str):
-    """Performs pgworkload initialization steps
+    """Process worker function to run the workload in a multiprocessing env
 
     Args:
-        args (argparse.Namespace): args passed at the CLI
-
-    Returns:
-        argparse.Namespace: updated args
+        thread_count(int): The number of threads to create
+        q (mp.Queue): queue to report query metrics
+        kill_q (mp.Queue): queue to handle stopping the worker
+        kill_q2 (mp.Queue): queue to handle stopping the worker
+        dburl (str): connection string to the database
+        autocommit (bool): whether to set autocommit for the connection
+        workload (object): workload class object
+        args (dict): args to init the workload class
+        iterations (int): count of workload iteration before returning
+        duration (int): seconds before returning
+        conn_duration (int): seconds before restarting the database connection
+        disable_stats: (bool): flag to send or not stats back to the mainthread
     """
+    logger.setLevel(log_level)
 
-    workload = pgworkload.utils.util.import_class_at_runtime(workload_path)
-
-    if not procs:
-        procs = os.cpu_count()
+    threads: list[threading.Thread] = []
 
-    if not re.search(r".*://.*/(.*)\?", dburl):
-        logger.error(
-            "The connection string needs to point to a database. Example: postgres://root@localhost:26257/postgres?sslmode=disable"
+    for _ in range(thread_count):
+        thread = threading.Thread(
+            target=worker,
+            daemon=True,
+            args=(
+                0,
+                q,
+                kill_q,
+                kill_q2,
+                log_level,
+                dburl,
+                autocommit,
+                workload,
+                args,
+                iterations,
+                duration,
+                conn_duration,
+                disable_stats,
+            ),
         )
-        sys.exit(1)
+        thread.start()
+        threads.append(thread)
+
+    if threading.current_thread().name == "MainThread":
+        # capture KeyboardInterrupt and do nothing
+        signal.signal(signal.SIGINT, signal.SIG_IGN)
+
+    # catch exception while instantiating the workload class
+    try:
+        w = workload(args)
+    except Exception as e:
+        stack_lines = traceback.format_exc()
+        q.put(Exception(stack_lines))
+        return
+
+    c = 0
+    endtime = 0
+    conn_endtime = 0
+
+    if duration:
+        endtime = time.time() + duration
+
+    while True:
+        if conn_duration:
+            # reconnect every conn_duration +/- 20%
+            conn_endtime = time.time() + int(conn_duration * random.uniform(0.8, 1.2))
+        # listen for termination messages (poison pill)
+        try:
+            kill_q.get(block=False)
+            logger.debug("Poison pill received")
+            kill_q2.put(None)
+            for x in threads:
+                x.join()
+
+            return
+        except queue.Empty:
+            pass
+        try:
+            with psycopg.connect(dburl, autocommit=autocommit) as conn:
+                logger.debug("Connection started")
+                while True:
+                    # listen for termination messages (poison pill)
+                    try:
+                        kill_q.get(block=False)
+                        logger.debug("Poison pill received")
+                        kill_q2.put(None)
+                        for x in threads:
+                            x.join()
+                        return
+                    except queue.Empty:
+                        pass
+
+                    # return if the limits of either iteration count and duration have been reached
+                    if (iterations and c >= iterations) or (
+                        duration and time.time() >= endtime
+                    ):
+                        logger.debug("Task completed!")
+
+                        # send task completed notification (a None)
+                        q.put(None)
+                        for x in threads:
+                            x.join()
+                        return
+
+                    # break from the inner loop if limit for connection duration has been reached
+                    # this will cause for the outer loop to reset the timer and restart with a new conn
+                    if conn_duration and time.time() >= conn_endtime:
+                        logger.debug(
+                            "conn_duration reached, will reset the connection."
+                        )
+                        break
+
+                    cycle_start = time.time()
+                    for txn in w.run():
+                        start = time.time()
+                        pgworkload.utils.common.run_transaction(
+                            conn, lambda conn: txn(conn)
+                        )
+                        if not q.full() and not disable_stats:
+                            q.put((txn.__name__, time.time() - start))
+
+                    c += 1
+                    if not q.full() and not disable_stats:
+                        q.put(("__cycle__", time.time() - cycle_start))
+
+        # catch any error, pass that error to the MainProcess
+        except psycopg.errors.UndefinedTable as e:
+            q.put(e)
+            return
+        # psycopg.OperationalErrors can either mean a disconnection
+        # or some other errors.
+        # We don't stop if a node goes doesn, instead, wait few seconds and attempt
+        # a new connection.
+        # If the error is not beacuse of a disconnection, then unfortunately
+        # the worker will continue forever
+        except psycopg.Error as e:
+            logger.error(f"{e.__class__.__name__} {e}")
+            logger.info("Sleeping for %s seconds" % (DEFAULT_SLEEP))
+            time.sleep(DEFAULT_SLEEP)
+        except Exception as e:
+            logger.error("Exception: %s" % (e), stack_info=True)
+            q.put(e)
+            return
 
-    dburl = pgworkload.utils.util.set_query_parameter(
-        url=dburl,
-        param_name="application_name",
-        param_value=app_name if app_name else workload.__name__,
-    )
 
-    # load args dict from file or string
-    if args:
-        if os.path.exists(args):
-            with open(args, "r") as f:
-                args = f.read()
-                # parse into JSON if it's a JSON string
-                try:
-                    args = json.load(args)
-                except Exception as e:
-                    pass
-        else:
-            args = yaml.safe_load(args)
-            if isinstance(args, str):
-                logger.error(
-                    f"The value passed to '--args' is not a valid path to a JSON/YAML file, nor has no key:value pairs: '{args}'"
-                )
-                sys.exit(1)
-    else:
-        args = {}
-    return procs, dburl, args
-
-
-def _version_callback(value: bool) -> None:
-    if value:
-        typer.echo(f"pgworkload : {__version__}")
-        typer.echo(f"Python     : {platform.python_version()}")
-        raise typer.Exit()
-
-
-@app.callback()
-def version_option(
-    _: bool = typer.Option(
-        False,
-        "--version",
-        "-v",
-        callback=_version_callback,
-        help="Print the version and exit",
-    ),
-) -> None:
-    pass
+def __print_stats():
+    print(tabulate.tabulate(stats.calculate_stats(), HEADERS), "\n")
```

### Comparing `pgworkload-0.1.6/pgworkload/models/init.py` & `pgworkload-0.1.7/pgworkload/models/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 
 import datetime as dt
 import logging
 import multiprocessing as mp
 import os
 import pgworkload.utils.simplefaker
-import pgworkload.utils.util
+import pgworkload.utils.common
 import psycopg
 import sys
 
 logger = logging.getLogger(__name__)
 
 
 def init(
@@ -37,15 +37,15 @@
     logger.debug("Running init")
 
     if not db:
         db = os.path.splitext(os.path.basename(workload_path))[0].lower()
 
     # PG or CRDB?
     try:
-        dbms: str = pgworkload.utils.util.get_dbms(dburl)
+        dbms: str = pgworkload.utils.common.get_dbms(dburl)
     except ValueError as e:
         logger.error(e)
         sys.exit(1)
     except Exception as e:
         logger.error(e)
         dbms: str = None
 
@@ -58,29 +58,29 @@
     # PART 2 - GENERATE THE DATA
     if skip_gen:
         logger.debug("Skipping init_generate_data")
     else:
         __init_generate_data(procs, workload_path, dbms, csv_max_rows)
 
     # PART 3 - IMPORT THE DATA
-    dburl = pgworkload.utils.util.get_new_dburl(dburl, db)
+    dburl = pgworkload.utils.common.get_new_dburl(dburl, db)
     if skip_import:
         logger.debug("Skipping init_import_data")
     else:
         if not http_server_hostname:
-            http_server_hostname = pgworkload.utils.util.get_hostname()
+            http_server_hostname = pgworkload.utils.common.get_hostname()
             logger.debug(f"Hostname identified as: '{http_server_hostname}'")
 
         __init_import_data(
             dburl, workload_path, dbms, http_server_hostname, http_server_port
         )
 
     # PART 4 - RUN WORKLOAD INIT
     logger.debug("Running workload.init()")
-    workload = pgworkload.utils.util.import_class_at_runtime(workload_path)
+    workload = pgworkload.utils.common.import_class_at_runtime(workload_path)
     try:
         with psycopg.connect(dburl, autocommit=True) as conn:
             workload(args).init(conn)
     except Exception as e:
         logger.error(e)
         sys.exit(1)
 
@@ -143,35 +143,37 @@
 
                 logger.info("Database '%s' created." % db_name)
 
     except Exception as e:
         logger.error("Exception: %s" % (e))
         sys.exit(1)
 
-    dburl = pgworkload.utils.util.get_new_dburl(dburl, db_name)
+    dburl = pgworkload.utils.common.get_new_dburl(dburl, db_name)
 
     # now that we've created the database, connect to that database
     # and load the schema, which can be in a <workload>.sql file
     # or in the self.schema variable of the workload.
 
     # find if the .sql file exists
     schema_sql_file = os.path.abspath(
-        pgworkload.utils.util.get_based_name_dir(workload_path) + ".sql"
+        pgworkload.utils.common.get_based_name_dir(workload_path) + ".sql"
     )
 
     if os.path.exists(path=schema_sql_file):
         logger.debug("Found schema SQL file %s" % schema_sql_file)
         with open(schema_sql_file, "r") as f:
             schema = f.read()
     else:
         logger.debug(
             f"Schema file {schema_sql_file} not found. Loading schema from the 'schema' variable"
         )
         try:
-            workload = pgworkload.utils.util.import_class_at_runtime(path=workload_path)
+            workload = pgworkload.utils.common.import_class_at_runtime(
+                path=workload_path
+            )
             schema = workload({}).schema
         except AttributeError as e:
             logger.error(f"{e}. Make sure self.schema is a valid variable in __init__")
             sys.exit(1)
     try:
         with psycopg.connect(conninfo=dburl, autocommit=True) as conn:
             with conn.cursor() as cur:
@@ -192,23 +194,23 @@
         procs (int): count of concurrent processes to be used to generate the datasets
         workload_path (str): filepath to the workload class
         dbms (str): DBMS technology (CockroachDB, PostgreSQL, etc..)
     """
     logger.debug("Running init_generate_data")
     # description of how to generate the data is in workload variable self.load
 
-    load = pgworkload.utils.util.get_workload_load(workload_path)
+    load = pgworkload.utils.common.get_workload_load(workload_path)
     if not load:
         logger.info(
             "Data generation definition file (.yaml) or variable (self.load) not defined. Skipping"
         )
         return
 
     # get the dirname to put the csv files
-    csv_dir: str = pgworkload.utils.util.get_based_name_dir(workload_path)
+    csv_dir: str = pgworkload.utils.common.get_based_name_dir(workload_path)
 
     # backup the current directory as to not override
     if os.path.isdir(csv_dir):
         os.rename(
             csv_dir, csv_dir + "." + dt.datetime.utcnow().strftime("%Y%m%d-%H%M%S")
         )
 
@@ -238,20 +240,20 @@
         workload_path (str): filepath to the workload class
         dbms (str): DBMS technology (CockroachDB, PostgreSQL, etc..)
         http_server_hostname (str): The hostname of the server that serves the CSV files
         http_server_port (str): The port of the server that serves the CSV files
     """
     logger.debug("Running init_import_data")
 
-    csv_dir = pgworkload.utils.util.get_based_name_dir(workload_path)
-    load = pgworkload.utils.util.get_workload_load(workload_path)
+    csv_dir = pgworkload.utils.common.get_based_name_dir(workload_path)
+    load = pgworkload.utils.common.get_workload_load(workload_path)
 
     # Start the http server in a new Process
     mp.Process(
-        target=pgworkload.utils.util.httpserver, args=(csv_dir, 3000), daemon=True
+        target=pgworkload.utils.common.httpserver, args=(csv_dir, 3000), daemon=True
     ).start()
 
     if os.path.isdir(csv_dir):
         csv_files = os.listdir(csv_dir)
     else:
         logger.debug("Nothing to import, skipping...")
         return
@@ -275,15 +277,15 @@
                         for i in range(0, len(table_csv_files), node_count)
                     ]
 
                     # we import only 'node_count' items at a time, as
                     # we parallelize imports
                     for chunk in chunked_list:
                         if dbms == "CockroachDB":
-                            stmt = pgworkload.utils.util.get_import_stmt(
+                            stmt = pgworkload.utils.common.get_import_stmt(
                                 chunk,
                                 table.replace("__", "."),
                                 http_server_hostname,
                                 http_server_port,
                             )
 
                         elif dbms == "PostgreSQL":
```

### Comparing `pgworkload-0.1.6/pgworkload/utils/builtin_workloads.py` & `pgworkload-0.1.7/pgworkload/utils/builtin_workloads.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.6/pgworkload/utils/simplefaker.py` & `pgworkload-0.1.7/pgworkload/utils/simplefaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,19 @@
             super().__init__(seed, null_pct, array)
             self.min: int = 10 if min is None or min < 0 else min
             self.max: int = self.min + 20 if max is None or max < self.min else max
 
             # make translation table from 0..255 to 97..122
             self.tbl = bytes.maketrans(
                 bytearray(range(256)),
-                bytearray([ord(b"a") + b % 26 for b in range(256)]),
+                bytearray(
+                    [ord(b"a") + b % 26 for b in range(113)]
+                    + [ord(b"0") + b % 10 for b in range(30)]
+                    + [ord(b"A") + b % 26 for b in range(113)]
+                ),
             )
 
         # generate random bytes and translate them to lowercase ascii
         def __next__(self):
             if self.null_pct and self.rng.random() < self.null_pct:
                 return ""
             else:
@@ -378,14 +382,15 @@
     >>> 
     >>> rng2 = random.Random(seed2)
     >>> rng2.randint(0, 1000000)
     140545
     >>> rng2.randint(0, 1000000)
     157597
     """
+
     def generate(
         self,
         load: dict,
         exec_threads: int,
         csv_dir: str,
         delimiter: str,
         compression: str,
```

### Comparing `pgworkload-0.1.6/pgworkload/utils/util.py` & `pgworkload-0.1.7/pgworkload/utils/common.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.6/pyproject.toml` & `pgworkload-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgworkload"
-version = "0.1.6"
+version = "0.1.7"
 description = "Workload framework for the PostgreSQL protocol"
 authors = ["Fabio Ghirardello"]
 license = "GPLv3+"
 readme = "README.md"
 homepage = "https://github.com/fabiog1901/pgworkload"
 repository = "https://github.com/fabiog1901/pgworkload"
 classifiers = [
```

### Comparing `pgworkload-0.1.6/PKG-INFO` & `pgworkload-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgworkload
-Version: 0.1.6
+Version: 0.1.7
 Summary: Workload framework for the PostgreSQL protocol
 Home-page: https://github.com/fabiog1901/pgworkload
 License: GPLv3+
 Author: Fabio Ghirardello
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
```

