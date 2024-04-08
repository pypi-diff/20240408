# Comparing `tmp/tunnelgraf-0.6.1.tar.gz` & `tmp/tunnelgraf-0.6.2.tar.gz`

## Comparing `tunnelgraf-0.6.1.tar` & `tunnelgraf-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/Makefile
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/README.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/cli.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/tunnelgraf.spec
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tests/test_tunnel_def.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tunnelgraf/__init__.py
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tunnelgraf/__main__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tunnelgraf/lastpass_secrets.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tunnelgraf/tunnel_builder.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tunnelgraf/tunnel_definition.py
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/src/tunnelgraf/tunnels.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/LICENSE
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 tunnelgraf-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/Makefile
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/README.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/cli.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/tunnelgraf.spec
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tests/test_tunnel_def.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tunnelgraf/__init__.py
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tunnelgraf/__main__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tunnelgraf/lastpass_secrets.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tunnelgraf/tunnel_builder.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tunnelgraf/tunnel_definition.py
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/src/tunnelgraf/tunnels.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 tunnelgraf-0.6.2/PKG-INFO
```

### Comparing `tunnelgraf-0.6.1/Makefile` & `tunnelgraf-0.6.2/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,14 @@
 	hatch run test:run --cov-config .coveragerc --verbose --cov-report term --cov-report xml --cov=src/tunnelgraf src/tests
 
 clean: ## Clean the project
 	rm -rf dist/ .pytest_cache/
 	find . -name __pycache__ -delete
 
 dev: ## Run the app
-	hatch run python3 src/tunnelgraf/
+	hatch run python3 src/tunnelgraf/ connect ./test.yml
 
 build: ## Build the package
 	hatch build
 
 publish: ## Publish the package
 	hatch publish
```

### Comparing `tunnelgraf-0.6.1/README.md` & `tunnelgraf-0.6.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 intuitive YAML definitions enable version-controlled management of complex
 hierarchical connections.
 
 Tunnelgraf supports the lookup of credentials and hostname/IP endpoints via your
 local ssh config file (~/.ssh/config) or Lastpass, making sharing connection
 schemes more secure.
 
-Tunnelgraf supports including one config file into another to keep the connection
-profiles DRY when managing many similar environments, which is common in most
-SDLCs.
+Tunnelgraf supports including one config file into another to keep the
+connection profiles DRY when managing many similar environments, which is common
+in most SDLCs.
 
 Finally, it can also populate host file entries to redirect DNS names to
 localhost.
 
 ## Advantages
 
 - Connect to arrays of sibling endpoints at any level, e.g. application servers,
@@ -180,7 +180,22 @@
 ]
 ```
 
 If no tunnel id is specified, all tunnels are displayed.
 
 If `--show-credentials` is added, the credentials used when connecting are also
 printed.
+
+## Print URLs
+
+To get json dump of the resulting URLs, run `tunnelgraf urls <config_file>`.
+This will show a default prefix of "ssh://" unless a "protocol" value is
+specified in the data. It will show the dns provided in hosts_file_entry or
+hosts_file_entries if provided, otherwise, the IP address is shown.
+
+```json
+{
+  "jumpbox": ["ssh://<ip address>:22"],
+  "jumpbox2": ["ssh://<domain name>:2224"],
+  "load_balancer": ["https://<fqdn>.local:8443", "https://<fqdn2>:8443"]
+}
+```
```

### Comparing `tunnelgraf-0.6.1/tunnelgraf.spec` & `tunnelgraf-0.6.2/tunnelgraf.spec`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.1/src/tests/test_tunnel_def.py` & `tunnelgraf-0.6.2/src/tests/test_tunnel_def.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.1/src/tunnelgraf/__init__.py` & `tunnelgraf-0.6.2/src/tunnelgraf/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 import click
 from tunnelgraf.tunnels import Tunnels
-from io import TextIOWrapper
 from importlib.metadata import version
 import sys
 import json
+import pathlib
 
 
 @click.group()
 @click.version_option(
     package_name="tunnelgraf", prog_name="tunnelgraf", version=version("tunnelgraf")
 )
 @click.pass_context
 def cli(ctx) -> None:
     pass
 
 
 @cli.command(
     help="Connect to the remote tunnels defined in a connection profile. Requires an argument containing the path to the connection profile, e.g `tunnelgraf connect <tunnelfile.yml>"
 )
-@click.argument("config_file", envvar="TUNNELGRAF_CONFIG", type=click.File("r"))
-def connect(config_file: TextIOWrapper) -> None:
+@click.argument(
+    "config_file",
+    envvar="TUNNELGRAF_CONFIG",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
+)
+def connect(config_file: pathlib.Path) -> None:
     Tunnels(config_file)
 
 
 @cli.command(help="Print the resulting tunnels configuration w/o connecting.")
-@click.argument("config_file", envvar="TUNNELGRAF_CONFIG", type=click.File("r"))
+@click.argument(
+    "config_file",
+    envvar="TUNNELGRAF_CONFIG",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
+)
 @click.option(
     "--tunnel-id",
     "-t",
     help="Print the resulting configuration of the specified tunnel id.",
     default=None,
 )
 @click.option(
     "--show-credentials",
     help="Print the credentials used when connecting. Default: false",
     is_flag=True,
     default=False,
 )
-def show(config_file: TextIOWrapper, tunnel_id: str, show_credentials: bool) -> None:
+def show(config_file: pathlib.Path, tunnel_id: str, show_credentials: bool) -> None:
     tunnels = Tunnels(
         config_file, connect_tunnels=False, show_credentials=show_credentials
     ).tunnel_configs
     if tunnel_id:
         try:
             this_tunnel = [tunnel for tunnel in tunnels if tunnel_id == tunnel["id"]][0]
         except IndexError:
@@ -51,16 +73,27 @@
     else:
         print(json.dumps(tunnels))
 
 
 @cli.command(
     help="Print the URLs to access each tunnel. Protocol is displayed as ssh unless specified."
 )
-@click.argument("config_file", envvar="TUNNELGRAF_CONFIG", type=click.File("r"))
-def urls(config_file: TextIOWrapper) -> None:
+@click.argument(
+    "config_file",
+    envvar="TUNNELGRAF_CONFIG",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
+)
+def urls(config_file: pathlib.Path) -> None:
     tunnels = Tunnels(config_file, connect_tunnels=False).tunnel_configs
     links: dict = {}
     for tunnel in tunnels:
         links[tunnel["id"]]: list = []
         if "hosts_file_entry" in tunnel.keys() and tunnel["hosts_file_entry"]:
             host = tunnel["hosts_file_entry"]
             links[tunnel["id"]].append(
```

### Comparing `tunnelgraf-0.6.1/src/tunnelgraf/lastpass_secrets.py` & `tunnelgraf-0.6.2/src/tunnelgraf/lastpass_secrets.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.1/src/tunnelgraf/tunnel_builder.py` & `tunnelgraf-0.6.2/src/tunnelgraf/tunnel_builder.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.1/src/tunnelgraf/tunnel_definition.py` & `tunnelgraf-0.6.2/src/tunnelgraf/tunnel_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import yaml
 from tunnelgraf.lastpass_secrets import LastpassSecret
 
 
 class TunnelDefinition(BaseModel):
     id: str = Field(..., alias="id")  # Required field
     include: Optional[str] = Field(None, alias="include")  # Not required
+    config_file_path: Optional[Path] = Field(
+        None, alias="config_file_path"
+    )  # Not required
     host: Optional[str] = Field(None, alias="host")  # Not Required
     port: Optional[int] = Field(22, alias="port")  # Not Required
     localbindaddress: Optional[str] = Field("127.0.0.1", alias="localbindaddress")
     localbindport: int = Field(..., alias="localbindport")  # Required field
     protocol: Optional[str] = Field("ssh", alias="protocol")  # Not required
     sshuser: Optional[str] = Field(None, alias="sshuser")  # Not required
     sshpass: Optional[str] = Field(None, alias="sshpass")  # Not required
@@ -53,16 +56,19 @@
         # Load defaults from lastpass if lastpass is provided
         self.get_lastpass_secret_config()
 
         # Validate the model
         self.validate()
 
     def fetch_include_values(self) -> None | dict:
-        if self.include:
-            f = open(self.include, "r")
+        if self.include and self.config_file_path is not None:
+            if path.isabs(self.include):
+                f = open(self.include, "r")
+            else:
+                f = open(self.config_file_path.joinpath(self.include), "r")
             return yaml.safe_load(f)
         else:
             return None
 
     def get_ssh_config(self) -> None:
         """Looks up the ssh config file for the host, port, and credentials."""
         this_ssh_config: SSHConfigDict = self._ssh_config.lookup(self.id)
```

### Comparing `tunnelgraf-0.6.1/src/tunnelgraf/tunnels.py` & `tunnelgraf-0.6.2/src/tunnelgraf/tunnels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 from time import sleep
-from io import TextIOWrapper
+from pathlib import Path
 
 import yaml
 from python_hosts import Hosts, HostsEntry, HostsException
 
 from tunnelgraf.tunnel_builder import TunnelBuilder
 from tunnelgraf.tunnel_definition import TunnelDefinition
 
@@ -14,20 +14,22 @@
     """
     Creates an ssh tunnel, connecting a remote endpoint through a bastion
     and binding it to a local port, as specified in the provided config file.
     """
 
     def __init__(
         self,
-        config_file: TextIOWrapper,
+        config_file_path: Path,
         connect_tunnels: bool = True,
         show_credentials: bool = False,
     ):
-        self._config_file: str = config_file.read()
+        with config_file_path.open() as cf:
+            self._config_file: str = cf.read()
         self.config: dict | list = self._get_config()
+        self.config["nexthop"]["config_file_path"] = config_file_path.parent
         self.tunnel_defs: TunnelDefinition | list[TunnelDefinition] = TunnelDefinition(
             **self.config
         )
         self._excluded_fields: list[str] = [
             "nexthop",
             "nexthops",
             "localbindaddress",
```

### Comparing `tunnelgraf-0.6.1/LICENSE` & `tunnelgraf-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.1/pyproject.toml` & `tunnelgraf-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tunnelgraf"
-version = "0.6.1"
+version = "0.6.2"
 dependencies = [
   "click~=8.0.0",
   "sshtunnel~=0.4.0",
   "pyyaml~=6.0.0",
   "python-hosts~=1.0.5",
   "pydantic~=2.5.0",
   "paramiko~=3.4.0",
```

### Comparing `tunnelgraf-0.6.1/PKG-INFO` & `tunnelgraf-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tunnelgraf
-Version: 0.6.1
+Version: 0.6.2
 Summary: Hierarchical SSH tunnel management made easy. Securely define and share multihop connection profiles that expose a graph of remote endpoints as localhost.
 Project-URL: Homepage, https://github.com/denniswalker/tunnelgraf
 Project-URL: Documentation, https://github.com/denniswalker/tunnelgraf/blob/main/README.md
 Project-URL: Repository, https://github.com/denniswalker/tunnelgraf
 Project-URL: Issues, https://github.com/denniswalker/tunnelgraf/issues
 Author-email: Dennis Walker <denniswalker@me.com>
 Maintainer-email: Dennis Walker <denniswalker@me.com>
```

