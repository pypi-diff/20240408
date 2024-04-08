# Comparing `tmp/sphinx_graph-0.2.2.tar.gz` & `tmp/sphinx_graph-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_graph-0.2.2.tar", max compression
+gzip compressed data, was "sphinx_graph-0.2.3.tar", max compression
```

## Comparing `sphinx_graph-0.2.2.tar` & `sphinx_graph-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2814 2023-03-07 17:22:07.401953 sphinx_graph-0.2.2/README.md
--rw-r--r--   0        0        0     2766 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1044 2023-03-14 10:03:27.309612 sphinx_graph-0.2.2/src/sphinx_graph/__init__.py
--rw-r--r--   0        0        0     2942 2023-03-07 17:22:07.401953 sphinx_graph-0.2.2/src/sphinx_graph/config.py
--rw-r--r--   0        0        0      698 2023-03-07 17:22:07.401953 sphinx_graph-0.2.2/src/sphinx_graph/format.py
--rw-r--r--   0        0        0     1539 2023-02-19 14:41:02.117327 sphinx_graph-0.2.2/src/sphinx_graph/parse.py
--rw-r--r--   0        0        0     1027 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/table/__init__.py
--rw-r--r--   0        0        0     1271 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/table/directive.py
--rw-r--r--   0        0        0     4327 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/table/events.py
--rw-r--r--   0        0        0      548 2023-03-07 17:22:07.401953 sphinx_graph-0.2.2/src/sphinx_graph/table/info.py
--rw-r--r--   0        0        0      298 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/table/node.py
--rw-r--r--   0        0        0     1447 2023-03-07 17:22:07.401953 sphinx_graph-0.2.2/src/sphinx_graph/table/state.py
--rw-r--r--   0        0        0      485 2023-02-19 14:41:02.117327 sphinx_graph-0.2.2/src/sphinx_graph/util.py
--rw-r--r--   0        0        0     1147 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/vertex/__init__.py
--rw-r--r--   0        0        0     1232 2023-03-07 17:22:07.405953 sphinx_graph-0.2.2/src/sphinx_graph/vertex/config.py
--rw-r--r--   0        0        0     3710 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/vertex/directive.py
--rw-r--r--   0        0        0     3598 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/vertex/events.py
--rw-r--r--   0        0        0     1098 2023-03-07 17:22:07.405953 sphinx_graph-0.2.2/src/sphinx_graph/vertex/info.py
--rw-r--r--   0        0        0     3216 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/vertex/layout.py
--rw-r--r--   0        0        0      299 2023-03-14 13:53:17.399035 sphinx_graph-0.2.2/src/sphinx_graph/vertex/node.py
--rw-r--r--   0        0        0      448 2023-03-07 17:22:07.405953 sphinx_graph-0.2.2/src/sphinx_graph/vertex/query.py
--rw-r--r--   0        0        0     4142 2023-03-07 17:22:07.405953 sphinx_graph-0.2.2/src/sphinx_graph/vertex/state.py
--rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 sphinx_graph-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2800 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/README.md
+-rw-r--r--   0        0        0     3896 2024-04-08 08:12:06.108863 sphinx_graph-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      997 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/__init__.py
+-rw-r--r--   0        0        0     2998 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/config.py
+-rw-r--r--   0        0        0      763 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/format.py
+-rw-r--r--   0        0        0     1540 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/parse.py
+-rw-r--r--   0        0        0      956 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/table/__init__.py
+-rw-r--r--   0        0        0     1365 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/table/directive.py
+-rw-r--r--   0        0        0     4429 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/table/events.py
+-rw-r--r--   0        0        0      548 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/table/info.py
+-rw-r--r--   0        0        0      277 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/table/node.py
+-rw-r--r--   0        0        0     1530 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/table/state.py
+-rw-r--r--   0        0        0      485 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/util.py
+-rw-r--r--   0        0        0     1015 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/__init__.py
+-rw-r--r--   0        0        0     1288 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/config.py
+-rw-r--r--   0        0        0     3702 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/directive.py
+-rw-r--r--   0        0        0     2880 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/events.py
+-rw-r--r--   0        0        0     1172 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/info.py
+-rw-r--r--   0        0        0     3264 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/layout.py
+-rw-r--r--   0        0        0      278 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/node.py
+-rw-r--r--   0        0        0      475 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/query.py
+-rw-r--r--   0        0        0     7902 2024-02-01 11:03:35.947857 sphinx_graph-0.2.3/src/sphinx_graph/vertex/state.py
+-rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 sphinx_graph-0.2.3/PKG-INFO
```

### Comparing `sphinx_graph-0.2.2/README.md` & `sphinx_graph-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
    of its parent.
 
    The fingerprint is a 4-character hash. If USR-001 is modified, then SYS-002 will fail the build
    until the fingerprint is updated (the build error provides the new fingerprint). This means that
    changing a Vertex will trigger a review of all dependent vertices.
 ```
 
-For more information, see [the docs](https://sphinx-graph.readthedocs.io/en/main/src/index.html).
+For more information, see [the docs](https://sphinx-graph.readthedocs.io/en/main/).
 
 or, build the local docs-
 
       cd docs
       poetry run make html
 
 ---
```

### Comparing `sphinx_graph-0.2.2/pyproject.toml` & `sphinx_graph-0.2.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-graph"
-version = "0.2.2"
+version = "0.2.3"
 description = "'Sphinx-Graph' is a plain-text, VCS-friendly, requirements management tool."
 authors = ["Daniel Eades <danieleades@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/danieleades/sphinx-graph"
 documentation = "https://sphinx-graph.readthedocs.io/en/latest/index.html"
 keywords = ["sphinx, requirements", "documentation", "plain-text"]
@@ -12,101 +12,133 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Utilities",
     "Topic :: Documentation",
     "Topic :: Utilities",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Intended Audience :: Manufacturing",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
-sphinx = "^6.1.3"
-networkx = "^3.0"
+python = "^3.9"
+sphinx = ">=6, <8"
 toml = "^0.10.2"
-
+rustworkx = "^0.14.0"
 
 [tool.poetry.group.dev.dependencies]
 
 # testing
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
 
 # typing
 mypy = "^1.0.1"
-types-docutils = "^0.19.1.1"
+types-docutils = "^0.20.0.0"
 types-toml = "^0.10.8.5"
 
+# linting
+pre-commit = "^3.4.0"
+
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
-sphinx-rtd-theme = "^1.1.1"
+sphinx-rtd-theme = "^2.0.0"
 
 
 [tool.mypy]
 strict = true
 show_error_codes = true
 files = "src,tests"
 exclude = "tests/roots"
 no_implicit_reexport = true
 
-[[tool.mypy.overrides]]
-module = ["networkx.*"]
-ignore_missing_imports = true
-
 
 [tool.ruff]
-target-version = "py38"
-select = [
-    "A00",  # flake8-builtins
-    "ARG",  # flake8-unused-arguments
-    "B",    # flake8-bugbear
-    "C4",   # flake8-comprehensions
-    "C901", # function cognitive complexity
-    "D",    # pydocstyle
-    "E",    # flake8 built-ins
-    "EM",   # flake8-errmsg
-    "ERA",  # flake8-eradicate
-    "F",    # flake8 built-ins
-    "FBT",  # boolean trap
-    "I001", # isort
-    "ISC",  # implicit-str-concat
-    "N8",   # pep8-naming
-    "PGH",  # pygrep-hooks
-    "PIE",  # flake8-pie
-    "PLC",  # pylint
-    "PLE",  # pylint
-    "PLR",  # pylint
-    "PLW",  # pylint
-    "PT",   # flake8-pytest-style"
-    "Q",    # flake8-quotes
-    "RET",  # flake8-return
-    "RUF",  # Ruff-specific lints
-    "S",    # flake8-bandit
-    "UP",   # pyupgrade
-    "W",    # flake8 built-ins
+target-version = "py39"
+lint.select = [
+    "A",      # flake8-builtins
+    "ANN",    # flake8-annotations
+    "ARG",    # flake8-unused-arguments
+    "ASYNC",  # flake8-async
+    "B",      # flake8-bugbear
+    "BLE",    # flake8-blind-except
+    "C4",     # flake8-comprehensions
+    "C90",    # cognitive complexity
+    "COM",    # flake8-commas
+    "D",      # pydocstyle
+    "DTZ",    # flake8-datetimez
+    "E",      # flake8 built-ins
+    "EM",     # flake8-errmsg
+    "ERA",    # flake8-eradicate
+    "EXE",    # flake8-executable
+    "F",      # flake8 built-ins
+    "FA",     # flake8-future-annotations
+    "FBT",    # boolean trap
+    "FLY",    # flynt
+    "FURB",   # refurb
+    "G",      # flake8-logging-format
+    "I",      # isort
+    "ICN",    # flake8-import-conventions
+    "INT",    # flake8-gettext
+    "ISC",    # implicit-str-concat
+    "LOG",    # flake8-logging
+    "N",      # pep8-naming
+    "PERF",   # perflint
+    "PGH",    # pygrep-hooks
+    "PIE",    # flake8-pie
+    "PL",     # pylint
+    "PT",     # flake8-pytest-style
+    "PTH",    # flake8-use-pathlib
+    "PYI",    # flake8-pyi
+    "Q",      # flake8-quotes
+    "RET",    # flake8-return
+    "RSE",    # flake8-raise
+    "RUF",    # Ruff-specific lints
+    "S",      # flake8-bandit
+    "SIM",    # flake8-simplify
+    "SLF",    # flake8-self
+    "SLOT",   # flake8-slots
+    "T20",    # flake8-print
+    "TCH",    # flake8-type-checking
+    "TID252", # ban relative imports
+    "TRY",    # tryceratops
+    "UP",     # pyupgrade
+    "W",      # flake8 built-ins
+    "TRY",    # tryceratops
+    "YTT",    # flake8-2020
+]
+lint.ignore = [
+    "ANN101", # missing type annotation for 'self' in method
+    "ANN102", # missing type annotation for 'cls' in method
+    "COM812", # ignore when using ruff-format
+    "G004",   # Logging statement uses f-string
+    "ISC001", # ignore when using ruff-format
 ]
 
-[tool.ruff.pydocstyle]
-convention = "google"
+lint.pydocstyle.convention = "google"
 
-[tool.ruff.per-file-ignores]
-"tests/*" = ["A001", "A002", "D100", "D103", "D104", "FBT001", "S101"]
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = [
+    "D100",  # missing docstring in public module
+    "D103",  # missing docstring in public function
+    "D104",  # missing docstring in public package
+    "S101",  # use of 'assert' detected
+]
 "docs/conf.py" = ["A001", "D100"]
 
-[tool.ruff.isort]
-known-first-party = ["sphinx_graph"]
+
+[tool.coverage.report]
+exclude_also = ["if TYPE_CHECKING:"]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/__init__.py` & `sphinx_graph-0.2.3/src/sphinx_graph/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     ]
 """
 
 from typing import TypedDict
 
 from sphinx.application import Sphinx
 
-from sphinx_graph import table, vertex
-from sphinx_graph.config import Config
-from sphinx_graph.vertex import Config as VertexConfig
-from sphinx_graph.vertex import Query
+from . import table, vertex
+from .config import Config
+from .vertex import Config as VertexConfig
+from .vertex import Query
 
 __all__ = [
     "Config",
-    "VertexConfig",
     "Query",
+    "VertexConfig",
     "vertex",
 ]
 
 
 class ExtensionMetadata(TypedDict):
     """The metadata returned by this extension."""
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/config.py` & `sphinx_graph-0.2.3/src/sphinx_graph/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Custom configuration for Sphinx Graph."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
 from sphinx_graph import vertex
-from sphinx_graph.vertex.query import Query
+
+if TYPE_CHECKING:
+    from sphinx_graph.vertex.query import Query
 
 
 @dataclass
 class Config:
     """Configuration for the sphinx-graph extension.
 
     Example::
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/format.py` & `sphinx_graph-0.2.3/src/sphinx_graph/format.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Helper functions for formating vertices into docutils nodes."""
 
 from __future__ import annotations
 
-from typing import Iterable, TypeVar
+from typing import TYPE_CHECKING, TypeVar
 
 from docutils import nodes
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
 T = TypeVar("T")
 
 __all__ = [
     "comma_separated_list",
 ]
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/parse.py` & `sphinx_graph-0.2.3/src/sphinx_graph/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for parsing restructured text directives into options."""
+
 from __future__ import annotations
 
 from sphinx.errors import ConfigError
 
 
 def boolean(value: str | None) -> bool:
     """Parse a boolean flag.
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/table/__init__.py` & `sphinx_graph-0.2.3/src/sphinx_graph/table/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Types and methods specific to the vertex-table directive."""
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
-from sphinx_graph.table import events
-from sphinx_graph.table.directive import Directive
-from sphinx_graph.table.info import Info
-from sphinx_graph.table.node import TableNode
+from . import events
+from .directive import Directive
+from .info import Info
+from .node import TableNode
 
 __all__ = [
-    "Info",
     "Directive",
+    "Info",
     "TableNode",
     "register",
 ]
 
 
 def visit_node(_self: nodes.GenericNodeVisitor, _node: nodes.Node) -> None:
     """Visits the Vertex node.
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/table/directive.py` & `sphinx_graph-0.2.3/src/sphinx_graph/table/directive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """Sphinx Directive for Vertex objects."""
 
 from __future__ import annotations
 
 import uuid
-from typing import Sequence
+from typing import TYPE_CHECKING, ClassVar
 
 import toml
-from docutils import nodes
 from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective
-from sphinx.util.typing import OptionSpec
 
 from sphinx_graph import parse
 from sphinx_graph.table.info import Info
 from sphinx_graph.table.node import TableNode
 from sphinx_graph.table.state import State
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+    from docutils import nodes
+    from sphinx.util.typing import OptionSpec
+
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "Directive",
 ]
 
 
 class Directive(SphinxDirective):
     """An RST node representing a table of Vertices."""
 
     has_content = True
     required_arguments = 0
-    option_spec: OptionSpec = {
+    option_spec: ClassVar[OptionSpec] = {
         "query": parse.string,
     }
 
     def run(self) -> Sequence[nodes.Node]:
         """Run the directive and return a Vertex node."""
         uid = uuid.uuid4()
         node = TableNode(graph_uid=uid)
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/table/events.py` & `sphinx_graph-0.2.3/src/sphinx_graph/table/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """Lifecycle events specific to the vertex-table directive."""
 
 from __future__ import annotations
 
-from typing import Iterable
+from typing import TYPE_CHECKING
 
 from docutils import nodes
-from sphinx.application import Sphinx
-from sphinx.builders import Builder
 from sphinx.errors import ConfigError
 
 from sphinx_graph import vertex
 from sphinx_graph.format import comma_separated_list
 from sphinx_graph.table.node import TableNode
 from sphinx_graph.table.state import State
 from sphinx_graph.vertex.events import relative_uris, vertex_reference
 from sphinx_graph.vertex.query import DEFAULT_QUERY, QUERIES
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from sphinx.application import Sphinx
+    from sphinx.builders import Builder
+
 __all__ = [
     "register",
 ]
 
 
 def relatives(
-    builder: Builder, docname: str, state: vertex.State, uid: str
+    builder: Builder,
+    docname: str,
+    state: vertex.State,
+    uid: str,
 ) -> tuple[Iterable[nodes.reference], Iterable[nodes.reference]]:
     """Find the realtive URIs of the immediate 'relatives' of a given vertex.
 
     Args:
         builder: The sphinx builder instance
         docname: the name of the current document
         state: the global vertex information
@@ -35,15 +42,15 @@
     Returns:
         a tuple of (parents, children) where each is an iterable over
         (target_uid, relative_uri)
     """
     info = state.vertices[uid]
     [parents, children] = [
         relative_uris(builder, docname, state.vertices, uids)
-        for uids in [info.parents.keys(), state.graph.successors(uid)]
+        for uids in [info.parents.keys(), state.children(uid)]
     ]
     return (parents, children)
 
 
 def process(app: Sphinx, doctree: nodes.document, _fromdocname: str) -> None:
     """Process Vertex nodes by formatting and adding links to graph neighbours."""
     builder = app.builder
@@ -60,15 +67,16 @@
         query = queries[info.query or DEFAULT_QUERY]
         vertices = query(vertex_state, **info.args)
         table = build_vertex_table(builder, info.docname, vertex_state, vertices)
         node.replace_self(table)
 
 
 def build_table(
-    headers: list[str], items: list[dict[str, nodes.paragraph]]
+    headers: list[str],
+    items: list[dict[str, nodes.paragraph]],
 ) -> nodes.table:
     """Construct a docutils nodes.table from a header and a list of dicts.
 
     Args:
         headers: a list of column headers, in order
         items: the rows of the table. The keys should match the headers. Missing keys
             are represented using an empty cell.
@@ -99,19 +107,22 @@
     tgroup += thead
     tgroup += tbody
 
     return table
 
 
 def build_vertex_table(
-    builder: Builder, docname: str, state: vertex.State, vertices: Iterable[str]
+    builder: Builder,
+    docname: str,
+    state: vertex.State,
+    vertices: Iterable[str],
 ) -> nodes.table:
     """Construct a table from a list of vertices."""
     headers = ["uid", "tags", "parents", "children"]
-    items: list[dict[str, nodes.Node]] = []
+    items: list[dict[str, nodes.paragraph]] = []
     for uid in vertices:
         uid_para = nodes.paragraph()
         uid_para += vertex_reference(builder, docname, state.vertices, uid)
 
         item = {
             "uid": uid_para,
             "tags": nodes.paragraph(text=", ".join(state.vertices[uid].tags)),
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/table/info.py` & `sphinx_graph-0.2.3/src/sphinx_graph/table/info.py`

 * *Files identical despite different names*

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/table/state.py` & `sphinx_graph-0.2.3/src/sphinx_graph/table/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Shared state for the sphinx-graph extension."""
 
 from __future__ import annotations
 
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Iterator
-from uuid import UUID
+from typing import TYPE_CHECKING
 
-from sphinx.environment import BuildEnvironment
 from sphinx.util import logging
 
-from sphinx_graph import table
-from sphinx_graph.table.info import Info
 from sphinx_graph.vertex.state import DuplicateIdError
 
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+    from uuid import UUID
+
+    from sphinx.environment import BuildEnvironment
+
+    from sphinx_graph import table
+    from sphinx_graph.table.info import Info
+
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "State",
 ]
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/vertex/__init__.py` & `sphinx_graph-0.2.3/src/sphinx_graph/vertex/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Types and methods specific to the vertex directive."""
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
-from sphinx_graph.vertex import events
-from sphinx_graph.vertex.config import Config
-from sphinx_graph.vertex.directive import Directive
-from sphinx_graph.vertex.info import Info
-from sphinx_graph.vertex.node import VertexNode
-from sphinx_graph.vertex.query import Query
-from sphinx_graph.vertex.state import State
+from . import events
+from .config import Config
+from .directive import Directive
+from .info import Info
+from .node import VertexNode
+from .query import Query
+from .state import State
 
 __all__ = [
     "Config",
     "Info",
-    "VertexNode",
-    "State",
     "Query",
+    "State",
+    "VertexNode",
 ]
 
 
 def visit_node(_self: nodes.GenericNodeVisitor, _node: nodes.Node) -> None:
     """Visits the Vertex node.
 
     This method is a no-op
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/vertex/config.py` & `sphinx_graph-0.2.3/src/sphinx_graph/vertex/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Vertex-specific configuration."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from re import Pattern
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from re import Pattern
 
 
 @dataclass
 class Config:
     """Optional additional configuration for a vertex directive.
 
     Args:
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/vertex/directive.py` & `sphinx_graph-0.2.3/src/sphinx_graph/vertex/directive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 """Sphinx Directive for Vertex objects."""
 
 from __future__ import annotations
 
 import base64
 import hashlib
-from typing import Sequence
+from typing import TYPE_CHECKING, ClassVar
 
 from docutils import nodes
 from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.nodes import nested_parse_with_titles
-from sphinx.util.typing import OptionSpec
 
 from sphinx_graph import parse
-from sphinx_graph.config import Config
+from sphinx_graph.vertex import state
 from sphinx_graph.vertex.config import Config as VertexConfig
 from sphinx_graph.vertex.info import Info
 from sphinx_graph.vertex.node import VertexNode
-from sphinx_graph.vertex.state import State
+
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+    from sphinx.util.typing import OptionSpec
+
+    from sphinx_graph.config import Config
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "Directive",
 ]
 
 
 class Directive(SphinxDirective):
     """An RST node representing a To-Do item."""
 
     has_content = True
     required_arguments = 1
-    option_spec: OptionSpec = {
+    option_spec: ClassVar[OptionSpec] = {
         "parents": parse.parents,
         "layout": parse.string,
         "require_fingerprints": parse.boolean,
         "type": parse.string,
         "tags": parse.comma_separated_list,
     }
 
     def run(self) -> Sequence[nodes.Node]:
         """Run the directive and return a Vertex node."""
         uid = self.arguments[0]
         content_node = VertexNode(graph_uid=uid)
         nested_parse_with_titles(self.state, self.content, content_node)
 
         fingerprint = base64.b64encode(
-            hashlib.md5(content_node.astext().encode()).digest()  # noqa: S324
+            hashlib.md5(content_node.astext().encode()).digest(),  # noqa: S324
         )[:4].decode()
 
         vertex_config = self.vertex_config()
         if vertex_config.regex and not vertex_config.regex.match(uid):
             logger.error(
-                (
-                    f"vertex '{uid}' doesn't satisfy the configured regex"
-                    f" ('{vertex_config.regex.pattern}')"
-                ),
+                f"vertex '{uid}' doesn't satisfy the configured regex"
+                f" ('{vertex_config.regex.pattern}')",
                 location=(self.env.docname, self.lineno),
             )
 
-        with State.get(self.env) as state:
-            state.insert(
-                uid,
-                Info(
-                    docname=self.env.docname,
-                    config=vertex_config,
-                    parents=self.options.get("parents", {}),
-                    fingerprint=fingerprint,
-                    tags=self.options.get("tags", []),
-                ),
-            )
+        state.insert_vertex(
+            self.env,
+            uid,
+            Info(
+                docname=self.env.docname,
+                config=vertex_config,
+                parents=self.options.get("parents", {}),
+                fingerprint=fingerprint,
+                tags=self.options.get("tags", []),
+            ),
+        )
 
         targetnode = nodes.target("", "", ids=[uid])
 
         return [targetnode, content_node]
 
     def _default_config(self) -> VertexConfig:
         """The global default vertex configuration."""
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/vertex/events.py` & `sphinx_graph-0.2.3/src/sphinx_graph/vertex/events.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Lifecycle events specific to the Vertex node."""
 
 from __future__ import annotations
 
-from typing import Iterable
+from typing import TYPE_CHECKING
 
 from docutils import nodes
-from sphinx.application import Sphinx
-from sphinx.builders import Builder
-from sphinx.environment import BuildEnvironment
 
 from sphinx_graph.vertex import layout
 from sphinx_graph.vertex.info import Info, InfoParsed
 from sphinx_graph.vertex.node import VertexNode
-from sphinx_graph.vertex.state import State
+from sphinx_graph.vertex.state import build_and_check_graph
+from sphinx_graph.vertex.state import merge as state_merge
+from sphinx_graph.vertex.state import purge as state_purge
+
+if TYPE_CHECKING:
+    from collections.abc import Iterable, Mapping
+
+    from sphinx.application import Sphinx
+    from sphinx.builders import Builder
 
 
 def vertex_reference(
     builder: Builder,
     from_docname: str,
-    vertices: dict[str, Info],
+    vertices: Mapping[str, Info],
     target_uid: str,
 ) -> nodes.reference:
     """Construct a reference to a vertex.
 
     Args:
         builder: The current sphinx 'builder'
         from_docname: The name of the document where the reference is located (the
@@ -39,71 +44,48 @@
     reference.append(nodes.Text(target_uid))
     return reference
 
 
 def relative_uris(
     builder: Builder,
     from_docname: str,
-    vertices: dict[str, Info],
+    vertices: Mapping[str, Info],
     target_uids: Iterable[str],
 ) -> Iterable[nodes.reference]:
     """Iterate over node UIDs and convert them to relative URIs."""
     return (
         vertex_reference(builder, from_docname, vertices, target_uid)
         for target_uid in target_uids
     )
 
 
 def process(app: Sphinx, doctree: nodes.document, _fromdocname: str) -> None:
     """Process Vertex nodes by formatting and adding links to graph neighbours."""
     builder = app.builder
-    with State.get(app.env) as state:
-        state.build_and_check_graph()
-        for vertex_node in doctree.findall(VertexNode):
-            uid = vertex_node["graph_uid"]
-            info = state.vertices[uid]
-            [parents, children] = [
-                relative_uris(builder, info.docname, state.vertices, uids)
-                for uids in [info.parents.keys(), state.graph.successors(uid)]
-            ]
-            parsed_info = InfoParsed(
-                content=vertex_node.deepcopy(),
-                parents=parents,
-                children=children,
-                tags=info.tags,
-            )
-            vertex_node.replace_self(
-                layout.apply_formatting(
-                    uid,
-                    parsed_info,
-                    info.config.layout,
-                )
-            )
-
-
-def purge(_app: Sphinx, env: BuildEnvironment, docname: str) -> None:
-    """Clear out all stale vertices.
-
-    All vertices whose docname matches the given one from the graph_all_vertices list
-    will be removed.
-
-    If there are vertices left in the document, they will be added again during parsing.
-    """
-    with State.get(env) as state:
-        state.vertices = {
-            uid: vert for uid, vert in state.vertices.items() if vert.docname != docname
-        }
-
-
-def merge(
-    _app: Sphinx, env: BuildEnvironment, _docnames: list[str], other: BuildEnvironment
-) -> None:
-    """Merge the vertices from multiple environments during parallel builds."""
-    with State.get(env) as state, State.get(other) as other_state:
-        state.vertices.update(other_state.vertices)
+    state = build_and_check_graph(app.env)
+    for vertex_node in doctree.findall(VertexNode):
+        uid = vertex_node["graph_uid"]
+        info = state.vertices[uid]
+        [parents, children] = [
+            relative_uris(builder, info.docname, state.vertices, uids)
+            for uids in [info.parents.keys(), state.children(uid)]
+        ]
+        parsed_info = InfoParsed(
+            content=vertex_node.deepcopy(),
+            parents=parents,
+            children=children,
+            tags=info.tags,
+        )
+        vertex_node.replace_self(
+            layout.apply_formatting(
+                uid,
+                parsed_info,
+                info.config.layout,
+            ),
+        )
 
 
 def register(app: Sphinx) -> None:
     """Register the vertex directive lifecycle events."""
+    app.connect("env-purge-doc", state_purge)
+    app.connect("env-merge-info", state_merge)
     app.connect("doctree-resolved", process)
-    app.connect("env-purge-doc", purge)
-    app.connect("env-merge-info", merge)
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/vertex/info.py` & `sphinx_graph-0.2.3/src/sphinx_graph/vertex/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Dataclass objects will store information about a Vertex directive."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Iterable
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from collections.abc import Iterable
 
-from docutils import nodes
+    from docutils import nodes
 
-from sphinx_graph.vertex.config import Config
+    from sphinx_graph.vertex.config import Config
 
 
 @dataclass
 class Info:
     """Vertex information dataclass.
 
     Args:
```

### Comparing `sphinx_graph-0.2.2/src/sphinx_graph/vertex/layout.py` & `sphinx_graph-0.2.3/src/sphinx_graph/vertex/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Tools and methods for formatting vertex nodes into docutils nodes."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Callable, Iterable, TypeVar
+from typing import TYPE_CHECKING, Callable, TypeVar
 
 from docutils import nodes
 from sphinx.util import logging
 
 from sphinx_graph.format import comma_separated_list
-from sphinx_graph.vertex.info import InfoParsed
+
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from sphinx_graph.vertex.info import InfoParsed
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
+    "DEFAULT",
+    "LAYOUTS",
     "FormatHelper",
     "Formatter",
-    "LAYOUTS",
-    "DEFAULT",
 ]
 
 DEFAULT = "subtle"
 
 
 T = TypeVar("T")
 
@@ -34,39 +38,41 @@
         uid: the unique identifier of the vertex
         info: vertex information
     """
 
     uid: str
     info: InfoParsed
 
-    def _list(self, references: Iterable[nodes.reference]) -> nodes.line | None:
-        refs = list(comma_separated_list(references))
-        if not refs:
-            return None
-
-        line = nodes.line()
-        line.extend(refs)
-
-        return line
-
     def child_list(self) -> nodes.line | None:
         """Format the list of child vertex references as a comma-separated list.
 
         Args:
             prefix: Optionally set a prefix for the list
         """
-        return self._list(self.info.children)
+        return _list(self.info.children)
 
     def parent_list(self) -> nodes.line | None:
         """Format the list of parent vertex references as a comma-separated list.
 
         Args:
             prefix: Optionally set a prefix for the list
         """
-        return self._list(self.info.parents)
+        return _list(self.info.parents)
+
+
+def _list(references: Iterable[nodes.reference]) -> nodes.line | None:
+    """Format nodes as a comma-separated list."""
+    refs = list(comma_separated_list(references))
+    if not refs:
+        return None
+
+    line = nodes.line()
+    line.extend(refs)
+
+    return line
 
 
 def transparent(helper: FormatHelper) -> nodes.Node:
     """Format a vertex Node as a docutils node."""
     return helper.info.content
 
 
@@ -89,23 +95,23 @@
     if children:
         one_liner += nodes.Text(" | Children: ")
         one_liner.extend(children)
 
     if helper.info.tags:
         one_liner += nodes.Text(" | Tags: ")
         one_liner.extend(
-            comma_separated_list(nodes.Text(tag) for tag in helper.info.tags)
+            comma_separated_list(nodes.Text(tag) for tag in helper.info.tags),
         )
 
     paragraph = nodes.paragraph()
     paragraph.append(one_liner)
 
     paragraph.append(helper.info.content)
 
-    return paragraph  # type: ignore[no-any-return]
+    return paragraph
 
 
 Formatter = Callable[[FormatHelper], nodes.Node]
 
 
 LAYOUTS: dict[str, Formatter] = {
     "transparent": transparent,
@@ -120,13 +126,13 @@
 ) -> nodes.Node:
     """Apply a given layout to a Vertex node."""
     if layout is None:
         layout = DEFAULT
     elif layout not in LAYOUTS:
         logger.error(
             f"vertex {uid} has unknown layout '{layout}'. Defaulting to '{DEFAULT}'"
-            " layout."
+            " layout.",
         )
         layout = DEFAULT
     helper = FormatHelper(uid, info)
     formatter = LAYOUTS[layout]
     return formatter(helper)
```

### Comparing `sphinx_graph-0.2.2/PKG-INFO` & `sphinx_graph-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: sphinx-graph
-Version: 0.2.2
+Version: 0.2.3
 Summary: 'Sphinx-Graph' is a plain-text, VCS-friendly, requirements management tool.
 Home-page: https://github.com/danieleades/sphinx-graph
 License: MIT
 Keywords: sphinx, requirements,documentation,plain-text
 Author: Daniel Eades
 Author-email: danieleades@hotmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
-Requires-Dist: networkx (>=3.0,<4.0)
-Requires-Dist: sphinx (>=6.1.3,<7.0.0)
+Requires-Dist: rustworkx (>=0.14.0,<0.15.0)
+Requires-Dist: sphinx (>=6,<8)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://sphinx-graph.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 
 # Sphinx Graph
 
 [![codecov](https://codecov.io/gh/danieleades/sphinx-graph/branch/main/graph/badge.svg?token=WLPNTQXHrK)](https://codecov.io/gh/danieleades/sphinx-graph)
@@ -79,15 +75,15 @@
    of its parent.
 
    The fingerprint is a 4-character hash. If USR-001 is modified, then SYS-002 will fail the build
    until the fingerprint is updated (the build error provides the new fingerprint). This means that
    changing a Vertex will trigger a review of all dependent vertices.
 ```
 
-For more information, see [the docs](https://sphinx-graph.readthedocs.io/en/main/src/index.html).
+For more information, see [the docs](https://sphinx-graph.readthedocs.io/en/main/).
 
 or, build the local docs-
 
       cd docs
       poetry run make html
 
 ---
```

