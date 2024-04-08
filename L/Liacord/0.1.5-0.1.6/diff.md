# Comparing `tmp/Liacord-0.1.5.tar.gz` & `tmp/Liacord-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liacord-0.1.5.tar", last modified: Mon Apr  8 08:59:11 2024, max compression
+gzip compressed data, was "Liacord-0.1.6.tar", last modified: Mon Apr  8 09:11:28 2024, max compression
```

## Comparing `Liacord-0.1.5.tar` & `Liacord-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 08:59:11.395298 Liacord-0.1.5/
-drwxrwxrwx   0        0        0        0 2024-04-08 08:59:11.384760 Liacord-0.1.5/Liacord/
--rw-rw-rw-   0        0        0       88 2024-04-07 22:17:01.000000 Liacord-0.1.5/Liacord/__init__.py
--rw-rw-rw-   0        0        0     6666 2024-04-07 22:23:59.000000 Liacord-0.1.5/Liacord/client.py
--rw-rw-rw-   0        0        0     1494 2024-04-07 22:24:16.000000 Liacord-0.1.5/Liacord/context.py
--rw-rw-rw-   0        0        0     1854 2024-04-07 22:24:16.000000 Liacord-0.1.5/Liacord/intents.py
-drwxrwxrwx   0        0        0        0 2024-04-08 08:59:11.393293 Liacord-0.1.5/Liacord.egg-info/
--rw-rw-rw-   0        0        0     2175 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-08 08:59:11.000000 Liacord-0.1.5/Liacord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2175 2024-04-08 08:59:11.395298 Liacord-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1856 2024-04-08 08:45:29.000000 Liacord-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 08:59:11.396295 Liacord-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      656 2024-04-08 08:58:48.000000 Liacord-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:11:27.992426 Liacord-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-04-08 09:11:27.980904 Liacord-0.1.6/Liacord/
+-rw-rw-rw-   0        0        0       88 2024-04-07 22:17:01.000000 Liacord-0.1.6/Liacord/__init__.py
+-rw-rw-rw-   0        0        0     6666 2024-04-07 22:23:59.000000 Liacord-0.1.6/Liacord/client.py
+-rw-rw-rw-   0        0        0     1494 2024-04-07 22:24:16.000000 Liacord-0.1.6/Liacord/context.py
+-rw-rw-rw-   0        0        0     1854 2024-04-07 22:24:16.000000 Liacord-0.1.6/Liacord/intents.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:11:27.991427 Liacord-0.1.6/Liacord.egg-info/
+-rw-rw-rw-   0        0        0     2600 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 09:11:27.000000 Liacord-0.1.6/Liacord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2600 2024-04-08 09:11:27.993428 Liacord-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2203 2024-04-08 09:11:03.000000 Liacord-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:11:27.993428 Liacord-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-08 09:07:05.000000 Liacord-0.1.6/setup.py
```

### Comparing `Liacord-0.1.5/Liacord/client.py` & `Liacord-0.1.6/Liacord/client.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.5/Liacord/context.py` & `Liacord-0.1.6/Liacord/context.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.5/Liacord/intents.py` & `Liacord-0.1.6/Liacord/intents.py`

 * *Files identical despite different names*

### Comparing `Liacord-0.1.5/Liacord.egg-info/PKG-INFO` & `Liacord-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,138 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 204c 6961  : 2.1..Name: Lia
-00000020: 636f 7264 0d0a 5665 7273 696f 6e3a 2030  cord..Version: 0
-00000030: 2e31 2e35 0d0a 5375 6d6d 6172 793a 2041  .1.5..Summary: A
-00000040: 2050 7974 686f 6e20 7772 6170 7065 7220   Python wrapper 
-00000050: 666f 7220 7468 6520 4469 7363 6f72 6420  for the Discord 
-00000060: 4150 490d 0a48 6f6d 652d 7061 6765 3a20  API..Home-page: 
-00000070: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000080: 6f6d 2f6d 6173 657a 6576 2f4c 6961 636f  om/masezev/Liaco
-00000090: 7264 2e70 790d 0a41 7574 686f 723a 204d  rd.py..Author: M
-000000a0: 6173 657a 6576 0d0a 4175 7468 6f72 2d65  asezev..Author-e
-000000b0: 6d61 696c 3a20 6373 676f 6d61 6e61 6765  mail: csgomanage
-000000c0: 6d65 6e74 3140 676d 6169 6c2e 636f 6d0d  ment1@gmail.com.
-000000d0: 0a4c 6963 656e 7365 3a20 4d49 540d 0a50  .License: MIT..P
-000000e0: 726f 6a65 6374 2d55 524c 3a20 4469 7363  roject-URL: Disc
-000000f0: 6f72 642c 2068 7474 7073 3a2f 2f64 6973  ord, https://dis
-00000100: 636f 7264 2e67 672f 4837 4651 4647 4550  cord.gg/H7FQFGEP
-00000110: 7a35 0d0a 4465 7363 7269 7074 696f 6e2d  z5..Description-
-00000120: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000130: 7874 2f6d 6172 6b64 6f77 6e0d 0a0d 0a4c  xt/markdown....L
-00000140: 6961 636f 7264 0d0a 3d3d 3d3d 3d3d 3d3d  iacord..========
-00000150: 3d3d 0d0a 0d0a 2e2e 2069 6d61 6765 3a3a  ==...... image::
-00000160: 2068 7474 7073 3a2f 2f64 6973 636f 7264   https://discord
-00000170: 2e63 6f6d 2f61 7069 2f67 7569 6c64 732f  .com/api/guilds/
-00000180: 3933 3034 3135 3130 3037 3138 3837 3837  9304151007188787
-00000190: 3530 2f65 6d62 6564 2e70 6e67 0d0a 2020  50/embed.png..  
-000001a0: 203a 7461 7267 6574 3a68 7474 7073 3a2f   :target:https:/
-000001b0: 2f64 6973 636f 7264 2e67 672f 4837 4651  /discord.gg/H7FQ
-000001c0: 4647 4550 7a35 0d0a 2020 203a 616c 743a  FGEPz5..   :alt:
-000001d0: 2044 6973 636f 7264 2073 6572 7665 7220   Discord server 
-000001e0: 696e 7669 7465 0d0a 2e2e 2069 6d61 6765  invite.... image
-000001f0: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000200: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000210: 2f4c 6961 636f 7264 2e73 7667 0d0a 2020  /Liacord.svg..  
-00000220: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000230: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000240: 672f 7079 7069 2f64 6973 636f 7264 2e70  g/pypi/discord.p
-00000250: 790d 0a20 2020 3a61 6c74 3a20 5079 5049  y..   :alt: PyPI
-00000260: 2076 6572 7369 6f6e 2069 6e66 6f0d 0a2e   version info...
-00000270: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
-00000280: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000290: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
-000002a0: 2f64 6973 636f 7264 2e70 792e 7376 670d  /discord.py.svg.
-000002b0: 0a20 2020 3a74 6172 6765 743a 2068 7474  .   :target: htt
-000002c0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-000002d0: 2e6f 7267 2f70 7970 692f 4c69 6163 6f72  .org/pypi/Liacor
-000002e0: 640d 0a20 2020 3a61 6c74 3a20 5079 5049  d..   :alt: PyPI
-000002f0: 2073 7570 706f 7274 6564 2050 7974 686f   supported Pytho
-00000300: 6e20 7665 7273 696f 6e73 0d0a 0d0a 4b65  n versions....Ke
-00000310: 7920 4665 6174 7572 6573 0d0a 2d2d 2d2d  y Features..----
-00000320: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a2d 204d  ---------....- M
-00000330: 6f64 6572 6e20 5079 7468 6f6e 6963 2041  odern Pythonic A
-00000340: 5049 2075 7369 6e67 2060 6061 7379 6e63  PI using ``async
-00000350: 6060 2061 6e64 2060 6061 7761 6974 6060  `` and ``await``
-00000360: 2e0d 0a2d 2050 726f 7065 7220 7261 7465  ...- Proper rate
-00000370: 206c 696d 6974 2068 616e 646c 696e 672e   limit handling.
-00000380: 0d0a 2d20 4f70 7469 6d69 7365 6420 696e  ..- Optimised in
-00000390: 2062 6f74 6820 7370 6565 6420 616e 6420   both speed and 
-000003a0: 6d65 6d6f 7279 2e0d 0a0d 0a49 6e73 7461  memory.....Insta
-000003b0: 6c6c 696e 670d 0a2d 2d2d 2d2d 2d2d 2d2d  lling..---------
-000003c0: 2d0d 0a0d 0a2a 2a50 7974 686f 6e20 332e  -....**Python 3.
-000003d0: 3820 6f72 2068 6967 6865 7220 6973 2072  8 or higher is r
-000003e0: 6571 7569 7265 642a 2a0d 0a0d 0a54 6f20  equired**....To 
-000003f0: 696e 7374 616c 6c20 7468 6520 6c69 6272  install the libr
-00000400: 6172 7920 7769 7468 6f75 7420 6675 6c6c  ary without full
-00000410: 2076 6f69 6365 2073 7570 706f 7274 2c20   voice support, 
-00000420: 796f 7520 6361 6e20 6a75 7374 2072 756e  you can just run
-00000430: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00000440: 6f6d 6d61 6e64 3a0d 0a0d 0a2e 2e20 636f  ommand:...... co
-00000450: 6465 3a3a 2073 680d 0a0d 0a20 2020 2023  de:: sh....    #
-00000460: 204c 696e 7578 2f6d 6163 4f53 0d0a 2020   Linux/macOS..  
-00000470: 2020 7079 7468 6f6e 3320 2d6d 2070 6970    python3 -m pip
-00000480: 2069 6e73 7461 6c6c 202d 5520 4c69 6163   install -U Liac
-00000490: 6f72 640d 0a0d 0a20 2020 2023 2057 696e  ord....    # Win
-000004a0: 646f 7773 0d0a 2020 2020 7079 202d 3320  dows..    py -3 
-000004b0: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
-000004c0: 5520 4c69 6163 6f72 640d 0a0d 0a42 6f74  U Liacord....Bot
-000004d0: 2045 7861 6d70 6c65 0d0a 7e7e 7e7e 7e7e   Example..~~~~~~
-000004e0: 7e7e 7e7e 7e7e 7e0d 0a0d 0a2e 2e20 636f  ~~~~~~~...... co
-000004f0: 6465 3a3a 2070 790d 0a0d 0a20 2020 2069  de:: py....    i
-00000500: 6d70 6f72 7420 6173 796e 6369 6f0d 0a20  mport asyncio.. 
-00000510: 2020 2066 726f 6d20 4c69 6163 6f72 6420     from Liacord 
-00000520: 696d 706f 7274 2043 6c69 656e 742c 2049  import Client, I
-00000530: 6e74 656e 7473 0d0a 2020 2020 0d0a 2020  ntents..    ..  
-00000540: 2020 696e 7465 6e74 7320 3d20 496e 7465    intents = Inte
-00000550: 6e74 7328 292e 616c 6c28 290d 0a20 2020  nts().all()..   
-00000560: 2063 6c69 656e 7420 3d20 436c 6965 6e74   client = Client
-00000570: 2822 796f 7572 5f74 6f6b 656e 5f68 6572  ("your_token_her
-00000580: 6522 2c20 7072 6566 6978 3d22 2322 2c20  e", prefix="#", 
-00000590: 696e 7465 6e74 733d 696e 7465 6e74 7329  intents=intents)
-000005a0: 0d0a 2020 2020 0d0a 2020 2020 4063 6c69  ..    ..    @cli
-000005b0: 656e 742e 636f 6d6d 616e 6428 6e61 6d65  ent.command(name
-000005c0: 3d22 6e61 6d65 2229 0d0a 2020 2020 6173  ="name")..    as
-000005d0: 796e 6320 6465 6620 6865 6c6c 6f28 6374  ync def hello(ct
-000005e0: 7829 3a0d 0a20 2020 2020 2020 2061 7761  x):..        awa
-000005f0: 6974 2063 7478 2e73 656e 6428 6622 7b63  it ctx.send(f"{c
-00000600: 7478 2e61 7574 686f 722e 6e61 6d65 7d22  tx.author.name}"
-00000610: 290d 0a20 2020 200d 0a20 2020 2040 636c  )..    ..    @cl
-00000620: 6965 6e74 2e63 6f6d 6d61 6e64 286e 616d  ient.command(nam
-00000630: 653d 2270 696e 6722 290d 0a20 2020 2061  e="ping")..    a
-00000640: 7379 6e63 2064 6566 2070 696e 6728 6374  sync def ping(ct
-00000650: 7829 3a0d 0a20 2020 2020 2020 2061 7761  x):..        awa
-00000660: 6974 2063 7478 2e73 656e 6428 6622 706f  it ctx.send(f"po
-00000670: 6e67 207b 726f 756e 6428 636c 6965 6e74  ng {round(client
-00000680: 2e6c 6174 656e 6379 297d 6d73 2e22 290d  .latency)}ms.").
-00000690: 0a20 2020 200d 0a20 2020 2040 636c 6965  .    ..    @clie
-000006a0: 6e74 2e63 6f6d 6d61 6e64 286e 616d 653d  nt.command(name=
-000006b0: 2773 6572 7665 725f 6964 272c 2062 7269  'server_id', bri
-000006c0: 6566 3d27 6765 7420 7468 6520 7365 7276  ef='get the serv
-000006d0: 6572 2069 6427 290d 0a20 2020 2061 7379  er id')..    asy
-000006e0: 6e63 2064 6566 2073 6572 7665 725f 6964  nc def server_id
-000006f0: 5f63 6f6d 6d61 6e64 2863 7478 293a 0d0a  _command(ctx):..
-00000700: 2020 2020 2020 2020 7365 7276 6572 5f69          server_i
-00000710: 6420 3d20 6374 782e 6775 696c 642e 6964  d = ctx.guild.id
-00000720: 0d0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00000730: 6374 782e 7365 6e64 2866 2273 6572 7665  ctx.send(f"serve
-00000740: 7220 6964 3a20 7b73 6572 7665 725f 6964  r id: {server_id
-00000750: 7d22 290d 0a20 2020 200d 0a20 2020 206c  }")..    ..    l
-00000760: 6f6f 7020 3d20 6173 796e 6369 6f2e 6765  oop = asyncio.ge
-00000770: 745f 6576 656e 745f 6c6f 6f70 2829 0d0a  t_event_loop()..
-00000780: 2020 2020 6c6f 6f70 2e72 756e 5f75 6e74      loop.run_unt
-00000790: 696c 5f63 6f6d 706c 6574 6528 636c 6965  il_complete(clie
-000007a0: 6e74 2e72 756e 2829 290d 0a0d 0a59 6f75  nt.run())....You
-000007b0: 2063 616e 2066 696e 6420 6d6f 7265 2065   can find more e
-000007c0: 7861 6d70 6c65 7320 696e 2074 6865 2065  xamples in the e
-000007d0: 7861 6d70 6c65 7320 6469 7265 6374 6f72  xamples director
-000007e0: 792e 0d0a 0d0a 4c69 6e6b 730d 0a2d 2d2d  y.....Links..---
-000007f0: 2d2d 2d0d 0a0d 0a2d 2060 446f 6375 6d65  ---....- `Docume
-00000800: 6e74 6174 696f 6e20 4e6f 605f 0d0a 2d20  ntation No`_..- 
-00000810: 604f 6666 6963 6961 6c20 4469 7363 6f72  `Official Discor
-00000820: 6420 5365 7276 6572 203c 6874 7470 733a  d Server <https:
-00000830: 2f2f 6469 7363 6f72 642e 6767 2f48 3746  //discord.gg/H7F
-00000840: 5146 4745 507a 353e 605f 0d0a 2d20 6044  QFGEPz5>`_..- `D
-00000850: 6973 636f 7264 2041 5049 203c 6874 7470  iscord API <http
-00000860: 733a 2f2f 6469 7363 6f72 642e 6767 2f64  s://discord.gg/d
-00000870: 6973 636f 7264 2d61 7069 3e60 5f0d 0a    iscord-api>`_..
+00000000: 4c69 6163 6f72 640d 0a3d 3d3d 3d3d 3d3d  Liacord..=======
+00000010: 3d3d 3d0d 0a0d 0a3c 7020 616c 6967 6e3d  ===....<p align=
+00000020: 2263 656e 7465 7222 3e0d 0a20 2020 203c  "center">..    <
+00000030: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000040: 6469 7363 6f72 642e 6767 2f48 3746 5146  discord.gg/H7FQF
+00000050: 4745 507a 3522 3e3c 696d 6720 7372 633d  GEPz5"><img src=
+00000060: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000070: 656c 6473 2e69 6f2f 6469 7363 6f72 642f  elds.io/discord/
+00000080: 3933 3034 3135 3130 3037 3138 3837 3837  9304151007188787
+00000090: 3530 3f73 7479 6c65 3d66 6c61 742d 7371  50?style=flat-sq
+000000a0: 7561 7265 2663 6f6c 6f72 3d35 3836 3566  uare&color=5865f
+000000b0: 3226 6c6f 676f 3d64 6973 636f 7264 266c  2&logo=discord&l
+000000c0: 6f67 6f43 6f6c 6f72 3d66 6666 6666 6626  ogoColor=ffffff&
+000000d0: 6c61 6265 6c3d 6469 7363 6f72 6422 2061  label=discord" a
+000000e0: 6c74 3d22 4469 7363 6f72 6420 7365 7276  lt="Discord serv
+000000f0: 6572 2069 6e76 6974 6522 202f 3e3c 2f61  er invite" /></a
+00000100: 3e0d 0a20 2020 203c 6120 6872 6566 3d22  >..    <a href="
+00000110: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000120: 2f70 726f 6a65 6374 2f4c 6961 636f 7264  /project/Liacord
+00000130: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000140: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000150: 696f 2f70 7970 692f 762f 4c69 6163 6f72  io/pypi/v/Liacor
+00000160: 642e 7376 673f 7374 796c 653d 666c 6174  d.svg?style=flat
+00000170: 2d73 7175 6172 6522 2061 6c74 3d22 5079  -square" alt="Py
+00000180: 5049 2076 6572 7369 6f6e 2069 6e66 6f22  PI version info"
+00000190: 202f 3e3c 2f61 3e0d 0a20 2020 203c 6120   /></a>..    <a 
+000001a0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+000001b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f4c  pi.org/project/L
+000001c0: 6961 636f 7264 2f22 3e3c 696d 6720 7372  iacord/"><img sr
+000001d0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001e0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+000001f0: 7976 6572 7369 6f6e 732f 4c69 6163 6f72  yversions/Liacor
+00000200: 642e 7376 673f 7374 796c 653d 666c 6174  d.svg?style=flat
+00000210: 2d73 7175 6172 6522 2061 6c74 3d22 5079  -square" alt="Py
+00000220: 5049 2073 7570 706f 7274 6564 2050 7974  PI supported Pyt
+00000230: 686f 6e20 7665 7273 696f 6e73 2220 2f3e  hon versions" />
+00000240: 3c2f 613e 0d0a 2020 2020 3c61 2068 7265  </a>..    <a hre
+00000250: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000260: 622e 636f 6d2f 6d61 7365 7a65 762f 4c69  b.com/masezev/Li
+00000270: 6163 6f72 642e 7079 2f63 6f6d 6d69 7473  acord.py/commits
+00000280: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000290: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000002a0: 696f 2f67 6974 6875 622f 636f 6d6d 6974  io/github/commit
+000002b0: 2d61 6374 6976 6974 792f 772f 6d61 7365  -activity/w/mase
+000002c0: 7a65 762f 4c69 6163 6f72 642e 7079 2e73  zev/Liacord.py.s
+000002d0: 7667 3f73 7479 6c65 3d66 6c61 742d 7371  vg?style=flat-sq
+000002e0: 7561 7265 2220 616c 743d 2243 6f6d 6d69  uare" alt="Commi
+000002f0: 7420 6163 7469 7669 7479 2220 2f3e 3c2f  t activity" /></
+00000300: 613e 0d0a 3c2f 703e 0d0a 0d0a 4b65 7920  a>..</p>....Key 
+00000310: 4665 6174 7572 6573 0d0a 2d2d 2d2d 2d2d  Features..------
+00000320: 2d2d 2d2d 2d2d 2d0d 0a0d 0a2d 204d 6f64  -------....- Mod
+00000330: 6572 6e20 5079 7468 6f6e 6963 2041 5049  ern Pythonic API
+00000340: 2075 7369 6e67 2060 6061 7379 6e63 6060   using ``async``
+00000350: 2061 6e64 2060 6061 7761 6974 6060 2e0d   and ``await``..
+00000360: 0a2d 2050 726f 7065 7220 7261 7465 206c  .- Proper rate l
+00000370: 696d 6974 2068 616e 646c 696e 672e 0d0a  imit handling...
+00000380: 2d20 4f70 7469 6d69 7365 6420 696e 2062  - Optimised in b
+00000390: 6f74 6820 7370 6565 6420 616e 6420 6d65  oth speed and me
+000003a0: 6d6f 7279 2e0d 0a0d 0a49 6e73 7461 6c6c  mory.....Install
+000003b0: 696e 670d 0a2d 2d2d 2d2d 2d2d 2d2d 2d0d  ing..----------.
+000003c0: 0a0d 0a2a 2a50 7974 686f 6e20 332e 3820  ...**Python 3.8 
+000003d0: 6f72 2068 6967 6865 7220 6973 2072 6571  or higher is req
+000003e0: 7569 7265 642a 2a0d 0a0d 0a54 6f20 696e  uired**....To in
+000003f0: 7374 616c 6c20 7468 6520 6c69 6272 6172  stall the librar
+00000400: 7920 7769 7468 6f75 7420 6675 6c6c 2076  y without full v
+00000410: 6f69 6365 2073 7570 706f 7274 2c20 796f  oice support, yo
+00000420: 7520 6361 6e20 6a75 7374 2072 756e 2074  u can just run t
+00000430: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00000440: 6d61 6e64 3a0d 0a0d 0a20 2020 2023 204c  mand:....    # L
+00000450: 696e 7578 2f6d 6163 4f53 0d0a 2020 2020  inux/macOS..    
+00000460: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
+00000470: 6e73 7461 6c6c 202d 5520 4c69 6163 6f72  nstall -U Liacor
+00000480: 640d 0a0d 0a20 2020 2023 2057 696e 646f  d....    # Windo
+00000490: 7773 0d0a 2020 2020 7079 202d 3320 2d6d  ws..    py -3 -m
+000004a0: 2070 6970 2069 6e73 7461 6c6c 202d 5520   pip install -U 
+000004b0: 4c69 6163 6f72 640d 0a0d 0a42 6f74 2045  Liacord....Bot E
+000004c0: 7861 6d70 6c65 0d0a 7e7e 7e7e 7e7e 7e7e  xample..~~~~~~~~
+000004d0: 7e7e 7e7e 7e0d 0a69 6d70 6f72 7420 6173  ~~~~~..import as
+000004e0: 796e 6369 6f0d 0a20 6672 6f6d 204c 6961  yncio.. from Lia
+000004f0: 636f 7264 2069 6d70 6f72 7420 436c 6965  cord import Clie
+00000500: 6e74 2c20 496e 7465 6e74 730d 0a20 0d0a  nt, Intents.. ..
+00000510: 2069 6e74 656e 7473 203d 2049 6e74 656e   intents = Inten
+00000520: 7473 2829 2e61 6c6c 2829 0d0a 2063 6c69  ts().all().. cli
+00000530: 656e 7420 3d20 436c 6965 6e74 2822 796f  ent = Client("yo
+00000540: 7572 5f74 6f6b 656e 5f68 6572 6522 2c20  ur_token_here", 
+00000550: 7072 6566 6978 3d22 2322 2c20 696e 7465  prefix="#", inte
+00000560: 6e74 733d 696e 7465 6e74 7329 0d0a 200d  nts=intents).. .
+00000570: 0a20 4063 6c69 656e 742e 636f 6d6d 616e  . @client.comman
+00000580: 6428 6e61 6d65 3d22 6e61 6d65 2229 0d0a  d(name="name")..
+00000590: 2061 7379 6e63 2064 6566 2068 656c 6c6f   async def hello
+000005a0: 2863 7478 293a 0d0a 2020 2020 2061 7761  (ctx):..     awa
+000005b0: 6974 2063 7478 2e73 656e 6428 6622 7b63  it ctx.send(f"{c
+000005c0: 7478 2e61 7574 686f 722e 6e61 6d65 7d22  tx.author.name}"
+000005d0: 290d 0a20 0d0a 2040 636c 6965 6e74 2e63  ).. .. @client.c
+000005e0: 6f6d 6d61 6e64 286e 616d 653d 2270 696e  ommand(name="pin
+000005f0: 6722 290d 0a20 6173 796e 6320 6465 6620  g").. async def 
+00000600: 7069 6e67 2863 7478 293a 0d0a 2020 2020  ping(ctx):..    
+00000610: 2061 7761 6974 2063 7478 2e73 656e 6428   await ctx.send(
+00000620: 6622 706f 6e67 207b 726f 756e 6428 636c  f"pong {round(cl
+00000630: 6965 6e74 2e6c 6174 656e 6379 297d 6d73  ient.latency)}ms
+00000640: 2e22 290d 0a20 0d0a 2040 636c 6965 6e74  .").. .. @client
+00000650: 2e63 6f6d 6d61 6e64 286e 616d 653d 2773  .command(name='s
+00000660: 6572 7665 725f 6964 272c 2062 7269 6566  erver_id', brief
+00000670: 3d27 6765 7420 7468 6520 7365 7276 6572  ='get the server
+00000680: 2069 6427 290d 0a20 6173 796e 6320 6465   id').. async de
+00000690: 6620 7365 7276 6572 5f69 645f 636f 6d6d  f server_id_comm
+000006a0: 616e 6428 6374 7829 3a0d 0a20 2020 2020  and(ctx):..     
+000006b0: 7365 7276 6572 5f69 6420 3d20 6374 782e  server_id = ctx.
+000006c0: 6775 696c 642e 6964 0d0a 2020 2020 2061  guild.id..     a
+000006d0: 7761 6974 2063 7478 2e73 656e 6428 6622  wait ctx.send(f"
+000006e0: 7365 7276 6572 2069 643a 207b 7365 7276  server id: {serv
+000006f0: 6572 5f69 647d 2229 0d0a 200d 0a20 6c6f  er_id}").. .. lo
+00000700: 6f70 203d 2061 7379 6e63 696f 2e67 6574  op = asyncio.get
+00000710: 5f65 7665 6e74 5f6c 6f6f 7028 290d 0a20  _event_loop().. 
+00000720: 6c6f 6f70 2e72 756e 5f75 6e74 696c 5f63  loop.run_until_c
+00000730: 6f6d 706c 6574 6528 636c 6965 6e74 2e72  omplete(client.r
+00000740: 756e 2829 290d 0a7e 7e7e 7e7e 7e7e 7e7e  un())..~~~~~~~~~
+00000750: 7e7e 7e7e 0d0a 596f 7520 6361 6e20 6669  ~~~~..You can fi
+00000760: 6e64 206d 6f72 6520 6578 616d 706c 6573  nd more examples
+00000770: 2069 6e20 7468 6520 6578 616d 706c 6573   in the examples
+00000780: 2064 6972 6563 746f 7279 205b 5468 6572   directory [Ther
+00000790: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000007a0: 622e 636f 6d2f 4d61 7365 5a65 762f 4c69  b.com/MaseZev/Li
+000007b0: 6163 6f72 642e 7079 2f74 7265 652f 6d61  acord.py/tree/ma
+000007c0: 696e 2f65 7861 6d70 6c65 7329 2e0d 0a0d  in/examples)....
+000007d0: 0a0d 0a4c 696e 6b73 0d0a 0d0a 0d0a 3c62  ...Links......<b
+000007e0: 723e 0d0a 3c70 2061 6c69 676e 3d22 6365  r>..<p align="ce
+000007f0: 6e74 6572 223e 0d0a 2020 2020 3c61 2068  nter">..    <a h
+00000800: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
+00000810: 636f 7264 2e67 672f 4837 4651 4647 4550  cord.gg/H7FQFGEP
+00000820: 7a35 223e 4469 7363 6f72 6420 5365 7276  z5">Discord Serv
+00000830: 6572 3c2f 613e 0d0a 2020 2020 e281 950d  er</a>..    ....
+00000840: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000850: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00000860: 2f64 6973 636f 7264 2d64 6576 656c 6f70  /discord-develop
+00000870: 6572 7322 3e44 6973 636f 7264 2044 6576  ers">Discord Dev
+00000880: 656c 6f70 6572 733c 2f61 3e0d 0a3c 2f70  elopers</a>..</p
+00000890: 3e0d 0a3c 6272 3e0d 0a0d 0a              >..<br>....
```

### Comparing `Liacord-0.1.5/setup.py` & `Liacord-0.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 setup(name='Liacord',
       author="Masezev",
       url="https://github.com/masezev/Liacord.py",
       project_urls={
           'Discord': 'https://discord.gg/H7FQFGEPz5',
       },
       repository='https://github.com/masezev/Liacord.py',
-      version='0.1.5',
+      version='0.1.6',
       description='A Python wrapper for the Discord API',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
+      python_requires='>=3.8.0',
+      keywords='A Python wrapper for the Discord API',
+      install_requires=[
+            'aiohttp'
+      ],
       packages=['Liacord'],
       license='MIT',
       author_email='csgomanagement1@gmail.com',
       zip_safe=False)
```

