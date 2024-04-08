# Comparing `tmp/jupyterlab_judge-1.24.1.tar.gz` & `tmp/jupyterlab_judge-1.24.2.tar.gz`

## Comparing `jupyterlab_judge-1.24.1.tar` & `jupyterlab_judge-1.24.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.copier-answers.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.yarnrc.yml
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/CHANGELOG.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/babel.config.js
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/conftest.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jest.config.js
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/setup.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/tsconfig.test.json
--rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyter-config/nb-config/jupyterlab_judge.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyter-config/server-config/jupyterlab_judge.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/_version.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/handlers.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/yjudge.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/package.json
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
--rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
--rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
--rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
--rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
--rw-r--r--   0        0        0    33276 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/960.248f24628be1ecbf1885.js
--rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/remoteEntry.5b4a6b2fd107c17f4d34.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/style.js
--rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/tests/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/tests/test_handlers.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/schema/plugin.json
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/commands.ts
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/constants.ts
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/handler.ts
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/index.ts
--rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/model.ts
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/tokens.ts
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/toolbar.tsx
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/__tests__/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionArea.tsx
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionControl.tsx
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItem.tsx
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItemStatus.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItemWait.tsx
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItemWaitStatus.tsx
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionList.tsx
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/index.ts
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/problemProvider/HardCodedProblemProvider.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/problemProvider/index.ts
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/problemProvider/problemProvider.ts
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeOutputArea.ts
--rw-r--r--   0        0        0    22446 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgePanel.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeProblemPanel.ts
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeSubmissionArea.tsx
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeTerminal.ts
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/index.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/judgeOutputArea.css
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/judgePanel.css
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/judgeTerminal.css
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/tests/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/LICENSE
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/pyproject.toml
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/.copier-answers.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/.yarnrc.yml
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/babel.config.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/conftest.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jest.config.js
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/tsconfig.test.json
+-rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyter-config/nb-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyter-config/server-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/_version.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/handlers.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/yjudge.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/package.json
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
+-rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
+-rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
+-rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
+-rw-r--r--   0        0        0    33282 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/960.46ea7479e4e32d5c60b4.js
+-rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/remoteEntry.72928ca07b9aae9d28c1.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/style.js
+-rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/tests/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/jupyterlab_judge/tests/test_handlers.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/schema/plugin.json
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/commands.ts
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/constants.ts
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/handler.ts
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/index.ts
+-rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/model.ts
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/tokens.ts
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/toolbar.tsx
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/__tests__/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionArea.tsx
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionControl.tsx
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionItem.tsx
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionItemStatus.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionItemWait.tsx
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionItemWaitStatus.tsx
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/SubmissionList.tsx
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/components/index.ts
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/problemProvider/HardCodedProblemProvider.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/problemProvider/index.ts
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/problemProvider/problemProvider.ts
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/widgets/JudgeOutputArea.ts
+-rw-r--r--   0        0        0    22452 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/widgets/JudgePanel.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/widgets/JudgeProblemPanel.ts
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/widgets/JudgeSubmissionArea.tsx
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/widgets/JudgeTerminal.ts
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/src/widgets/index.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/style/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/style/judgeOutputArea.css
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/style/judgePanel.css
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/style/judgeTerminal.css
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/ui-tests/tests/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/LICENSE
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/pyproject.toml
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.2/PKG-INFO
```

### Comparing `jupyterlab_judge-1.24.1/.copier-answers.yml` & `jupyterlab_judge-1.24.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/CHANGELOG.md` & `jupyterlab_judge-1.24.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 1.24.1
+## 1.24.2
 
-No merged PRs
+([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.1...bb8c572290dcd744d538cf09d98459c85bdbd4ac))
+
+### Merged PRs
+
+- fix: add prompt parameter to input function [#56](https://github.com/team-monolith-product/jupyterlab-judge/pull/56) ([@a3626a](https://github.com/a3626a))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-04-05&to=2024-04-08&type=c))
+
+[@a3626a](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Aa3626a+updated%3A2024-04-05..2024-04-08&type=Issues)
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 1.24.1
+
+No merged PRs
+
 ## 1.24.0
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.23.0...79c3c0c4960119fb18d7d5af68ab1734edb4d1d6))
 
 ### Merged PRs
 
 - Implement robust input mechanism [#55](https://github.com/team-monolith-product/jupyterlab-judge/pull/55) ([@a3626a](https://github.com/a3626a))
```

### Comparing `jupyterlab_judge-1.24.1/RELEASE.md` & `jupyterlab_judge-1.24.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jest.config.js` & `jupyterlab_judge-1.24.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/package.json` & `jupyterlab_judge-1.24.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.24.2'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.1"
+    "version": "1.24.2"
 }
```

### Comparing `jupyterlab_judge-1.24.1/tsconfig.json` & `jupyterlab_judge-1.24.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/yarn.lock` & `jupyterlab_judge-1.24.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/__init__.py` & `jupyterlab_judge-1.24.2/jupyterlab_judge/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/handlers.py` & `jupyterlab_judge-1.24.2/jupyterlab_judge/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/yjudge.py` & `jupyterlab_judge-1.24.2/jupyterlab_judge/yjudge.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/package.json` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796666666666667%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.72928ca07b9aae9d28c1.js'}}",*

 * * "'version'": "'1.24.2'"}*

```diff
@@ -135,15 +135,15 @@
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/team-monolith-product/jupyterlab-judge",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5b4a6b2fd107c17f4d34.js",
+            "load": "static/remoteEntry.72928ca07b9aae9d28c1.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_judge"
                 },
@@ -236,9 +236,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.1"
+    "version": "1.24.2"
 }
```

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.24.2'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.1"
+    "version": "1.24.2"
 }
```

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/960.248f24628be1ecbf1885.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/960.46ea7479e4e32d5c60b4.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -297,15 +297,15 @@
                     }, this._submitted.emit({
                         widget: this,
                         submission: m,
                         problem: s
                     })
                 }
                 async runWithInput(e, t, s, n) {
-                    const o = `\nimport io\nimport base64\n\ndef input():  \t\n    r = JUDGE_INPUT_STRING_IO.${"one_line"===s.inputTransferType?"readline":"read"}()  \t\n    if not r:  \t\t\n        return ''\n    return r\n\nJUDGE_INPUT_STRING_IO = io.StringIO()\n`;
+                    const o = `\nimport io\nimport base64\n\ndef input(prompt):  \t\n    r = JUDGE_INPUT_STRING_IO.${"one_line"===s.inputTransferType?"readline":"read"}()  \t\n    if not r:  \t\t\n        return ''\n    return r\n\nJUDGE_INPUT_STRING_IO = io.StringIO()\n`;
                     await e.requestExecute({
                         code: o,
                         stop_on_error: !0
                     }, !0, {}).done;
                     const i = 1e6;
                     for (let t = 0; t < n.length; t += i) {
                         const s = n.slice(t, t + i),
```

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/remoteEntry.5b4a6b2fd107c17f4d34.js` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/remoteEntry.72928ca07b9aae9d28c1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
         732: "d368cf762f465d394900",
         747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "248f24628be1ecbf1885"
+        960: "46ea7479e4e32d5c60b4"
     } [e] + ".js?v=" + {
         29: "d2153138b471f40c1c27",
         146: "ffbfc6be3b1d44378330",
         316: "18d9e632074f3acc892c",
         378: "2c7a4a82fbc8f09f2463",
         505: "fe5d2436cfe6faec3918",
         599: "7e6937b28ad247ccde7c",
@@ -73,15 +73,15 @@
         732: "d368cf762f465d394900",
         747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "248f24628be1ecbf1885"
+        960: "46ea7479e4e32d5c60b4"
     } [e], T.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -133,15 +133,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.24.1", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.24.2", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         T.g.importScripts && (e = T.g.location + "");
         var r = T.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/third-party-licenses.json` & `jupyterlab_judge-1.24.2/jupyterlab_judge/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json` & `jupyterlab_judge-1.24.2/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po` & `jupyterlab_judge-1.24.2/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/commands.ts` & `jupyterlab_judge-1.24.2/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/handler.ts` & `jupyterlab_judge-1.24.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/index.ts` & `jupyterlab_judge-1.24.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/model.ts` & `jupyterlab_judge-1.24.2/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/tokens.ts` & `jupyterlab_judge-1.24.2/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/toolbar.tsx` & `jupyterlab_judge-1.24.2/src/toolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionArea.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionControl.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionControl.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionItem.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionItem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionItemStatus.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionItemStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionItemWait.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionItemWait.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionItemWaitStatus.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionItemWaitStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/components/SubmissionList.tsx` & `jupyterlab_judge-1.24.2/src/components/SubmissionList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/problemProvider/HardCodedProblemProvider.ts` & `jupyterlab_judge-1.24.2/src/problemProvider/HardCodedProblemProvider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/problemProvider/problemProvider.ts` & `jupyterlab_judge-1.24.2/src/problemProvider/problemProvider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/widgets/JudgeOutputArea.ts` & `jupyterlab_judge-1.24.2/src/widgets/JudgeOutputArea.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/widgets/JudgePanel.ts` & `jupyterlab_judge-1.24.2/src/widgets/JudgePanel.ts`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
 
     // Step 1: Override input function
     //         Prepare StringIO for input
     const prepareInput = `
 import io
 import base64
 
-def input():  	
+def input(prompt):  	
     r = JUDGE_INPUT_STRING_IO.${
       problem.inputTransferType === 'one_line' ? 'readline' : 'read'
     }()  	
     if not r:  		
         return ''
     return r
```

### Comparing `jupyterlab_judge-1.24.1/src/widgets/JudgeProblemPanel.ts` & `jupyterlab_judge-1.24.2/src/widgets/JudgeProblemPanel.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/widgets/JudgeSubmissionArea.tsx` & `jupyterlab_judge-1.24.2/src/widgets/JudgeSubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/src/widgets/JudgeTerminal.ts` & `jupyterlab_judge-1.24.2/src/widgets/JudgeTerminal.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/style/judgePanel.css` & `jupyterlab_judge-1.24.2/style/judgePanel.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/style/judgeTerminal.css` & `jupyterlab_judge-1.24.2/style/judgeTerminal.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/ui-tests/README.md` & `jupyterlab_judge-1.24.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/ui-tests/tests/jupyterlab_judge.spec.ts` & `jupyterlab_judge-1.24.2/ui-tests/tests/jupyterlab_judge.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/.gitignore` & `jupyterlab_judge-1.24.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/LICENSE` & `jupyterlab_judge-1.24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/README.md` & `jupyterlab_judge-1.24.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/pyproject.toml` & `jupyterlab_judge-1.24.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.1/PKG-INFO` & `jupyterlab_judge-1.24.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_judge
-Version: 1.24.1
+Version: 1.24.2
 Dynamic: Keywords
 Summary: A simple online judge for Jupyter Lab.
 Project-URL: Homepage, https://github.com/team-monolith-product/jupyterlab-judge
 Project-URL: Bug Tracker, https://github.com/team-monolith-product/jupyterlab-judge/issues
 Project-URL: Repository, https://github.com/team-monolith-product/jupyterlab-judge.git
 Author-email: ChangHwan Lee <lch@team-mono.com>
 License: BSD 3-Clause License
```

