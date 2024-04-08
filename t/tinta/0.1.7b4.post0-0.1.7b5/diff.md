# Comparing `tmp/tinta-0.1.7b4.post0.tar.gz` & `tmp/tinta-0.1.7b5.tar.gz`

## Comparing `tinta-0.1.7b4.post0.tar` & `tinta-0.1.7b5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.gitattributes
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.pylintrc
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/DESCRIPTION.rst
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/HIPPOCRATIC_LICENSE.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/MANIFEST.in
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/Pipfile
--rw-r--r--   0        0        0    45957 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/requirements-dev.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/requirements.txt
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/setup.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.github/workflows/publish-test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.vscode/launch.json
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.vscode/settings.json
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.vscode/tasks.json
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/examples/basic_example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/examples/colors.ini
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/examples/complete_example.py
--rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/examples/tinta-discover.png
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/junit/test-results.xml
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tests/conftest.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tests/test_colors_invalid.ini
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tests/test_discover.py
--rw-r--r--   0        0        0    24946 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tests/test_tinta.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/__main__.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/ansi.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/colorize.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/colors.ini
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/constants.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/discover.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/multi_version_imports.py
--rw-r--r--   0        0        0    25619 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/tinta.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/typ.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/tinta/utils.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/LICENSE
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/README.md
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/pyproject.toml
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 tinta-0.1.7b4.post0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b5/DESCRIPTION.rst
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b5/HIPPOCRATIC_LICENSE.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b5/MANIFEST.in
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tinta-0.1.7b5/Pipfile
+-rw-r--r--   0        0        0    39666 2020-02-02 00:00:00.000000 tinta-0.1.7b5/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b5/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tinta-0.1.7b5/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b5/requirements.txt
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b5/setup.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.vscode/launch.json
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.vscode/settings.json
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.vscode/tasks.json
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/basic_example.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/colors.ini
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/complete_example.py
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/tinta-discover.png
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b5/junit/test-results.xml
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/conftest.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/test_colors_invalid.ini
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/test_discover.py
+-rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/test_tinta.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/__main__.py
+-rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/ansi.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/colors.ini
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/constants.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/discover.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/multi_version_imports.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/stylize.py
+-rw-r--r--   0        0        0    28887 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/tinta.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/typ.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/utils.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b5/LICENSE
+-rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 tinta-0.1.7b5/README.md
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 tinta-0.1.7b5/pyproject.toml
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 tinta-0.1.7b5/PKG-INFO
```

### Comparing `tinta-0.1.7b4.post0/CODE_OF_CONDUCT.md` & `tinta-0.1.7b5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/HIPPOCRATIC_LICENSE.md` & `tinta-0.1.7b5/HIPPOCRATIC_LICENSE.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/Pipfile.lock` & `tinta-0.1.7b5/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8540719696969696%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'21ab7bdebcd985cd17de47821f4ac04925d0d95a1918970f91b64077845e2a7c'}}",*

 * * "'default'": '{replace: OrderedDict()}',*

 * * "'develop'": "{'filelock': {'hashes': "*

 * *              "['sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb', "*

 * *              "'sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546'], "*

 * *              "'version': '==3.13.3'}, 'hatchling': {'hashes': "*

 * *              "['sha256:30ec7ee09f6e17b73257eedfd7f5bb5a9b0 […]*

```diff
@@ -1,111 +1,25 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "d43dc087babb30228f18b4eda5df26c38f0dcb585bdbe4bf905541c18dda801e"
+            "sha256": "21ab7bdebcd985cd17de47821f4ac04925d0d95a1918970f91b64077845e2a7c"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.6"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
-    "default": {
-        "deprecated": {
-            "hashes": [
-                "sha256:6fac8b097794a90302bdbb17b9b815e732d3c4720583ff1b198499d78470466c",
-                "sha256:e5323eb936458dccc2582dc6f9c322c852a775a27065ff2b0c4970b9d53d01b3"
-            ],
-            "index": "pypi",
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.2.14"
-        },
-        "wrapt": {
-            "hashes": [
-                "sha256:0d2691979e93d06a95a26257adb7bfd0c93818e89b1406f5a28f36e0d8c1e1fc",
-                "sha256:14d7dc606219cdd7405133c713f2c218d4252f2a469003f8c46bb92d5d095d81",
-                "sha256:1a5db485fe2de4403f13fafdc231b0dbae5eca4359232d2efc79025527375b09",
-                "sha256:1acd723ee2a8826f3d53910255643e33673e1d11db84ce5880675954183ec47e",
-                "sha256:1ca9b6085e4f866bd584fb135a041bfc32cab916e69f714a7d1d397f8c4891ca",
-                "sha256:1dd50a2696ff89f57bd8847647a1c363b687d3d796dc30d4dd4a9d1689a706f0",
-                "sha256:2076fad65c6736184e77d7d4729b63a6d1ae0b70da4868adeec40989858eb3fb",
-                "sha256:2a88e6010048489cda82b1326889ec075a8c856c2e6a256072b28eaee3ccf487",
-                "sha256:3ebf019be5c09d400cf7b024aa52b1f3aeebeff51550d007e92c3c1c4afc2a40",
-                "sha256:418abb18146475c310d7a6dc71143d6f7adec5b004ac9ce08dc7a34e2babdc5c",
-                "sha256:43aa59eadec7890d9958748db829df269f0368521ba6dc68cc172d5d03ed8060",
-                "sha256:44a2754372e32ab315734c6c73b24351d06e77ffff6ae27d2ecf14cf3d229202",
-                "sha256:490b0ee15c1a55be9c1bd8609b8cecd60e325f0575fc98f50058eae366e01f41",
-                "sha256:49aac49dc4782cb04f58986e81ea0b4768e4ff197b57324dcbd7699c5dfb40b9",
-                "sha256:5eb404d89131ec9b4f748fa5cfb5346802e5ee8836f57d516576e61f304f3b7b",
-                "sha256:5f15814a33e42b04e3de432e573aa557f9f0f56458745c2074952f564c50e664",
-                "sha256:5f370f952971e7d17c7d1ead40e49f32345a7f7a5373571ef44d800d06b1899d",
-                "sha256:66027d667efe95cc4fa945af59f92c5a02c6f5bb6012bff9e60542c74c75c362",
-                "sha256:66dfbaa7cfa3eb707bbfcd46dab2bc6207b005cbc9caa2199bcbc81d95071a00",
-                "sha256:685f568fa5e627e93f3b52fda002c7ed2fa1800b50ce51f6ed1d572d8ab3e7fc",
-                "sha256:6906c4100a8fcbf2fa735f6059214bb13b97f75b1a61777fcf6432121ef12ef1",
-                "sha256:6a42cd0cfa8ffc1915aef79cb4284f6383d8a3e9dcca70c445dcfdd639d51267",
-                "sha256:6dcfcffe73710be01d90cae08c3e548d90932d37b39ef83969ae135d36ef3956",
-                "sha256:6f6eac2360f2d543cc875a0e5efd413b6cbd483cb3ad7ebf888884a6e0d2e966",
-                "sha256:72554a23c78a8e7aa02abbd699d129eead8b147a23c56e08d08dfc29cfdddca1",
-                "sha256:73870c364c11f03ed072dda68ff7aea6d2a3a5c3fe250d917a429c7432e15228",
-                "sha256:73aa7d98215d39b8455f103de64391cb79dfcad601701a3aa0dddacf74911d72",
-                "sha256:75ea7d0ee2a15733684badb16de6794894ed9c55aa5e9903260922f0482e687d",
-                "sha256:7bd2d7ff69a2cac767fbf7a2b206add2e9a210e57947dd7ce03e25d03d2de292",
-                "sha256:807cc8543a477ab7422f1120a217054f958a66ef7314f76dd9e77d3f02cdccd0",
-                "sha256:8e9723528b9f787dc59168369e42ae1c3b0d3fadb2f1a71de14531d321ee05b0",
-                "sha256:9090c9e676d5236a6948330e83cb89969f433b1943a558968f659ead07cb3b36",
-                "sha256:9153ed35fc5e4fa3b2fe97bddaa7cbec0ed22412b85bcdaf54aeba92ea37428c",
-                "sha256:9159485323798c8dc530a224bd3ffcf76659319ccc7bbd52e01e73bd0241a0c5",
-                "sha256:941988b89b4fd6b41c3f0bfb20e92bd23746579736b7343283297c4c8cbae68f",
-                "sha256:94265b00870aa407bd0cbcfd536f17ecde43b94fb8d228560a1e9d3041462d73",
-                "sha256:98b5e1f498a8ca1858a1cdbffb023bfd954da4e3fa2c0cb5853d40014557248b",
-                "sha256:9b201ae332c3637a42f02d1045e1d0cccfdc41f1f2f801dafbaa7e9b4797bfc2",
-                "sha256:a0ea261ce52b5952bf669684a251a66df239ec6d441ccb59ec7afa882265d593",
-                "sha256:a33a747400b94b6d6b8a165e4480264a64a78c8a4c734b62136062e9a248dd39",
-                "sha256:a452f9ca3e3267cd4d0fcf2edd0d035b1934ac2bd7e0e57ac91ad6b95c0c6389",
-                "sha256:a86373cf37cd7764f2201b76496aba58a52e76dedfaa698ef9e9688bfd9e41cf",
-                "sha256:ac83a914ebaf589b69f7d0a1277602ff494e21f4c2f743313414378f8f50a4cf",
-                "sha256:aefbc4cb0a54f91af643660a0a150ce2c090d3652cf4052a5397fb2de549cd89",
-                "sha256:b3646eefa23daeba62643a58aac816945cadc0afaf21800a1421eeba5f6cfb9c",
-                "sha256:b47cfad9e9bbbed2339081f4e346c93ecd7ab504299403320bf85f7f85c7d46c",
-                "sha256:b935ae30c6e7400022b50f8d359c03ed233d45b725cfdd299462f41ee5ffba6f",
-                "sha256:bb2dee3874a500de01c93d5c71415fcaef1d858370d405824783e7a8ef5db440",
-                "sha256:bc57efac2da352a51cc4658878a68d2b1b67dbe9d33c36cb826ca449d80a8465",
-                "sha256:bf5703fdeb350e36885f2875d853ce13172ae281c56e509f4e6eca049bdfb136",
-                "sha256:c31f72b1b6624c9d863fc095da460802f43a7c6868c5dda140f51da24fd47d7b",
-                "sha256:c5cd603b575ebceca7da5a3a251e69561bec509e0b46e4993e1cac402b7247b8",
-                "sha256:d2efee35b4b0a347e0d99d28e884dfd82797852d62fcd7ebdeee26f3ceb72cf3",
-                "sha256:d462f28826f4657968ae51d2181a074dfe03c200d6131690b7d65d55b0f360f8",
-                "sha256:d5e49454f19ef621089e204f862388d29e6e8d8b162efce05208913dde5b9ad6",
-                "sha256:da4813f751142436b075ed7aa012a8778aa43a99f7b36afe9b742d3ed8bdc95e",
-                "sha256:db2e408d983b0e61e238cf579c09ef7020560441906ca990fe8412153e3b291f",
-                "sha256:db98ad84a55eb09b3c32a96c576476777e87c520a34e2519d3e59c44710c002c",
-                "sha256:dbed418ba5c3dce92619656802cc5355cb679e58d0d89b50f116e4a9d5a9603e",
-                "sha256:dcdba5c86e368442528f7060039eda390cc4091bfd1dca41e8046af7c910dda8",
-                "sha256:decbfa2f618fa8ed81c95ee18a387ff973143c656ef800c9f24fb7e9c16054e2",
-                "sha256:e4fdb9275308292e880dcbeb12546df7f3e0f96c6b41197e0cf37d2826359020",
-                "sha256:eb1b046be06b0fce7249f1d025cd359b4b80fc1c3e24ad9eca33e0dcdb2e4a35",
-                "sha256:eb6e651000a19c96f452c85132811d25e9264d836951022d6e81df2fff38337d",
-                "sha256:ed867c42c268f876097248e05b6117a65bcd1e63b779e916fe2e33cd6fd0d3c3",
-                "sha256:edfad1d29c73f9b863ebe7082ae9321374ccb10879eeabc84ba3b69f2579d537",
-                "sha256:f2058f813d4f2b5e3a9eb2eb3faf8f1d99b81c3e51aeda4b168406443e8ba809",
-                "sha256:f6b2d0c6703c988d334f297aa5df18c45e97b0af3679bb75059e0e0bd8b1069d",
-                "sha256:f8212564d49c50eb4565e502814f694e240c55551a5f1bc841d4fcaabb0a9b8a",
-                "sha256:ffa565331890b90056c01db69c0fe634a776f8019c143a5ae265f9c6bc4bd6d4"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.16.0"
-        }
-    },
+    "default": {},
     "develop": {
         "astroid": {
             "hashes": [
                 "sha256:951798f922990137ac090c53af473db7ab4e70c770e6d7fae0cec59f74411819",
                 "sha256:ac248253bfa4bd924a0de213707e7ebeeb3138abeb48d798784ead1e56d419d4"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -116,14 +30,22 @@
                 "sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7",
                 "sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==2.1.0"
         },
+        "backports.tarfile": {
+            "hashes": [
+                "sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75",
+                "sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4"
+            ],
+            "markers": "python_version < '3.12'",
+            "version": "==1.0.0"
+        },
         "black": {
             "hashes": [
                 "sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f",
                 "sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93",
                 "sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11",
                 "sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0",
                 "sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9",
@@ -343,44 +265,44 @@
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.20.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e",
-                "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"
+                "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb",
+                "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.13.1"
+            "version": "==3.13.3"
         },
         "hatchling": {
             "hashes": [
-                "sha256:5fdf7b689c1e76cf280bfe002e5e3d7efe99f63e559d2dc3e5d5f49de489d57d",
-                "sha256:f2dfce8e5d389c53c41c87f5c643c5ef2f9519510eaaddda0aac63eb52470684"
+                "sha256:30ec7ee09f6e17b73257eedfd7f5bb5a9b028a6cf6d144d9faad1d826fa203b8",
+                "sha256:ca260a5adad376563dcd5df799e79ec1d5c0a3be41e2fbe335613c451772b09e"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==1.22.2"
+            "version": "==1.22.5"
         },
         "idna": {
             "hashes": [
                 "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
                 "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.6"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:198f568f3230878cb1b44fbd7975f87906c22336dba2e4a7f05278c281fbd792",
-                "sha256:f4bc4c0c070c490abf4ce96d715f68e95923320370efb66143df00199bb6c100"
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.0.2"
+            "version": "==7.1.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -392,27 +314,43 @@
                 "sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6"
             ],
             "markers": "python_full_version >= '3.8.0'",
             "version": "==5.13.2"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:86b534de565381f6b3c1c830d13f931d7be1a75f0081c57dff615578676e2206",
-                "sha256:cb28a5ebda8bc47d8c8015307d93163464f9f2b91ab4006e09ff0ce07e8bfb30"
+                "sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd",
+                "sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.3.1"
+            "version": "==3.4.0"
+        },
+        "jaraco.context": {
+            "hashes": [
+                "sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266",
+                "sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==5.3.0"
+        },
+        "jaraco.functools": {
+            "hashes": [
+                "sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925",
+                "sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.0"
         },
         "keyring": {
             "hashes": [
-                "sha256:c3327b6ffafc0e8befbdb597cacdb4928ffe5c1212f7645f186e6d9957a898db",
-                "sha256:df38a4d7419a6a60fea5cef1e45a948a3e8430dd12ad88b0f423c5c143906218"
+                "sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427",
+                "sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==24.3.1"
+            "version": "==25.1.0"
         },
         "markdown-it-py": {
             "hashes": [
                 "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
                 "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
             "markers": "python_version >= '3.8'",
@@ -482,32 +420,32 @@
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "nh3": {
             "hashes": [
-                "sha256:0d02d0ff79dfd8208ed25a39c12cbda092388fff7f1662466e27d97ad011b770",
-                "sha256:3277481293b868b2715907310c7be0f1b9d10491d5adf9fce11756a97e97eddf",
-                "sha256:3b803a5875e7234907f7d64777dfde2b93db992376f3d6d7af7f3bc347deb305",
-                "sha256:427fecbb1031db085eaac9931362adf4a796428ef0163070c484b5a768e71601",
-                "sha256:5f0d77272ce6d34db6c87b4f894f037d55183d9518f948bba236fe81e2bb4e28",
-                "sha256:60684857cfa8fdbb74daa867e5cad3f0c9789415aba660614fe16cd66cbb9ec7",
-                "sha256:6f42f99f0cf6312e470b6c09e04da31f9abaadcd3eb591d7d1a88ea931dca7f3",
-                "sha256:86e447a63ca0b16318deb62498db4f76fc60699ce0a1231262880b38b6cff911",
-                "sha256:8d595df02413aa38586c24811237e95937ef18304e108b7e92c890a06793e3bf",
-                "sha256:9c0d415f6b7f2338f93035bba5c0d8c1b464e538bfbb1d598acd47d7969284f0",
-                "sha256:a5167a6403d19c515217b6bcaaa9be420974a6ac30e0da9e84d4fc67a5d474c5",
-                "sha256:ac19c0d68cd42ecd7ead91a3a032fdfff23d29302dbb1311e641a130dfefba97",
-                "sha256:b1e97221cedaf15a54f5243f2c5894bb12ca951ae4ddfd02a9d4ea9df9e1a29d",
-                "sha256:bc2d086fb540d0fa52ce35afaded4ea526b8fc4d3339f783db55c95de40ef02e",
-                "sha256:d1e30ff2d8d58fb2a14961f7aac1bbb1c51f9bdd7da727be35c63826060b0bf3",
-                "sha256:f3b53ba93bb7725acab1e030bc2ecd012a817040fd7851b332f86e2f9bb98dc6"
+                "sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a",
+                "sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911",
+                "sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb",
+                "sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a",
+                "sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc",
+                "sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028",
+                "sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9",
+                "sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3",
+                "sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351",
+                "sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10",
+                "sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71",
+                "sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f",
+                "sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b",
+                "sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a",
+                "sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062",
+                "sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a"
             ],
-            "version": "==0.2.15"
+            "version": "==0.2.17"
         },
         "packaging": {
             "hashes": [
                 "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
                 "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
@@ -586,20 +524,20 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==8.1.1"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
-                "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
+                "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652",
+                "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==4.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         },
         "readme-renderer": {
             "hashes": [
                 "sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311",
                 "sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9"
             ],
             "markers": "python_version >= '3.8'",
@@ -635,35 +573,35 @@
                 "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.7.1"
         },
         "ruff": {
             "hashes": [
-                "sha256:0171aab5fecdc54383993389710a3d1227f2da124d76a2784a7098e818f92d61",
-                "sha256:0da458989ce0159555ef224d5b7c24d3d2e4bf4c300b85467b08c3261c6bc6a8",
-                "sha256:1eca7ff7a47043cf6ce5c7f45f603b09121a7cc047447744b029d1b719278eb5",
-                "sha256:2700a804d5336bcffe063fd789ca2c7b02b552d2e323a336700abb8ae9e6a3f8",
-                "sha256:352e95ead6964974b234e16ba8a66dad102ec7bf8ac064a23f95371d8b198aab",
-                "sha256:38671be06f57a2f8aba957d9f701ea889aa5736be806f18c0cd03d6ff0cbca8d",
-                "sha256:45817af234605525cdf6317005923bf532514e1ea3d9270acf61ca2440691376",
-                "sha256:5a6cbf216b69c7090f0fe4669501a27326c34e119068c1494f35aaf4cc683778",
-                "sha256:79bca3a03a759cc773fca69e0bdeac8abd1c13c31b798d5bb3c9da4a03144a9f",
-                "sha256:8d6ab88c81c4040a817aa432484e838aaddf8bfd7ca70e4e615482757acb64f8",
-                "sha256:973a0e388b7bc2e9148c7f9be8b8c6ae7471b9be37e1cc732f8f44a6f6d7720d",
-                "sha256:b24c19e8598916d9c6f5a5437671f55ee93c212a2c4c569605dc3842b6820386",
-                "sha256:be90bcae57c24d9f9d023b12d627e958eb55f595428bafcb7fec0791ad25ddfc",
-                "sha256:cfa60d23269d6e2031129b053fdb4e5a7b0637fc6c9c0586737b962b2f834493",
-                "sha256:e7d3f6762217c1da954de24b4a1a70515630d29f71e268ec5000afe81377642d",
-                "sha256:f2831ec6a580a97f1ea82ea1eda0401c3cdf512cf2045fa3c85e8ef109e87de0",
-                "sha256:fd66469f1a18fdb9d32e22b79f486223052ddf057dc56dea0caaf1a47bdfaf4e"
+                "sha256:122de171a147c76ada00f76df533b54676f6e321e61bd8656ae54be326c10296",
+                "sha256:3a05f3793ba25f194f395578579c546ca5d83e0195f992edc32e5907d142bfa3",
+                "sha256:5e55771559c89272c3ebab23326dc23e7f813e492052391fe7950c1a5a139d89",
+                "sha256:712e71283fc7d9f95047ed5f793bc019b0b0a29849b14664a60fd66c23b96da1",
+                "sha256:87258e0d4b04046cf1d6cc1c56fadbf7a880cc3de1f7294938e923234cf9e498",
+                "sha256:89b1e92b3bd9fca249153a97d23f29bed3992cff414b222fcd361d763fc53f12",
+                "sha256:9d8605aa990045517c911726d21293ef4baa64f87265896e491a05461cae078d",
+                "sha256:a067daaeb1dc2baf9b82a32dae67d154d95212080c80435eb052d95da647763d",
+                "sha256:a532a90b4a18d3f722c124c513ffb5e5eaff0cc4f6d3aa4bda38e691b8600c9f",
+                "sha256:a759d33a20c72f2dfa54dae6e85e1225b8e302e8ac655773aff22e542a300985",
+                "sha256:a7b6e63194c68bca8e71f81de30cfa6f58ff70393cf45aab4c20f158227d5936",
+                "sha256:aef5bd3b89e657007e1be6b16553c8813b221ff6d92c7526b7e0227450981eac",
+                "sha256:d80a6b18a6c3b6ed25b71b05eba183f37d9bc8b16ace9e3d700997f00b74660b",
+                "sha256:dabc62195bf54b8a7876add6e789caae0268f34582333cda340497c886111c39",
+                "sha256:dc56bb16a63c1303bd47563c60482a1512721053d93231cf7e9e1c6954395a0e",
+                "sha256:dfd3504e881082959b4160ab02f7a205f0fadc0a9619cc481982b6837b2fd4c0",
+                "sha256:faeeae9905446b975dcf6d4499dc93439b131f1443ee264055c5716dd947af55"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
-            "version": "==0.3.3"
+            "version": "==0.3.5"
         },
         "setuptools": {
             "hashes": [
                 "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e",
                 "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"
             ],
             "index": "pypi",
@@ -676,44 +614,35 @@
                 "sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.12.4"
         },
         "trove-classifiers": {
             "hashes": [
-                "sha256:3a84096861b385ec422c79995d1f6435dde47a9b63adaa3c886e53232ba7e6e0",
-                "sha256:df7edff9c67ff86b733628998330b180e81d125b1e096536d83ac0fd79673fdc"
+                "sha256:6de68d06edd6fec5032162b6af22e818a4bb6f4ae2258e74699f8a41064b7cad",
+                "sha256:c400e0bdceb018913339d53b07682d09a42aada687d070e90ee3c08477bec024"
             ],
-            "version": "==2024.3.3"
+            "version": "==2024.3.25"
         },
         "twine": {
             "hashes": [
                 "sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4",
                 "sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==5.0.0"
         },
-        "types-deprecated": {
-            "hashes": [
-                "sha256:0680e89989a8142707de8103f15d182445a533c1047fd9b7e8c5459101e9b90a",
-                "sha256:d7793aaf32ff8f7e49a8ac781de4872248e0694c4b75a7a8a186c51167463f9d"
-            ],
-            "index": "pypi",
-            "markers": "python_version >= '3.8'",
-            "version": "==1.2.9.20240311"
-        },
         "typing-extensions": {
             "hashes": [
-                "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475",
-                "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.10.0"
+            "version": "==4.11.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
                 "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
             "markers": "python_version >= '3.8'",
```

### Comparing `tinta-0.1.7b4.post0/setup.py` & `tinta-0.1.7b5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from setuptools import setup
 
 with Path("README.md").open(encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="tinta",
-    version="0.1.7b4-post0",
+    version="0.1.7b5",
     description="Tinta, a magical console output tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/brandonscript/tinta",
     author="Brandon Shelley",
     author_email="brandon@pacificaviator.co",
     install_requires=[],
```

### Comparing `tinta-0.1.7b4.post0/.github/workflows/publish-test.yml` & `tinta-0.1.7b5/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/.github/workflows/publish.yml` & `tinta-0.1.7b5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/.github/workflows/run-tests.yml` & `tinta-0.1.7b5/.github/workflows/run-tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,19 +22,19 @@
           python-version: ${{ matrix.python-version }}
           cache: "pip"
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pytest deprecated
+          pip install pytest
       - name: Test with pytest
         run: |
           pip install pytest
-          pytest -xv -s
+          pytest -vv -s
 
   build-newer-python:
     runs-on: ubuntu-22.04
     strategy:
       matrix:
         python-version: ["3.11", "3.12"]
 
@@ -46,12 +46,12 @@
           python-version: ${{ matrix.python-version }}
           cache: "pip"
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pytest deprecated
+          pip install pytest
       - name: Test with pytest
         run: |
           pip install pytest
           pytest -xv -s
```

### Comparing `tinta-0.1.7b4.post0/.vscode/launch.json` & `tinta-0.1.7b5/.vscode/launch.json`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
       "type": "debugpy",
       "request": "launch",
       "console": "integratedTerminal",
       "module": "pytest",
       "env": {
         "_PYTEST_RAISE": "1"
       },
-      "args": ["-xv"]
+      "args": ["-v"]
     },
     {
       "name": "Run Tinta tests (all versions)",
       "type": "debugpy",
       "preLaunchTask": "Run All Pytest Versions",
       "request": "launch"
     }
```

### Comparing `tinta-0.1.7b4.post0/.vscode/settings.json` & `tinta-0.1.7b5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/.vscode/tasks.json` & `tinta-0.1.7b5/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/examples/basic_example.py` & `tinta-0.1.7b5/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/examples/complete_example.py` & `tinta-0.1.7b5/examples/complete_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             ),
         )
     )
 
 
 def complete():
 
-    _orig_colors_ini = Tinta.colors._colors_ini_path
+    _orig_colors_ini = Tinta._colors._colors_ini_path
 
     Tinta.load_colors("examples/colors.ini")
 
     # from colors.ini:
 
     # [colors]
     # green = 35
@@ -162,12 +162,12 @@
         print("".ljust(width + 1) * indent, end="")
         for i in range(256):
             end = "\n" if i % cols == cols - indent - 1 else " "
             Tinta().tint(f"{str(i).ljust(width)}", color=i).print(end=end)
 
     print_columns(12, indent=8)
 
-    Tinta.colors._colors_ini_path = _orig_colors_ini
+    Tinta._colors._colors_ini_path = _orig_colors_ini
 
 
 if __name__ == "__main__":
     complete()
```

### Comparing `tinta-0.1.7b4.post0/examples/tinta-discover.png` & `tinta-0.1.7b5/examples/tinta-discover.png`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/junit/test-results.xml` & `tinta-0.1.7b5/junit/test-results.xml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/tests/test_discover.py` & `tinta-0.1.7b5/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/tests/test_tinta.py` & `tinta-0.1.7b5/tests/test_tinta.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,23 +18,27 @@
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 
 import os
 import re
+import time
+import timeit
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, List, Tuple
 
 import pytest
 from pytest import CaptureFixture
 
-# pylint: disable=import-error
 from tinta import Tinta
 
+# pylint: disable=import-error
+from tinta.stylize import _join, ansi_styles
+
 Tinta.load_colors("examples/colors.ini")
 
 O = "\x1b[0m"
 GREEN = "\x1b[38;5;35m"
 RED = "\x1b[38;5;1m"
 BLUE = "\x1b[38;5;32m"
 L_BLUE = "\x1b[38;5;37m"
@@ -45,14 +49,24 @@
 ORANGE = "\x1b[38;5;166m"
 PURPLE = "\x1b[38;5;18m"
 PINK = "\x1b[38;5;197m"
 GRAY = "\x1b[38;5;243m"
 D_GRAY = "\x1b[38;5;235m"
 L_GRAY = "\x1b[38;5;248m"
 WHITE = "\x1b[38;5;255m"
+BOLD, BOLD_OFF = ansi_styles("bold")
+UNDERLINE, UNDERLINE_OFF = ansi_styles("underline")
+DIM, DIM_OFF = ansi_styles("dim")
+STRIKE, STRIKE_OFF = ansi_styles("strikethrough")
+
+
+def _stitch(*args):
+    # get everything after \x1b[ for each arg
+    codes = [re.search(r"\x1b\[(.*?)m", arg).group(1) for arg in args]
+    return f"\x1b[{_join(*codes).strip(';')}m"
 
 
 @contextmanager
 def skip_on_github_actions():
     gh = bool(os.getenv("GITHUB_ACTIONS") == "true")
     if gh:
         pytest.mark.skipif(True, reason="Function skipped on GitHub Actions")
@@ -60,46 +74,245 @@
 
 
 class TestInit:
 
     def test_init(self):
         assert len(Tinta("initialized").parts) == 1
 
+    def test_accepts_string_on_init(self):
+        assert Tinta("initialized").to_str() == "initialized"
+
 
 class TestBasicColorizing:
 
+    basic_colors = [
+        # fmt: off
+        ("green", lambda: Tinta().green("green"), f"{GREEN}green{O}"),
+        ("green", lambda: Tinta().tint(35, "green"), f"{GREEN}green{O}"),
+        ("green", lambda: Tinta().tint("green", "green"), f"{GREEN}green{O}"),
+        ("red", lambda: Tinta().red("red"), f"{RED}red{O}"),
+        ("blue", lambda: Tinta().blue("blue"), f"{BLUE}blue{O}"),
+        ("blue", lambda: Tinta().blue("green (but actually blue)"), f"{BLUE}green (but actually blue){O}"),
+        ("light_blue", lambda: Tinta().light_blue("light_blue"), f"{L_BLUE}light_blue{O}"),
+        ("yellow", lambda: Tinta().yellow("yellow"), f"{YELLOW}yellow{O}"),
+        ("amber", lambda: Tinta().amber("amber"), f"{AMBER}amber{O}"),
+        ("mint", lambda: Tinta().mint("mint"), f"{MINT}mint{O}"),
+        ("olive", lambda: Tinta().olive("olive"), f"{OLIVE}olive{O}"),
+        ("orange", lambda: Tinta().orange("orange"), f"{ORANGE}orange{O}"),
+        ("purple", lambda: Tinta().purple("purple"), f"{PURPLE}purple{O}"),
+        ("pink", lambda: Tinta().pink("pink"), f"{PINK}pink{O}"),
+        ("gray", lambda: Tinta().gray("gray"), f"{GRAY}gray{O}"),
+        ("dark_gray", lambda: Tinta().dark_gray("dark_gray"), f"{D_GRAY}dark_gray{O}"),
+        ("light_gray", lambda: Tinta().light_gray("light_gray"), f"{L_GRAY}light_gray{O}"),
+        ("white", lambda: Tinta().white("white"), f"{WHITE}white{O}"),
+        # fmt: on
+    ]
+
     @pytest.mark.parametrize(
         "color,Testa,expected",
-        [
-            # fmt: off
-            ("green", lambda: Tinta().green("green"), f"{GREEN}green{O}"),
-            ("green", lambda: Tinta().tint(35, "green"), f"{GREEN}green{O}"),
-            ("green", lambda: Tinta().tint("green", "green"), f"{GREEN}green{O}"),
-            ("red", lambda: Tinta().red("red"), f"{RED}red{O}"),
-            ("blue", lambda: Tinta().blue("blue"), f"{BLUE}blue{O}"),
-            ("blue", lambda: Tinta().blue("Green"), f"{BLUE}Green{O}"),
-            ("light_blue", lambda: Tinta().light_blue("light_blue"), f"{L_BLUE}light_blue{O}"),
-            ("yellow", lambda: Tinta().yellow("yellow"), f"{YELLOW}yellow{O}"),
-            ("amber", lambda: Tinta().amber("amber"), f"{AMBER}amber{O}"),
-            ("mint", lambda: Tinta().mint("Mint"), f"{MINT}Mint{O}"),
-            ("olive", lambda: Tinta().olive("olive"), f"{OLIVE}olive{O}"),
-            ("orange", lambda: Tinta().orange("orange"), f"{ORANGE}orange{O}"),
-            ("purple", lambda: Tinta().purple("purple"), f"{PURPLE}purple{O}"),
-            ("pink", lambda: Tinta().pink("pink"), f"{PINK}pink{O}"),
-            ("gray", lambda: Tinta().gray("gray"), f"{GRAY}gray{O}"),
-            ("dark_gray", lambda: Tinta().dark_gray("dark_gray"), f"{D_GRAY}dark_gray{O}"),
-            ("light_gray", lambda: Tinta().light_gray("light_gray"), f"{L_GRAY}light_gray{O}"),
-            ("white", lambda: Tinta().white("white"), f"{WHITE}white{O}"),
-            # fmt: on
-        ],
+        basic_colors,
     )
-    def test_colors(self, color, Testa, expected):
+    def test_print_colors(self, color, Testa, expected, perf):
         Testa().print()
+
+    @pytest.mark.parametrize(
+        "color,Testa,expected",
+        basic_colors,
+    )
+    def test_check_output(self, color, Testa, expected, perf):
         assert Testa().to_str() == expected
 
+    def test_sandwich_colors(self):
+        assert (
+            Tinta("plain").green("green").default("plain").to_str()
+            == f"plain {GREEN}green{O} plain"
+        )
+
+    def test_clear_resets_color(self):
+        Tinta().green("green").clear("plain").print()
+        assert (
+            Tinta().green("green").clear("plain")("string").to_str()
+            == f"{GREEN}green{O} plain string"
+        )
+
+
+class TestBasicStylizing:
+
+    def test_bold(self):
+        b = Tinta().bold("bold")
+        assert b.to_str() == f"{BOLD}bold{O}"
+        b.print()
+
+        b = Tinta().b("bold")
+        assert b.to_str() == f"{BOLD}bold{O}"
+        b.print()
+
+    def test_normal_resets_bold(self):
+        b = Tinta().bold("bold").normal("normal")
+        assert b.to_str() == f"{BOLD}bold{O} normal"
+        b.print()
+
+    def test_bold_resets_bold(self):
+        b = Tinta("To").bold().red("boldly").bold().white("go")
+        assert b.to_str() == f"To {_stitch(BOLD, RED)}boldly{O} {WHITE}go{O}"
+        b.print()
+
+    def test_bold_resets_only_bold(self):
+        b = Tinta("To").bold().underline().red("boldly").bold().white("go")
+        assert (
+            b.to_str()
+            == f"To {_stitch(BOLD, UNDERLINE, RED)}boldly{BOLD_OFF} {WHITE}go{O}"
+        )
+        b.print()
+
+    def test_underline(self):
+        u = Tinta().underline("underline")
+        assert u.to_str() == f"{UNDERLINE}underline{O}"
+        u.print()
+
+        _ = Tinta()._("underscore")
+        assert _.to_str() == f"{UNDERLINE}underscore{O}"
+        _.print()
+
+    def test_normal_resets_underline(self):
+        u = Tinta().underline("underline").normal("normal")
+        assert u.to_str() == f"{UNDERLINE}underline{O} normal"
+        u.print()
+
+    def test_underline_resets_underline(self):
+        u = Tinta("To")._().amber("underlinely")._().purple("go")
+        assert (
+            u.to_str() == f"To {_stitch(UNDERLINE, AMBER)}underlinely{O} {PURPLE}go{O}"
+        )
+        u.print()
+
+    def test_underline_resets_only_underline(self):
+        u = Tinta("To").underline().bold().amber("underlinely").underline().olive("go")
+        assert (
+            u.to_str()
+            == f"To {_stitch(BOLD, UNDERLINE, AMBER)}underlinely{UNDERLINE_OFF} {OLIVE}go{O}"
+        )
+        u.print()
+
+    def test_dim(self):
+        d = Tinta().dim("dim")
+        assert d.to_str() == f"{DIM}dim{O}"
+        d.print()
+
+    def test_normal_resets_dim(self):
+        t = Tinta().dim("dim").normal("normal")
+        assert t.to_str() == f"{DIM}dim{O} normal"
+        t.print()
+
+    def test_dim_resets_dim(self):
+        d = Tinta("To").dim().olive("dimly").dim().blue("go")
+        assert d.to_str() == f"To {_stitch(DIM, OLIVE)}dimly{O} {BLUE}go{O}"
+        d.print()
+
+    def test_dim_resets_only_dim(self):
+        d = Tinta("To").dim().underline().olive("dimly").dim().blue("go")
+        assert (
+            d.to_str()
+            == f"To {_stitch(DIM, UNDERLINE, OLIVE)}dimly{DIM_OFF} {BLUE}go{O}"
+        )
+        d.print()
+
+    def test_strikethrough(self):
+        s = Tinta().strikethrough("strikethrough")
+        assert s.to_str() == f"{STRIKE}strikethrough{O}"
+        s.print()
+
+    def test_normal_resets_strikethrough(self):
+        s = Tinta().strikethrough("strikethrough").normal("normal")
+        assert s.to_str() == f"{STRIKE}strikethrough{O} normal"
+        s.print()
+
+    def test_strikethrough_resets_strikethrough(self):
+        s = (
+            Tinta("To")
+            .strikethrough()
+            .olive("strikethroughly")
+            .strikethrough()
+            .blue("go")
+        )
+        assert (
+            s.to_str() == f"To {_stitch(STRIKE, OLIVE)}strikethroughly{O} {BLUE}go{O}"
+        )
+        s.print()
+
+    def test_strikethrough_resets_only_strikethrough(self):
+        s = (
+            Tinta("To")
+            .strikethrough()
+            .underline()
+            .olive("strikethroughly")
+            .strikethrough()
+            .blue("go")
+        )
+        assert (
+            s.to_str()
+            == f"To {_stitch(UNDERLINE, STRIKE, OLIVE)}strikethroughly{STRIKE_OFF} {BLUE}go{O}"
+        )
+        s.print()
+
+    def test_bold_underline(self):
+        bu = Tinta().bold("bold").underline("underline")
+        assert bu.to_str() == f"{BOLD}bold {UNDERLINE}underline{O}"
+        bu.print()
+
+    def test_bold_dim(self):
+        bd = Tinta().bold("bold").dim("dim")
+        assert bd.to_str() == f"{BOLD}bold {DIM}dim{O}"
+        bd.print()
+
+    def test_underline_dim(self):
+        ud = Tinta().underline("underline").dim("dim")
+        assert ud.to_str() == f"{UNDERLINE}underline {DIM}dim{O}"
+        ud.print()
+
+    def test_bold_underline_dim(self):
+        bud = Tinta().bold("bold").underline("underline").dim("dim")
+        assert bud.to_str() == f"{BOLD}bold {UNDERLINE}underline {DIM}dim{O}"
+        bud.print()
+
+    def test_underline_bold_dim(self):
+        ubd = Tinta().underline("underline").bold("bold").dim("dim")
+        assert ubd.to_str() == f"{UNDERLINE}underline {BOLD}bold {DIM}dim{O}"
+        ubd.print()
+
+    def test_bold_strikethrough(self):
+        bs = Tinta().bold("bold").strikethrough("strikethrough")
+        assert bs.to_str() == f"{BOLD}bold {STRIKE}strikethrough{O}"
+        bs.print()
+
+    def test_underline_strikethrough(self):
+        us = Tinta().underline("underline").strikethrough("strikethrough")
+        assert us.to_str() == f"{UNDERLINE}underline {STRIKE}strikethrough{O}"
+        us.print()
+
+    def test_bold_underline_strikethrough(self):
+        bus = Tinta().bold("bold").underline("underline").strikethrough("strikethrough")
+        assert (
+            bus.to_str() == f"{BOLD}bold {UNDERLINE}underline {STRIKE}strikethrough{O}"
+        )
+        bus.print()
+
+    def test_styles_remain_until_normal(self):
+        assert (
+            Tinta()
+            .bold("bold")
+            .underline("underline")
+            .dim("dim")
+            .pink("pink")
+            .normal()
+            .pink("pink")
+            .to_str()
+            == f"{BOLD}bold {UNDERLINE}underline {DIM}dim {PINK}pink{_stitch(BOLD_OFF, UNDERLINE_OFF)} pink{O}"
+        )
+
 
 class TestChaining:
 
     @pytest.mark.parametrize(
         "Testa, kwargs, expected",
         [
             # fmt: off
@@ -133,27 +346,32 @@
         [
             (
                 lambda: Tinta().mint("Mint\nice cream"),
                 f"{MINT}Mint\nice cream{O}",
             ),
             (
                 lambda: Tinta().mint("Mint").white("\nice cream\nis the")._("\nbest"),
-                f"{MINT}Mint{WHITE}\nice cream\nis the\x1b[38;5;255;4m\nbest{O}",
+                f"{MINT}Mint{WHITE}\nice cream\nis the{UNDERLINE}\nbest{O}",
             ),
             (
                 lambda: Tinta("\n").mint("Mint\n").white("ice cream is the")._("best"),
-                f"\n{MINT}Mint\n{WHITE}ice cream is the \x1b[38;5;255;4mbest{O}",
+                f"\n{MINT}Mint\n{WHITE}ice cream is the {UNDERLINE}best{O}",
             ),
         ],
     )
     def test_newlines_in_chaining(self, Testa: Callable[[], Tinta], expected: str):
         s = Testa().to_str()
         Testa().print()
         assert s == expected
 
+    def test_chaining_same_styles_doesnt_dupe(self):
+        t = Tinta().green("green").green("green").green("green")
+        assert t.to_str() == f"{GREEN}green green green{O}"
+        t.print()
+
 
 class TestUnicode:
 
     def test_unicode(self):
         Tinta().pink("I ♡ Unicorns").print()
         assert Tinta().pink("I ♡ Unicorns").to_str() == f"{PINK}I ♡ Unicorns{O}"
 
@@ -166,27 +384,35 @@
         )
 
     def test_emoji(self):
         Tinta("🦄").print()
         assert Tinta("🦄").to_str() == "🦄"
 
     def test_emoji_with_color(self):
-        Tinta().purple("🦄").print()
+        t = Tinta().purple("🦄")
         assert Tinta().purple("🦄").to_str() == f"{PURPLE}🦄{O}"
+        t.print()
 
     def test_emoji_with_color_and_clear(self):
-        Tinta().pink("🦄").clear("🦄").print()
-        assert Tinta().pink("🦄").clear("🦄").to_str(sep="") == f"{PINK}🦄\x1b[0m🦄{O}"
+        t = Tinta().pink("🦄").clear("🦄")
+        assert t.to_str(sep="") == f"{PINK}🦄{O}🦄"
+        t.print(sep="")
 
-    def test_emoji_with_color_and_clear_and_emoji(self):
-        Tinta().purple("🦄").clear("🦄").pink("🦄").print()
+    def test_emoji_with_color_style_and_normal(self):
+        t = Tinta().purple()._("🦄").normal("🦄").pink("🦄")
         assert (
-            Tinta().purple("🦄").clear("🦄").pink("🦄").to_str()
-            == f"{PURPLE}🦄 \x1b[0m🦄 {PINK}🦄{O}"
+            t.to_str()
+            == f"{_stitch(UNDERLINE, PURPLE)}🦄{UNDERLINE_OFF} 🦄 {PINK}🦄{O}"
         )
+        t.print()
+
+    def test_emoji_with_color_style_and_clear(self):
+        t = Tinta().purple()._("🦄").clear("🦄").pink("🦄")
+        assert t.to_str() == f"{_stitch(UNDERLINE, PURPLE)}🦄{O} 🦄 {PINK}🦄{O}"
+        t.print()
 
 
 class TestLowerLevel:
 
     ITS_NOT_EASY = "it's not easy being green"
 
     def assert_its_not_easy_being_green(self, out: str):
@@ -239,19 +465,25 @@
 
 
 class TestExamples:
 
     def test_basic_example(self):
         from examples.basic_example import basic
 
+        Tinta._initialized = False
+        Tinta._colors._initialized = False
+
         basic()
 
     def test_complete_example(self):
         from examples.complete_example import complete
 
+        Tinta._initialized = False
+        Tinta._colors._initialized = False
+
         complete()
 
 
 class TestWhiteSpace:
 
     def test_print_whitespace(self):
         Tinta(" ").print()
@@ -595,25 +827,38 @@
 
         assert len(t.parts) == 0
 
         t.pop(2)  # Shouldn't error if we remove more than we have
 
         assert len(t.parts) == 0
 
-    def test_zero_handles_clear(self):
+    def test_pop_updates_current_style(self):
+        t = Tinta().green("green").red("red").blue("blue")
+        t.pop()
+        assert t.to_str(plaintext=True) == "green red"
+        t.pop()
+        assert t.to_str(plaintext=True) == "green"
+        t.pop()
+        assert t.to_str(plaintext=True) == ""
+
+        t = Tinta().green("green").red("red").blue("blue").bold("bold n' blue")
+        t.pop(2)
+        assert t._styler == Tinta.Styler(color=RED)
+
+    def test_tint_handles_zero(self):
         s = (
-            Tinta("White")
-            .red("Red")
-            .green("Green")
-            .blue("Blue")
-            .tint(0, "Clear")
+            Tinta("white")
+            .red("red")
+            .green("green")
+            .blue("blue")
+            .tint(0, "default")
             .to_str(sep=" ")
         )
         print(s)
-        assert s == f"White {RED}Red {GREEN}Green {BLUE}Blue {O}Clear{O}"
+        assert s == f"white {RED}red {GREEN}green {BLUE}blue{O} default"
 
 
 class TestUtils:
 
     @pytest.mark.parametrize(
         "Testa,expected",
         [
@@ -693,7 +938,111 @@
                 " ",
                 f"{' '*70} a {PURPLE}b {PINK}c d {MINT}e{O}",
             ),
         ],
     )
     def test_rjust(self, Testa: Callable, rjust: int, fillchar: str, expected: str):
         assert Tinta.rjust(Testa().to_str(), rjust, fillchar) == expected
+
+
+class TestTiming:
+
+    def test_basic_time_against_raw(self):
+        base_start = time.perf_counter()
+        print(
+            f"{BLUE}blue {GREEN}green {L_BLUE}light blue {YELLOW}yellow {AMBER}amber {MINT}mint {OLIVE}olive {ORANGE}orange {PURPLE}purple {PINK}pink {GRAY}gray {D_GRAY}dark gray {L_GRAY}light gray {WHITE}white{O}"
+        )
+        base_end = time.perf_counter()
+
+        tinta_start = time.perf_counter()
+
+        (
+            Tinta()
+            .blue("blue")
+            .green("green")
+            .light_blue("light blue")
+            .yellow("yellow")
+            .amber("amber")
+            .mint("mint")
+            .olive("olive")
+            .orange("orange")
+            .purple("purple")
+            .pink("pink")
+            .gray("gray")
+            .dark_gray("dark gray")
+            .light_gray("light gray")
+            .white("white")
+            .print()
+        )
+        tinta_end = time.perf_counter()
+
+        raw_diff = base_end - base_start
+        tinta_diff = tinta_end - tinta_start
+
+        print(f"Raw: {raw_diff:.4f} seconds")
+        print(f"Tinta: {tinta_diff:.4f} seconds")
+
+        assert tinta_diff - raw_diff < 0.001
+
+    def test_with_timeit(self):
+
+        count = 500
+
+        tinta_time = timeit.timeit(
+            lambda: Tinta()
+            .blue("blue")
+            .green("green")
+            .light_blue("light blue")
+            .yellow("yellow")
+            .amber("amber")
+            .mint("mint")
+            .olive("olive")
+            .orange("orange")
+            .purple("purple")
+            .pink("pink")
+            .gray("gray")
+            .dark_gray("dark gray")
+            .light_gray("light gray")
+            .white("white")
+            .print(),
+            number=count,
+        )
+
+        class FakeClass:
+            def __init__(self):
+                self.blue = "blue"
+                self.green = "green"
+                self.light_blue = "light blue"
+                self.yellow = "yellow"
+                self.amber = "amber"
+                self.mint = "mint"
+                self.olive = "olive"
+                self.orange = "orange"
+                self.purple = "purple"
+                self.pink = "pink"
+                self.gray = "gray"
+                self.dark_gray = "dark gray"
+                self.light_gray = "light gray"
+                self.white = "white"
+
+            def print(self):
+                print(
+                    f"{BLUE}{self.blue} {GREEN}{self.green} {L_BLUE}{self.light_blue} {YELLOW}{self.yellow} {AMBER}{self.amber} {MINT}{self.mint} {OLIVE}{self.olive} {ORANGE}{self.orange} {PURPLE}{self.purple} {PINK}{self.pink} {GRAY}{self.gray} {D_GRAY}{self.dark_gray} {L_GRAY}{self.light_gray} {WHITE}{self.white}{O}"
+                )
+
+        class_time = timeit.timeit(
+            lambda: FakeClass().print(),
+            number=count,
+        )
+
+        raw_time = timeit.timeit(
+            lambda: print(
+                f"{BLUE}blue {GREEN}green {L_BLUE}light blue {YELLOW}yellow {AMBER}amber {MINT}mint {OLIVE}olive {ORANGE}orange {PURPLE}purple {PINK}pink {GRAY}gray {D_GRAY}dark gray {L_GRAY}light gray {WHITE}white{O}"
+            ),
+            number=count,
+        )
+
+        print(f"Raw: {raw_time:.4f} seconds")
+        print(f"Class: {class_time:.4f} seconds")
+        print(f"Tinta: {tinta_time:.4f} seconds")
+
+        assert tinta_time - raw_time < 0.5
```

### Comparing `tinta-0.1.7b4.post0/tinta/__init__.py` & `tinta-0.1.7b5/tinta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = "0.1.7b4-post0"
+__version__ = "0.1.7b5"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 
     assert bool(Tinta)
```

### Comparing `tinta-0.1.7b4.post0/tinta/__main__.py` & `tinta-0.1.7b5/tinta/__main__.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/tinta/colorize.py` & `tinta-0.1.7b5/tinta/stylize.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,45 +15,41 @@
 
 # This module is a modified version of the original AnsiColors module, and further
 # modified by github.com/brandoncript to be used in the Tinta project. It is
 # distributed under the same license as the original module, as well as the
 # MIT License.
 
 import re
-from typing import Any, List, Optional, overload, Tuple, TYPE_CHECKING, Union
+from typing import (
+    Any,
+    cast,
+    List,
+    Optional,
+    overload,
+    Tuple,
+    TYPE_CHECKING,
+    Union,
+)
 
-from .constants import ANSI_RESET_HEX, ANSI_RESET_OCT, SEP
-from .typ import MissingColorError
+from .constants import ANSI_RESET, ANSI_RESET_OCT, ANSI_STYLES, ANSI_STYLES_OFF, SEP
+from .typ import InvalidStyleError
 
 if TYPE_CHECKING:
     from .tinta import Tinta
 
-STYLES = (
-    "none",
-    "bold",
-    "faint",
-    "italic",
-    "underline",
-    "blink",
-    "blink2",
-    "negative",
-    "concealed",
-    "crossed",
-)
-
 
 def was_reset(s: str) -> bool:
-    return s.strip().endswith(ANSI_RESET_HEX) or s.endswith(ANSI_RESET_OCT)
+    return s.strip().endswith(ANSI_RESET) or s.endswith(ANSI_RESET_OCT)
 
 
-def ensure_reset(s: str) -> str:
-    if was_reset(s):
+def ensure_reset(s: str, np: "Union[Tinta.Part, None]" = None) -> str:
+    if was_reset(s) or (np and np.has_formatting):
         return s
     last_char_idx = len(s.rstrip())
-    return f"{s[:last_char_idx]}{ANSI_RESET_HEX}{s[last_char_idx:]}"
+    return f"{s[:last_char_idx]}{ANSI_RESET}{s[last_char_idx:]}"
 
 
 def _parse_rgb(s: str) -> Tuple[int, ...]:
     if not isinstance(s, str):
         raise ValueError(f"Could not parse color '{s}'")
     s = s.strip().replace(" ", "").lower()
 
@@ -79,33 +75,37 @@
 def _join(*values: Union[int, str]) -> str:
     """
     Join a series of values with semicolons. The values
     are either integers or strings, so stringify each for
     good measure. Worth breaking out as its own function
     because semicolon-joined lists are core to ANSI coding.
     """
-    return ";".join(str(v) for v in values)
+    return ";".join(str(v) for v in values).strip(";").strip()
 
 
 def _color_code(
     spec: Union[str, int, Tuple[int, int, int], List[int]], base: int
 ) -> str:
-    """
-    Workhorse of encoding a color. Give preference to named colors from
+    """Workhorse of encoding a color. Give preference to named colors from
     ANSI, then to specific numeric or tuple specs. If those don't work,
     try looking up look CSS color names or parsing CSS hex and rgb color
     specifications.
 
-    :param spec: Unparsed color specification
-    :param base: Either 30 or 40, signifying the base value
-        for color encoding (foreground and background respectively).
-        Low values are added directly to the base. Higher values use `
-        base + 8` (i.e. 38 or 48) then extended codes.
-    :returns: Discovered ANSI color encoding.
-    :raises: ValueError if cannot parse the color spec.
+    Args:
+        spec: Unparsed color specification
+        base (int): Either 30 or 40, signifying the base value
+                    for color encoding (foreground and background respectively).
+                    Low values are added directly to the base. Higher values use `
+                    base + 8` (i.e. 38 or 48) then extended codes.
+
+    Returns:
+        Discovered ANSI color encoding.
+
+    Raises:
+        ValueError if cannot parse the color spec.
     """
     if isinstance(spec, str):
         spec = spec.strip().lower()
 
     if spec == "default" or spec == 0:
         return "0"
     elif isinstance(spec, int) and 1 <= spec <= 255:
@@ -116,110 +116,189 @@
         rgb = _parse_rgb(str(spec))
         # parse_rgb raises ValueError if cannot parse spec
         return _join(base + 8, 2, _join(*rgb))
     else:
         raise ValueError(f"Could not parse color '{spec}'")
 
 
-def colorize(
-    s: str,
-    fg: Optional[int] = None,
-    bg: Optional[int] = None,
-    style: Optional[str] = None,
-    reset: bool = False,
-) -> str:
-    """
-    Add ANSI colors and styles to a string.
+def _style_name(code: int) -> str:
+    try:
+        return ANSI_STYLES[code]
+    except IndexError:
+        raise InvalidStyleError(f"Invalid style code '{code}'")
+
+
+def _style_codes(style: Union[str, int]) -> Tuple[int, int]:
+    if isinstance(style, str):
+        style = style.lower()
+    on = ANSI_STYLES.index(style) + 1
+    off = next((c for i, c in ANSI_STYLES_OFF for s in i if s == style), 0)
+    return on, off
+
+
+def ansi_styles(style: Union[str, int]) -> Tuple[str, str]:
+    """Returns ANSI on and off strings for a style name or code.
 
     Args:
-    s: String to format.
-    fg: Foreground color specification.
-    bg: Background color specification.
-    style: Style names, separated by '+'
-    reset: Whether to reset the formatting at the end of the string. Default is False.
-
-    Returns: Formatted string.
-    """
-    codes: List[str] = []
-
-    if fg is not None:
-        codes.append(_color_code(fg, 30))
-    # TODO: Background is not implemented
-    # if bg is not None:
-    #     codes.append(_color_code(bg, 40))
-    if style is not None:
-        for style_part in style.split("+"):
-            if style_part in STYLES:
-                codes.append(str(STYLES.index(style_part)))
-            else:
-                raise ValueError(f'Invalid style "{style_part}"')
-
-    if codes:
-        template = "\x1b[{0}m{1}"
-        if reset:
-            template += ANSI_RESET_HEX
-        return template.format(_join(*codes), s)
-    else:
-        return s
+        style (str | int): A style name or code.
+
+    Returns:
+        Tuple[str, str]: The on and off ANSI codes for the style.
+    """
+    on, off = _style_codes(style)
+    return f"\x1b[{on}m", f"\x1b[{off}m"
+
+
+def validate_styles(*styles: Union[int, str]) -> Tuple[str, ...]:
+    """Validates a list of style names. If a style is not found in the ANSI
+    styles, it is removed from the list.
+    """
+
+    _styles: List[Union[int, str]] = list(styles)
+
+    if next((isinstance(s, int) for s in styles), False):
+        _styles = [_style_name(int(s)) for s in _styles]
+
+    _styles = [str(s).lower() for s in _styles]
+
+    if not all([s in ANSI_STYLES for s in _styles]):
+        available_styles = ", ".join([f"'{s}'" for s in ANSI_STYLES])
+        err = f"Invalid style string '{_styles}', must be one of {available_styles}."
+        raise InvalidStyleError(err)
+
+    return cast(Tuple[str, ...], tuple(_styles))
 
 
 @overload
 def tint(
     instance: "Tinta", *s: Any, color: Union[str, int], sep: str = SEP
 ) -> "Tinta": ...
 
 
 @overload
 def tint(
     instance: "Tinta", color: Union[str, int], *s: Any, sep: str = SEP
 ) -> "Tinta": ...
 
 
-# pylint: disable=redefined-outer-name
 def tint(instance: "Tinta", *args, **kwargs) -> "Tinta":
     """Adds segments of text colored with the specified color.
     Can be used in place of calling named color methods.
 
     Args:
         instance (Tinta): The Tinta instance.
         color (str | int, optional): A color name or ANSI color index. Defaults to first argument.
         *s: Any: Segments of text to add.
         sep (str, optional): Used to join strings. Defaults to ' '.
 
     Returns:
         self
     """
+    from .tinta import Tinta
 
-    # color: Optional[Union[str, int]] = None, *s: Any, sep: str = SEP
+    if not isinstance(instance, Tinta):
+        raise AttributeError("tint() must be called from a Tinta instance.")
 
-    # check if the first argument is a known color or valid ANSI code, or comes from kwargs
     self = instance
+
+    # check if the first argument is a known color or valid ANSI code, or comes from kwargs
     s = args
     color = kwargs.get("color", None)
     sep = kwargs.get("sep", SEP)
     if color is None:
         if not len(s) > 1:
             raise AttributeError(
                 "If no color is specified, tint() requires at least two arguments."
             )
-        if args and isinstance(args[0], (str, int)):
-            color = s[0]
-            s = s[1:]
+        color = s[0]
+        s = s[1:]
+
+    self.set_color(color)
+    self.push(*s, sep=sep)
+    return self
+
+
+def stylize(
+    s: Optional[str],
+    lp: "Union[Tinta.Part, None]",
+    mp: "Tinta.Part",
+    np: "Union[Tinta.Part, None]",
+) -> str:
+    """Wraps a string with ANSI styles.
+
+    Args:
+        s (str): The string to format - may be plain or pre-formatted.
+        lp (Tinta.Part): The previous part.
+        mp (Tinta.Part): The current (middle) part.
+        np (Tinta.Part): The next part.
+    """
+
+    if s is None:
+        s = ""
+
+    if not mp:
+        return s
+
+    # On
+    on = ""
+    if mp.has_formatting:
+        if not lp or not lp.has_formatting:
+            on = _join(*[_style_codes(st)[0] for st in mp.style])
         else:
-            raise AttributeError(
-                "Could not determine color from arguments. Either pass a color as the first argument, or use the color keyword argument."
+            if mp.style != lp.style:
+                on = _join(
+                    *[_style_codes(st)[0] for st in mp.style if st not in lp.style]
+                )
+        if mp.color_code and (not lp or (mp.color_code != lp.color_code)):
+            on = _join(on, _color_code(mp.color_code, 30))
+
+    # Off
+    off = ""
+    if mp.has_formatting:
+        if (
+            not np
+            or not np.has_formatting
+            or mp.styler._force_clear
+            or bool(mp.style and not np.style and mp.color_code != np.color_code)
+        ):
+            off = "0"
+        elif mp.style != np.style:
+            styles_not_in_n = [s for s in mp.style if s not in np.style]
+            off = _join(
+                *list(sorted(set([_style_codes(st)[1] for st in styles_not_in_n])))
             )
 
-    # if color is numeric integer string, assume it's an ANSI color code
-    if isinstance(color, int) or (isinstance(color, str) and color.isdigit()):
-        self.color = int(color)
-
-    # Check if color_name is a valid color if color is a string
-    if isinstance(color, str):
-        if not hasattr(self.colors, color):  # type: ignore
-            raise MissingColorError(
-                f"Invalid color name: {color}. Is it in colors.ini?"
-            )
-        self.color = self.colors.get(color)  # type: ignore
+    # Apply formatting
+    left = f"\x1b[{on}m" if on else ""
+    right = f"\x1b[{off}m" if off else ""
 
-    self.push(*s, sep=sep)
-    return self
+    last_char_idx = len(s.rstrip())
+
+    return f"{left}{s[:last_char_idx]}{right}{s[last_char_idx:]}"
+
+
+def is_ansi_str(s: str) -> bool:
+    return s.startswith("\x1b[") or s.startswith("\033[")
+
+
+def ansi_color_to_int(s: str) -> int:
+    """Converts an ANSI escape sequence to a base 10 integer. Accepts both octal and decimal sequences, and from 1 to 3 segments separated by semicolons."""
+
+    if not is_ansi_str(s):
+        raise ValueError(f"String '{s}' is not an ANSI escape sequence.")
+
+    if s.startswith("\x1b["):
+        s = s[2:]
+    elif s.startswith("\033["):
+        s = s[3:]
+
+    if s.endswith("m"):
+        s = s[:-1]
+
+    seg = s.split(";")
+    if len(seg) >= 3:
+        ch = seg[-3]
+        if ch == "38" or ch == "48":
+            return int(seg[-1])
+        return int(seg[-1])
+
+    raise ValueError(f"Could not parse ANSI escape sequence '{s}'")
```

### Comparing `tinta-0.1.7b4.post0/tinta/constants.py` & `tinta-0.1.7b5/tinta/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,13 +18,36 @@
 
 import os
 
 from .typ import parse_bool
 
 CURSOR_UP_ONE = "\x1b[1A"
 ERASE_LINE = "\x1b[2K"
-ANSI_RESET_HEX = "\x1b[0m"
+ANSI_RESET = "\x1b[0m"
 ANSI_RESET_OCT = "\033[0m"
 SEP = os.getenv("TINTA_SEPARATOR", " ")
 STEALTH = parse_bool(os.getenv("TINTA_STEALTH", False))
 PREFER_PLAINTEXT = parse_bool(os.getenv("TINTA_PLAINTEXT", False))
 SMART_FIX_PUNCTUATION = parse_bool(os.getenv("TINTA_SMART_FIX_PUNCTUATION", True))
+PERF_MEASURE = parse_bool(os.getenv("TINTA_PERF_MEASURE", True))
+
+ANSI_COLORS = ("black", "red", "green", "yellow", "blue", "magenta", "cyan", "white")
+ANSI_STYLES = (
+    "bold",
+    "dim",
+    "italic",
+    "underline",
+    "blink",
+    "rapid_blink",
+    "invert",
+    "conceal",
+    "strikethrough",
+)
+ANSI_STYLES_OFF = (
+    (("reset", "normal", "clear", 0), 0),
+    (("bold", "dim", 1, 2), 22),
+    (("italic", 3), 23),
+    (("underline", 4), 24),
+    (("invert", 7), 27),
+    (("strikethrough", 9), 29),
+)
+PUNC = [".", ",", ";", ":", "!", "?"]
```

### Comparing `tinta-0.1.7b4.post0/tinta/discover.py` & `tinta-0.1.7b5/tinta/discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/tinta/multi_version_imports.py` & `tinta-0.1.7b5/tinta/multi_version_imports.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,21 +21,13 @@
 
     P = ParamSpec("P")
     R = TypeVar("R")  # type: ignore
     GenericCallable = Callable[P, R]
 else:
     GenericCallable = Any
 
-# Deprecated
-try:
-    from warnings import deprecated
-except ImportError:
-    from deprecated import deprecated
-deprecated = deprecated
-
 all = [
-    deprecated,
     GenericCallable,
     Literal,
     T,
     TypeVar,
 ]
```

### Comparing `tinta-0.1.7b4.post0/tinta/typ.py` & `tinta-0.1.7b5/tinta/typ.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,26 @@
 
 class MissingColorError(Exception):
     """Raised when a color is not found in the colors.ini file."""
 
     pass
 
 
+class InvalidStyleError(Exception):
+    """Raised when an invalid style is passed to a function."""
+
+    pass
+
+
+class InvalidColorError(Exception):
+    """Raised when an invalid color is passed to a function."""
+
+    pass
+
+
 def copy_kwargs(func: GenericCallable) -> Callable[..., GenericCallable]:
     """Decorator does nothing but casts the original function to match the given function signature"""
 
     @functools.wraps(func, updated=())
     def _cast_func(_func: Callable[..., Any]) -> GenericCallable:
         return cast(GenericCallable, _func)
```

### Comparing `tinta-0.1.7b4.post0/.gitignore` & `tinta-0.1.7b5/.gitignore`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/LICENSE` & `tinta-0.1.7b5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b4.post0/README.md` & `tinta-0.1.7b5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b4-post0-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b5-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -189,15 +189,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b4-post0 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b5 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -224,15 +224,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b4-post0 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b5 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
 
@@ -347,15 +347,15 @@
 
 ## Running Tests
 
 To run tests, run the following command:
 
 ```bash
 pip install pytest
-python -m pytest -xv
+python -m pytest -v
 ```
 
 ## Contributing
 
 Contributions are welcome! Please send in a PR with a clear explanation of what you're adding and why, and where applicable, add tests to validate. Please read our [_code of conduct_](CODE_OF_CONDUCT.md) before contributing.
 
 ## Acknowledgements
```

### Comparing `tinta-0.1.7b4.post0/pyproject.toml` & `tinta-0.1.7b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 [project]
 name = "tinta"
-version = "0.1.7b4-post0"
+version = "0.1.7b5"
 description = "Tinta, a magical console output tool."
 authors = [{ name = "Brandon Shelley", email = "brandon@pacificaviator.co" }]
 license = "MIT"
 readme = "README.md"
-dependencies = ["deprecated==1.2.14"]
+dependencies = []
 keywords = [
   "console",
   "colors",
   "ansi",
   "print",
   "term",
   "cli",
@@ -64,15 +64,14 @@
 [tool.hatchling.build]
 packages = ["tinta"]
 include = ["tinta/**/*.py", "tinta/**/*.pyi", "tinta/colors.ini", "/tests"]
 exclude = [".*", "dist"]
 
 [tool.hatchling.dependencies]
 python = "^3.6"
-deprecated = "^1.2.14"
 
 [tool.hatchling.dev-dependencies]
 pytest = "^6.2.4"
 twine = "^3.4.2"
 wheel = "^0.36.2"
 
 [tool.mypy]
```

### Comparing `tinta-0.1.7b4.post0/PKG-INFO` & `tinta-0.1.7b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinta
-Version: 0.1.7b4.post0
+Version: 0.1.7b5
 Summary: Tinta, a magical console output tool.
 Project-URL: homepage, https://github.com/brandonscript/tinta
 Project-URL: repository, https://github.com/brandonscript/tinta
 Author-email: Brandon Shelley <brandon@pacificaviator.co>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ansi,cli,colors,console,development,print,term,terminal
@@ -17,24 +17,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Utilities
-Requires-Dist: deprecated==1.2.14
 Description-Content-Type: text/markdown
 
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b4-post0-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b5-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -215,15 +214,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b4-post0 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b5 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -250,15 +249,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b4-post0 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b5 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
 
@@ -373,15 +372,15 @@
 
 ## Running Tests
 
 To run tests, run the following command:
 
 ```bash
 pip install pytest
-python -m pytest -xv
+python -m pytest -v
 ```
 
 ## Contributing
 
 Contributions are welcome! Please send in a PR with a clear explanation of what you're adding and why, and where applicable, add tests to validate. Please read our [_code of conduct_](CODE_OF_CONDUCT.md) before contributing.
 
 ## Acknowledgements
```

