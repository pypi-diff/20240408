# Comparing `tmp/mergify_cli-2024.3.27.9.45.tar.gz` & `tmp/mergify_cli-2024.4.8.14.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergify_cli-2024.3.27.9.45.tar", max compression
+gzip compressed data, was "mergify_cli-2024.4.8.14.47.tar", max compression
```

## Comparing `mergify_cli-2024.3.27.9.45.tar` & `mergify_cli-2024.4.8.14.47.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10143 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/LICENSE
--rw-r--r--   0        0        0     1127 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/README.md
--rwxr-xr-x   0        0        0    24776 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/mergify_cli/__init__.py
--rw-r--r--   0        0        0     1797 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/mergify_cli/hooks/commit-msg
--rw-r--r--   0        0        0        0 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/mergify_cli/tests/__init__.py
--rw-r--r--   0        0        0    11731 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/mergify_cli/tests/test_mergify_cli.py
--rw-r--r--   0        0        0     1886 2024-03-27 09:45:43.484694 mergify_cli-2024.3.27.9.45/mergify_cli/tests/utils.py
--rw-r--r--   0        0        0     2598 2024-03-27 09:45:43.488694 mergify_cli-2024.3.27.9.45/pyproject.toml
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 mergify_cli-2024.3.27.9.45/PKG-INFO
+-rw-r--r--   0        0        0    10143 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/LICENSE
+-rw-r--r--   0        0        0     1127 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/README.md
+-rwxr-xr-x   0        0        0    25540 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/hooks/commit-msg
+-rw-r--r--   0        0        0        0 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/tests/__init__.py
+-rw-r--r--   0        0        0    16887 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/tests/test_mergify_cli.py
+-rw-r--r--   0        0        0     2093 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/tests/utils.py
+-rw-r--r--   0        0        0     2598 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/pyproject.toml
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 mergify_cli-2024.4.8.14.47/PKG-INFO
```

### Comparing `mergify_cli-2024.3.27.9.45/LICENSE` & `mergify_cli-2024.4.8.14.47/LICENSE`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.3.27.9.45/README.md` & `mergify_cli-2024.4.8.14.47/README.md`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.3.27.9.45/mergify_cli/__init__.py` & `mergify_cli-2024.4.8.14.47/mergify_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,15 @@
     stacked_dest_branch: str,
     changeid: ChangeId,
     commit: str,
     title: str,
     message: str,
     known_changeids: KnownChangeIDs,
     create_as_draft: bool,
+    keep_pull_request_title_and_body: bool,
 ) -> tuple[PullRequest, str]:
     if changeid in known_changeids:
         pull = known_changeids.get(changeid)
         with console.status(
             f"* updating stacked branch `{stacked_dest_branch}` ({commit[-7:]}) - {pull['html_url'] if pull else '<stack branch without associated pull>'})",
         ):
             r = await client.patch(
@@ -343,23 +344,22 @@
     if pull and pull["head"]["sha"] == commit:
         action = "nothing"
     elif pull:
         action = "updated"
         with console.status(
             f"* updating pull request `{title}` (#{pull['number']}) ({commit[-7:]})",
         ):
-            r = await client.patch(
-                f"pulls/{pull['number']}",
-                json={
-                    "title": title,
-                    "body": message,
-                    "head": stacked_dest_branch,
-                    "base": stacked_base_branch,
-                },
-            )
+            pull_changes = {
+                "head": stacked_dest_branch,
+                "base": stacked_base_branch,
+            }
+            if not keep_pull_request_title_and_body:
+                pull_changes.update({"title": title, "body": message})
+
+            r = await client.patch(f"pulls/{pull['number']}", json=pull_changes)
             check_for_status(r)
     else:
         action = "created"
         with console.status(
             f"* creating stacked pull request `{title}` ({commit[-7:]})",
         ):
             r = await client.post(
@@ -492,19 +492,21 @@
         raise LocalBranchInvalidError(msg)
 
 
 # TODO(charly): fix PLR0913,PLR0914,PLR0915,PLR0917 (number of arguments, local
 # variables and statements)
 async def stack(  # noqa: PLR0913,PLR0914,PLR0915,PLR0917
     token: str,
+    skip_rebase: bool,
     next_only: bool,
     branch_prefix: str,
     dry_run: bool,
     trunk: tuple[str, str],
     create_as_draft: bool = False,
+    keep_pull_request_title_and_body: bool = False,
 ) -> None:
     os.chdir((await git("rev-parse --show-toplevel")).strip())
     dest_branch = await git("rev-parse --abbrev-ref HEAD")
 
     try:
         check_local_branch(branch_name=dest_branch, branch_prefix=branch_prefix)
     except LocalBranchInvalidError as e:
@@ -521,19 +523,22 @@
     if base_branch == dest_branch:
         console.log("[red] base branch and destination branch are the same [/]")
         sys.exit(1)
 
     stack_prefix = f"{branch_prefix}/{dest_branch}"
 
     if not dry_run:
-        with console.status(
-            f"Rebasing branch `{dest_branch}` on `{remote}/{base_branch}`...",
-        ):
-            await git(f"pull --rebase {remote} {base_branch}")
-        console.log(f"branch `{dest_branch}` rebased on `{remote}/{base_branch}`")
+        if skip_rebase:
+            console.log(f"branch `{dest_branch}` rebase skipped (--skip-rebase)")
+        else:
+            with console.status(
+                f"Rebasing branch `{dest_branch}` on `{remote}/{base_branch}`...",
+            ):
+                await git(f"pull --rebase {remote} {base_branch}")
+            console.log(f"branch `{dest_branch}` rebased on `{remote}/{base_branch}`")
 
         with console.status(
             f"Pushing branch `{dest_branch}` to `{remote}/{stack_prefix}/aio`...",
         ):
             await git(f"push -f {remote} {dest_branch}:{stack_prefix}/aio")
         console.log(f"branch `{dest_branch}` pushed to `{remote}/{stack_prefix}/aio` ")
 
@@ -620,14 +625,15 @@
                     stacked_dest_branch,
                     changeid,
                     commit,
                     title,
                     format_pull_description(message, depends_on),
                     known_changeids,
                     create_as_draft,
+                    keep_pull_request_title_and_body,
                 )
                 pulls.append(pull)
             else:
                 action = "skipped"
                 pull = known_changeids.get(changeid) or PullRequest(
                     {
                         "title": "<not yet created>",
@@ -715,19 +721,21 @@
 async def stack_main(args: argparse.Namespace) -> None:
     if args.setup:
         await do_setup()
         return
 
     await stack(
         args.token,
+        args.skip_rebase,
         args.next_only,
         args.branch_prefix,
         args.dry_run,
         args.trunk,
         args.draft,
+        args.keep_pull_request_title_and_body,
     )
 
 
 def parse_args(args: typing.MutableSequence[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--version",
@@ -762,20 +770,32 @@
     stack_parser.add_argument(
         "--next-only",
         "-x",
         action="store_true",
         help="Only rebase and update the next pull request of the stack",
     )
     stack_parser.add_argument(
+        "--skip-rebase",
+        "-R",
+        action="store_true",
+        help="Skip stack rebase",
+    )
+    stack_parser.add_argument(
         "--draft",
         "-d",
         action="store_true",
         help="Create stacked pull request as draft",
     )
     stack_parser.add_argument(
+        "--keep-pull-request-title-and-body",
+        "-k",
+        action="store_true",
+        help="Don't update the title and body of already opened pull requests",
+    )
+    stack_parser.add_argument(
         "--trunk",
         "-t",
         type=trunk_type,
         default=get_trunk(),
         help="Change the target branch of the stack",
     )
     stack_parser.add_argument(
```

### Comparing `mergify_cli-2024.3.27.9.45/mergify_cli/hooks/commit-msg` & `mergify_cli-2024.4.8.14.47/mergify_cli/hooks/commit-msg`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.3.27.9.45/mergify_cli/tests/test_mergify_cli.py` & `mergify_cli-2024.4.8.14.47/mergify_cli/tests/test_mergify_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -160,14 +160,15 @@
     respx_mock.get("/repos/user/repo/issues/2/comments").respond(200, json=[])
     post_comment2_mock = respx_mock.post("/repos/user/repo/issues/2/comments").respond(
         200,
     )
 
     await mergify_cli.stack(
         token="",
+        skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
 
     # First pull request is created
@@ -247,14 +248,15 @@
             "node_id": "",
         },
     )
     respx_mock.get("/repos/user/repo/issues/1/comments").respond(200, json=[])
 
     await mergify_cli.stack(
         token="",
+        skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
 
     # Pull request is created without stack comment
@@ -265,14 +267,93 @@
         "title": "Title commit 1",
         "body": "Message commit 1",
         "draft": False,
     }
 
 
 @pytest.mark.respx(base_url="https://api.github.com/")
+async def test_stack_update_no_rebase(
+    git_mock: test_utils.GitMock,
+    respx_mock: respx.MockRouter,
+) -> None:
+    # Mock 1 commits on branch `current-branch`
+    git_mock.commit(
+        test_utils.Commit(
+            sha="commit_sha",
+            title="Title",
+            message="Message",
+            change_id="I29617d37762fd69809c255d7e7073cb11f8fbf50",
+        ),
+    )
+
+    # Mock HTTP calls: the stack already exists but it's out of date, it should
+    # be updated
+    respx_mock.get("/repos/user/repo/git/matching-refs/heads//current-branch/").respond(
+        200,
+        json=[
+            {
+                "ref": "refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
+            },
+        ],
+    )
+    respx_mock.get(
+        "/repos/user/repo/pulls?head=user:/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50&state=open",
+    ).respond(
+        200,
+        json=[
+            {
+                "html_url": "",
+                "number": "123",
+                "title": "Title",
+                "head": {"sha": "previous_commit_sha"},
+                "state": "open",
+                "draft": False,
+                "node_id": "",
+            },
+        ],
+    )
+    respx_mock.patch(
+        "/repos/user/repo/git/refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
+    ).respond(200, json={})
+    patch_pull_mock = respx_mock.patch("/repos/user/repo/pulls/123").respond(
+        200,
+        json={},
+    )
+    respx_mock.get("/repos/user/repo/issues/123/comments").respond(
+        200,
+        json=[
+            {
+                "body": "This pull request is part of a stack:\n...",
+                "url": "https://api.github.com/repos/user/repo/issues/comments/456",
+            },
+        ],
+    )
+    respx_mock.patch("/repos/user/repo/issues/comments/456").respond(200)
+
+    await mergify_cli.stack(
+        token="",
+        skip_rebase=True,
+        next_only=False,
+        branch_prefix="",
+        dry_run=False,
+        trunk=("origin", "main"),
+    )
+    assert not git_mock.has_been_called_with("pull --rebase origin main")
+
+    # The pull request is updated
+    assert len(patch_pull_mock.calls) == 1
+    assert json.loads(patch_pull_mock.calls.last.request.content) == {
+        "head": "/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
+        "base": "main",
+        "title": "Title",
+        "body": "Message",
+    }
+
+
+@pytest.mark.respx(base_url="https://api.github.com/")
 async def test_stack_update(
     git_mock: test_utils.GitMock,
     respx_mock: respx.MockRouter,
 ) -> None:
     # Mock 1 commits on branch `current-branch`
     git_mock.commit(
         test_utils.Commit(
@@ -325,39 +406,119 @@
             },
         ],
     )
     respx_mock.patch("/repos/user/repo/issues/comments/456").respond(200)
 
     await mergify_cli.stack(
         token="",
+        skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
+    assert git_mock.has_been_called_with("pull --rebase origin main")
 
     # The pull request is updated
     assert len(patch_pull_mock.calls) == 1
     assert json.loads(patch_pull_mock.calls.last.request.content) == {
         "head": "/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
         "base": "main",
         "title": "Title",
         "body": "Message",
     }
 
 
 @pytest.mark.respx(base_url="https://api.github.com/")
+async def test_stack_update_keep_title_and_body(
+    git_mock: test_utils.GitMock,
+    respx_mock: respx.MockRouter,
+) -> None:
+    # Mock 1 commits on branch `current-branch`
+    git_mock.commit(
+        test_utils.Commit(
+            sha="commit_sha",
+            title="New Title that should be ignored",
+            message="New Message that should be ignored",
+            change_id="I29617d37762fd69809c255d7e7073cb11f8fbf50",
+        ),
+    )
+
+    # Mock HTTP calls: the stack already exists but it's out of date, it should
+    # be updated
+    respx_mock.get("/repos/user/repo/git/matching-refs/heads//current-branch/").respond(
+        200,
+        json=[
+            {
+                "ref": "refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
+            },
+        ],
+    )
+    respx_mock.get(
+        "/repos/user/repo/pulls?head=user:/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50&state=open",
+    ).respond(
+        200,
+        json=[
+            {
+                "html_url": "",
+                "number": "123",
+                "title": "Title",
+                "head": {"sha": "previous_commit_sha"},
+                "state": "open",
+                "draft": False,
+                "node_id": "",
+            },
+        ],
+    )
+    respx_mock.patch(
+        "/repos/user/repo/git/refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
+    ).respond(200, json={})
+    patch_pull_mock = respx_mock.patch("/repos/user/repo/pulls/123").respond(
+        200,
+        json={},
+    )
+    respx_mock.get("/repos/user/repo/issues/123/comments").respond(
+        200,
+        json=[
+            {
+                "body": "This pull request is part of a stack:\n...",
+                "url": "https://api.github.com/repos/user/repo/issues/comments/456",
+            },
+        ],
+    )
+    respx_mock.patch("/repos/user/repo/issues/comments/456").respond(200)
+
+    await mergify_cli.stack(
+        token="",
+        skip_rebase=False,
+        next_only=False,
+        branch_prefix="",
+        dry_run=False,
+        trunk=("origin", "main"),
+        keep_pull_request_title_and_body=True,
+    )
+
+    # The pull request is updated
+    assert len(patch_pull_mock.calls) == 1
+    assert json.loads(patch_pull_mock.calls.last.request.content) == {
+        "head": "/current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
+        "base": "main",
+    }
+
+
+@pytest.mark.respx(base_url="https://api.github.com/")
 async def test_stack_on_destination_branch_raises_an_error(
     git_mock: test_utils.GitMock,
 ) -> None:
     git_mock.mock("rev-parse --abbrev-ref HEAD", "main")
 
     with pytest.raises(SystemExit, match="1"):
         await mergify_cli.stack(
             token="",
+            skip_rebase=False,
             next_only=False,
             branch_prefix="",
             dry_run=False,
             trunk=("origin", "main"),
         )
 
 
@@ -366,12 +527,13 @@
     git_mock: test_utils.GitMock,
 ) -> None:
     git_mock.mock("merge-base --fork-point origin/main", "")
 
     with pytest.raises(SystemExit, match="1"):
         await mergify_cli.stack(
             token="",
+            skip_rebase=False,
             next_only=False,
             branch_prefix="",
             dry_run=False,
             trunk=("origin", "main"),
         )
```

### Comparing `mergify_cli-2024.3.27.9.45/mergify_cli/tests/utils.py` & `mergify_cli-2024.4.8.14.47/mergify_cli/tests/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,20 +23,25 @@
     change_id: str
 
 
 @dataclasses.dataclass
 class GitMock:
     _mocked: dict[str, str] = dataclasses.field(init=False, default_factory=dict)
     _commits: list[Commit] = dataclasses.field(init=False, default_factory=list)
+    _called: list[str] = dataclasses.field(init=False, default_factory=list)
 
     def mock(self, command: str, output: str) -> None:
         self._mocked[command] = output
 
+    def has_been_called_with(self, args: str) -> bool:
+        return args in self._called
+
     async def __call__(self, args: str) -> str:
         if args in self._mocked:
+            self._called.append(args)
             return self._mocked[args]
 
         msg = f"git_mock called with `{args}`, not mocked!"
         raise AssertionError(msg)
 
     def commit(self, commit: Commit) -> None:
         self._commits.append(commit)
```

### Comparing `mergify_cli-2024.3.27.9.45/pyproject.toml` & `mergify_cli-2024.4.8.14.47/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.group.dev.dependencies]
 mypy = {version = ">=0.930"}
 mypy-extensions = "^1.0.0"
-ruff = ">=0.0.277,<0.3.5"
+ruff = ">=0.0.277,<0.3.6"
 pytest = {version = ">=6.2.5"}
 poethepoet = ">=0.21,<0.26"
 pytest-asyncio = "^0.23.2"
 respx = ">=0.20.2,<0.22.0"
 types-aiofiles = "^23.2.0.20240106"
 
 [tool.poetry.scripts]
```

### Comparing `mergify_cli-2024.3.27.9.45/PKG-INFO` & `mergify_cli-2024.4.8.14.47/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergify_cli
-Version: 2024.3.27.9.45
+Version: 2024.4.8.14.47
 Summary: Mergify CLI is a tool that automates the creation and management of stacked pull requests on GitHub
 License: Apache License
 Author: Mehdi Abaakouk
 Author-email: sileht@mergify.com
 Requires-Python: >=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

