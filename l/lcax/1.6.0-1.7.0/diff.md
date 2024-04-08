# Comparing `tmp/lcax-1.6.0.tar.gz` & `tmp/lcax-1.7.0.tar.gz`

## Comparing `lcax-1.6.0.tar` & `lcax-1.7.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0     1224 1970-01-01 00:00:00.000000 lcax-1.6.0/Cargo.toml
--rw-r--r--   0     1001      127       11 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/CODEOWNERS
--rw-r--r--   0     1001      127       64 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127      845 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/build_csharp.yaml
--rw-r--r--   0     1001      127      843 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/build_javascript.yaml
--rw-r--r--   0     1001      127     1171 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/build_python.yaml
--rw-r--r--   0     1001      127      659 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/build_rust.yaml
--rw-r--r--   0     1001      127     1849 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/cicd.yaml
--rw-r--r--   0     1001      127     2550 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/create_release.yaml
--rw-r--r--   0     1001      127     1175 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/publish_csharp.yaml
--rw-r--r--   0     1001      127      881 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/publish_javascript.yaml
--rw-r--r--   0     1001      127     1089 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/publish_python.yaml
--rw-r--r--   0     1001      127     2083 2024-03-26 14:53:06.000000 lcax-1.6.0/.github/workflows/release_docs.yaml
--rw-r--r--   0     1001      127     3433 2024-03-26 14:53:06.000000 lcax-1.6.0/.gitignore
--rw-r--r--   0     1001      127      886 2024-03-26 14:53:06.000000 lcax-1.6.0/.releaserc.yaml
--rw-r--r--   0     1001      127     4119 2024-03-26 14:53:06.000000 lcax-1.6.0/CHANGELOG.md
--rw-r--r--   0     1001      127      560 2024-03-26 14:53:06.000000 lcax-1.6.0/COPYRIGHT
--rw-r--r--   0     1001      127    21165 2024-03-26 14:53:07.000000 lcax-1.6.0/Cargo.lock
--rw-r--r--   0     1001      127    10173 2024-03-26 14:53:06.000000 lcax-1.6.0/LICENSE
--rw-r--r--   0     1001      127     1555 2024-03-26 14:53:06.000000 lcax-1.6.0/README.md
--rw-r--r--   0     1001      127       79 2024-03-26 14:53:06.000000 lcax-1.6.0/codegen.template.json
--rw-r--r--   0     1001      127     2238 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/CHANGELOG.md
--rw-r--r--   0     1001      127    45567 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/assets/benchmark.png
--rw-r--r--   0     1001      127    23752 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/assets/epdx.png
--rw-r--r--   0     1001      127   253397 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/assets/lcax_structure.png
--rw-r--r--   0     1001      127    13935 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/code/data/lcabyg_project.json
--rw-r--r--   0     1001      127      259 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/code/javascript/usage.js
--rw-r--r--   0     1001      127      527 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/code/python/usage.py
--rw-r--r--   0     1001      127     1341 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/data_structure.md
--rw-r--r--   0     1001      127    16059 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/examples/basic_project.json
--rw-r--r--   0     1001      127      127 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/examples.md
--rw-r--r--   0     1001      127     2104 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/index.md
--rw-r--r--   0     1001      127      122 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/overrides/partials/integrations/analytics/custom.html
--rw-r--r--   0     1001      127      418 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/overrides/stylesheets/extra.css
--rw-r--r--   0     1001      127        0 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/schemas/.gitkeep
--rw-r--r--   0     1001      127      692 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/schemas.md
--rw-r--r--   0     1001      127      157 2024-03-26 14:53:06.000000 lcax-1.6.0/docs/usage.md
--rw-r--r--   0     1001      127     1118 2024-03-26 14:53:06.000000 lcax-1.6.0/mkdocs.yml
--rw-r--r--   0     1001      127     6280 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/csharp/lcax/lcax.cs
--rw-r--r--   0     1001      127      705 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/csharp/lcax/lcax.csproj
--rw-r--r--   0     1001      127    10173 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/LICENSE
--rw-r--r--   0     1001      127     1485 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/README.md
--rw-r--r--   0     1001      127    50825 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/package-lock.json
--rw-r--r--   0     1001      127      753 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/package.json
--rw-r--r--   0     1001      127     3983 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/src/lcax.d.ts
--rw-r--r--   0     1001      127      139 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/src/lcax.js
--rw-r--r--   0     1001      127     4563 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/src/lcax_bg.js
--rw-r--r--   0     1001      127   345131 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/src/lcax_bg.wasm
--rw-r--r--   0     1001      127      451 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/src/lcax_bg.wasm.d.ts
--rw-r--r--   0     1001      127      516 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/tests/convertLCAbyg.spec.tsx
--rw-r--r--   0     1001      127    13935 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/tests/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127      222 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/javascript/vitest.config.js
--rw-r--r--   0     1001      127     1131 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      127      149 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/python/src/lcax/lcax.pyi
--rw-r--r--   0     1001      127    17703 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/python/src/lcax/lcax.schema.json
--rw-r--r--   0     1001      127    10294 2024-03-26 14:53:07.000000 lcax-1.6.0/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      127    13935 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/python/tests/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127      671 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/python/tests/test_lcabyg.py
--rw-r--r--   0     1001      127      544 2024-03-26 14:53:06.000000 lcax-1.6.0/packages/python/tests/test_lcax.py
--rw-r--r--   0     1001      127      687 2024-03-26 14:53:06.000000 lcax-1.6.0/src/javascript.rs
--rw-r--r--   0     1001      127     4042 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lcabyg/categories.rs
--rw-r--r--   0     1001      127     2045 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lcabyg/edges.rs
--rw-r--r--   0     1001      127       66 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lcabyg/mod.rs
--rw-r--r--   0     1001      127     4004 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lcabyg/nodes.rs
--rw-r--r--   0     1001      127    12422 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lcabyg/parse.rs
--rw-r--r--   0     1001      127     1788 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lcabyg/results.rs
--rw-r--r--   0     1001      127      448 2024-03-26 14:53:06.000000 lcax-1.6.0/src/lib.rs
--rw-r--r--   0     1001      127    10180 2024-03-26 14:53:06.000000 lcax-1.6.0/src/project.rs
--rw-r--r--   0     1001      127      804 2024-03-26 14:53:06.000000 lcax-1.6.0/src/python.rs
--rw-r--r--   0     1001      127      200 2024-03-26 14:53:06.000000 lcax-1.6.0/src/schemars.rs
--rw-r--r--   0     1001      127      686 2024-03-26 14:53:06.000000 lcax-1.6.0/src/utils.rs
--rw-r--r--   0     1001      127    25028 2024-03-26 14:53:06.000000 lcax-1.6.0/tests/datafixtures/lcabyg_example_project.json
--rw-r--r--   0     1001      127  2051524 2024-03-26 14:53:06.000000 lcax-1.6.0/tests/datafixtures/lcabyg_example_results.json
--rw-r--r--   0     1001      127    13935 2024-03-26 14:53:06.000000 lcax-1.6.0/tests/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127     1024 2024-03-26 14:53:06.000000 lcax-1.6.0/tests/test_lcax.rs
--rw-r--r--   0     1001      127     2383 2024-03-26 14:53:06.000000 lcax-1.6.0/tests/test_parse_lcabyg.rs
--rw-r--r--   0     1001      127     1311 2024-03-26 14:53:06.000000 lcax-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 lcax-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 lcax-1.7.0/Cargo.toml
+-rw-r--r--   0     1001      127       11 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/CODEOWNERS
+-rw-r--r--   0     1001      127       64 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      845 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_csharp.yaml
+-rw-r--r--   0     1001      127      843 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_javascript.yaml
+-rw-r--r--   0     1001      127     1171 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_python.yaml
+-rw-r--r--   0     1001      127      659 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/build_rust.yaml
+-rw-r--r--   0     1001      127     1849 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/cicd.yaml
+-rw-r--r--   0     1001      127     2550 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/create_release.yaml
+-rw-r--r--   0     1001      127     1175 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/publish_csharp.yaml
+-rw-r--r--   0     1001      127      881 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/publish_javascript.yaml
+-rw-r--r--   0     1001      127     1089 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/publish_python.yaml
+-rw-r--r--   0     1001      127     2083 2024-04-08 10:17:44.000000 lcax-1.7.0/.github/workflows/release_docs.yaml
+-rw-r--r--   0     1001      127     3433 2024-04-08 10:17:44.000000 lcax-1.7.0/.gitignore
+-rw-r--r--   0     1001      127      886 2024-04-08 10:17:44.000000 lcax-1.7.0/.releaserc.yaml
+-rw-r--r--   0     1001      127     4329 2024-04-08 10:17:44.000000 lcax-1.7.0/CHANGELOG.md
+-rw-r--r--   0     1001      127      560 2024-04-08 10:17:44.000000 lcax-1.7.0/COPYRIGHT
+-rw-r--r--   0     1001      127    21165 2024-04-08 10:17:44.000000 lcax-1.7.0/Cargo.lock
+-rw-r--r--   0     1001      127    10173 2024-04-08 10:17:44.000000 lcax-1.7.0/LICENSE
+-rw-r--r--   0     1001      127     1555 2024-04-08 10:17:44.000000 lcax-1.7.0/README.md
+-rw-r--r--   0     1001      127       79 2024-04-08 10:17:44.000000 lcax-1.7.0/codegen.template.json
+-rw-r--r--   0     1001      127     2238 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/CHANGELOG.md
+-rw-r--r--   0     1001      127    45567 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/assets/benchmark.png
+-rw-r--r--   0     1001      127    23752 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/assets/epdx.png
+-rw-r--r--   0     1001      127   253397 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/assets/lcax_structure.png
+-rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/code/data/lcabyg_project.json
+-rw-r--r--   0     1001      127      259 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/code/javascript/usage.js
+-rw-r--r--   0     1001      127      527 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/code/python/usage.py
+-rw-r--r--   0     1001      127     1341 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/data_structure.md
+-rw-r--r--   0     1001      127    16059 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/examples/basic_project.json
+-rw-r--r--   0     1001      127      127 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/examples.md
+-rw-r--r--   0     1001      127     2104 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/index.md
+-rw-r--r--   0     1001      127      122 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/overrides/partials/integrations/analytics/custom.html
+-rw-r--r--   0     1001      127      418 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/overrides/stylesheets/extra.css
+-rw-r--r--   0     1001      127        0 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/schemas/.gitkeep
+-rw-r--r--   0     1001      127      692 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/schemas.md
+-rw-r--r--   0     1001      127      157 2024-04-08 10:17:44.000000 lcax-1.7.0/docs/usage.md
+-rw-r--r--   0     1001      127     1118 2024-04-08 10:17:44.000000 lcax-1.7.0/mkdocs.yml
+-rw-r--r--   0     1001      127     6280 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/csharp/lcax/lcax.cs
+-rw-r--r--   0     1001      127      705 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/csharp/lcax/lcax.csproj
+-rw-r--r--   0     1001      127    10173 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/LICENSE
+-rw-r--r--   0     1001      127     1485 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/README.md
+-rw-r--r--   0     1001      127    50825 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/package-lock.json
+-rw-r--r--   0     1001      127      753 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/package.json
+-rw-r--r--   0     1001      127     3983 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax.d.ts
+-rw-r--r--   0     1001      127      139 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax.js
+-rw-r--r--   0     1001      127     4563 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax_bg.js
+-rw-r--r--   0     1001      127   345131 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax_bg.wasm
+-rw-r--r--   0     1001      127      451 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/src/lcax_bg.wasm.d.ts
+-rw-r--r--   0     1001      127      516 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/tests/convertLCAbyg.spec.tsx
+-rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/tests/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127      222 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/javascript/vitest.config.js
+-rw-r--r--   0     1001      127     1131 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      127      149 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/src/lcax/lcax.pyi
+-rw-r--r--   0     1001      127    17703 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/src/lcax/lcax.schema.json
+-rw-r--r--   0     1001      127    15367 2024-04-08 10:17:45.000000 lcax-1.7.0/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/tests/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127      671 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/tests/test_lcabyg.py
+-rw-r--r--   0     1001      127      545 2024-04-08 10:17:44.000000 lcax-1.7.0/packages/python/tests/test_lcax.py
+-rw-r--r--   0     1001      127     2431 2024-04-08 10:17:44.000000 lcax-1.7.0/src/country.rs
+-rw-r--r--   0     1001      127      687 2024-04-08 10:17:44.000000 lcax-1.7.0/src/javascript.rs
+-rw-r--r--   0     1001      127     4042 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/categories.rs
+-rw-r--r--   0     1001      127     2045 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/edges.rs
+-rw-r--r--   0     1001      127       66 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/mod.rs
+-rw-r--r--   0     1001      127     4004 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/nodes.rs
+-rw-r--r--   0     1001      127    12863 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/parse.rs
+-rw-r--r--   0     1001      127     1788 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lcabyg/results.rs
+-rw-r--r--   0     1001      127      465 2024-04-08 10:17:44.000000 lcax-1.7.0/src/lib.rs
+-rw-r--r--   0     1001      127    11588 2024-04-08 10:17:44.000000 lcax-1.7.0/src/project.rs
+-rw-r--r--   0     1001      127      804 2024-04-08 10:17:44.000000 lcax-1.7.0/src/python.rs
+-rw-r--r--   0     1001      127      200 2024-04-08 10:17:44.000000 lcax-1.7.0/src/schemars.rs
+-rw-r--r--   0     1001      127      686 2024-04-08 10:17:44.000000 lcax-1.7.0/src/utils.rs
+-rw-r--r--   0     1001      127    25028 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/datafixtures/lcabyg_example_project.json
+-rw-r--r--   0     1001      127  2051524 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/datafixtures/lcabyg_example_results.json
+-rw-r--r--   0     1001      127    13935 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127     1047 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/test_lcax.rs
+-rw-r--r--   0     1001      127     2383 2024-04-08 10:17:44.000000 lcax-1.7.0/tests/test_parse_lcabyg.rs
+-rw-r--r--   0     1001      127     1311 2024-04-08 10:17:44.000000 lcax-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 lcax-1.7.0/PKG-INFO
```

### Comparing `lcax-1.6.0/Cargo.toml` & `lcax-1.7.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "lcax"
 description = "LCAx is an open, machine and human-readable data format for exchanging LCA results."
-version = "1.6.0"
+version = "1.7.0"
 authors = ["Christian Kongsgaard <christian@kongsgaard.eu>"]
 edition = "2018"
 readme = "README.md"
 license-file = "LICENSE"
 homepage = "https://lcax.kongsgaard.eu"
 documentation = "https://lcax.kongsgaard.eu"
 repository = "https://github.com/ocni-dtu/lcax"
@@ -26,15 +26,14 @@
 jsbindings = ["wasm-bindgen", "console_error_panic_hook", "tsify"]
 
 [dependencies]
 schemars = { version = "0.8.12", features = ["chrono"] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 epdx = "1.2.0"
-
 pkg-version = "1.0.0"
 field_access = "0.1.4"
 
 # Python Bindings
 pyo3 = { version = "0.20.2", features = ["abi3-py310"], optional = true }
 
 # JS Bindings
```

### Comparing `lcax-1.6.0/.github/workflows/build_csharp.yaml` & `lcax-1.7.0/.github/workflows/build_csharp.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/build_javascript.yaml` & `lcax-1.7.0/.github/workflows/build_javascript.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/build_python.yaml` & `lcax-1.7.0/.github/workflows/build_python.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/build_rust.yaml` & `lcax-1.7.0/.github/workflows/build_rust.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/cicd.yaml` & `lcax-1.7.0/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/create_release.yaml` & `lcax-1.7.0/.github/workflows/create_release.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/publish_csharp.yaml` & `lcax-1.7.0/.github/workflows/publish_csharp.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/publish_javascript.yaml` & `lcax-1.7.0/.github/workflows/publish_javascript.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/publish_python.yaml` & `lcax-1.7.0/.github/workflows/publish_python.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.github/workflows/release_docs.yaml` & `lcax-1.7.0/.github/workflows/release_docs.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.gitignore` & `lcax-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/.releaserc.yaml` & `lcax-1.7.0/.releaserc.yaml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/CHANGELOG.md` & `lcax-1.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [1.6.0](https://github.com/ocni-dtu/lcax/compare/v1.5.0...v1.6.0) (2024-03-26)
+
+
+### Features
+
+* renamed fields ([e37d35b](https://github.com/ocni-dtu/lcax/commit/e37d35bd6da80b0295d2a8f2be5ac280699aaff8))
+
 ## [1.5.0](https://github.com/ocni-dtu/lcax/compare/v1.4.2...v1.5.0) (2024-03-26)
 
 
 ### Features
 
 * added convert functions to JS and Python ([7d22438](https://github.com/ocni-dtu/lcax/commit/7d22438fa4793d67965ede591fa1613dda2ff535))
 * added support for LCAbyg result files ([0dd026f](https://github.com/ocni-dtu/lcax/commit/0dd026f08f7a3fede61b43e138e39fde1f7381aa))
```

### Comparing `lcax-1.6.0/COPYRIGHT` & `lcax-1.7.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/Cargo.lock` & `lcax-1.7.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lcax"
-version = "1.6.0"
+version = "1.7.0"
 dependencies = [
  "console_error_panic_hook",
  "epdx",
  "field_access",
  "pkg-version",
  "pyo3",
  "schemars",
@@ -203,17 +203,17 @@
  "tsify",
  "wasm-bindgen",
  "wee_alloc",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.147"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
```

### Comparing `lcax-1.6.0/LICENSE` & `lcax-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/README.md` & `lcax-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/CHANGELOG.md` & `lcax-1.7.0/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/assets/benchmark.png` & `lcax-1.7.0/docs/assets/benchmark.png`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/assets/epdx.png` & `lcax-1.7.0/docs/assets/epdx.png`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/assets/lcax_structure.png` & `lcax-1.7.0/docs/assets/lcax_structure.png`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/code/data/lcabyg_project.json` & `lcax-1.7.0/docs/code/data/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/code/python/usage.py` & `lcax-1.7.0/docs/code/python/usage.py`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/data_structure.md` & `lcax-1.7.0/docs/data_structure.md`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/examples/basic_project.json` & `lcax-1.7.0/docs/examples/basic_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/index.md` & `lcax-1.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/docs/schemas.md` & `lcax-1.7.0/docs/schemas.md`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/mkdocs.yml` & `lcax-1.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/csharp/lcax/lcax.cs` & `lcax-1.7.0/packages/csharp/lcax/lcax.cs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/csharp/lcax/lcax.csproj` & `lcax-1.7.0/packages/csharp/lcax/lcax.csproj`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/LICENSE` & `lcax-1.7.0/packages/javascript/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/README.md` & `lcax-1.7.0/packages/javascript/README.md`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/package-lock.json` & `lcax-1.7.0/packages/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/package.json` & `lcax-1.7.0/packages/javascript/package.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/src/lcax.d.ts` & `lcax-1.7.0/packages/javascript/src/lcax.d.ts`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/src/lcax_bg.js` & `lcax-1.7.0/packages/javascript/src/lcax_bg.js`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/src/lcax_bg.wasm` & `lcax-1.7.0/packages/javascript/src/lcax_bg.wasm`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/tests/convertLCAbyg.spec.tsx` & `lcax-1.7.0/packages/javascript/tests/convertLCAbyg.spec.tsx`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/javascript/tests/datafixtures/lcabyg_project.json` & `lcax-1.7.0/packages/javascript/tests/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/python/src/lcax/__init__.py` & `lcax-1.7.0/packages/python/src/lcax/__init__.py`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/python/src/lcax/lcax.schema.json` & `lcax-1.7.0/packages/python/src/lcax/lcax.schema.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/python/src/lcax/pydantic.py` & `lcax-1.7.0/packages/python/src/lcax/pydantic.py`

 * *Files 27% similar despite different names*

```diff
@@ -46,23 +46,282 @@
         allow_population_by_field_name = True
 
     code: str
     name: str
     system: str
 
 
+class Country(Enum):
+    afg = 'afg'
+    ala = 'ala'
+    alb = 'alb'
+    dza = 'dza'
+    asm = 'asm'
+    and_ = 'and'
+    ago = 'ago'
+    aia = 'aia'
+    ata = 'ata'
+    atg = 'atg'
+    arg = 'arg'
+    arm = 'arm'
+    abw = 'abw'
+    aus = 'aus'
+    aut = 'aut'
+    aze = 'aze'
+    bhs = 'bhs'
+    bhr = 'bhr'
+    bgd = 'bgd'
+    brb = 'brb'
+    blr = 'blr'
+    bel = 'bel'
+    blz = 'blz'
+    ben = 'ben'
+    bmu = 'bmu'
+    btn = 'btn'
+    bol = 'bol'
+    bes = 'bes'
+    bih = 'bih'
+    bwa = 'bwa'
+    bvt = 'bvt'
+    bra = 'bra'
+    iot = 'iot'
+    brn = 'brn'
+    bgr = 'bgr'
+    bfa = 'bfa'
+    bdi = 'bdi'
+    cpv = 'cpv'
+    khm = 'khm'
+    cmr = 'cmr'
+    can = 'can'
+    cym = 'cym'
+    caf = 'caf'
+    tcd = 'tcd'
+    chl = 'chl'
+    chn = 'chn'
+    cxr = 'cxr'
+    cck = 'cck'
+    col = 'col'
+    com = 'com'
+    cog = 'cog'
+    cod = 'cod'
+    cok = 'cok'
+    cri = 'cri'
+    civ = 'civ'
+    hrv = 'hrv'
+    cub = 'cub'
+    cuw = 'cuw'
+    cyp = 'cyp'
+    cze = 'cze'
+    dnk = 'dnk'
+    dji = 'dji'
+    dma = 'dma'
+    dom = 'dom'
+    ecu = 'ecu'
+    egy = 'egy'
+    slv = 'slv'
+    gnq = 'gnq'
+    eri = 'eri'
+    est = 'est'
+    swz = 'swz'
+    eth = 'eth'
+    flk = 'flk'
+    fro = 'fro'
+    fji = 'fji'
+    fin = 'fin'
+    fra = 'fra'
+    guf = 'guf'
+    pyf = 'pyf'
+    atf = 'atf'
+    gab = 'gab'
+    gmb = 'gmb'
+    geo = 'geo'
+    deu = 'deu'
+    gha = 'gha'
+    gib = 'gib'
+    grc = 'grc'
+    grl = 'grl'
+    grd = 'grd'
+    glp = 'glp'
+    gum = 'gum'
+    gtm = 'gtm'
+    ggy = 'ggy'
+    gin = 'gin'
+    gnb = 'gnb'
+    guy = 'guy'
+    hti = 'hti'
+    hmd = 'hmd'
+    vat = 'vat'
+    hnd = 'hnd'
+    hkg = 'hkg'
+    hun = 'hun'
+    isl = 'isl'
+    ind = 'ind'
+    idn = 'idn'
+    irn = 'irn'
+    irq = 'irq'
+    irl = 'irl'
+    imn = 'imn'
+    isr = 'isr'
+    ita = 'ita'
+    jam = 'jam'
+    jpn = 'jpn'
+    jey = 'jey'
+    jor = 'jor'
+    kaz = 'kaz'
+    ken = 'ken'
+    kir = 'kir'
+    prk = 'prk'
+    kor = 'kor'
+    kwt = 'kwt'
+    kgz = 'kgz'
+    lao = 'lao'
+    lva = 'lva'
+    lbn = 'lbn'
+    lso = 'lso'
+    lbr = 'lbr'
+    lby = 'lby'
+    lie = 'lie'
+    ltu = 'ltu'
+    lux = 'lux'
+    mac = 'mac'
+    mdg = 'mdg'
+    mwi = 'mwi'
+    mys = 'mys'
+    mdv = 'mdv'
+    mli = 'mli'
+    mlt = 'mlt'
+    mhl = 'mhl'
+    mtq = 'mtq'
+    mrt = 'mrt'
+    mus = 'mus'
+    myt = 'myt'
+    mex = 'mex'
+    fsm = 'fsm'
+    mda = 'mda'
+    mco = 'mco'
+    mng = 'mng'
+    mne = 'mne'
+    msr = 'msr'
+    mar = 'mar'
+    moz = 'moz'
+    mmr = 'mmr'
+    nam = 'nam'
+    nru = 'nru'
+    npl = 'npl'
+    nld = 'nld'
+    ncl = 'ncl'
+    nzl = 'nzl'
+    nic = 'nic'
+    ner = 'ner'
+    nga = 'nga'
+    niu = 'niu'
+    nfk = 'nfk'
+    mkd = 'mkd'
+    mnp = 'mnp'
+    nor = 'nor'
+    omn = 'omn'
+    pak = 'pak'
+    plw = 'plw'
+    pse = 'pse'
+    pan = 'pan'
+    png = 'png'
+    pry = 'pry'
+    per = 'per'
+    phl = 'phl'
+    pcn = 'pcn'
+    pol = 'pol'
+    prt = 'prt'
+    pri = 'pri'
+    qat = 'qat'
+    reu = 'reu'
+    rou = 'rou'
+    rus = 'rus'
+    rwa = 'rwa'
+    blm = 'blm'
+    shn = 'shn'
+    kna = 'kna'
+    lca = 'lca'
+    maf = 'maf'
+    spm = 'spm'
+    vct = 'vct'
+    wsm = 'wsm'
+    smr = 'smr'
+    stp = 'stp'
+    sau = 'sau'
+    sen = 'sen'
+    srb = 'srb'
+    syc = 'syc'
+    sle = 'sle'
+    sgp = 'sgp'
+    sxm = 'sxm'
+    svk = 'svk'
+    svn = 'svn'
+    slb = 'slb'
+    som = 'som'
+    zaf = 'zaf'
+    sgs = 'sgs'
+    ssd = 'ssd'
+    esp = 'esp'
+    lka = 'lka'
+    sdn = 'sdn'
+    sur = 'sur'
+    sjm = 'sjm'
+    swe = 'swe'
+    che = 'che'
+    syr = 'syr'
+    twn = 'twn'
+    tjk = 'tjk'
+    tza = 'tza'
+    tha = 'tha'
+    tls = 'tls'
+    tgo = 'tgo'
+    tkl = 'tkl'
+    ton = 'ton'
+    tto = 'tto'
+    tun = 'tun'
+    tur = 'tur'
+    tkm = 'tkm'
+    tca = 'tca'
+    tuv = 'tuv'
+    uga = 'uga'
+    ukr = 'ukr'
+    are = 'are'
+    gbr = 'gbr'
+    usa = 'usa'
+    umi = 'umi'
+    ury = 'ury'
+    uzb = 'uzb'
+    vut = 'vut'
+    ven = 'ven'
+    vnm = 'vnm'
+    vgb = 'vgb'
+    vir = 'vir'
+    wlf = 'wlf'
+    esh = 'esh'
+    yem = 'yem'
+    zmb = 'zmb'
+    zwe = 'zwe'
+
+
 class ExternalImpactData(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
     format: str
     url: str
     version: Optional[str] = None
 
 
+class GeneralEnergyClass(Enum):
+    existing = 'existing'
+    standard = 'standard'
+    advanced = 'advanced'
+    unknown = 'unknown'
+
+
 class ImpactCategory(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
     a1a3: Optional[float] = None
     a4: Optional[float] = None
     a5: Optional[float] = None
@@ -143,15 +402,15 @@
 
 class Location(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
     address: Optional[str] = None
     city: Optional[str] = None
-    country: str
+    country: Country
 
 
 class ProjectInfo2(BaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -161,14 +420,22 @@
 class ProjectPhase(Enum):
     design = 'design'
     ongoing = 'ongoing'
     built = 'built'
     other = 'other'
 
 
+class RoofType(Enum):
+    flat = 'flat'
+    pitched = 'pitched'
+    saddle = 'saddle'
+    pyramid = 'pyramid'
+    other = 'other'
+
+
 class SoftwareInfo(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
     calculation_type: Optional[str] = Field(None, alias='calculationType')
     goal_and_scope_definition: Optional[str] = Field(
         None, alias='goalAndScopeDefinition'
@@ -207,39 +474,66 @@
     l = 'L'
     m2_r1 = 'M2R1'
     km = 'KM'
     tones_km = 'TONES_KM'
     unknown = 'UNKNOWN'
 
 
+class ValueUnit(BaseModel):
+    class Config:
+        allow_population_by_field_name = True
+
+    unit: Unit
+    value: float
+
+
+class AreaType(BaseModel):
+    class Config:
+        allow_population_by_field_name = True
+
+    definition: str
+    unit: Unit
+    value: float
+
+
 class BuildingInfo(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    building_completion_year: int = Field(..., alias='buildingCompletionYear', ge=0)
-    building_mass: str = Field(..., alias='buildingMass')
+    building_completion_year: Optional[int] = Field(
+        None, alias='buildingCompletionYear', ge=0
+    )
+    building_footprint: Optional[ValueUnit] = Field(None, alias='buildingFootprint')
+    building_height: Optional[ValueUnit] = Field(None, alias='buildingHeight')
+    building_mass: Optional[ValueUnit] = Field(None, alias='buildingMass')
     building_model_scope: Optional[BuildingModelScope] = Field(
         None, alias='buildingModelScope'
     )
+    building_permit_year: Optional[int] = Field(None, alias='buildingPermitYear', ge=0)
     building_type: BuildingType = Field(..., alias='buildingType')
     building_typology: BuildingTypology = Field(..., alias='buildingTypology')
-    certifications: str
-    energy_class: str = Field(..., alias='energyClass')
-    energy_demand_electricity: float = Field(..., alias='energyDemandElectricity')
-    energy_demand_heating: float = Field(..., alias='energyDemandHeating')
-    energy_supply_electricity: float = Field(..., alias='energySupplyElectricity')
-    energy_supply_heating: float = Field(..., alias='energySupplyHeating')
-    exported_electricity: float = Field(..., alias='exportedElectricity')
+    building_users: Optional[int] = Field(None, alias='buildingUsers', ge=0)
+    certifications: Optional[List[str]] = None
+    energy_demand_electricity: Optional[float] = Field(
+        None, alias='energyDemandElectricity'
+    )
+    energy_demand_heating: Optional[float] = Field(None, alias='energyDemandHeating')
+    energy_supply_electricity: Optional[float] = Field(
+        None, alias='energySupplyElectricity'
+    )
+    energy_supply_heating: Optional[float] = Field(None, alias='energySupplyHeating')
+    exported_electricity: Optional[float] = Field(None, alias='exportedElectricity')
     floors_above_ground: int = Field(..., alias='floorsAboveGround', ge=0)
-    floors_below_ground: int = Field(..., alias='floorsBelowGround', ge=0)
-    frame_type: str = Field(..., alias='frameType')
-    gross_floor_area: float = Field(..., alias='grossFloorArea')
-    gross_floor_area_definition: str = Field(..., alias='grossFloorAreaDefinition')
-    heated_floor_area: float = Field(..., alias='heatedFloorArea')
-    heated_floor_area_definition: str = Field(..., alias='heatedFloorAreaDefinition')
+    floors_below_ground: Optional[int] = Field(None, alias='floorsBelowGround', ge=0)
+    frame_type: Optional[str] = Field(None, alias='frameType')
+    general_energy_class: GeneralEnergyClass = Field(..., alias='generalEnergyClass')
+    gross_floor_area: Optional[AreaType] = Field(None, alias='grossFloorArea')
+    heated_floor_area: Optional[AreaType] = Field(None, alias='heatedFloorArea')
+    local_energy_class: Optional[str] = Field(None, alias='localEnergyClass')
+    roof_type: RoofType = Field(..., alias='roofType')
 
 
 class Conversion(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
     meta_data: str
```

### Comparing `lcax-1.6.0/packages/python/tests/datafixtures/lcabyg_project.json` & `lcax-1.7.0/packages/python/tests/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/python/tests/test_lcabyg.py` & `lcax-1.7.0/packages/python/tests/test_lcabyg.py`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/packages/python/tests/test_lcax.py` & `lcax-1.7.0/packages/python/tests/test_lcax.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 
     assert LCAxProject
 
 
 def test_lcax_project():
     from lcax import LCAxProject
 
-    project = LCAxProject(id=str(uuid.uuid4()), name='Test', description="Test Project", location={"country": "DK"},
+    project = LCAxProject(id=str(uuid.uuid4()), name='Test', description="Test Project", location={"country": "dnk"},
                           format_version=importlib.metadata.version('lcax'), life_cycle_stages=[], impact_categories=[],
                           assemblies={}, software_info={"lca_software": "LCAx"}, project_phase="other")
 
     assert project
```

### Comparing `lcax-1.6.0/src/javascript.rs` & `lcax-1.7.0/src/javascript.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/src/lcabyg/categories.rs` & `lcax-1.7.0/src/lcabyg/categories.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/src/lcabyg/edges.rs` & `lcax-1.7.0/src/lcabyg/edges.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/src/lcabyg/nodes.rs` & `lcax-1.7.0/src/lcabyg/nodes.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/src/lcabyg/parse.rs` & `lcax-1.7.0/src/lcabyg/parse.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use crate::country::Country;
 use epdx::epd::{Unit, EPD};
 use field_access::FieldAccess;
 use serde::{Deserialize, Deserializer, Serialize};
 use serde_json::Error;
 use std::collections::HashMap;
 
 use crate::lcabyg::edges::EdgeType;
@@ -168,15 +169,15 @@
 }
 
 fn add_project_data(project: &mut LCAxProject, node: &nodes::Project) {
     project.id = node.id.to_string();
     project.name = node.name.danish.clone().unwrap();
     project.description = Some(String::from(""));
     project.location = Location {
-        country: String::from("Denmark"),
+        country: Country::DNK,
         city: Some(String::from("")),
         address: Some(node.address.to_string()),
     };
     project.impact_categories = vec![
         ImpactCategoryKey::AP,
         ImpactCategoryKey::ADPE,
         ImpactCategoryKey::ADPF,
@@ -205,31 +206,43 @@
 
 fn add_building_data(project: &mut LCAxProject, node: &nodes::Building) {
     project.reference_study_period = Some(node.calculation_timespan as u8);
     project.project_info = Some(ProjectInfo::BuildingInfo {
         0: BuildingInfo {
             building_type: BuildingType::NEW,
             building_typology: BuildingTypology::from(&node.building_type),
-            certifications: "".to_string(),
-            building_mass: "".to_string(),
-            gross_floor_area: node.gross_area,
-            gross_floor_area_definition: "".to_string(),
-            heated_floor_area: node.heated_floor_area,
-            heated_floor_area_definition: "".to_string(),
+            certifications: None,
+            building_mass: None,
+            building_height: None,
+            gross_floor_area: Some(AreaType {
+                value: node.gross_area,
+                unit: Unit::M2,
+                definition: "".to_string(),
+            }),
+            heated_floor_area: Some(AreaType {
+                value: node.heated_floor_area,
+                unit: Unit::M2,
+                definition: "".to_string(),
+            }),
+            building_footprint: None,
             floors_above_ground: node.storeys_above_ground,
-            floors_below_ground: node.storeys_below_ground,
-            frame_type: "".to_string(),
-            building_completion_year: 0,
-            energy_demand_heating: 0.0,
-            energy_supply_heating: 0.0,
-            energy_demand_electricity: 0.0,
-            energy_supply_electricity: 0.0,
-            exported_electricity: 0.0,
-            energy_class: node.energy_class.to_string(),
+            floors_below_ground: Some(node.storeys_below_ground),
+            roof_type: RoofType::OTHER,
+            frame_type: Some("".to_string()),
+            building_completion_year: Some(0),
+            building_permit_year: None,
+            energy_demand_heating: Some(0.0),
+            energy_supply_heating: Some(0.0),
+            energy_demand_electricity: Some(0.0),
+            energy_supply_electricity: Some(0.0),
+            exported_electricity: Some(0.0),
+            general_energy_class: GeneralEnergyClass::from(&node.energy_class),
+            local_energy_class: None,
             building_model_scope: None,
+            building_users: None,
         },
     })
 }
 
 fn add_element_data(
     project: &mut LCAxProject,
     node: &nodes::Element,
```

### Comparing `lcax-1.6.0/src/lcabyg/results.rs` & `lcax-1.7.0/src/lcabyg/results.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/src/project.rs` & `lcax-1.7.0/src/project.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-use std::collections::HashMap;
-use std::fmt;
-
 use epdx::epd::{Unit, EPD};
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
+use std::collections::HashMap;
+use std::fmt;
 
 #[cfg(feature = "jsbindings")]
 use tsify::Tsify;
 
 #[derive(Deserialize, Serialize, JsonSchema, Default)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(
@@ -58,15 +57,15 @@
     OTHER,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Default)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub struct Location {
-    pub country: String,
+    pub country: crate::country::Country,
     pub city: Option<String>,
     pub address: Option<String>,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema)]
 #[serde(rename_all = "lowercase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
@@ -77,34 +76,85 @@
 
 #[derive(Deserialize, Serialize, JsonSchema)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub struct BuildingInfo {
     pub building_type: BuildingType,
     pub building_typology: BuildingTypology,
-    pub certifications: String,
-    pub building_mass: String,
-    pub gross_floor_area: f64,
-    pub gross_floor_area_definition: String,
-    pub heated_floor_area: f64,
-    pub heated_floor_area_definition: String,
+    pub certifications: Option<Vec<String>>,
+    pub building_mass: Option<ValueUnit>,
+    pub building_height: Option<ValueUnit>,
+    pub gross_floor_area: Option<AreaType>,
+    pub heated_floor_area: Option<AreaType>,
+    pub building_footprint: Option<ValueUnit>,
     pub floors_above_ground: u16,
-    pub floors_below_ground: u16,
-    pub frame_type: String,
-    pub building_completion_year: u64,
-    pub energy_demand_heating: f64,
-    pub energy_supply_heating: f64,
-    pub energy_demand_electricity: f64,
-    pub energy_supply_electricity: f64,
-    pub exported_electricity: f64,
-    pub energy_class: String,
+    pub floors_below_ground: Option<u16>,
+    pub roof_type: RoofType,
+    pub frame_type: Option<String>,
+    pub building_completion_year: Option<u64>,
+    pub building_permit_year: Option<u64>,
+    pub energy_demand_heating: Option<f64>,
+    pub energy_supply_heating: Option<f64>,
+    pub energy_demand_electricity: Option<f64>,
+    pub energy_supply_electricity: Option<f64>,
+    pub exported_electricity: Option<f64>,
+    pub general_energy_class: GeneralEnergyClass,
+    pub local_energy_class: Option<String>,
+    pub building_users: Option<u64>,
     pub building_model_scope: Option<BuildingModelScope>,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema)]
+#[serde(rename_all = "camelCase")]
+#[cfg_attr(feature = "jsbindings", derive(Tsify))]
+pub struct AreaType {
+    pub value: f64,
+    pub unit: Unit,
+    pub definition: String,
+}
+
+#[derive(Deserialize, Serialize, JsonSchema)]
+#[serde(rename_all = "camelCase")]
+#[cfg_attr(feature = "jsbindings", derive(Tsify))]
+pub struct ValueUnit {
+    value: f64,
+    unit: Unit,
+}
+
+#[derive(Deserialize, Serialize, JsonSchema)]
+#[serde(rename_all = "lowercase")]
+#[cfg_attr(feature = "jsbindings", derive(Tsify))]
+pub enum RoofType {
+    FLAT,
+    PITCHED,
+    SADDLE,
+    PYRAMID,
+    OTHER,
+}
+
+#[derive(Deserialize, Serialize, JsonSchema)]
+#[serde(rename_all = "lowercase")]
+#[cfg_attr(feature = "jsbindings", derive(Tsify))]
+pub enum GeneralEnergyClass {
+    EXISTING,
+    STANDARD,
+    ADVANCED,
+    UNKNOWN,
+}
+
+impl From<&String> for GeneralEnergyClass {
+    fn from(class: &String) -> Self {
+        match class.to_ascii_lowercase().as_str() {
+            "lowenergy" => GeneralEnergyClass::ADVANCED,
+            _ => GeneralEnergyClass::UNKNOWN,
+        }
+    }
+}
+
+#[derive(Deserialize, Serialize, JsonSchema)]
 #[serde(rename_all = "lowercase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub struct BuildingModelScope {
     pub facilitating_works: bool,
     pub substructure: bool,
     pub superstructure_frame: bool,
     pub superstructure_envelope: bool,
```

### Comparing `lcax-1.6.0/src/python.rs` & `lcax-1.7.0/src/python.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/src/utils.rs` & `lcax-1.7.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/tests/datafixtures/lcabyg_example_project.json` & `lcax-1.7.0/tests/datafixtures/lcabyg_example_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/tests/datafixtures/lcabyg_example_results.json` & `lcax-1.7.0/tests/datafixtures/lcabyg_example_results.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/tests/datafixtures/lcabyg_project.json` & `lcax-1.7.0/tests/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/tests/test_lcax.rs` & `lcax-1.7.0/tests/test_lcax.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #[cfg(test)]
 mod tests {
     use lcax::project::Location;
+    use lcax::country::Country;
 
     #[test]
     fn test_lcax() -> Result<(), String> {
         lcax::project::LCAxProject {
             id: "2e257f19-50cc-47de-b54e-2af1add052eb".to_string(),
             name: "Test".to_string(),
             description: Some("Test Project".to_string()),
             comment: None,
             location: Location {
-                country: "Denmark".to_string(),
+                country: Country::DNK,
                 city: None,
                 address: None,
             },
             owner: None,
             format_version: "1.1.0".to_string(),
             lcia_method: None,
             classification_system: None,
```

### Comparing `lcax-1.6.0/tests/test_parse_lcabyg.rs` & `lcax-1.7.0/tests/test_parse_lcabyg.rs`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/pyproject.toml` & `lcax-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-1.6.0/PKG-INFO` & `lcax-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lcax
-Version: 1.6.0
+Version: 1.7.0
 Requires-Dist: cffi
 Requires-Dist: pydantic >=1.8.2, <2.0.0
 Requires-Dist: mkdocs-material >=8.1.4, <9.0.0 ; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1, <2.0.0 ; extra == 'doc'
 Requires-Dist: datamodel-code-generator ; extra == 'codegen'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-datafixtures ; extra == 'tests'
```

