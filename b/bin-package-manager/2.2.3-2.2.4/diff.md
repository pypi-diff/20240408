# Comparing `tmp/bin_package_manager-2.2.3.tar.gz` & `tmp/bin_package_manager-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bin_package_manager-2.2.3.tar", max compression
+gzip compressed data, was "bin_package_manager-2.2.4.tar", max compression
```

## Comparing `bin_package_manager-2.2.3.tar` & `bin_package_manager-2.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      192 2024-03-27 13:22:23.708873 bin_package_manager-2.2.3/bpm/__init__.py
--rw-r--r--   0        0        0       65 2024-02-15 09:27:57.497385 bin_package_manager-2.2.3/bpm/__main__.py
--rw-r--r--   0        0        0     4006 2024-03-03 15:57:06.428638 bin_package_manager-2.2.3/bpm/cli.py
--rw-r--r--   0        0        0     6219 2024-03-07 05:49:02.057295 bin_package_manager-2.2.3/bpm/command.py
--rw-r--r--   0        0        0    18204 2024-03-27 13:24:48.372447 bin_package_manager-2.2.3/bpm/install/__init__.py
--rw-r--r--   0        0        0     4103 2024-02-19 09:51:08.195821 bin_package_manager-2.2.3/bpm/lib/windowspathadder.py
--rw-r--r--   0        0        0    11070 2024-03-27 13:22:23.709874 bin_package_manager-2.2.3/bpm/search.py
--rw-r--r--   0        0        0     4545 2024-03-04 13:37:18.442871 bin_package_manager-2.2.3/bpm/storage.py
--rw-r--r--   0        0        0     4053 2024-03-27 13:22:23.709874 bin_package_manager-2.2.3/bpm/utils/__init__.py
--rw-r--r--   0        0        0      568 2024-02-20 06:49:42.600431 bin_package_manager-2.2.3/bpm/utils/constants.py
--rw-r--r--   0        0        0     1025 2024-02-20 12:24:21.046111 bin_package_manager-2.2.3/bpm/utils/exceptions.py
--rw-r--r--   0        0        0     1087 2024-02-04 04:59:52.630709 bin_package_manager-2.2.3/LICENSE
--rw-r--r--   0        0        0     1062 2024-03-27 13:25:56.535852 bin_package_manager-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     2757 2024-03-03 15:58:29.375065 bin_package_manager-2.2.3/README.md
--rw-r--r--   0        0        0     3614 1970-01-01 00:00:00.000000 bin_package_manager-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-03 15:14:27.236806 bin_package_manager-2.2.4/LICENSE
+-rw-r--r--   0        0        0     3822 2024-04-08 16:38:00.593122 bin_package_manager-2.2.4/README.md
+-rw-r--r--   0        0        0      184 2024-03-25 08:16:31.955639 bin_package_manager-2.2.4/bpm/__init__.py
+-rw-r--r--   0        0        0       61 2024-02-14 06:21:44.497403 bin_package_manager-2.2.4/bpm/__main__.py
+-rw-r--r--   0        0        0     4031 2024-04-08 16:23:47.314764 bin_package_manager-2.2.4/bpm/cli.py
+-rw-r--r--   0        0        0     6855 2024-04-08 16:26:54.032376 bin_package_manager-2.2.4/bpm/command.py
+-rw-r--r--   0        0        0    17653 2024-04-08 17:12:36.984564 bin_package_manager-2.2.4/bpm/install/__init__.py
+-rw-r--r--   0        0        0     4103 2024-02-19 11:56:44.850635 bin_package_manager-2.2.4/bpm/lib/windowspathadder.py
+-rw-r--r--   0        0        0    11303 2024-04-08 17:12:41.197879 bin_package_manager-2.2.4/bpm/search.py
+-rw-r--r--   0        0        0     4410 2024-03-06 14:53:06.937647 bin_package_manager-2.2.4/bpm/storage.py
+-rw-r--r--   0        0        0     3882 2024-03-25 08:19:26.282328 bin_package_manager-2.2.4/bpm/utils/__init__.py
+-rw-r--r--   0        0        0      545 2024-04-08 17:12:31.247925 bin_package_manager-2.2.4/bpm/utils/constants.py
+-rw-r--r--   0        0        0      988 2024-02-21 10:21:37.512797 bin_package_manager-2.2.4/bpm/utils/exceptions.py
+-rw-r--r--   0        0        0     1026 2024-04-08 17:12:45.534529 bin_package_manager-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 bin_package_manager-2.2.4/PKG-INFO
```

### Comparing `bin_package_manager-2.2.3/bpm/command.py` & `bin_package_manager-2.2.4/bpm/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,208 @@
-import logging as log
-from pathlib import Path
-from tempfile import TemporaryDirectory
-
-from simpleufcs import UFCS
-
-from .install import auto_install, download_and_extract, extract, remove
-from .search import RepoHandler
-from .storage import repo_group
-from .utils import check_root, error_exit, set_dry_run, trace
-from .utils.constants import BIN_PATH, WINDOWS
-from .utils.exceptions import RepoNotFoundError
-
-
-def cli_install(args):
-    if args.interactive and args.quiet:
-        log.error("Cannot use both --interactive and --quiet.")
-        exit(1)
-    if args.dry_run:
-        set_dry_run()
-    else:
-        check_root()
-    if args.local and len(args.packages) > 1:
-        log.error(
-            "Cannot install multiple packages from local. Please install them separately."
-        )
-        exit(1)
-    for package in args.packages:
-        if not args.dry_run and repo_group.find_repo(package)[1]:
-            log.info(f"{package} is already installed.")
-            continue
-        try:
-            repo = RepoHandler(
-                package,
-                prefer_gnu=args.prefer_gnu,
-                one_bin=args.one_bin,
-            ).with_bin_name(args.bin_name)
-            if not args.local:
-                repo = repo.ask(quiet=args.quiet, sort=args.sort).get_asset(
-                    interactive=args.interactive
-                )
-
-        except Exception as e:
-            log.error(f"Failed on searching `{package}`: {e}")
-            trace()
-            exit(1)
-        with TemporaryDirectory() as tmp_dir:
-            tmp_dir = Path(tmp_dir)
-            try:
-                if args.local:
-                    with Path(args.local).open("rb") as f:
-                        main_path = extract(f, tmp_dir)
-                else:
-                    main_path = download_and_extract(repo.asset, tmp_dir)
-                auto_install(repo, main_path, rename=True)
-                log.info(f"Successfully installed `{repo.name}`.")
-                if WINDOWS:
-                    bins = (
-                        UFCS(repo.file_list)
-                        .filter(lambda x: x.endswith(".lnk"))
-                        .map(lambda x: Path(x).stem)
-                        .map(lambda x: f"`{x}`")
-                    )
-                    log.info(
-                        f"You can press `Win+r`, enter {', '.join(bins)} to start software, or execute in cmd."
-                    )
-                if not args.dry_run:
-                    repo_group.insert_repo(repo)
-
-            except Exception as e:
-                log.error(f"Failed to install `{repo.name}`: {e}")
-                trace()
-                log.error("Restoring...")
-                # rollback.
-                remove(repo.file_list)
-                error_exit("Files restored. Exiting...")
-
-
-def cli_remove(args):
-    check_root()
-    failed = []
-    for package in args.packages:
-        repo = repo_group.find_repo(package)[1]
-        if not repo:
-            log.info(f"Package `{package}` is not installed.")
-            failed.append(package)
-            continue
-        try:
-            log.info(
-                f"""Removing `{package}`{" in soft mode" if args.soft else ""}..."""
-            )
-            args.soft or remove(repo.file_list)
-            repo_group.remove_repo(package)
-        except Exception as e:
-            failed.append(package)
-            log.error(f"Failed to remove `{package}`: {e}")
-            trace()
-            continue
-        log.info(f"`{package}` removed successfully.")
-    log.info(
-        f"Removing complete. Total: {len(args.packages)}, Success: {len(args.packages)-len(failed)}"
-    )
-    if failed:
-        log.info(f"Failed list: {failed}")
-
-
-def cli_update(args):
-    check_root()
-    failed = []
-
-    def update(repo: RepoHandler):
-        try:
-            log.info(f"Updating `{repo.name}`...")
-            if result := repo.update_asset():
-                log.info(
-                    f"`{repo.name}` has an update: {result[0]} -> {result[1]}. Updating..."
-                )
-                with TemporaryDirectory() as tmp_dir:
-                    tmp_dir = Path(tmp_dir)
-                    main_path = download_and_extract(repo.asset, tmp_dir)
-                    auto_install(repo, main_path, rename=False)
-                log.info(f"`{repo.name}` updated successfully.")
-            else:
-                log.info(f"`{repo.name}` is the newest.")
-        except Exception as e:
-            failed.append(repo.name)
-            log.error(f"Failed to update {repo.name}: {e}")
-            trace()
-
-    if not args.packages:  # update all
-        num = len(repo_group.repos)
-        for repo in repo_group.repos:
-            update(repo)
-    else:  # update some
-        num = len(args.packages)
-        for name in args.packages:
-            _, repo = repo_group.find_repo(name)
-            if repo:
-                update(repo)
-                repo_group.save()
-            else:
-                failed.append(name)
-                log.error(f"Package `{name}` not found.")
-
-    log.info(f"Update complete. Total: {num}, Success: {num-len(failed)}")
-    if failed:
-        log.info(f"Failed: {failed}")
-
-
-def cli_info(args):
-    try:
-        if not args.package:
-            repo_group.info_repos()
-        else:
-            repo_group.info_one_repo(str(args.package))
-    except RepoNotFoundError as e:
-        log.error(e)
-        exit(1)
-
-
-def cli_alias(args):
-    assert WINDOWS, "Alias command is only supported on Windows."
-    assert (
-        args.old_name != args.new_name
-    ), "Alias name cannot be the same as the original."
-
-    file = list(BIN_PATH.glob(args.old_name + "*"))
-    if not file:
-        log.error(f"Script `{args.old_name}` not found.")
-        exit(1)
-    if len(file) > 1:
-        name = file[0].with_suffix("")
-        assert name == file[1].with_suffix(
-            ""
-        ), "Both lnk should point to the same file."
-
-    repo_group.alias_lnk(args.old_name, args.new_name)
-    log.info(f"Alias `{args.old_name}` to `{args.new_name}`.")
+import logging as log
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from urllib.parse import urlparse
+
+from simpleufcs import UFCS
+
+from .install import auto_install, download_and_extract, extract, remove
+from .search import RepoHandler
+from .storage import repo_group
+from .utils import check_root, error_exit, set_dry_run, trace
+from .utils.constants import BIN_PATH, WINDOWS
+from .utils.exceptions import RepoNotFoundError
+
+
+def parse_name_or_url(name_or_url: str) -> tuple[str, bool]:
+    """
+    Parse the name or url of a package.
+    `Returns`: a tuple with two elements: first is the true name, second is the flag of whether it is a url.
+    """
+    test_parse = urlparse(name_or_url)
+    if test_parse.netloc == "github.com":
+        return RepoHandler.get_info_by_url(name_or_url)[1], True
+    return name_or_url, False
+
+
+def download_and_install(args, repo: RepoHandler, rename=True):
+    try:
+        with TemporaryDirectory() as tmp_dir:
+            tmp_dir = Path(tmp_dir)
+            if args.local:
+                with Path(args.local).open("rb") as f:
+                    main_path = extract(f, tmp_dir)
+            else:
+                main_path = download_and_extract(repo.asset, tmp_dir)
+            auto_install(repo, main_path, rename=rename)
+    except Exception as e:
+        raise e
+
+
+def cli_install(args):
+    if args.interactive and args.quiet:
+        log.error("Cannot use both --interactive and --quiet.")
+        exit(1)
+    if args.dry_run:
+        set_dry_run()
+    else:
+        check_root()
+    if args.local and len(args.packages) > 1:
+        log.error(
+            "Cannot install multiple packages from local. Please install them separately."
+        )
+        exit(1)
+    for package in args.packages:
+        real_name, is_url = parse_name_or_url(package)
+        if not args.dry_run and repo_group.find_repo(real_name)[1]:
+            log.info(f"{real_name} is already installed.")
+            continue
+
+        # search
+        try:
+            if is_url:
+                repo = (
+                    RepoHandler(
+                        real_name,
+                        prefer_gnu=args.prefer_gnu,
+                        one_bin=args.one_bin,
+                    )
+                    .set_by_url(package)
+                    .with_bin_name(args.bin_name)
+                )
+            else:
+                repo = RepoHandler(
+                    package,
+                    prefer_gnu=args.prefer_gnu,
+                    one_bin=args.one_bin,
+                ).with_bin_name(args.bin_name)
+                if not args.local:
+                    repo.ask(quiet=args.quiet, sort=args.sort)
+            if not args.local:
+                repo.get_asset(interactive=args.interactive)
+        except Exception as e:
+            log.error(f"Failed on searching `{package}`: {e}")
+            trace()
+            exit(1)
+
+        # install
+        try:
+            download_and_install(args, repo)
+            log.info(f"Successfully installed `{repo.name}`.")
+            if WINDOWS:
+                bins = (
+                    UFCS(repo.file_list)
+                    .filter(lambda x: x.endswith(".lnk"))
+                    .map(lambda x: Path(x).stem)
+                    .map(lambda x: f"`{x}`")
+                )
+                log.info(
+                    f"You can press `Win+r`, enter {', '.join(bins)} to start software, or execute in cmd."
+                )
+            if not args.dry_run:
+                repo_group.insert_repo(repo)
+        except Exception as e:
+            log.error(f"Failed to install `{repo.name}`: {e}")
+            trace()
+            log.error("Restoring...")
+            # rollback.
+            remove(repo.file_list)
+            error_exit("Files restored. Exiting...")
+
+
+def cli_remove(args):
+    check_root()
+    failed = []
+    for package in args.packages:
+        repo = repo_group.find_repo(package)[1]
+        if not repo:
+            log.info(f"Package `{package}` is not installed.")
+            failed.append(package)
+            continue
+        try:
+            log.info(
+                f"""Removing `{package}`{" in soft mode" if args.soft else ""}..."""
+            )
+            args.soft or remove(repo.file_list)
+            repo_group.remove_repo(package)
+        except Exception as e:
+            failed.append(package)
+            log.error(f"Failed to remove `{package}`: {e}")
+            trace()
+            continue
+        log.info(f"`{package}` removed successfully.")
+    log.info(
+        f"Removing complete. Total: {len(args.packages)}, Success: {len(args.packages)-len(failed)}"
+    )
+    if failed:
+        log.info(f"Failed list: {failed}")
+
+
+def cli_update(args):
+    check_root()
+    failed = []
+
+    def update(repo: RepoHandler):
+        try:
+            log.info(f"Updating `{repo.name}`...")
+            if result := repo.update_asset():
+                log.info(
+                    f"`{repo.name}` has an update: {result[0]} -> {result[1]}. Updating..."
+                )
+                download_and_install(args, repo, rename=False)
+                log.info(f"`{repo.name}` updated successfully.")
+            else:
+                log.info(f"`{repo.name}` is the newest.")
+        except Exception as e:
+            failed.append(repo.name)
+            log.error(f"Failed to update {repo.name}: {e}")
+            trace()
+
+    if not args.packages:  # update all
+        num = len(repo_group.repos)
+        for repo in repo_group.repos:
+            update(repo)
+    else:  # update some
+        num = len(args.packages)
+        for name in args.packages:
+            _, repo = repo_group.find_repo(name)
+            if repo:
+                update(repo)
+                repo_group.save()
+            else:
+                failed.append(name)
+                log.error(f"Package `{name}` not found.")
+
+    log.info(f"Update complete. Total: {num}, Success: {num-len(failed)}")
+    if failed:
+        log.info(f"Failed: {failed}")
+
+
+def cli_info(args):
+    try:
+        if not args.package:
+            repo_group.info_repos()
+        else:
+            repo_group.info_one_repo(str(args.package))
+    except RepoNotFoundError as e:
+        log.error(e)
+        exit(1)
+
+
+def cli_alias(args):
+    assert WINDOWS, "Alias command is only supported on Windows."
+    assert (
+        args.old_name != args.new_name
+    ), "Alias name cannot be the same as the original."
+
+    file = list(BIN_PATH.glob(args.old_name + "*"))
+    if not file:
+        log.error(f"Script `{args.old_name}` not found.")
+        exit(1)
+    if len(file) > 1:
+        name = file[0].with_suffix("")
+        assert name == file[1].with_suffix(
+            ""
+        ), "Both lnk should point to the same file."
+
+    repo_group.alias_lnk(args.old_name, args.new_name)
+    log.info(f"Alias `{args.old_name}` to `{args.new_name}`.")
```

### Comparing `bin_package_manager-2.2.3/bpm/lib/windowspathadder.py` & `bin_package_manager-2.2.4/bpm/lib/windowspathadder.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.3/bpm/storage.py` & `bin_package_manager-2.2.4/bpm/storage.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import bisect
-import logging as log
-import pickle
-from contextlib import suppress
-from pathlib import Path
-from pprint import pprint
-from tempfile import TemporaryDirectory
-from typing import Optional
-
-from .search import RepoHandler
-from .utils.constants import DATABASE_PATH, INFO_BASE_STRING, WINDOWS
-from .utils.exceptions import RepoNotFoundError
-
-
-class RepoGroup:
-    def __init__(self, db_path=DATABASE_PATH):
-        self.repos: list[RepoHandler] = []
-        self.db_path = db_path
-        # read config once in the init of RepoGroup.
-        self.read()
-
-    def read(self):
-        with suppress(FileNotFoundError):
-            self.repos = pickle.loads(self.db_path.read_bytes())
-        return self
-
-    def save(self):
-        self.db_path.parent.mkdir(parents=True, exist_ok=True)
-        self.db_path.write_bytes(pickle.dumps(self.repos))
-
-    def info_repos(self):
-        print(INFO_BASE_STRING.format("Name", "Url", "Version"))
-        for repo in self.repos:
-            print(repo)
-
-    def find_repo(self, repo: str | RepoHandler) -> tuple[int, Optional[RepoHandler]]:
-        """
-        Find a repo.
-        return the index and the object of repo.
-        """
-        if isinstance(repo, str):
-            repo = RepoHandler(repo)
-        index = bisect.bisect_left(self.repos, repo)
-        if index != len(self.repos) and self.repos[index] == repo:
-            return (index, self.repos[index])
-        return (-1, None)
-
-    def info_one_repo(self, repo: str | RepoHandler) -> RepoHandler:
-        """
-        Print ALL messages about one repo.
-        If not found, raise exception `RepoNotFoundError`.
-        """
-        _, result = self.find_repo(repo)
-        if result:
-            pprint(vars(result))
-            return result
-        else:
-            raise RepoNotFoundError(getattr(repo, "name", repo))
-
-    def insert_repo(self, repo: RepoHandler):
-        """
-        Insert repo to RepoGroup, and save.
-        """
-        index = bisect.bisect_left(self.repos, repo)
-        self.repos.insert(index, repo)
-        self.save()
-
-    def remove_repo(self, repo: str | RepoHandler) -> RepoHandler:
-        """
-        Remove repo and save.
-        """
-        index, result = self.find_repo(repo)
-        if result:
-            self.repos.pop(index)
-            self.save()
-        else:
-            raise RepoNotFoundError(getattr(repo, "name", repo))
-
-    def alias_lnk(self, old_name: str, new_name: str):
-        """
-        Find `old_name` in all repo_group's `file_list`, and change the lnk and cmd name to `new_name`.
-
-        Note that the `old_name` and `new_name` should not include suffix.
-        """
-        assert WINDOWS, "alias is not supported on non-Windows systems."
-
-        # only change two files: lnk, cmd
-        count = 0
-        for repo in self.repos:
-            for i, s in enumerate(repo.installed_files):
-                s = Path(s)
-                assert s.exists(), "file in installed_list not found: " + s
-                if s.is_dir():
-                    continue
-                if s.stem == old_name and s.suffix in (".lnk", ".cmd", ""):
-                    new_path = s.with_stem(new_name)
-                    s.replace(new_path)
-                    repo.installed_files[i] = str(new_path)
-                    count += 1
-                    self.save()
-                if count >= 3:
-                    return
-        log.warning(
-            "You can update bpm and reinstall softwares to get cmd and sh support."
-        )
-
-
-import unittest  # noqa: E402
-
-
-class Test(unittest.TestCase):
-    def test_repogroup_operations(self):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir) / "repos.db"
-            test_group = RepoGroup(db_path=tmpdir)
-            # insert, save
-            test_group.insert_repo(RepoHandler("test_repo"))
-            test_group.insert_repo(RepoHandler("abc"))
-            test_group.insert_repo(RepoHandler("z"))
-            test_group.repos.clear()
-            # read
-            test_group.read()
-            self.assertListEqual(
-                ["abc", "test_repo", "z"], [r.name for r in test_group.repos]
-            )
-            # remove
-            test_group.remove_repo("test_repo")
-            self.assertListEqual(["abc", "z"], [r.name for r in test_group.repos])
-
-
-if __name__ == "__main__":
-    unittest.main()
-    exit(0)
-else:
-    repo_group = RepoGroup()
+import bisect
+import logging as log
+import pickle
+from contextlib import suppress
+from pathlib import Path
+from pprint import pprint
+from tempfile import TemporaryDirectory
+from typing import Optional
+
+from .search import RepoHandler
+from .utils.constants import DATABASE_PATH, INFO_BASE_STRING, WINDOWS
+from .utils.exceptions import RepoNotFoundError
+
+
+class RepoGroup:
+    def __init__(self, db_path=DATABASE_PATH):
+        self.repos: list[RepoHandler] = []
+        self.db_path = db_path
+        # read config once in the init of RepoGroup.
+        self.read()
+
+    def read(self):
+        with suppress(FileNotFoundError):
+            self.repos = pickle.loads(self.db_path.read_bytes())
+        return self
+
+    def save(self):
+        self.db_path.parent.mkdir(parents=True, exist_ok=True)
+        self.db_path.write_bytes(pickle.dumps(self.repos))
+
+    def info_repos(self):
+        print(INFO_BASE_STRING.format("Name", "Url", "Version"))
+        for repo in self.repos:
+            print(repo)
+
+    def find_repo(self, repo: str | RepoHandler) -> tuple[int, Optional[RepoHandler]]:
+        """
+        Find a repo.
+        return the index and the object of repo.
+        """
+        if isinstance(repo, str):
+            repo = RepoHandler(repo)
+        index = bisect.bisect_left(self.repos, repo)
+        if index != len(self.repos) and self.repos[index] == repo:
+            return (index, self.repos[index])
+        return (-1, None)
+
+    def info_one_repo(self, repo: str | RepoHandler) -> RepoHandler:
+        """
+        Print ALL messages about one repo.
+        If not found, raise exception `RepoNotFoundError`.
+        """
+        _, result = self.find_repo(repo)
+        if result:
+            pprint(vars(result))
+            return result
+        else:
+            raise RepoNotFoundError(getattr(repo, "name", repo))
+
+    def insert_repo(self, repo: RepoHandler):
+        """
+        Insert repo to RepoGroup, and save.
+        """
+        index = bisect.bisect_left(self.repos, repo)
+        self.repos.insert(index, repo)
+        self.save()
+
+    def remove_repo(self, repo: str | RepoHandler) -> RepoHandler:
+        """
+        Remove repo and save.
+        """
+        index, result = self.find_repo(repo)
+        if result:
+            self.repos.pop(index)
+            self.save()
+        else:
+            raise RepoNotFoundError(getattr(repo, "name", repo))
+
+    def alias_lnk(self, old_name: str, new_name: str):
+        """
+        Find `old_name` in all repo_group's `file_list`, and change the lnk and cmd name to `new_name`.
+
+        Note that the `old_name` and `new_name` should not include suffix.
+        """
+        assert WINDOWS, "alias is not supported on non-Windows systems."
+
+        # only change two files: lnk, cmd
+        count = 0
+        for repo in self.repos:
+            for i, s in enumerate(repo.installed_files):
+                s = Path(s)
+                assert s.exists(), "file in installed_list not found: " + s
+                if s.is_dir():
+                    continue
+                if s.stem == old_name and s.suffix in (".lnk", ".cmd", ""):
+                    new_path = s.with_stem(new_name)
+                    s.replace(new_path)
+                    repo.installed_files[i] = str(new_path)
+                    count += 1
+                    self.save()
+                if count >= 3:
+                    return
+        log.warning(
+            "You can update bpm and reinstall softwares to get cmd and sh support."
+        )
+
+
+import unittest  # noqa: E402
+
+
+class Test(unittest.TestCase):
+    def test_repogroup_operations(self):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir) / "repos.db"
+            test_group = RepoGroup(db_path=tmpdir)
+            # insert, save
+            test_group.insert_repo(RepoHandler("test_repo"))
+            test_group.insert_repo(RepoHandler("abc"))
+            test_group.insert_repo(RepoHandler("z"))
+            test_group.repos.clear()
+            # read
+            test_group.read()
+            self.assertListEqual(
+                ["abc", "test_repo", "z"], [r.name for r in test_group.repos]
+            )
+            # remove
+            test_group.remove_repo("test_repo")
+            self.assertListEqual(["abc", "z"], [r.name for r in test_group.repos])
+
+
+if __name__ == "__main__":
+    unittest.main()
+    exit(0)
+else:
+    repo_group = RepoGroup()
```

### Comparing `bin_package_manager-2.2.3/pyproject.toml` & `bin_package_manager-2.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[tool.poetry]
-name = "bin-package-manager"
-version = "2.2.3"
-description = "Bin package manager, a package manager based on Github release"
-authors = ["lxl66566 <lxl66566@gmail.com>"]
-license = "MIT"
-readme = ["README.md"]
-keywords = ["binary", "packaging", "release"]
-repository = "https://github.com/lxl66566/bpm"
-homepage = "https://github.com/lxl66566/bpm"
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-]
-packages = [{ include = "bpm" }]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-py7zr = { version = "^0.20.8", markers = "sys_platform == 'win32'" }
-requests = "^2.31.0"
-tqdm = "^4.66.2"
-pylnk3 = { version = "^0.4.2", markers = "sys_platform == 'win32'" }
-simpleufcs = "^1.0.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.scripts]
-bpm = 'bpm.cli:main'
-
-[[tool.poetry.source]]
-name = "tsinghua-pypi"
-url = "https://pypi.tuna.tsinghua.edu.cn/simple"
-priority = "default"
+[tool.poetry]
+name = "bin-package-manager"
+version = "2.2.4"
+description = "Bin package manager, a package manager based on Github release"
+authors = ["lxl66566 <lxl66566@gmail.com>"]
+license = "MIT"
+readme = ["README.md"]
+keywords = ["binary", "packaging", "release"]
+repository = "https://github.com/lxl66566/bpm"
+homepage = "https://github.com/lxl66566/bpm"
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+packages = [{ include = "bpm" }]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+py7zr = { version = "^0.20.8", markers = "sys_platform == 'win32'" }
+requests = "^2.31.0"
+tqdm = "^4.66.2"
+pylnk3 = { version = "^0.4.2", markers = "sys_platform == 'win32'" }
+simpleufcs = "^1.0.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+bpm = 'bpm.cli:main'
+
+[[tool.poetry.source]]
+name = "tsinghua-pypi"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
+priority = "default"
```

