# Comparing `tmp/novelai_python-0.4.6.tar.gz` & `tmp/novelai_python-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelai_python-0.4.6.tar", last modified: Sat Apr  6 06:10:41 2024, max compression
+gzip compressed data, was "novelai_python-0.4.7.tar", last modified: Mon Apr  8 16:26:06 2024, max compression
```

## Comparing `novelai_python-0.4.6.tar` & `novelai_python-0.4.7.tar`

### file list

```diff
@@ -1,62 +1,77 @@
--rwxr-xr-x   0        0        0    11357 2024-04-06 06:10:20.329774 novelai_python-0.4.6/LICENSE
--rwxr-xr-x   0        0        0      522 2024-04-06 06:10:20.329774 novelai_python-0.4.6/NOTICE.MD
--rwxr-xr-x   0        0        0     2854 2024-04-06 06:10:20.329774 novelai_python-0.4.6/README.md
--rw-r--r--   0        0        0     1131 2024-04-06 06:10:41.165893 novelai_python-0.4.6/pyproject.toml
--rwxr-xr-x   0        0        0     1101 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/__init__.py
--rwxr-xr-x   0        0        0     1761 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_exceptions.py
--rwxr-xr-x   0        0        0      410 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/__init__.py
--rwxr-xr-x   0        0        0      127 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/__init__.py
--rwxr-xr-x   0        0        0      828 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/generate_image.py
--rw-r--r--   0        0        0      185 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/generate_voice.py
--rwxr-xr-x   0        0        0      397 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/upscale.py
--rwxr-xr-x   0        0        0      195 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/schema.py
--rwxr-xr-x   0        0        0      128 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/__init__.py
--rwxr-xr-x   0        0        0      721 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/information.py
--rwxr-xr-x   0        0        0      204 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/login.py
--rwxr-xr-x   0        0        0     2359 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/subscription.py
--rwxr-xr-x   0        0        0     1548 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/ApiToken.py
--rwxr-xr-x   0        0        0     1628 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/JwtToken.py
--rwxr-xr-x   0        0        0     1701 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/UserAuth.py
--rwxr-xr-x   0        0        0      424 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/__init__.py
--rwxr-xr-x   0        0        0      462 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/_base.py
--rwxr-xr-x   0        0        0      624 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/__init__.py
--rwxr-xr-x   0        0        0     1082 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/ai/LICENSE
--rwxr-xr-x   0        0        0      130 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/ai/__init__.py
--rwxr-xr-x   0        0        0    34284 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/__init__.py
--rw-r--r--   0        0        0    52850 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_const.py
--rwxr-xr-x   0        0        0     3578 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_enum.py
--rwxr-xr-x   0        0        0     5306 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
--rw-r--r--   0        0        0     7379 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/__init__.py
--rw-r--r--   0        0        0     2008 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/_enum.py
--rwxr-xr-x   0        0        0     8223 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/upscale.py
--rwxr-xr-x   0        0        0      945 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/schema.py
--rwxr-xr-x   0        0        0      130 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/__init__.py
--rwxr-xr-x   0        0        0     4772 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/information.py
--rwxr-xr-x   0        0        0     5285 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/login.py
--rwxr-xr-x   0        0        0     5045 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/subscription.py
--rwxr-xr-x   0        0        0     6287 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/server.py
--rw-r--r--   0        0        0     1075 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/tokenizer/__init__.py
--rw-r--r--   0        0        0  1033724 2024-04-06 06:10:20.353774 novelai_python-0.4.6/src/novelai_python/tokenizer/novelai.model
--rw-r--r--   0        0        0  1033744 2024-04-06 06:10:20.357774 novelai_python-0.4.6/src/novelai_python/tokenizer/novelai_v2.model
--rw-r--r--   0        0        0       24 2024-04-06 06:10:20.357774 novelai_python-0.4.6/src/novelai_python/tool/__init__.py
--rw-r--r--   0        0        0     7948 2024-04-06 06:10:20.357774 novelai_python-0.4.6/src/novelai_python/tool/image_metadata/__init__.py
--rw-r--r--   0        0        0     3316 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_extractor.py
--rw-r--r--   0        0        0     2211 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_injector.py
--rw-r--r--   0        0        0     3181 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/paint_mask/__init__.py
--rw-r--r--   0        0        0    17162 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/__init__.py
--rw-r--r--   0        0        0    84988 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag.py
--rw-r--r--   0        0        0    21015 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_character.py
--rw-r--r--   0        0        0    15814 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_nsfw.py
--rwxr-xr-x   0        0        0      533 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/utils/__init__.py
--rwxr-xr-x   0        0        0     1881 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/utils/encode.py
--rwxr-xr-x   0        0        0     1243 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/utils/useful.py
--rwxr-xr-x   0        0        0        0 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0      870 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_generate_voice.py
--rwxr-xr-x   0        0        0     2273 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_random_prompt.py
--rwxr-xr-x   0        0        0      422 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_server.py
--rwxr-xr-x   0        0        0     1375 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_server_run.py
--rwxr-xr-x   0        0        0     2772 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_upscale.py
--rwxr-xr-x   0        0        0     2592 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_user_information.py
--rwxr-xr-x   0        0        0     3244 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_user_login.py
--rwxr-xr-x   0        0        0     3270 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_user_subscription.py
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 novelai_python-0.4.6/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2024-04-08 16:25:50.010580 novelai_python-0.4.7/LICENSE
+-rwxr-xr-x   0        0        0      522 2024-04-08 16:25:50.010580 novelai_python-0.4.7/NOTICE.MD
+-rwxr-xr-x   0        0        0     3405 2024-04-08 16:25:50.010580 novelai_python-0.4.7/README.md
+-rw-r--r--   0        0        0     1201 2024-04-08 16:26:06.682767 novelai_python-0.4.7/pyproject.toml
+-rwxr-xr-x   0        0        0     1239 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/__init__.py
+-rwxr-xr-x   0        0        0     1761 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_exceptions.py
+-rwxr-xr-x   0        0        0      410 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/__init__.py
+-rwxr-xr-x   0        0        0      127 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate.py
+-rwxr-xr-x   0        0        0      828 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate_image.py
+-rw-r--r--   0        0        0      724 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate_stream.py
+-rw-r--r--   0        0        0      185 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate_voice.py
+-rwxr-xr-x   0        0        0      397 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/upscale.py
+-rwxr-xr-x   0        0        0      195 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/schema.py
+-rwxr-xr-x   0        0        0      128 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/__init__.py
+-rwxr-xr-x   0        0        0      721 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/information.py
+-rwxr-xr-x   0        0        0      204 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/login.py
+-rwxr-xr-x   0        0        0     2359 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/subscription.py
+-rwxr-xr-x   0        0        0     1548 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/ApiToken.py
+-rwxr-xr-x   0        0        0     1628 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/JwtToken.py
+-rwxr-xr-x   0        0        0     1701 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/UserAuth.py
+-rwxr-xr-x   0        0        0      424 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/__init__.py
+-rwxr-xr-x   0        0        0      462 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/_base.py
+-rwxr-xr-x   0        0        0      743 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/__init__.py
+-rwxr-xr-x   0        0        0     1082 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/LICENSE
+-rwxr-xr-x   0        0        0      130 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/__init__.py
+-rw-r--r--   0        0        0     9436 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_const.py
+-rw-r--r--   0        0        0     1819 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_enum.py
+-rw-r--r--   0        0        0     6467 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_preset.py
+-rwxr-xr-x   0        0        0    34778 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/__init__.py
+-rw-r--r--   0        0        0    52850 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_const.py
+-rwxr-xr-x   0        0        0     3578 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_enum.py
+-rwxr-xr-x   0        0        0     5306 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
+-rw-r--r--   0        0        0     7170 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_stream.py
+-rw-r--r--   0        0        0     7379 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/_enum.py
+-rwxr-xr-x   0        0        0     8223 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/upscale.py
+-rwxr-xr-x   0        0        0      945 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/schema.py
+-rwxr-xr-x   0        0        0      130 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/__init__.py
+-rwxr-xr-x   0        0        0     4772 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/information.py
+-rwxr-xr-x   0        0        0     5285 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/login.py
+-rwxr-xr-x   0        0        0     5045 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/subscription.py
+-rwxr-xr-x   0        0        0     7524 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/server.py
+-rw-r--r--   0        0        0      534 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/tokenizer/NOTICE.MD
+-rw-r--r--   0        0        0     8173 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/tokenizer/__init__.py
+-rw-r--r--   0        0        0  1356917 2024-04-08 16:25:50.034581 novelai_python-0.4.7/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0  1494140 2024-04-08 16:25:50.042580 novelai_python-0.4.7/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json
+-rw-r--r--   0        0        0  1355257 2024-04-08 16:25:50.050581 novelai_python-0.4.7/src/novelai_python/tokenizer/gpt2_tokenizer.json
+-rw-r--r--   0        0        0  1033724 2024-04-08 16:25:50.054581 novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v1.model
+-rw-r--r--   0        0        0  1033744 2024-04-08 16:25:50.058581 novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v2.model
+-rw-r--r--   0        0        0  1033724 2024-04-08 16:25:50.058581 novelai_python-0.4.7/src/novelai_python/tokenizer/novelai.model
+-rw-r--r--   0        0        0  1033744 2024-04-08 16:25:50.062581 novelai_python-0.4.7/src/novelai_python/tokenizer/novelai_v2.model
+-rw-r--r--   0        0        0  1357239 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tokenizer/pile_tokenizer.json
+-rw-r--r--   0        0        0     4854 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tokenizer/simple_tokenizer.py
+-rw-r--r--   0        0        0       24 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/__init__.py
+-rw-r--r--   0        0        0     7948 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/image_metadata/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_extractor.py
+-rw-r--r--   0        0        0     2211 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_injector.py
+-rw-r--r--   0        0        0     3181 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/paint_mask/__init__.py
+-rw-r--r--   0        0        0    17162 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/__init__.py
+-rw-r--r--   0        0        0    84988 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag.py
+-rw-r--r--   0        0        0    21015 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_character.py
+-rw-r--r--   0        0        0    15814 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_nsfw.py
+-rwxr-xr-x   0        0        0      525 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/utils/__init__.py
+-rwxr-xr-x   0        0        0     2419 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/utils/encode.py
+-rwxr-xr-x   0        0        0     1243 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/utils/useful.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_generate_voice.py
+-rwxr-xr-x   0        0        0     2273 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_random_prompt.py
+-rwxr-xr-x   0        0        0      422 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_server.py
+-rwxr-xr-x   0        0        0     1375 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_server_run.py
+-rwxr-xr-x   0        0        0     2772 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_upscale.py
+-rwxr-xr-x   0        0        0     2592 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_user_information.py
+-rwxr-xr-x   0        0        0     3244 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_user_login.py
+-rwxr-xr-x   0        0        0     3270 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_user_subscription.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 novelai_python-0.4.7/PKG-INFO
```

### Comparing `novelai_python-0.4.6/LICENSE` & `novelai_python-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/NOTICE.MD` & `novelai_python-0.4.7/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/README.md` & `novelai_python-0.4.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![banner](https://github.com/LlmKira/novelai-python/blob/dev/playground/banner-raw.png?raw=true)
 
 ---
 
 [![PyPI version](https://badge.fury.io/py/novelai-python.svg)](https://badge.fury.io/py/novelai-python)
 [![Downloads](https://pepy.tech/badge/novelai_python)](https://pepy.tech/project/novelai_python)
 
-✨ NovelAI api python sdk with Pydantic.
+✨ NovelAI api python sdk with Pydantic, modern and user-friendly.
 
 The goal of this repository is to use Pydantic to build legitimate requests to access the NovelAI API service.
 
 ### Roadmap 🚧
 
 - [x] tool.random_prompt
 - [x] tool.paint_mask
@@ -17,18 +17,19 @@
 - [x] /ai/generate-image
 - [x] /user/subscription
 - [x] /user/login
 - [x] /user/information
 - [x] /ai/upscale
 - [x] /ai/generate-image/suggest-tags
 - [x] /ai/generate-voice
+- [x] /ai/generate-stream
+- [x] /ai/generate
 - [ ] /ai/annotate-image
 - [ ] /ai/classify
 - [ ] /ai/generate-prompt
-- [ ] /ai/generate
 
 > GenerateImageInfer.calculate_cost is correct in most cases, but please request account information to get accurate
 > consumption information.
 
 > This repo is maintained by me personally now. If you have any questions, please feel free to open an issue.
 
 ### Usage 🖥️
@@ -43,59 +44,79 @@
 ```python
 import asyncio
 import os
 
 from dotenv import load_dotenv
 from pydantic import SecretStr
 
-from novelai_python import GenerateImageInfer, ImageGenerateResp, JwtCredential, LoginCredential, ApiCredential
+from novelai_python import GenerateImageInfer, ImageGenerateResp, ApiCredential
 
 load_dotenv()
-
 enhance = "year 2023,dynamic angle,  best quality, amazing quality, very aesthetic, absurdres"
+session = ApiCredential(api_token=SecretStr(os.getenv("NOVELAI_JWT")))  # pst-***
 
 
 async def main():
-    globe_s = JwtCredential(
-        jwt_token=SecretStr(os.getenv("NOVELAI_JWT"))  # ey****
-    )
-    globe_s1 = ApiCredential(
-        api_token=SecretStr(os.getenv("NOVELAI_JWT"))  # pst-***
-    )
-    globe_s2 = LoginCredential(
-        username=os.getenv("NOVELAI_USERNAME"),
-        password=SecretStr(os.getenv("NOVELAI_PASSWORD"))
-    )
-
-    gen = await GenerateImageInfer.build(
-        prompt=f"1girl,{enhance}")
+    gen = await GenerateImageInfer.build(prompt=f"1girl,{enhance}")
     cost = gen.calculate_cost(is_opus=True)
     print(f"charge: {cost} if you are vip3")
-
-    resp = gen.request(session=globe_s)
+    resp = gen.request(session=session)
     resp: ImageGenerateResp
     print(resp.meta)
-
     file = resp.files[0]
     with open(file[0], "wb") as f:
         f.write(file[1])
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 
 ```
 
+#### LLM
+
+```python
+import asyncio
+import os
+
+from dotenv import load_dotenv
+
+from novelai_python import APIError, Login
+from novelai_python.sdk.ai.generate import TextLLMModel, LLM
+
+load_dotenv()
+username = os.getenv("NOVELAI_USER", None)
+assert username is not None
+# credential = JwtCredential(jwt_token=SecretStr(jwt))
+login_credential = Login.build(
+    user_name=os.getenv("NOVELAI_USER"),
+    password=os.getenv("NOVELAI_PASS")
+)
+
+
+async def chat(prompt: str):
+    try:
+        agent = LLM.build(prompt=prompt, model=TextLLMModel.Kayra)
+        result = await agent.request(session=login_credential)
+    except APIError as e:
+        raise Exception(f"Error: {e.message}")
+    print(f"Result: \n{result.text}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(chat("Hello"))
+```
+
 #### Random Prompt
 
 ```python
 from novelai_python.tool.random_prompt import RandomPromptGenerator
 
-s = RandomPromptGenerator(nsfw_enabled=False).random_prompt()
-print(s)
+prompt = RandomPromptGenerator(nsfw_enabled=False).random_prompt()
+print(prompt)
 ```
 
 #### Run A Server
 
 ```shell
 pip install novelai_python
 python3 -m novelai_python.server -h '127.0.0.1' -p 7888
```

### Comparing `novelai_python-0.4.6/pyproject.toml` & `novelai_python-0.4.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novelai-python"
-version = "0.4.6"
+version = "0.4.7"
 description = "NovelAI Python Binding With Pydantic"
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
     "elara>=0.5.5",
     "loguru>=0.7.2",
@@ -19,14 +19,17 @@
     "numpy>=1.24.4",
     "argon2-cffi>=23.1.0",
     "opencv-python>=4.8.1.78",
     "fake-useragent>=1.4.0",
     "tenacity>=8.2.3",
     "sentencepiece>=0.2.0",
     "pynacl>=1.5.0",
+    "ftfy>=6.2.0",
+    "regex>=2023.12.25",
+    "tokenizers>=0.15.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "Apache License 2.0"
```

### Comparing `novelai_python-0.4.6/src/novelai_python/__init__.py` & `novelai_python-0.4.7/src/novelai_python/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,22 +8,30 @@
     APIError,
     AuthError,
     ConcurrentGenerationError,
     SessionHttpError
 )
 from .credential import JwtCredential, LoginCredential, ApiCredential
 from .sdk import GenerateImageInfer, ImageGenerateResp
-from .sdk import VoiceGenerate, VoiceResponse
-from .sdk import SuggestTags, SuggestTagsResp
 from .sdk import Information, InformationResp
+from .sdk import LLM, LLMResp
+from .sdk import LLMStream, LLMStreamResp
 from .sdk import Login, LoginResp
 from .sdk import Subscription, SubscriptionResp
+from .sdk import SuggestTags, SuggestTagsResp
 from .sdk import Upscale, UpscaleResp
+from .sdk import VoiceGenerate, VoiceResponse
 
 __all__ = [
+    "LLM",
+    "LLMResp",
+
+    "LLMStream",
+    "LLMStreamResp",
+
     "GenerateImageInfer",
     "ImageGenerateResp",
 
     "VoiceGenerate",
     "VoiceResponse",
 
     "Upscale",
```

### Comparing `novelai_python-0.4.6/src/novelai_python/_exceptions.py` & `novelai_python-0.4.7/src/novelai_python/_exceptions.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/_response/ai/generate_image.py` & `novelai_python-0.4.7/src/novelai_python/_response/ai/generate_image.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/_response/user/information.py` & `novelai_python-0.4.7/src/novelai_python/_response/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/_response/user/subscription.py` & `novelai_python-0.4.7/src/novelai_python/_response/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/credential/ApiToken.py` & `novelai_python-0.4.7/src/novelai_python/credential/ApiToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/credential/JwtToken.py` & `novelai_python-0.4.7/src/novelai_python/credential/JwtToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/credential/UserAuth.py` & `novelai_python-0.4.7/src/novelai_python/credential/UserAuth.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/__init__.py` & `novelai_python-0.4.7/src/novelai_python/sdk/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2024/1/26 上午10:51
 # @Author  : sudoskys
 # @File    : __init__.py.py
 # @Software: PyCharm
 
+from .ai.generate import LLM, LLMResp  # noqa 401
 from .ai.generate_image import GenerateImageInfer, ImageGenerateResp  # noqa 401
 from .ai.generate_image.suggest_tags import SuggestTags, SuggestTagsResp  # noqa 401
+from .ai.generate_stream import LLMStream, LLMStreamResp  # noqa 401
 from .ai.generate_voice import VoiceGenerate, VoiceResponse  # noqa 401
 from .ai.upscale import Upscale, UpscaleResp  # noqa 401
 from .user.information import Information, InformationResp  # noqa 401
 from .user.login import Login, LoginResp  # noqa 401
 from .user.subscription import Subscription, SubscriptionResp  # noqa 401
```

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/LICENSE` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/__init__.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,16 +250,22 @@
             self.reference_image_multiple = new_images
         # 如果都不是 None 时，比较他们的长度
         if all([self.reference_strength_multiple,
                 self.reference_image_multiple,
                 self.reference_information_extracted_multiple]):
             if len(self.reference_strength_multiple) != len(self.reference_image_multiple) != len(
                     self.reference_information_extracted_multiple):
-                raise ValueError("All three reference_* must be of equal length")
-
+                raise ValueError(
+                    f"All three reference_* must be of equal length, "
+                    f"strength:{len(self.reference_strength_multiple)}, "
+                    f"image:{len(self.reference_image_multiple)}, "
+                    f"information:{len(self.reference_information_extracted_multiple)}"
+                )
+            if len(self.reference_image_multiple) > 16:
+                raise ValueError("The maximum number of reference images is 16")
         # 如果有一个存在，其他都必须存在
         ref_items = [self.reference_strength_multiple,
                      self.reference_image_multiple,
                      self.reference_information_extracted_multiple]
         if any(ref_items) and not all(ref_items):
             raise ValueError("All fields must be present together or none should be present")
 
@@ -616,19 +622,21 @@
                 "image": image,
                 "strength": strength,
                 "noise": noise,
             }
         )
         # 清理空值
         param = {k: v for k, v in kwargs.items() if v is not None}
+        _build_prop = Params(**param)
+        assert _build_prop, "Params validate failed"
         return cls(
             input=prompt,
             model=model,
             action=action,
-            parameters=Params(**param)
+            parameters=_build_prop
         )
 
     async def necessary_headers(self, request_data) -> dict:
         """
         :param request_data:
         :return:
         """
```

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_const.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_const.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_enum.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/suggest_tags.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/suggest_tags.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/__init__.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/_enum.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/ai/upscale.py` & `novelai_python-0.4.7/src/novelai_python/sdk/ai/upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/schema.py` & `novelai_python-0.4.7/src/novelai_python/sdk/schema.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/user/information.py` & `novelai_python-0.4.7/src/novelai_python/sdk/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/user/login.py` & `novelai_python-0.4.7/src/novelai_python/sdk/user/login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/sdk/user/subscription.py` & `novelai_python-0.4.7/src/novelai_python/sdk/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/server.py` & `novelai_python-0.4.7/src/novelai_python/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 
 import uvicorn
 from fastapi import FastAPI, Depends, Security
 from fastapi.security import APIKeyHeader
 from loguru import logger
 from starlette.responses import JSONResponse, StreamingResponse
 
+from novelai_python import LLMStream, LLMStreamResp
 from .credential import JwtCredential, SecretStr
+from .sdk.ai.generate import LLM
 from .sdk.ai.generate_image import GenerateImageInfer, Model
 from .sdk.ai.generate_image.suggest_tags import SuggestTags
+from .sdk.ai.generate_voice import VoiceGenerate
 from .sdk.ai.upscale import Upscale
-from .sdk.ai.generate_voice import VoiceGenerate, VoiceResponse
 from .sdk.user.information import Information
 from .sdk.user.login import Login
 from .sdk.user.subscription import Subscription
 
 app = FastAPI()
 token_key = APIKeyHeader(name="Authorization")
 session = {}
@@ -166,14 +168,57 @@
             'Content-Disposition': 'attachment;filename=image.zip'
         })
     except Exception as e:
         logger.exception(e)
         return JSONResponse(status_code=500, content=e.__dict__)
 
 
+@app.post("/ai/generate-stream")
+async def generate(
+        req: LLMStream,
+        current_token: str = Depends(get_current_token)
+):
+    """
+    流式生成
+    :param current_token: Authorization
+    :param req: LLMStream
+    :return:
+    """
+
+    async def generator():
+        agent = req
+        session = await get_session(current_token)  # Assume 'get_session()' is a function to get session by token
+        generator = agent.request(session=session)
+        async for data in generator:
+            data: LLMStreamResp
+            print(data)  # 或者做其他需要的处理
+            yield data.text  # Yield data for streaming response
+
+    return StreamingResponse(generator())
+
+
+@app.post("/ai/generate")
+async def generate(
+        req: LLM,
+        current_token: str = Depends(get_current_token)
+):
+    """
+    对话生成
+    :param current_token: Authorization
+    :param req: LLM
+    :return:
+    """
+    try:
+        _result = await req.request(session=get_session(current_token))
+        return _result.model_dump()
+    except Exception as e:
+        logger.exception(e)
+        return JSONResponse(status_code=500, content=e.__dict__)
+
+
 @app.get("/ai/generate-voice")
 async def generate_voice(
         text: str,
         voice: int = -1,
         seed: Optional[str] = None,
         opus: bool = False,
         version: Union[Literal["v2", "v1"], str] = "v2",
```

### Comparing `novelai_python-0.4.6/src/novelai_python/tokenizer/novelai.model` & `novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v1.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tokenizer/novelai_v2.model` & `novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v2.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/image_metadata/__init__.py` & `novelai_python-0.4.7/src/novelai_python/tool/image_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_extractor.py` & `novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_extractor.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_injector.py` & `novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_injector.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/paint_mask/__init__.py` & `novelai_python-0.4.7/src/novelai_python/tool/paint_mask/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/__init__.py` & `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag.py` & `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_character.py` & `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_character.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_nsfw.py` & `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_nsfw.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/src/novelai_python/utils/__init__.py` & `novelai_python-0.4.7/src/novelai_python/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2024/1/26 上午10:51
 # @Author  : sudoskys
 # @File    : __init__.py.py
 # @Software: PyCharm
-import io
 import json
 from typing import Union
+
 from loguru import logger
+
 from .encode import encode_access_key  # noqa 401
 
 
 def try_jsonfy(obj: Union[str, dict, list, tuple]):
     """
     try to jsonfy a object
     :param obj:
```

### Comparing `novelai_python-0.4.6/src/novelai_python/utils/encode.py` & `novelai_python-0.4.7/src/novelai_python/utils/encode.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2024/2/7 上午11:41
 # @Author  : sudoskys
 # @File    : encode.py
 # @Software: PyCharm
 from base64 import urlsafe_b64encode
 from hashlib import blake2b
+from typing import Iterable, List
 
 import argon2
 
 
 # https://github.com/HanaokaYuzu/NovelAI-API/blob/master/src/novelai/utils.py#L12
 def encode_access_key(username: str, password: str) -> str:
     """
@@ -36,23 +37,14 @@
 
     return hashed[:64]
 
 
 import base64
 import hashlib
 import hmac
-import json
-from io import BytesIO
-from typing import Union
-
-import numpy as np
-from PIL import Image
-from PIL.PngImagePlugin import PngInfo
-from loguru import logger
-from pydantic import BaseModel
 
 
 def sign_message(message, key):
     # 使用 HMAC 算法对消息进行哈希签名
     hmac_digest = hmac.new(key.encode(), message.encode(), hashlib.sha256).digest()
     signed_hash = base64.b64encode(hmac_digest).decode()
     return signed_hash
@@ -65,7 +57,27 @@
 
 
 # 解码
 def decode_base64(encoded_data):
     byte_data = encoded_data.encode('UTF-8')
     decoded_data = base64.b64decode(byte_data)
     return decoded_data.decode("UTF-8")
+
+
+# MIT: https://github.com/Aedial/novelai-api/blob/794c4f3d89cc86df3c7d2c401b320f1822822ac0/novelai_api/utils.py
+def tokens_to_b64(tokens: Iterable[int]) -> str:
+    """
+    Encode a list of tokens into a base64 string that can be sent to the API
+    """
+
+    return base64.b64encode(b"".join(t.to_bytes(2, "little") for t in tokens)).decode()
+
+
+# MIT:https://github.com/Aedial/novelai-api/blob/794c4f3d89cc86df3c7d2c401b320f1822822ac0/novelai_api/utils.py#L332
+def b64_to_tokens(b64: str) -> List[int]:
+    """
+    Decode a base64 string returned by the API into a list of tokens
+    """
+
+    b = base64.b64decode(b64)
+
+    return [int.from_bytes(b[i: i + 2], "little") for i in range(0, len(b), 2)]
```

### Comparing `novelai_python-0.4.6/src/novelai_python/utils/useful.py` & `novelai_python-0.4.7/src/novelai_python/utils/useful.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_generate_voice.py` & `novelai_python-0.4.7/tests/test_generate_voice.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_random_prompt.py` & `novelai_python-0.4.7/tests/test_random_prompt.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_server_run.py` & `novelai_python-0.4.7/tests/test_server_run.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_upscale.py` & `novelai_python-0.4.7/tests/test_upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_user_information.py` & `novelai_python-0.4.7/tests/test_user_information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_user_login.py` & `novelai_python-0.4.7/tests/test_user_login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/tests/test_user_subscription.py` & `novelai_python-0.4.7/tests/test_user_subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.6/PKG-INFO` & `novelai_python-0.4.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelai-python
-Version: 0.4.6
+Version: 0.4.7
 Summary: NovelAI Python Binding With Pydantic
 Author-Email: sudoskys <coldlando@hotmail.com>
 License: Apache License 2.0
 Project-URL: Repository, https://github.com/LlmKira/novelai-python/
 Project-URL: Issues, https://github.com/LlmKira/novelai-python/issues
 Requires-Python: >=3.8
 Requires-Dist: elara>=0.5.5
@@ -20,27 +20,30 @@
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: argon2-cffi>=23.1.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: fake-useragent>=1.4.0
 Requires-Dist: tenacity>=8.2.3
 Requires-Dist: sentencepiece>=0.2.0
 Requires-Dist: pynacl>=1.5.0
+Requires-Dist: ftfy>=6.2.0
+Requires-Dist: regex>=2023.12.25
+Requires-Dist: tokenizers>=0.15.2
 Requires-Dist: pytest>=7.4.4; extra == "testing"
 Requires-Dist: pytest-asyncio>=0.23.4; extra == "testing"
 Provides-Extra: testing
 Description-Content-Type: text/markdown
 
 ![banner](https://github.com/LlmKira/novelai-python/blob/dev/playground/banner-raw.png?raw=true)
 
 ---
 
 [![PyPI version](https://badge.fury.io/py/novelai-python.svg)](https://badge.fury.io/py/novelai-python)
 [![Downloads](https://pepy.tech/badge/novelai_python)](https://pepy.tech/project/novelai_python)
 
-✨ NovelAI api python sdk with Pydantic.
+✨ NovelAI api python sdk with Pydantic, modern and user-friendly.
 
 The goal of this repository is to use Pydantic to build legitimate requests to access the NovelAI API service.
 
 ### Roadmap 🚧
 
 - [x] tool.random_prompt
 - [x] tool.paint_mask
@@ -48,18 +51,19 @@
 - [x] /ai/generate-image
 - [x] /user/subscription
 - [x] /user/login
 - [x] /user/information
 - [x] /ai/upscale
 - [x] /ai/generate-image/suggest-tags
 - [x] /ai/generate-voice
+- [x] /ai/generate-stream
+- [x] /ai/generate
 - [ ] /ai/annotate-image
 - [ ] /ai/classify
 - [ ] /ai/generate-prompt
-- [ ] /ai/generate
 
 > GenerateImageInfer.calculate_cost is correct in most cases, but please request account information to get accurate
 > consumption information.
 
 > This repo is maintained by me personally now. If you have any questions, please feel free to open an issue.
 
 ### Usage 🖥️
@@ -74,59 +78,79 @@
 ```python
 import asyncio
 import os
 
 from dotenv import load_dotenv
 from pydantic import SecretStr
 
-from novelai_python import GenerateImageInfer, ImageGenerateResp, JwtCredential, LoginCredential, ApiCredential
+from novelai_python import GenerateImageInfer, ImageGenerateResp, ApiCredential
 
 load_dotenv()
-
 enhance = "year 2023,dynamic angle,  best quality, amazing quality, very aesthetic, absurdres"
+session = ApiCredential(api_token=SecretStr(os.getenv("NOVELAI_JWT")))  # pst-***
 
 
 async def main():
-    globe_s = JwtCredential(
-        jwt_token=SecretStr(os.getenv("NOVELAI_JWT"))  # ey****
-    )
-    globe_s1 = ApiCredential(
-        api_token=SecretStr(os.getenv("NOVELAI_JWT"))  # pst-***
-    )
-    globe_s2 = LoginCredential(
-        username=os.getenv("NOVELAI_USERNAME"),
-        password=SecretStr(os.getenv("NOVELAI_PASSWORD"))
-    )
-
-    gen = await GenerateImageInfer.build(
-        prompt=f"1girl,{enhance}")
+    gen = await GenerateImageInfer.build(prompt=f"1girl,{enhance}")
     cost = gen.calculate_cost(is_opus=True)
     print(f"charge: {cost} if you are vip3")
-
-    resp = gen.request(session=globe_s)
+    resp = gen.request(session=session)
     resp: ImageGenerateResp
     print(resp.meta)
-
     file = resp.files[0]
     with open(file[0], "wb") as f:
         f.write(file[1])
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 
 ```
 
+#### LLM
+
+```python
+import asyncio
+import os
+
+from dotenv import load_dotenv
+
+from novelai_python import APIError, Login
+from novelai_python.sdk.ai.generate import TextLLMModel, LLM
+
+load_dotenv()
+username = os.getenv("NOVELAI_USER", None)
+assert username is not None
+# credential = JwtCredential(jwt_token=SecretStr(jwt))
+login_credential = Login.build(
+    user_name=os.getenv("NOVELAI_USER"),
+    password=os.getenv("NOVELAI_PASS")
+)
+
+
+async def chat(prompt: str):
+    try:
+        agent = LLM.build(prompt=prompt, model=TextLLMModel.Kayra)
+        result = await agent.request(session=login_credential)
+    except APIError as e:
+        raise Exception(f"Error: {e.message}")
+    print(f"Result: \n{result.text}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(chat("Hello"))
+```
+
 #### Random Prompt
 
 ```python
 from novelai_python.tool.random_prompt import RandomPromptGenerator
 
-s = RandomPromptGenerator(nsfw_enabled=False).random_prompt()
-print(s)
+prompt = RandomPromptGenerator(nsfw_enabled=False).random_prompt()
+print(prompt)
 ```
 
 #### Run A Server
 
 ```shell
 pip install novelai_python
 python3 -m novelai_python.server -h '127.0.0.1' -p 7888
```

