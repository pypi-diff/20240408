# Comparing `tmp/literategit-0.3.1rc1.tar.gz` & `tmp/literategit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/literategit-0.3.1rc1.tar", last modified: Sat Feb 15 07:31:47 2020, max compression
+gzip compressed data, was "literategit-0.4.6.tar", max compression
```

## Comparing `literategit-0.3.1rc1.tar` & `literategit-0.4.6.tar`

### file list

```diff
@@ -1,27 +1,19 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/
--rw-rw-r--   0 ben       (1000) ben       (1000)       27 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/MANIFEST.in
--rw-rw-r--   0 ben       (1000) ben       (1000)     1180 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)    10358 2020-02-11 14:52:40.000000 literategit-0.3.1rc1/README.md
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit/
--rw-rw-r--   0 ben       (1000) ben       (1000)     9638 2020-02-11 14:52:40.000000 literategit-0.3.1rc1/literategit/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)       50 2020-02-15 07:31:33.000000 literategit-0.3.1rc1/literategit/_version.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit/cli/
--rw-rw-r--   0 ben       (1000) ben       (1000)      100 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/literategit/cli/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     2371 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/literategit/cli/dump_all_trees.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     2726 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/literategit/cli/render.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      986 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/literategit/cli/repo_for_path.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      268 2020-02-11 14:52:40.000000 literategit-0.3.1rc1/literategit/content.html.tmpl
--rw-rw-r--   0 ben       (1000) ben       (1000)      787 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/literategit/diff.html.tmpl
--rw-rw-r--   0 ben       (1000) ben       (1000)     3365 2020-01-16 15:41:46.000000 literategit-0.3.1rc1/literategit/dump_all_trees.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      475 2020-02-15 07:25:21.000000 literategit-0.3.1rc1/literategit/example_create_url.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      988 2020-02-15 07:25:21.000000 literategit-0.3.1rc1/literategit/node.html.tmpl
--rw-rw-r--   0 ben       (1000) ben       (1000)     1513 2020-02-11 14:52:40.000000 literategit-0.3.1rc1/literategit/page.html.tmpl
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/
--rw-rw-r--   0 ben       (1000) ben       (1000)     1180 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      596 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)      116 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       53 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       12 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/literategit.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       63 2020-02-15 07:31:47.000000 literategit-0.3.1rc1/setup.cfg
--rw-rw-r--   0 ben       (1000) ben       (1000)     1401 2020-02-15 07:05:58.000000 literategit-0.3.1rc1/setup.py
+-rw-r--r--   0        0        0     1930 2024-04-08 15:49:49.991908 literategit-0.4.6/COPYING
+-rw-r--r--   0        0        0    35147 2024-04-06 16:10:11.658789 literategit-0.4.6/LICENCE.txt
+-rw-r--r--   0        0        0      512 2024-04-08 15:49:49.991908 literategit-0.4.6/README-short.md
+-rw-r--r--   0        0        0     9443 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/_version.py
+-rw-r--r--   0        0        0      141 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/cli/__init__.py
+-rw-r--r--   0        0        0     2182 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/cli/dump_all_trees.py
+-rw-r--r--   0        0        0     2770 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/cli/render.py
+-rw-r--r--   0        0        0      986 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/cli/repo_for_path.py
+-rw-r--r--   0        0        0      268 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/content.html.tmpl
+-rw-r--r--   0        0        0      787 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/diff.html.tmpl
+-rw-r--r--   0        0        0     3405 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/dump_all_trees.py
+-rw-r--r--   0        0        0      475 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/example_create_url.py
+-rw-r--r--   0        0        0     6333 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/literate-git.css
+-rw-r--r--   0        0        0     8346 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/literate-git.js
+-rw-r--r--   0        0        0      988 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/node.html.tmpl
+-rw-r--r--   0        0        0     1513 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/page.html.tmpl
+-rw-r--r--   0        0        0     1046 2024-04-08 15:49:49.991908 literategit-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 literategit-0.4.6/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `literategit-0.3.1rc1/literategit/__init__.py` & `literategit-0.4.6/literategit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016, 2019 Ben North and others; see COPYING
+# Copyright (C) 2016, 2019, 2024 Ben North and others; see COPYING
 #
 # This file is part of literate-git tools --- render a literate git repository
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,32 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from functools import partial
 import markdown2
 import os
 import functools
 import pygit2 as git
 from collections import namedtuple
 import jinja2
+import markupsafe
 import pygments
 import pygments.lexers
 import pygments.formatters
 import pygments.util
 
-class NakedHtmlFormatter(pygments.formatters.HtmlFormatter):
-    """A HTML formatter that doesn't wrap the lines in a <div>"""
-    def wrap(self, source, outfile):
-        for i, t in source:
-            yield i, t
-
 
 class TemplateSuite:
     def __init__(self, create_url, title, has_results=True):
         """
         Create a TemplateSuite instance from the given 'URL factory' and title.
 
         The 'create_url' argument should have attributes:
@@ -71,20 +65,21 @@
         self.page = env.get_template('page.html.tmpl')
 
     def as_html_fragment(self, x):
         return x.as_html_fragment(self)
 
     @staticmethod
     def markdown(source_text):
-        return jinja2.Markup(markdown2.markdown(source_text,
-                                                extras=['fenced-code-blocks']))
+        return markupsafe.Markup(
+            markdown2.markdown(source_text, extras=['fenced-code-blocks'])
+        )
 
     @staticmethod
     def markdown_inner_only(source_text):
-        full_markdown = jinja2.Markup(markdown2.markdown(source_text)).rstrip()
+        full_markdown = markupsafe.Markup(markdown2.markdown(source_text)).rstrip()
 
         outermost_is_p = (full_markdown.startswith('<p>')
                           and full_markdown.endswith('</p>'))
 
         if not outermost_is_p:
             raise ValueError(
                 'expecting markdown which converts to a paragraph; got "{}"'
@@ -147,15 +142,17 @@
             ch = repo[ch].parent_ids[0]
             seqnum -= 1
         children.reverse()
         return cls(repo, commit, children, seqnum_path)
 
 
 class Diff(namedtuple('Diff', 'repo tree_1 tree_0')):
-    formatter = NakedHtmlFormatter(linenos=False, wrapcode=True)
+    formatter = pygments.formatters.HtmlFormatter(
+        nowrap=True, linenos=False, wrapcode=True
+    )
     repo_being_cached = None
 
     def as_html_fragment(self, template_suite):
         diff = self.repo.diff(self.repo[self.tree_0], self.repo[self.tree_1])
 
         old_highlighted = self.collect_highlights(self.tree_0)
         new_highlighted = self.collect_highlights(self.tree_1)
@@ -214,33 +211,36 @@
 
     @staticmethod
     def suppress_no_lineno(lineno):
         if lineno == -1:
             return ''
         return str(lineno)
 
+
 def leaf_or_section(repo, oid, seqnum_path):
     commit = _commit(repo, oid)
     n_parents = len(commit.parent_ids)
     if n_parents == 1:
         return LeafCommit.from_commit(repo, oid, seqnum_path)
     elif n_parents == 2:
         return SectionCommit.from_commit(repo, oid, seqnum_path)
     else:
         raise ValueError('cannot handle {} parents of {}'
                          .format(n_parents, oid))
 
+
 def n_steps_between(repo, begin_oid, end_oid):
     n = 0
     oid = begin_oid
     while oid != end_oid:
         n += 1
         oid = repo[oid].parent_ids[0]
     return n
 
+
 def list_from_range(repo, base_branch_name, branch_name):
     end_oid = repo.lookup_branch(base_branch_name).target
     oid = repo.lookup_branch(branch_name).target
     elements = []
     seqnum = n_steps_between(repo, oid, end_oid)
     while oid != end_oid:
         element = leaf_or_section(repo, oid, [seqnum])
```

### Comparing `literategit-0.3.1rc1/literategit/cli/dump_all_trees.py` & `literategit-0.4.6/literategit/cli/dump_all_trees.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016 Ben North
+# Copyright (C) 2016, 2024 Ben North
 #
 # This file is part of literate-git tools --- render a literate git repository
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,50 +11,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""git-dump-all-trees
-
-Usage:
-  git-dump-all-trees (-h | --help)
-  git-dump-all-trees --version
-  git-dump-all-trees <output-root> <rev1> <rev2>
-
-Options:
-  -h --help    Show this help info
-  --version    Display version info and exit
-
-Write, to <output-root>, a collection of files which represent snapshots
-of all commits reachable from <rev2> but not reachable from <rev1>.
-
-The newly-created output directory contains two directories:
-
-    blobs/ --- Contains one file per blob reachable from any commit in
-        rev1..rev2.  Each blob resides in a directory named by the first
-        two characters of the blob's SHA1.  The remaining 38 characters
-        of the SHA1 give the filename within that directory.
-
-    commit-trees/ --- Contains one directory per commit, in the same
-        2/38 format as the blobs.  Each commit's directory contains the
-        files and directories making up the tree corresponding to that
-        commit.  (Files are hard links to the appropriate blob within
-        the blobs directory; directories are real directories.)
-"""
-
 import os
-import pygit2 as git
-import docopt
+import click
 import literategit.dump_all_trees
 from literategit._version import __version__
 from literategit.cli.repo_for_path import repo_for_path
 
-def dump_all_trees():
-    args = docopt.docopt(__doc__,
-                         version='git-dump-all-trees {}'.format(__version__))
-    repo = repo_for_path(os.getcwd())
 
+@click.command
+@click.version_option(__version__)
+@click.argument("output_root")
+@click.argument("rev1")
+@click.argument("rev2")
+def dump_all_trees(output_root, rev1, rev2):
+    """
+    Write, to OUTPUT_ROOT, a collection of files which represent snapshots
+    of all commits reachable from REV2 but not reachable from REV1.
+
+    The newly-created output directory contains two directories:
+
+        blobs/ --- Contains one file per blob reachable from any commit in
+            REV1..REV2.  Each blob resides in a directory named by the first
+            two characters of the blob's SHA1.  The remaining 38 characters
+            of the SHA1 give the filename within that directory.
+
+        commit-trees/ --- Contains one directory per commit, in the same
+            2/38 format as the blobs.  Each commit's directory contains the
+            files and directories making up the tree corresponding to that
+            commit.  (Files are hard links to the appropriate blob within
+            the blobs directory; directories are real directories.)
+    """
+    repo = repo_for_path(os.getcwd())
     literategit.dump_all_trees.dump_all_trees(repo,
-                                              args['<rev1>'], args['<rev2>'],
-                                              args['<output-root>'])
+                                              rev1, rev2,
+                                              output_root)
```

### Comparing `literategit-0.3.1rc1/literategit/cli/repo_for_path.py` & `literategit-0.4.6/literategit/cli/repo_for_path.py`

 * *Files identical despite different names*

### Comparing `literategit-0.3.1rc1/literategit/diff.html.tmpl` & `literategit-0.4.6/literategit/diff.html.tmpl`

 * *Files identical despite different names*

### Comparing `literategit-0.3.1rc1/literategit/dump_all_trees.py` & `literategit-0.4.6/literategit/dump_all_trees.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
+import pygit2
 
 
 def collect_commits(repo, rev1, rev2):
     """
     List of all Commit objects which are reachable from rev2 but not
     reachable from rev1.  Commits are not returned in any particular
     order.
@@ -73,18 +74,18 @@
     def new_nested_for_commit(self, commit):
         sha1 = commit.id.hex
         dirname = os.path.join(sha1[:2], sha1[2:])
         return self.new_nested(dirname)
 
     def create_all(self, tree_oid):
         for entry in self.repo[tree_oid]:
-            if entry.type == 'blob':
+            if entry.type == pygit2.GIT_OBJ_BLOB:
                 blob_filename = self.write_blobs.ensure_exists(entry.oid)
                 os.link(blob_filename, os.path.join(self.outdir, entry.name))
-            elif entry.type == 'tree':
+            elif entry.type == pygit2.GIT_OBJ_TREE:
                 self.new_nested(entry.name).create_all(entry.oid)
             else:
                 raise ValueError('unhandled type "{}"'.format(entry.type))
 
 
 def dump_all_trees(repo, rev1, rev2, out_root):
     write_blobs = WriteBlobs(repo, os.path.join(out_root, 'blobs'))
```

### Comparing `literategit-0.3.1rc1/literategit/node.html.tmpl` & `literategit-0.4.6/literategit/node.html.tmpl`

 * *Files identical despite different names*

### Comparing `literategit-0.3.1rc1/literategit/page.html.tmpl` & `literategit-0.4.6/literategit/page.html.tmpl`

 * *Files identical despite different names*

