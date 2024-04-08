# Comparing `tmp/mat3ra-code-2024.3.25.post3.tar.gz` & `tmp/mat3ra-code-2024.4.8.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-code-2024.3.25.post3.tar", last modified: Mon Mar 25 23:09:01 2024, max compression
+gzip compressed data, was "mat3ra-code-2024.4.8.post0.tar", last modified: Mon Apr  8 02:12:44 2024, max compression
```

## Comparing `mat3ra-code-2024.3.25.post3.tar` & `mat3ra-code-2024.4.8.post0.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.901527 mat3ra-code-2024.3.25.post3/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.873526 mat3ra-code-2024.3.25.post3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.877526 mat3ra-code-2024.3.25.post3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.877526 mat3ra-code-2024.3.25.post3/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.nycrc
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-25 23:09:01.901527 mat3ra-code-2024.3.25.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   350189 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 23:09:01.901527 mat3ra-code-2024.3.25.post3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.873526 mat3ra-code-2024.3.25.post3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.877526 mat3ra-code-2024.3.25.post3/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/constants.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.881526 mat3ra-code-2024.3.25.post3/src/js/context/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/context/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/context/json_schema_provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/context/mixins.ts
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/context/pickers.js
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/context/provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/context/registry.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.881526 mat3ra-code-2024.3.25.post3/src/js/entity/
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/in_memory.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.881526 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/context.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/context_runtime.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/flowchart.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/hash.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/props.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/repetition.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/mixins/runtime_items.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/other.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.885526 mat3ra-code-2024.3.25.post3/src/js/entity/set/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/enums.ts
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/factory.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/mixins.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.885526 mat3ra-code-2024.3.25.post3/src/js/entity/set/ordered/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/ordered/mixins.ts
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/ordered/utils.ts
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/ordered.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set/selectors.ts
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/entity/set.ts
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/math.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.885526 mat3ra-code-2024.3.25.post3/src/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/array.js
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/class.js
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/clone.js
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/codemirror.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/file.js
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/filter.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/github.js
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/graph.ts
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/hash.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/object.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/schemas.ts
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/selector.js
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/str.js
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/tree.js
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/url.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/uuid.js
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/js/utils/yaml.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.889526 mat3ra-code-2024.3.25.post3/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.889526 mat3ra-code-2024.3.25.post3/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.889526 mat3ra-code-2024.3.25.post3/src/py/mat3ra/code/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra/code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.897527 mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-25 23:09:01.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-25 23:09:01.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 23:09:01.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-25 23:09:01.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 23:09:01.000000 mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.873526 mat3ra-code-2024.3.25.post3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.889526 mat3ra-code-2024.3.25.post3/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/context.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/enums.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.893526 mat3ra-code-2024.3.25.post3/tests/js/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.873526 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.893526 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/1.json
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/2.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/3.json
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/5.json
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/rjsf_schemas.js
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/test_content.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_combine_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_concatString_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_esse_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_flatten_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_include_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_listToString_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_parameter_ref.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_parameter_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_readFile_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/in_memory.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/mixin.flowchart.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/provider.tests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.897527 mat3ra-code-2024.3.25.post3/tests/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/class.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/file.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/filter.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/object.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/schemas.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/str.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/tree.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/utils.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.combine.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.concatString.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.esse.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.flatten.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.include.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.listToString.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.parameter.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.readFile.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/js/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.897527 mat3ra-code-2024.3.25.post3/tests/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 23:09:01.897527 mat3ra-code-2024.3.25.post3/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/py/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tests/py/unit/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 23:08:39.000000 mat3ra-code-2024.3.25.post3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.279558 mat3ra-code-2024.4.8.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.251558 mat3ra-code-2024.4.8.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.nycrc
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-08 02:12:44.279558 mat3ra-code-2024.4.8.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   350189 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:12:44.279558 mat3ra-code-2024.4.8.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.251558 mat3ra-code-2024.4.8.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/constants.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/src/js/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/json_schema_provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/mixins.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/pickers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/registry.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/src/js/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/in_memory.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.263558 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context_runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/flowchart.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/hash.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/props.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/repetition.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/runtime_items.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/other.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.263558 mat3ra-code-2024.4.8.post0/src/js/entity/set/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/enums.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/factory.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/mixins.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.263558 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/mixins.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/selectors.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/math.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/array.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/class.js
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/clone.js
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/codemirror.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/file.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/filter.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/github.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/graph.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/hash.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/object.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/schemas.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/selector.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/str.js
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/tree.js
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/url.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/uuid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/yaml.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/mixins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.275558 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.255558 mat3ra-code-2024.4.8.post0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.271558 mat3ra-code-2024.4.8.post0/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/context.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/enums.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.271558 mat3ra-code-2024.4.8.post0/tests/js/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.255558 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.271558 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/rjsf_schemas.js
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/test_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_combine_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_concatString_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_esse_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_flatten_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_include_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_listToString_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_parameter_ref.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_parameter_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_readFile_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/in_memory.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/mixin.flowchart.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/provider.tests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.275558 mat3ra-code-2024.4.8.post0/tests/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/class.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/file.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/filter.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/object.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/schemas.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/str.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/tree.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/utils.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.combine.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.concatString.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.esse.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.flatten.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.include.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.listToString.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.parameter.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.readFile.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.255558 mat3ra-code-2024.4.8.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.275558 mat3ra-code-2024.4.8.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/py/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/py/unit/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tsconfig.json
```

### Comparing `mat3ra-code-2024.3.25.post3/.github/workflows/cicd.yml` & `mat3ra-code-2024.4.8.post0/.github/workflows/cicd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         uses: actions/checkout@v4
         with:
           repository: Exabyte-io/actions
           token: ${{ secrets.BOT_GITHUB_TOKEN }}
           path: actions
 
       - name: Run python unit tests
-        uses: ./actions/py/test
+        uses: ./actions/py/pytest
         with:
           python-version: ${{ matrix.python-version }}
           unit-test-directory: tests/py/unit
           bot-ssh-key: ${{ secrets.BOT_GITHUB_KEY }}
 
   run-js-tests:
     runs-on: ubuntu-latest
```

### Comparing `mat3ra-code-2024.3.25.post3/.gitignore` & `mat3ra-code-2024.4.8.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/LICENSE.md` & `mat3ra-code-2024.4.8.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/PKG-INFO` & `mat3ra-code-2024.4.8.post0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-code
-Version: 2024.3.25.post3
+Version: 2024.4.8.post0
 Summary: COre DEfinitions.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2022 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -23,22 +23,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
+Requires-Dist: jsonschema>=2.6.0
+Requires-Dist: mat3ra-utils
 Provides-Extra: tests
 Requires-Dist: coverage[toml]>=5.3; extra == "tests"
 Requires-Dist: pre-commit; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: mypy; extra == "tests"
 Requires-Dist: pip-tools; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: all
 Requires-Dist: mat3ra-code[tests]; extra == "all"
 
 [![npm version](https://badge.fury.io/js/%40exabyte-io%2Fcode.js.svg)](https://badge.fury.io/js/%40exabyte-io%2Fcode.js)
 [![License: Apache](https://img.shields.io/badge/License-Apache-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 # @exabyte-io/code.js
@@ -82,8 +86,7 @@
 
 # compile the library
 npm run transpile
 
 # run tests
 npm run test
 ```
-
```

### Comparing `mat3ra-code-2024.3.25.post3/README.md` & `mat3ra-code-2024.4.8.post0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
 
 # compile the library
 npm run transpile
 
 # run tests
 npm run test
 ```
-
```

### Comparing `mat3ra-code-2024.3.25.post3/package-lock.json` & `mat3ra-code-2024.4.8.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/package.json` & `mat3ra-code-2024.4.8.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/pyproject.toml` & `mat3ra-code-2024.4.8.post0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,30 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development",
 ]
 dependencies = [
     # add requirements here
-    "numpy"
+    "numpy",
+    "jsonschema>=2.6.0",
+    "mat3ra-utils",
 ]
 
 [project.optional-dependencies]
 tests = [
     "coverage[toml]>=5.3",
     "pre-commit",
     "black",
     "ruff",
     "isort",
     "mypy",
-    "pip-tools"
+    "pip-tools",
+    "pytest",
+    "pytest-cov",
 ]
 all = ["mat3ra-code[tests]"]
 
 # Entrypoint scripts can be defined here, see examples below.
 [project.scripts]
 # my-script = "my_package.my_module:my_function"
```

### Comparing `mat3ra-code-2024.3.25.post3/src/js/constants.js` & `mat3ra-code-2024.4.8.post0/src/js/constants.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/context/index.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/context/json_schema_provider.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/json_schema_provider.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/context/mixins.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/mixins.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/context/provider.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/provider.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/context/registry.js` & `mat3ra-code-2024.4.8.post0/src/js/context/registry.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/in_memory.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/in_memory.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/index.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/context.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/context_runtime.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context_runtime.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/flowchart.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/flowchart.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/hash.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/hash.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/props.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/props.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/repetition.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/repetition.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/mixins/runtime_items.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/runtime_items.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/other.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/other.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/set/factory.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/factory.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/set/mixins.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/mixins.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/set/ordered/mixins.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/mixins.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/set/ordered/utils.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/utils.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/set/selectors.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/selectors.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/entity/set.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/math.ts` & `mat3ra-code-2024.4.8.post0/src/js/math.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/array.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/array.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/class.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/class.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/file.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/file.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/filter.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/filter.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/github.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/github.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/graph.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/graph.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/hash.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/hash.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/index.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/object.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/object.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/schemas.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/schemas.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/selector.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/selector.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/str.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/str.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/tree.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/tree.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/js/utils/yaml.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/yaml.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/PKG-INFO` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-code
-Version: 2024.3.25.post3
+Version: 2024.4.8.post0
 Summary: COre DEfinitions.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2022 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -23,22 +23,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
+Requires-Dist: jsonschema>=2.6.0
+Requires-Dist: mat3ra-utils
 Provides-Extra: tests
 Requires-Dist: coverage[toml]>=5.3; extra == "tests"
 Requires-Dist: pre-commit; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: mypy; extra == "tests"
 Requires-Dist: pip-tools; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: all
 Requires-Dist: mat3ra-code[tests]; extra == "all"
 
 [![npm version](https://badge.fury.io/js/%40exabyte-io%2Fcode.js.svg)](https://badge.fury.io/js/%40exabyte-io%2Fcode.js)
 [![License: Apache](https://img.shields.io/badge/License-Apache-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 # @exabyte-io/code.js
@@ -82,8 +86,7 @@
 
 # compile the library
 npm run transpile
 
 # run tests
 npm run test
 ```
-
```

### Comparing `mat3ra-code-2024.3.25.post3/src/py/mat3ra_code.egg-info/SOURCES.txt` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 src/js/utils/tree.js
 src/js/utils/url.js
 src/js/utils/uuid.js
 src/js/utils/yaml.ts
 src/py/__init__.py
 src/py/mat3ra/__init__.py
 src/py/mat3ra/code/__init__.py
+src/py/mat3ra/code/constants.py
+src/py/mat3ra/code/entity.py
+src/py/mat3ra/code/mixins/__init__.py
 src/py/mat3ra_code.egg-info/PKG-INFO
 src/py/mat3ra_code.egg-info/SOURCES.txt
 src/py/mat3ra_code.egg-info/dependency_links.txt
 src/py/mat3ra_code.egg-info/requires.txt
 src/py/mat3ra_code.egg-info/top_level.txt
 tests/js/context.tests.ts
 tests/js/enums.ts
@@ -102,10 +105,9 @@
 tests/js/utils/yaml.concatString.tests.ts
 tests/js/utils/yaml.esse.tests.ts
 tests/js/utils/yaml.flatten.tests.ts
 tests/js/utils/yaml.include.tests.ts
 tests/js/utils/yaml.listToString.tests.ts
 tests/js/utils/yaml.parameter.tests.ts
 tests/js/utils/yaml.readFile.tests.ts
-tests/py/__init__.py
 tests/py/unit/__init__.py
-tests/py/unit/test_sample.py
+tests/py/unit/test_entity.py
```

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/context.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/context.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/enums.ts` & `mat3ra-code-2024.4.8.post0/tests/js/enums.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/fixtures/json/example/5.json` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/5.json`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/fixtures/rjsf_schemas.js` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/rjsf_schemas.js`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_combine_tag.yml` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_combine_tag.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/fixtures/yaml_parameter_tag.yml` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_parameter_tag.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/in_memory.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/in_memory.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/mixin.flowchart.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/mixin.flowchart.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/provider.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/provider.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/class.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/class.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/filter.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/filter.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/object.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/object.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/schemas.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/schemas.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/str.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/str.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/tree.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/tree.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/utils.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/utils.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.combine.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.combine.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.concatString.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.concatString.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.esse.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.esse.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.flatten.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.flatten.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.include.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.include.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.listToString.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.listToString.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.parameter.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.parameter.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-code-2024.3.25.post3/tests/js/utils/yaml.readFile.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.readFile.tests.ts`

 * *Files identical despite different names*

