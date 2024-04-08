# Comparing `tmp/mdapi-3.1.4.tar.gz` & `tmp/mdapi-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdapi-3.1.4.tar", max compression
+gzip compressed data, was "mdapi-3.1.5.tar", max compression
```

## Comparing `mdapi-3.1.4.tar` & `mdapi-3.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-06-06 09:38:09.611985 mdapi-3.1.4/LICENSE
--rw-r--r--   0        0        0     6010 2023-06-06 09:38:09.611985 mdapi-3.1.4/README.md
--rw-r--r--   0        0        0     2452 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/__init__.py
--rw-r--r--   0        0        0      878 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/confdata/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/confdata/servlogr.py
--rw-r--r--   0        0        0     2432 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/confdata/standard.py
--rw-r--r--   0        0        0     1039 2023-06-06 09:42:10.553996 mdapi-3.1.4/mdapi/database/__init__.py
--rw-r--r--   0        0        0     5817 2023-07-20 09:55:32.668613 mdapi-3.1.4/mdapi/database/base.py
--rw-r--r--   0        0        0    11651 2023-11-15 09:47:37.564946 mdapi-3.1.4/mdapi/database/main.py
--rw-r--r--   0        0        0     4421 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/database/sqlq.py
--rw-r--r--   0        0        0     2414 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/main.py
--rw-r--r--   0        0        0     7420 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/services/__init__.py
--rw-r--r--   0        0        0     2535 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/services/apimodel.py
--rw-r--r--   0        0        0     4267 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/services/appviews.py
--rw-r--r--   0        0        0     5528 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/services/homepage.html
--rw-r--r--   0        0        0     2811 2023-06-06 09:38:09.615318 mdapi-3.1.4/mdapi/services/main.py
--rw-r--r--   0        0        0     2362 2023-11-15 10:06:24.758229 mdapi-3.1.4/pyproject.toml
--rw-r--r--   0        0        0     7890 1970-01-01 00:00:00.000000 mdapi-3.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-02 06:10:16.763448 mdapi-3.1.5/LICENSE
+-rw-r--r--   0        0        0     6010 2024-04-02 06:10:16.764448 mdapi-3.1.5/README.md
+-rw-r--r--   0        0        0     2452 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/__init__.py
+-rw-r--r--   0        0        0      878 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/confdata/__init__.py
+-rw-r--r--   0        0        0     1357 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/confdata/servlogr.py
+-rw-r--r--   0        0        0     2447 2024-04-08 07:42:05.217644 mdapi-3.1.5/mdapi/confdata/standard.py
+-rw-r--r--   0        0        0      878 2024-04-08 07:42:05.217644 mdapi-3.1.5/mdapi/database/__init__.py
+-rw-r--r--   0        0        0     5746 2024-04-08 07:42:05.217644 mdapi-3.1.5/mdapi/database/base.py
+-rw-r--r--   0        0        0    11603 2024-04-08 07:42:05.218644 mdapi-3.1.5/mdapi/database/main.py
+-rw-r--r--   0        0        0     4421 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/database/sqlq.py
+-rw-r--r--   0        0        0     2439 2024-04-08 07:42:05.219644 mdapi-3.1.5/mdapi/main.py
+-rw-r--r--   0        0        0     7359 2024-04-08 07:42:05.219644 mdapi-3.1.5/mdapi/services/__init__.py
+-rw-r--r--   0        0        0     2535 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/services/apimodel.py
+-rw-r--r--   0        0        0     4264 2024-04-08 07:42:05.219644 mdapi-3.1.5/mdapi/services/appviews.py
+-rw-r--r--   0        0        0     5581 2024-04-08 07:50:54.158037 mdapi-3.1.5/mdapi/services/homepage.html
+-rw-r--r--   0        0        0     2811 2024-04-02 06:10:16.765448 mdapi-3.1.5/mdapi/services/main.py
+-rw-r--r--   0        0        0     2219 2024-04-08 07:50:54.158037 mdapi-3.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7941 1970-01-01 00:00:00.000000 mdapi-3.1.5/PKG-INFO
```

### Comparing `mdapi-3.1.4/LICENSE` & `mdapi-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/README.md` & `mdapi-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/mdapi/__init__.py` & `mdapi-3.1.5/mdapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/mdapi/confdata/__init__.py` & `mdapi-3.1.5/mdapi/confdata/__init__.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/mdapi/confdata/servlogr.py` & `mdapi-3.1.5/mdapi/confdata/servlogr.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/mdapi/confdata/standard.py` & `mdapi-3.1.5/mdapi/confdata/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 """
 mdapi default configuration.
 """
 
 # url to the database server:
-DB_FOLDER = "/var/tmp"
+DB_FOLDER = "/var/tmp"  # noqa : S108
 
 LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "standard": {
             "format": "%(asctime)s [%(levelname)s] %(message)s",
```

### Comparing `mdapi-3.1.4/mdapi/database/__init__.py` & `mdapi-3.1.5/mdapi/database/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,7 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Any Red Hat trademarks that are incorporated in the source
 code or documentation are not subject to the GNU General Public
 License and may only be used or replicated with the express permission
 of Red Hat, Inc.
 """
-
-
-def check_archive_validity():
-    """
-    This is a workaround and not a fix.
-    See https://github.com/fedora-infra/mdapi/issues/161
-    """
-    return True
```

### Comparing `mdapi-3.1.4/mdapi/database/base.py` & `mdapi-3.1.5/mdapi/database/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import sqlite3
 
 from mdapi.confdata import servlogr
 from mdapi.database.sqlq import DEFAULT_QUERY, INDEX_DATABASE, OBTAIN_TABLE_NAMES, queries
 
 
 def index_database(name, tempdtbs):
-    servlogr.logrobjc.info("[%s] Indexing database %s" % (name, tempdtbs))
+    servlogr.logrobjc.info(f"[{name}] Indexing database {tempdtbs}")
     if tempdtbs.endswith("primary.sqlite"):
         # TODO: Try the "with sqlite3.connect(tempdtbs) as connobjc" statement here
         connobjc = sqlite3.connect(tempdtbs)
         connobjc.execute(INDEX_DATABASE)
         connobjc.commit()
         connobjc.close()
 
@@ -76,63 +76,60 @@
         else:
             name = rowe[0]
         return name.split("(")[0]
 
     def obtain_all_rows(self, location, tableobj, cacheobj):
         connobjc = sqlite3.connect(location)
         sqlquery = queries.get(tableobj, DEFAULT_QUERY).format(table=tableobj)
-        for indx, rowe in enumerate(connobjc.execute(sqlquery)):
+        for indx, rowe in enumerate(connobjc.execute(sqlquery)):  # noqa : B007
             if tableobj in self.cache_dependent_tables:
                 if rowe[0] in cacheobj:
                     yield (cacheobj[rowe[0]], *rowe[1:])
                 else:
-                    servlogr.logrobjc.debug(
-                        "[%s] %s does not appear in the %s cache for %s"
-                        % (self.name, rowe[0], tableobj, location)
-                    )
-                    servlogr.logrobjc.debug("[%s] Dropping from comparison" % self.name)
+                    servlogr.logrobjc.debug(f"[{self.name}] {rowe[0]} does not appear in the {tableobj} cache for {location}")  # noqa : E501
+                    servlogr.logrobjc.debug(f"[{self.name}] Dropping from comparison")
             else:
                 yield rowe
         connobjc.close()
 
     def build_cache(self, location, tableobj, cacheobjc):
         connobjc = sqlite3.connect(location)
         sqlquery = queries.get(tableobj, DEFAULT_QUERY).format(table=tableobj)
-        for pkgId, pkgname, *args in connobjc.execute(sqlquery):
+        for pkgId, pkgname, *args in connobjc.execute(sqlquery):  # noqa : B007
             cacheobjc[pkgId] = pkgname
         connobjc.close()
 
     def should_compare(self, tableobj):
         for test, trgt in self.ignored_database_tables:
             if test in self.dbsA and tableobj == trgt:
                 return False
         return True
 
     def main(self):
-        servlogr.logrobjc.info("[%s] Comparing %s against %s" % (self.name, self.dbsA, self.dbsB))
+        servlogr.logrobjc.info(f"[{self.name}] Comparing {self.dbsA} against {self.dbsB}")
 
         tablistA = list(self.obtain_table_names(self.dbsA))
         tablistB = list(self.obtain_table_names(self.dbsB))
 
         if not tablistA and not tablistB:
             servlogr.logrobjc.error("Something is not right")
             raise RuntimeError("Something is not right")
 
         if not tablistB:
             # We have never downloaded this before...
             # so we have nothing to compare it against. Just return and say there
             # are "no differences".
-            servlogr.logrobjc.warning(
-                "[%s] Database empty - %s cannot compare" % (self.name, self.dbsB)
-            )
+            servlogr.logrobjc.warning(f"[{self.name}] Database empty - {self.dbsB} cannot compare")
             return set()
 
-        assert len(tablistA) == len(tablistB), "Cannot compare disparate databases"
+        if len(tablistA) != len(tablistB):
+            raise ValueError("Cannot compare disparate databases")
+
         # These should be the same
-        tblelist = tablistA = tablistB
+        tblelist = tablistA
 
         tblelist = [tableobj for tableobj in tblelist if self.should_compare(tableobj)]
 
         # Compare the contents of both tables and return a list of changed packages
         rsltdata = set()
         for tableobj in tblelist:
             if tableobj in self.cache_producing_tables:
```

### Comparing `mdapi-3.1.4/mdapi/database/main.py` & `mdapi-3.1.5/mdapi/database/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,106 +28,98 @@
 import os.path
 import shutil
 import tarfile
 import tempfile
 import time
 from xml.etree import ElementTree
 
+import pyzstd
 import requests
 from fedora_messaging.api import publish
 from fedora_messaging.exceptions import ConnectionException, PublishReturned
 from mdapi_messages.messages import RepoUpdateV1
 
 from mdapi.confdata import servlogr, standard
-from mdapi.database import check_archive_validity
 from mdapi.database.base import compare_databases, index_database
 
 
 def list_branches(status="Active"):
-    urlx = "%s/api/collections?clt_status=%s" % (standard.PKGDB2_URL, status)
-    resp = requests.get(urlx, verify=standard.PKGDB2_VERIFY)
+    urlx = f"{standard.PKGDB2_URL}/api/collections?clt_status={status}"
+    resp = requests.get(urlx, verify=standard.PKGDB2_VERIFY)  # noqa : S113
     resp.raise_for_status()
     data = resp.json()
     servlogr.logrobjc.info("Branches metadata acquired.")
     return data["collections"]
 
 
 def fetch_database(name, repmdurl, location):
-    servlogr.logrobjc.info("[%s] Downloading file %s to %s" % (name, repmdurl, location))
-    resp = requests.get(repmdurl, verify=standard.DL_VERIFY)
+    servlogr.logrobjc.info(f"[{name}] Downloading file {repmdurl} to {location}")
+    resp = requests.get(repmdurl, verify=standard.DL_VERIFY)  # noqa : S113
     resp.raise_for_status()
     with open(location, "wb") as filestrm:
         filestrm.write(resp.content)
 
 
 def extract_database(name, arcvname, location):
-    servlogr.logrobjc.info("[%s] Extracting %s to %s" % (name, arcvname, location))
+    servlogr.logrobjc.info(f"[{name}] Extracting {arcvname} to {location}")
     if arcvname.endswith(".xz"):
         with lzma.open(arcvname) as inp, open(location, "wb") as otptfile:
             otptfile.write(inp.read())
     elif arcvname.endswith(".tar.gz"):
         with tarfile.open(arcvname) as tararchv:
-            tararchv.extractall(path=location, members=check_archive_validity())
+            tararchv.extractall(path=location, filter="data")
     elif arcvname.endswith(".gz"):
         with gzip.open(arcvname, "rb") as inp, open(location, "wb") as otptfile:
             otptfile.write(inp.read())
     elif arcvname.endswith(".bz2"):
         with bz2.open(arcvname) as inp, open(location, "wb") as otptfile:
             otptfile.write(inp.read())
     elif arcvname.endswith(".zst"):
-        import pyzstd
-
         with open(arcvname, "rb") as inp, open(location, "wb") as otptfile:
             pyzstd.decompress_stream(inp, otptfile)
     else:
-        servlogr.logrobjc.error("Could not extract %s" % (arcvname))
+        servlogr.logrobjc.error(f"Could not extract {arcvname}")
         raise NotImplementedError(arcvname)
 
 
 def publish_changes(name, packages, repmdurl):
-    servlogr.logrobjc.info("[%s] Publishing differences to Fedora Messaging bus" % (name))
+    servlogr.logrobjc.info(f"[{name}] Publishing differences to Fedora Messaging bus")
 
     modified = bool(packages)
     if not modified:
-        servlogr.logrobjc.warning(
-            "[%s] No real changes detected - Skipping publishing on Fedora Messaging bus" % (name)
-        )
+        servlogr.logrobjc.warning(f"[{name}] No real changes detected - Skipping publishing on Fedora Messaging bus")  # noqa : E501
         return
 
     # Just publish the suffix of the URL.  The prefix is dl.fedoraproject.org
     # for lots of these, but we don't want to encourage people to download from
     # there.  It is the master mirror.  We want people to use
     # download.fedoraproject.org.. so, just obscure *exactly* which repo we're
     # talking about.
 
     urlx = "/".join(repmdurl.split("/")[4:])
-    servlogr.logrobjc.info("[%s] URL %s" % (name, urlx))
+    servlogr.logrobjc.info(f"[{name}] URL {urlx}")
 
     mesgobjc = RepoUpdateV1(
         body=dict(
             name=name,
             packages=list(packages),
             url=urlx,
         )
     )
 
     try:
         publish(mesgobjc)
     except PublishReturned as excp:
-        servlogr.logrobjc.error(
-            "Fedora Messaging broker rejected message %s - %s" % (mesgobjc.id, excp)
-        )
+        servlogr.logrobjc.error(f"Fedora Messaging broker rejected message {mesgobjc.id} - {excp}")
     except ConnectionException as excp:
-        servlogr.logrobjc.error(
-            "Error occurred while sending message %s - %s" % (mesgobjc.id, excp)
-        )
+        servlogr.logrobjc.error(f"Error occurred while sending message {mesgobjc.id} - {excp}")
 
 
 def install_database(name, srce, dest):
-    servlogr.logrobjc.info("[%s] Installing %s to %s" % (name, srce, dest))
+    servlogr.logrobjc.info(f"[{name}] Installing {srce} to {dest}")
     shutil.move(srce, dest)
 
 
 def needs_update(loclfile, srcehash, hashtype):
     """
     Compare SHA of the local and remote file
     Return True if our local file needs to be updated
@@ -151,27 +143,27 @@
 
 
 def process_repo(repo):
     """
     Retrieve the repo metadata at the given URL and store them using the provided name.
     """
     urlx, name = repo
-    repmdurl = "%s/repomd.xml" % urlx
-    response = requests.get(repmdurl, verify=standard.DL_VERIFY)
+    repmdurl = f"{urlx}/repomd.xml"
+    response = requests.get(repmdurl, verify=standard.DL_VERIFY)  # noqa : S113
     if not response:
-        servlogr.logrobjc.error("[%s] Failed to obtain %s - %s" % (name, repmdurl, response))
+        servlogr.logrobjc.error(f"[{name}] Failed to obtain {repmdurl} - {response}")
         return
 
     # Parse the XML document and get a list of locations and their SHAsum
     filelist = (
         (
             node.find("repo:location", standard.repomd_xml_namespace),
             node.find("repo:open-checksum", standard.repomd_xml_namespace),
         )
-        for node in ElementTree.fromstring(response.text)
+        for node in ElementTree.fromstring(response.text)  # noqa : S314
     )
 
     # Extract out the attributes that we are really interested in
     filelist = (
         (fobj.attrib["href"].replace("repodata/", ""), sobj.text, sobj.attrib["type"])
         for fobj, sobj in filelist
         if fobj is not None and sobj is not None
@@ -185,33 +177,33 @@
     filelist = sorted(filelist, key=prmyfrst)
 
     # Primary key caches built from the primary databases, so we can make sense
     # of the contents of the filelist and changelog databases.
     cacA, cacB = {}, {}
 
     if not filelist:
-        servlogr.logrobjc.warning("No SQLite database could be found in %s" % (urlx))
+        servlogr.logrobjc.warning(f"No SQLite database could be found in {urlx}")
 
     for filename, hashdata, hashtype in filelist:
-        repmdurl = "%s/%s" % (urlx, filename)
+        repmdurl = f"{urlx}/{filename}"
 
         # First, determine if the file has changed by comparing hash
         database = None
         if "primary.sqlite" in filename:
-            database = "mdapi-%s-primary.sqlite" % name
+            database = f"mdapi-{name}-primary.sqlite"
         elif "filelists.sqlite" in filename:
-            database = "mdapi-%s-filelists.sqlite" % name
+            database = f"mdapi-{name}-filelists.sqlite"
         elif "other.sqlite" in filename:
-            database = "mdapi-%s-other.sqlite" % name
+            database = f"mdapi-{name}-other.sqlite"
 
         # Have we downloaded this before?
         # Did it change?
         destfile = os.path.join(standard.DB_FOLDER, database)
         if not needs_update(destfile, hashdata, hashtype):
-            servlogr.logrobjc.info("[%s] No change detected from %s" % (name, repmdurl))
+            servlogr.logrobjc.info(f"[{name}] No change detected from {repmdurl}")
             continue
 
         # Creating temporary directories with formatted names to remove them later easily, if needed
         tempargs = dict(prefix="mdapi-tempdrct-", dir=standard.DB_FOLDER)
 
         # If it has changed, then download it and move it into place
         with tempfile.TemporaryDirectory(**tempargs) as workdrct:
@@ -220,82 +212,78 @@
             fetch_database(name, repmdurl, archname)
             extract_database(name, archname, tempdtbs)
             index_database(name, tempdtbs)
             if standard.PUBLISH_CHANGES:
                 packages = compare_databases(name, tempdtbs, destfile, cacA, cacB).main()
                 publish_changes(name, packages, repmdurl)
             else:
-                servlogr.logrobjc.warning(
-                    "[%s] Not publishing to Fedora Messaging bus - Not comparing databases" % (name)
-                )
+                servlogr.logrobjc.warning(f"[{name}] Not publishing to Fedora Messaging bus - Not comparing databases")  # noqa : E501
             install_database(name, tempdtbs, destfile)
 
 
 def index_repositories():
     repolist = []
 
     # Obtain the development repos (rawhide + eventually Fn+1 branched)
     dev_releases = list_branches(status="Under Development")
     for rels in dev_releases:
         if rels["status"] != "Under Development":
             continue
         versdata = rels["version"]
         if versdata == "devel":
             versdata = "rawhide"
-        urlx = "%s/pub/fedora/linux/development/%s/Everything/x86_64/os/repodata" % (
-            standard.DL_SERVER,
-            versdata,
-        )
-        servlogr.logrobjc.info(
-            "Acquired repo for %s/%s of '%s' branch at %s"
-            % (rels["koji_name"], versdata, rels["status"], urlx)
-        )
+        urlx = f"{standard.DL_SERVER}/pub/fedora/linux/development/{versdata}/Everything/x86_64/os/repodata"  # noqa : E501
+        servlogr.logrobjc.info(f"Acquired repo for {rels['koji_name']}/{versdata} of '{rels['status']}' branch at {urlx}")  # noqa : E501
         repolist.append((urlx, rels["koji_name"]))
         urlx = urlx.replace("/x86_64/os/", "/source/tree/")
-        repolist.append((urlx, "src_%s" % rels["koji_name"]))
+        repolist.append((urlx, f"src_{rels['koji_name']}"))
 
     urls = {
         "Fedora Linux": [
-            "%s/pub/fedora/linux/releases/%s/Everything/x86_64/os/repodata",
-            "%s/pub/fedora/linux/updates/%s/Everything/x86_64/repodata",
-            "%s/pub/fedora/linux/updates/testing/%s/Everything/x86_64/repodata",
+            "{dlserver}/pub/fedora/linux/releases/{versname}/Everything/x86_64/os/repodata",
+            "{dlserver}/pub/fedora/linux/updates/{versname}/Everything/x86_64/repodata",
+            "{dlserver}/pub/fedora/linux/updates/testing/{versname}/Everything/x86_64/repodata",
         ],
         "Fedora EPEL": [
-            "%s/pub/epel/%s/x86_64/repodata/",
-            "%s/pub/epel/testing/%s/x86_64/repodata",
+            "{dlserver}/pub/epel/{versname}/x86_64/repodata/",
+            "{dlserver}/pub/epel/testing/{versname}/x86_64/repodata",
         ],
     }
 
     urls["Fedora"] = urls["Fedora Linux"]
-    repodict = {"fedora": ["%s", "%s-updates", "%s-updates-testing"], "epel": ["%s", "%s-testing"]}
+
+    repodict = {
+        "fedora": ["{rlid}", "{rlid}-updates", "{rlid}-updates-testing"],
+        "epel": ["{rlid}", "{rlid}-testing"]
+    }
 
     # Obtain the stable repos
     stable_releases = list_branches(status="Active")
     for rels in stable_releases:
         if rels["status"] != "Active":
             continue
         versdata = rels["version"]
         for jndx, urli in enumerate(urls[rels["name"]]):
             if rels["name"] in ("Fedora Linux", "Fedora"):
-                name = repodict["fedora"][jndx] % rels["koji_name"]
+                name = repodict["fedora"][jndx].format(ridx = rels["koji_name"])
             elif rels["name"] == "Fedora EPEL" and versdata == "8":
-                name = repodict["epel"][jndx] % rels["koji_name"]
+                name = repodict["epel"][jndx].format(rlid = rels["koji_name"])
                 urli = urli.replace("/x86_64/", "/Everything/x86_64/")
             elif rels["name"] == "Fedora EPEL" and versdata == "9":
-                name = repodict["epel"][jndx] % rels["koji_name"]
+                name = repodict["epel"][jndx].format(rlid = rels["koji_name"])
                 urli = urli.replace("/x86_64/", "/Everything/x86_64/")
             else:
-                name = repodict["epel"][jndx] % rels["koji_name"]
-            rurl = urli % (standard.DL_SERVER, versdata)
+                name = repodict["epel"][jndx].format(rlid = rels["koji_name"])
+            rurl = urli.format(dlserver = standard.DL_SERVER, versname = versdata)
             repolist.append((rurl, name))
             rurl = rurl.replace("/x86_64/os", "/source/tree")
-            repolist.append((rurl, "src_%s" % name))
+            repolist.append((rurl, f"src_{name}"))
 
     # Finish with the koji repo
-    repolist.append(("%s/rawhide/latest/x86_64/repodata" % standard.KOJI_REPO, "koji"))
+    repolist.append((f"{standard.KOJI_REPO}/rawhide/latest/x86_64/repodata", "koji"))
 
     # In serial
     for repo in repolist:
         loop = True
         qant = 0
         while loop:
             qant += 1
```

### Comparing `mdapi-3.1.4/mdapi/database/sqlq.py` & `mdapi-3.1.5/mdapi/database/sqlq.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/mdapi/main.py` & `mdapi-3.1.5/mdapi/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 def main(conffile=None):
     """
     A simple API for serving the metadata from the RPM repositories
     """
     if conffile is not None:
         # Load the configuration file to use
         CONFIG = {}
-        with open(conffile, "r") as confobjc:
-            exec(compile(confobjc.read(), conffile, "exec"), CONFIG)
+        with open(conffile) as confobjc:
+            exec(compile(confobjc.read(), conffile, "exec"), CONFIG)  # noqa : S102
         compile_configuration(CONFIG)
 
 
 @main.command(
     name="database", help="Fetch SQLite databases from all active Fedora Linux and EPEL branches"
 )
 def database():
@@ -66,15 +66,15 @@
             "gunicorn mdapi.services.main:buildapp --bind %s --worker-class %s --log-level %s"  # noqa
             % (
                 APPSERVE["bind"],
                 APPSERVE["worker_class"],
                 APPSERVE["logging"]["level"],
             )
         )
-        subprocess.run(startcmd.split())
+        subprocess.run(startcmd.split())  # noqa : S603
     except KeyError:
         print("Invalid configuration detected")
         return 1
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mdapi-3.1.4/mdapi/services/__init__.py` & `mdapi-3.1.5/mdapi/services/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,17 +49,17 @@
         raise HTTPBadRequest()
 
     pckg = None
     wrongdbs = False
 
     for repotype in ["updates-testing", "updates", "testing", None]:
         if repotype:
-            dtbsfile = "%s/mdapi-%s-%s-primary.sqlite" % (standard.DB_FOLDER, brch, repotype)
+            dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-{repotype}-primary.sqlite"
         else:
-            dtbsfile = "%s/mdapi-%s-primary.sqlite" % (standard.DB_FOLDER, brch)
+            dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-primary.sqlite"
 
         if not os.path.exists(dtbsfile):
             wrongdbs = True
             continue
 
         wrongdbs = False
         async with aiosqlite.connect(dtbsfile) as dtbsobjc:
@@ -70,28 +70,28 @@
                 sqlquery = GET_PACKAGE_BY.format(actn)
                 async with dtbsobjc.execute(sqlquery, (name,)) as dbcursor:
                     pkgc = await dbcursor.fetchall()
                 if pkgc:
                     pckg = [Packages(*item) for item in pkgc]
                     break
             elif srcn:
-                async with dtbsobjc.execute(GET_PACKAGE_BY_SRC, ("%s-%%" % srcn,)) as dbcursor:
+                async with dtbsobjc.execute(GET_PACKAGE_BY_SRC, (f"{srcn}-%",)) as dbcursor:
                     pkgc = await dbcursor.fetchall()
                 if pkgc:
                     for pkgx in pkgc:
                         # Try to match the package with the source name at first
                         if pkgx[2] == srcn:
                             pckg = Packages(*pkgx)
                             break
 
                     if pckg:
                         break
 
                     srcn = re.escape(srcn)
-                    ptrn = re.compile("%s-[0-9]" % srcn)
+                    ptrn = re.compile(f"{srcn}-[0-9]")
                     for pkgx in pkgc:
                         if ptrn.match(pkgx[3]):
                             pckg = Packages(*pkgx)
                             break
             else:
                 async with dtbsobjc.execute(GET_PACKAGE, (name,)) as dbcursor:
                     pkgc = await dbcursor.fetchone()
@@ -120,17 +120,17 @@
         pkgs = [pkgs]
 
     rslt = []
 
     for pkgx in pkgs:
         otpt = pkgx.to_json()
         if repotype:
-            dtbsfile = "%s/mdapi-%s-%s-primary.sqlite" % (standard.DB_FOLDER, brch, repotype)
+            dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-{repotype}-primary.sqlite"
         else:
-            dtbsfile = "%s/mdapi-%s-primary.sqlite" % (standard.DB_FOLDER, brch)
+            dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-primary.sqlite"
 
         async with aiosqlite.connect(dtbsfile) as dtbsobjc:
             """
             Fill in some extra info
             Basic information is always present regardless of the version of the repository
             """
             for datatype in [
@@ -173,17 +173,17 @@
 
 
 async def _get_files(pkid, brch, repotype):
     """
     Return the list of files for the given package in the specified branch.
     """
     if repotype:
-        dtbsfile = "%s/mdapi-%s-%s-filelists.sqlite" % (standard.DB_FOLDER, brch, repotype)
+        dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-{repotype}-filelists.sqlite"
     else:
-        dtbsfile = "%s/mdapi-%s-filelists.sqlite" % (standard.DB_FOLDER, brch)
+        dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-filelists.sqlite"
 
     if not os.path.exists(dtbsfile):
         raise HTTPBadRequest()
 
     async with aiosqlite.connect(dtbsfile) as dtbsobjc:
         async with dtbsobjc.execute(GET_FILES, (pkid,)) as dbcursor:
             filelist = await dbcursor.fetchall()
@@ -199,17 +199,17 @@
 
 
 async def _get_changelog(pkid, brch, repotype):
     """
     Return the changelog for the given packages in the specified branch.
     """
     if repotype:
-        dtbsfile = "%s/mdapi-%s-%s-other.sqlite" % (standard.DB_FOLDER, brch, repotype)
+        dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-{repotype}-other.sqlite"
     else:
-        dtbsfile = "%s/mdapi-%s-other.sqlite" % (standard.DB_FOLDER, brch)
+        dtbsfile = f"{standard.DB_FOLDER}/mdapi-{brch}-other.sqlite"
 
     if not os.path.exists(dtbsfile):
         raise HTTPBadRequest()
 
     async with aiosqlite.connect(dtbsfile) as dtbsfile:
         async with dtbsfile.execute(GET_CHANGELOGS, (pkid,)) as dbcursor:
             changeloglist = await dbcursor.fetchall()
```

### Comparing `mdapi-3.1.4/mdapi/services/apimodel.py` & `mdapi-3.1.5/mdapi/services/apimodel.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/mdapi/services/appviews.py` & `mdapi-3.1.5/mdapi/services/appviews.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,41 +28,41 @@
 from mdapi.confdata import servlogr, standard
 from mdapi.services import _expand_package_info, _get_changelog, _get_files, _get_package
 
 homepage = os.path.join(os.path.dirname(os.path.abspath(__file__)), "homepage.html")
 
 
 async def index(rqst):
-    servlogr.logrobjc.info("index %s" % rqst)
+    servlogr.logrobjc.info(f"index {rqst}")
     return FileResponse(homepage)
 
 
 async def get_pkg(rqst):
-    servlogr.logrobjc.info("get_pkg %s" % rqst)
+    servlogr.logrobjc.info(f"get_pkg {rqst}")
     brch = rqst.match_info.get("brch")
     name = rqst.match_info.get("name")
     pckg, repotype = await _get_package(brch, name)
     rslt = await _expand_package_info(pckg, brch, repotype)
     return json_response(rslt)
 
 
 async def get_src_pkg(rqst):
-    servlogr.logrobjc.info("get_src_pkg %s" % rqst)
+    servlogr.logrobjc.info(f"get_src_pkg {rqst}")
     brch = rqst.match_info.get("brch")
     name = rqst.match_info.get("name")
     pckg, repotype = await _get_package(brch, srcn=name)
     rslt = await _expand_package_info(pckg, brch, repotype)
     return json_response(rslt)
 
 
 async def list_branches(rqst):
     """
     Return the list of all branches currently supported by mdapi
     """
-    servlogr.logrobjc.info("list_branches %s" % rqst)
+    servlogr.logrobjc.info(f"list_branches {rqst}")
     rslt = sorted(
         {
             # Remove the front part `mdapi-` and the end part `-<type>.sqlite` from the filenames
             filename.replace("mdapi-", "").rsplit("-", 2)[0].replace("-updates", "")
             for filename in os.listdir(standard.DB_FOLDER)
             if filename.startswith("mdapi") and filename.endswith(".sqlite")
         }
@@ -71,22 +71,22 @@
 
 
 async def _process_dep(rqst, actn):
     """
     Return the information about the packages having the specified action
     (as in provides, requires, obsoletes etc.)
     """
-    servlogr.logrobjc.info("process_dep %s %s" % (actn, rqst))
+    servlogr.logrobjc.info(f"process_dep {actn} {rqst}")
     brch = rqst.match_info.get("brch")
     name = rqst.match_info.get("name")
 
     try:
         pckg, repotype = await _get_package(brch, name, actn=actn)
     except:  # noqa
-        raise HTTPBadRequest
+        raise HTTPBadRequest  # noqa : B904
 
     rslt = await _expand_package_info(pckg, brch, repotype)
     return json_response(rslt)
 
 
 async def get_provides(rqst):
     return await _process_dep(rqst, "provides")
@@ -117,22 +117,22 @@
 
 
 async def get_supplements(rqst):
     return await _process_dep(rqst, "supplements")
 
 
 async def get_pkg_files(rqst):
-    servlogr.logrobjc.info("get_pkg_files %s" % rqst)
+    servlogr.logrobjc.info(f"get_pkg_files {rqst}")
     brch = rqst.match_info.get("brch")
     name = rqst.match_info.get("name")
     pckg, repotype = await _get_package(brch, name)
     rslt = await _get_files(pckg.pkgId, brch, repotype)
     return json_response(rslt)
 
 
 async def get_pkg_changelog(rqst):
-    servlogr.logrobjc.info("get_pkg_changelog %s" % rqst)
+    servlogr.logrobjc.info(f"get_pkg_changelog {rqst}")
     brch = rqst.match_info.get("brch")
     name = rqst.match_info.get("name")
     pckg, repotype = await _get_package(brch, name)
     rslt = await _get_changelog(pckg.pkgId, brch, repotype)
     return json_response(rslt)
```

### Comparing `mdapi-3.1.4/mdapi/services/homepage.html` & `mdapi-3.1.5/mdapi/services/homepage.html`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 | '_ ` _ \ / _` |/ _` | '_ \| |
 | | | | | | (_| | (_| | |_) | |
 |_| |_| |_|\__,_|\__,_| .__/|_|
                       | |
                       |_|
 
 
-mdapi is a small API exposing the metadata contained in different RPM
+<a href="https://pypi.org/project/mdapi/3.1.5/">mdapi</a> is a small API exposing the metadata contained in different RPM
 repositories.
 
 mdapi has access to the metadata of the different Fedora repositories and will
 serve you the most recent information available, from updates-testing, if
 there is nothing in updates-testing, it will look for information from the
 updates repository and if there is still nothing, it will look for information
 in the releases repository.
@@ -177,8 +177,8 @@
                                             | | (‾| | |‾) | |‾) | | | | | |
                                             | |\ ‾, | ,‾ /| ,‾ / \ ‾ , ‾, |
                                              ‾  ‾‾ ‾ ‾ ‾‾ | |‾‾   ‾‾‾ ‾‾ ‾
                                             (‾)           | |
                                              ‾             ‾
 © 2015-2022 - Red Hat, Inc. - GPLv3+ - Sources: <a href="https://github.com/fedora-infra/mdapi/">https://github.com/fedora-infra/mdapi/</a>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _ _ | | (_) _ __ ___ __| | __ _ _ __ _ | '_ ` _ \ / _` |/ _` | '_ \| | | | | |
-| | (_| | (_| | |_) | | |_| |_| |_|\__,_|\__,_| .__/|_| | | |_| mdapi is a
+| | (_| | (_| | |_) | | |_| |_| |_|\__,_|\__,_| .__/|_| | | |_| _m_d_a_p_i is a
 small API exposing the metadata contained in different RPM repositories. mdapi
 has access to the metadata of the different Fedora repositories and will serve
 you the most recent information available, from updates-testing, if there is
 nothing in updates-testing, it will look for information from the updates
 repository and if there is still nothing, it will look for information in the
 releases repository. If you query for a non-existing branch (for example: f14),
 it will return a 400 error. If you query for a non-existing package (for
```

### Comparing `mdapi-3.1.4/mdapi/services/main.py` & `mdapi-3.1.5/mdapi/services/main.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.4/pyproject.toml` & `mdapi-3.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdapi"
-version = "3.1.4"
+version = "3.1.5"
 description = "A simple API for serving the metadata from the RPM repositories"
 authors = ["Pierre-Yves Chibon <pingou@pingoured.fr>", "Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Pierre-Yves Chibon <pingou@pingoured.fr>", "Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fedora-infra/mdapi"
 repository = "https://github.com/fedora-infra/mdapi"
@@ -30,49 +30,41 @@
 	"Topic :: Software Development",
 	"Topic :: System :: Archiving :: Packaging",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.1"
-aiosqlite = "^0.18.0 || ^0.19.0"
+aiosqlite = "^0.18.0 || ^0.19.0 || ^0.20.0"
 fedora-messaging = "^3.0.2"
 requests = "^2.28.1"
 uvloop = "^0.17.0 || ^0.18.0 || ^0.19.0"
-gunicorn = "^20.1.0"
+gunicorn = "^20.1.0 || ^21.0.0"
 mdapi-messages = "^1.0.0"
 click = "^8.1.3"
 pyzstd = "^0.15.0"
 setuptools = "*"
 
 [tool.poetry.dev-dependencies]
-black = "^23.0.0"
-isort = "^5.10.1"
-pytest = "^7.1.3"
-flake8 = "<6.1.1"
-pytest-black = "^0.3.12"
-pytest-flake8 = "^1.0.7"
-pytest-isort = "^3.0.0"
-beautifulsoup4 = "^4.11.1"
 tox = "^4.0.0"
+pytest = "^7.1.3 || ^8.0.0"
+pytest-cov = "^4.1.0 || ^5.0.0"
+ruff = "^0.2.0 || ^0.3.0"
+beautifulsoup4 = "^4.11.1"
 pytest-aiohttp = "^1.0.4"
-pytest-cov = "^4.0.0"
-bandit = "^1.7.4"
 
-[tool.pytest.ini_options]
-addopts = "--black --isort --flake8 --cov=mdapi --cov-report=term --cov-report=xml --cov-report=html"
-flake8-max-line-length = 100
-asyncio_mode = "auto"
+[tool.ruff]
+line-length = 100
 
-[tool.isort]
-line_length = 100
-profile = "black"
+[tool.ruff.lint]
+select = ["E", "F", "W", "I", "S", "B", "UP"]
 
-[tool.black]
-line-length = 100
+[tool.pytest.ini_options]
+markers = ["download_required", "download_needless"]
+asyncio_mode = "auto"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 mdapi = "mdapi.main:main"
```

### Comparing `mdapi-3.1.4/PKG-INFO` & `mdapi-3.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdapi
-Version: 3.1.4
+Version: 3.1.5
 Summary: A simple API for serving the metadata from the RPM repositories
 Home-page: https://github.com/fedora-infra/mdapi
 License: GPL-3.0-or-later
 Keywords: rpm,centos,fedora,metadata,repositories
 Author: Pierre-Yves Chibon
 Author-email: pingou@pingoured.fr
 Maintainer: Pierre-Yves Chibon
@@ -19,24 +19,25 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Operating System
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: aiosqlite (>=0.18.0,<0.20.0)
+Requires-Dist: aiosqlite (>=0.18.0,<0.21.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fedora-messaging (>=3.0.2,<4.0.0)
-Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: gunicorn (>=20.1.0,<22.0.0)
 Requires-Dist: mdapi-messages (>=1.0.0,<2.0.0)
 Requires-Dist: pyzstd (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: setuptools
 Requires-Dist: uvloop (>=0.17.0,<0.20.0)
 Project-URL: Documentation, https://github.com/fedora-infra/mdapi/blob/develop/README.md
 Project-URL: Repository, https://github.com/fedora-infra/mdapi
```

