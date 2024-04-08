# Comparing `tmp/marops_cli-2.9.4.tar.gz` & `tmp/marops_cli-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marops_cli-2.9.4.tar", last modified: Fri Oct  6 07:08:29 2023, max compression
+gzip compressed data, was "marops_cli-2.9.5.tar", last modified: Thu Oct 12 22:27:13 2023, max compression
```

## Comparing `marops_cli-2.9.4.tar` & `marops_cli-2.9.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:29.424647 marops_cli-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-06 07:08:29.424647 marops_cli-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-06 07:07:51.000000 marops_cli-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:29.424647 marops_cli-2.9.4/marops_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:29.424647 marops_cli-2.9.4/marops_cli/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/docker/docker-compose.base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/docker/docker-compose.demo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/docker/docker-compose.dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/docker/docker-compose.prod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:29.424647 marops_cli-2.9.4/marops_cli/groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/groups/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/groups/poetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/groups/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-10-06 07:07:51.000000 marops_cli-2.9.4/marops_cli/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:29.424647 marops_cli-2.9.4/marops_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 07:08:29.000000 marops_cli-2.9.4/marops_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-10-06 07:08:29.424647 marops_cli-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 07:07:51.000000 marops_cli-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:13.168230 marops_cli-2.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-12 22:27:13.164229 marops_cli-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-12 22:26:33.000000 marops_cli-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:13.164229 marops_cli-2.9.5/marops_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:13.164229 marops_cli-2.9.5/marops_cli/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/docker/docker-compose.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/docker/docker-compose.demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/docker/docker-compose.dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/docker/docker-compose.prod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:13.164229 marops_cli-2.9.5/marops_cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/groups/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/groups/poetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/groups/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-10-12 22:26:33.000000 marops_cli-2.9.5/marops_cli/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:13.164229 marops_cli-2.9.5/marops_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 22:27:13.000000 marops_cli-2.9.5/marops_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-10-12 22:27:13.168230 marops_cli-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 22:26:33.000000 marops_cli-2.9.5/setup.py
```

### Comparing `marops_cli-2.9.4/PKG-INFO` & `marops_cli-2.9.5/marops_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: marops_cli
-Version: 2.9.4
+Name: marops-cli
+Version: 2.9.5
 Summary: A CLI for interacting with the MarOps platform
 Home-page: https://github.com/Greenroom-Robotics/marops
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `marops_cli-2.9.4/README.md` & `marops_cli-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `marops_cli-2.9.4/marops_cli/cli.py` & `marops_cli-2.9.5/marops_cli/cli.py`

 * *Files identical despite different names*

### Comparing `marops_cli-2.9.4/marops_cli/docker/docker-compose.base.yaml` & `marops_cli-2.9.5/marops_cli/docker/docker-compose.base.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
       - /var/run/docker.sock:/var/run/docker.sock
 
   marops_ui:
     container_name: marops_ui
     image: ghcr.io/greenroom-robotics/marops_ui:$MAROPS_VERSION
     build:
       dockerfile: ./docker/Dockerfile.marops_ui
-      args:
-        VITE_HASURA_HTTP_URL: http://localhost:7003/v1/graphql
-        VITE_HASURA_WS_URL: ws://localhost:7003/v1/graphql
-        VITE_CORE_URL: http://localhost:7004
-        VITE_TILER_URL: http://localhost:7001
-        VITE_DOCS_URL: http://localhost:7005
-        VITE_STUDIO_URL: http://localhost:7006
+    environment:
+      HASURA_HTTP_URL: http://localhost:7003/v1/graphql
+      HASURA_WS_URL: ws://localhost:7003/v1/graphql
+      CORE_URL: http://localhost:7004
+      TILER_URL: http://localhost:7001
+      DOCS_URL: http://localhost:7005
+      STUDIO_URL: http://localhost:7006
     ports:
       - "7000:7000"
     restart: unless-stopped
 
   marops_docs:
     container_name: marops_docs
     image: ghcr.io/greenroom-robotics/marops_docs:$MAROPS_VERSION
```

### Comparing `marops_cli-2.9.4/marops_cli/docker/docker-compose.demo.yaml` & `marops_cli-2.9.5/marops_cli/docker/docker-compose.demo.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -15,23 +15,21 @@
       - "443:443"
       - "8080:8080"
     restart: unless-stopped
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock:ro"
 
   marops_ui:
-    build:
-      dockerfile: ./docker/Dockerfile.marops_ui
-      args:
-        VITE_HASURA_HTTP_URL: https://hasura.$PROXY_HOST/v1/graphql
-        VITE_HASURA_WS_URL: wss://hasura.$PROXY_HOST/v1/graphql
-        VITE_CORE_URL: https://core.$PROXY_HOST
-        VITE_TILER_URL: https://tiler.$PROXY_HOST
-        VITE_DOCS_URL: https://docs.$PROXY_HOST
-        VITE_STUDIO_URL: https://studio.$PROXY_HOST
+    environment:
+      HASURA_HTTP_URL: https://hasura.$PROXY_HOST/v1/graphql
+      HASURA_WS_URL: wss://hasura.$PROXY_HOST/v1/graphql
+      CORE_URL: https://core.$PROXY_HOST
+      TILER_URL: https://tiler.$PROXY_HOST
+      DOCS_URL: https://docs.$PROXY_HOST
+      STUDIO_URL: https://studio.$PROXY_HOST
     command: yarn serve
     labels:
       - "traefik.enable=true"
       - "traefik.http.routers.ui.rule=Host(`$PROXY_HOST`)"
       - "traefik.http.routers.ui.entrypoints=web,websecure"
 
   marops_docs:
@@ -55,18 +53,18 @@
       - "traefik.enable=true"
       - "traefik.http.routers.hasura.rule=Host(`hasura.$PROXY_HOST`)"
       - "traefik.http.routers.hasura.entrypoints=web,websecure"
 
   studio:
     labels:
       - "traefik.enable=true"
-      - "traefik.http.services.$SUBDOMAIN-studio-docker.loadbalancer.server.port=8080"
-      - "traefik.http.routers.studio.rule=Host(`studio.$SUBDOMAIN.greenroomrobotics.com`)"
+      - "traefik.http.services.studio.loadbalancer.server.port=8080"
+      - "traefik.http.routers.studio.rule=Host(`studio.$PROXY_HOST`)"
       - "traefik.http.routers.studio.entrypoints=web,websecure"
 
   marops_chart_tiler:
     entrypoint: node ./src/main.js --config /app/data/config.json --public_url https://tiler.$PROXY_HOST
     labels:
       - "traefik.enable=true"
-      - "traefik.http.services.chart-tiler-docker.loadbalancer.server.port=8080" # this container also exposes port 80 (it shouldn't)
+      - "traefik.http.services.chart-tiler.loadbalancer.server.port=8080" # this container also exposes port 80 (it shouldn't)
       - "traefik.http.routers.tiler.rule=Host(`tiler.$PROXY_HOST`)"
       - "traefik.http.routers.tiler.entrypoints=web,websecure"
```

### Comparing `marops_cli-2.9.4/marops_cli/docker/docker-compose.dev.yaml` & `marops_cli-2.9.5/marops_cli/docker/docker-compose.dev.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 version: "3.8"
 
 services:
   marops_ui:
-    environment:
-      NODE_ENV: development
-      VITE_HASURA_HTTP_URL: http://localhost:7003/v1/graphql
-      VITE_HASURA_WS_URL: ws://localhost:7003/v1/graphql
-      VITE_CORE_URL: http://localhost:7004
-      VITE_TILER_URL: http://localhost:7001
-      VITE_DOCS_URL: http://localhost:7005
-      VITE_STUDIO_URL: http://localhost:7006
     volumes:
       - ./libs/marops_interfaces/src:/app/libs/marops_interfaces/src
       - ./projects/marops_ui/src:/app/projects/marops_ui/src
 
   marops_docs:
     volumes:
       - ./projects/docs:/app
```

### Comparing `marops_cli-2.9.4/marops_cli/groups/base.py` & `marops_cli-2.9.5/marops_cli/groups/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "traefik"
 ]
 
 def marops_config_read():
     config = marops_config.read()
     version = get_marops_version()
 
-    if version is not "latest" and not config.prod:
+    if version != "latest" and not config.prod:
         click.echo(click.style(f"Setting config.prod to True.", fg="red"))
         click.echo(click.style(f"You cannot run MarOps in developer mode when using the production vesion of marops-cli", fg="red"))
         config.prod = True
 
     return config
 
 
@@ -107,32 +107,37 @@
 
 @click.command(name="up")
 @click.option(
     "--build",
     help="Should we do a docker build",
     is_flag=True,
 )
+@click.option(
+    "--pull",
+    help="Should we do a docker pull",
+    is_flag=True,
+)
 @click.argument(
     "services",
     required=False,
     nargs=-1,
     type=click.Choice(SERVICES),
 )
-def up(build: bool, services: List[str]):
+def up(build: bool, pull: bool, services: List[str]):
     """Starts MarOps"""
     config = marops_config_read()
     _log_config(config)
     _set_config_to_env(config)
 
     docker = DockerClient(
         compose_files=_get_compose_files(config),
         compose_project_directory=get_project_root(),
     )
     services_list = list(services) if services else None
-    docker.compose.up(detach=True, build=build, services=services_list)
+    docker.compose.up(detach=True, build=build, services=services_list, pull="always" if pull else "missing")
    
 @click.command(name="restart")
 @click.argument(
     "services",
     required=False,
     nargs=-1,
     type=click.Choice(SERVICES),
@@ -175,16 +180,22 @@
     result = click.prompt(
         "Are you sure you want to upgrade?", default="y", type=click.Choice(["y", "n"])
     )
     if result == "n":
         return
 
     if version:
+        click.echo(click.style("Upgrading marops-config...", fg="blue"))
+        call(f"pip install --upgrade marops-config=={version}")
+        click.echo(click.style("Upgrading marops-cli...", fg="blue"))
         call(f"pip install --upgrade marops-cli=={version}")
     else:
+        click.echo(click.style("Upgrading marops-config...", fg="blue"))
+        call("pip install --upgrade marops-config")
+        click.echo(click.style("Upgrading marops-cli...", fg="blue"))
         call("pip install --upgrade marops-cli")
 
     click.echo(click.style("Upgrade of MarOps CLI complete.", fg="green"))
     click.echo(
         click.style(
             "Run `marops up` to upgrade MarOps.", fg="green"
         )
```

### Comparing `marops_cli-2.9.4/marops_cli/groups/poetry.py` & `marops_cli-2.9.5/marops_cli/groups/poetry.py`

 * *Files identical despite different names*

### Comparing `marops_cli-2.9.4/marops_cli/groups/setup.py` & `marops_cli-2.9.5/marops_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `marops_cli-2.9.4/marops_cli/helpers.py` & `marops_cli-2.9.5/marops_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `marops_cli-2.9.4/marops_cli.egg-info/PKG-INFO` & `marops_cli-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: marops-cli
-Version: 2.9.4
+Name: marops_cli
+Version: 2.9.5
 Summary: A CLI for interacting with the MarOps platform
 Home-page: https://github.com/Greenroom-Robotics/marops
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `marops_cli-2.9.4/marops_cli.egg-info/SOURCES.txt` & `marops_cli-2.9.5/marops_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marops_cli-2.9.4/setup.cfg` & `marops_cli-2.9.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = marops_cli
-version = 2.9.4
+version = 2.9.5
 url = https://github.com/Greenroom-Robotics/marops
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

