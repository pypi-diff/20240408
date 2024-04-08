# Comparing `tmp/hyperglot-0.6.2.tar.gz` & `tmp/hyperglot-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperglot-0.6.2.tar", last modified: Fri Mar 22 13:32:25 2024, max compression
+gzip compressed data, was "hyperglot-0.6.3.tar", last modified: Mon Apr  8 12:22:08 2024, max compression
```

## Comparing `hyperglot-0.6.2.tar` & `hyperglot-0.6.3.tar`

### file list

```diff
@@ -1,814 +1,814 @@
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.427056 hyperglot-0.6.2/
--rw-r--r--   0 johannes   (501) staff       (20)    35145 2022-06-21 08:09:24.000000 hyperglot-0.6.2/LICENSE.txt
--rw-r--r--   0 johannes   (501) staff       (20)    14560 2024-03-22 13:32:25.426795 hyperglot-0.6.2/PKG-INFO
--rw-r--r--   0 johannes   (501) staff       (20)    13584 2024-03-22 13:19:29.000000 hyperglot-0.6.2/README.md
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.319668 hyperglot-0.6.2/lib/
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.321359 hyperglot-0.6.2/lib/hyperglot/
--rw-r--r--   0 johannes   (501) staff       (20)     1306 2024-03-22 13:32:09.000000 hyperglot-0.6.2/lib/hyperglot/__init__.py
--rw-r--r--   0 johannes   (501) staff       (20)    17713 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/checker.py
--rw-r--r--   0 johannes   (501) staff       (20)    22319 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/cli.py
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.425299 hyperglot-0.6.2/lib/hyperglot/data/
--rw-r--r--   0 johannes   (501) staff       (20)      215 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aae.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      319 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aaq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aar.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      936 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      341 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      520 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      498 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      556 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      419 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      220 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/abv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      331 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ace.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      607 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ach.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      642 2024-01-03 13:03:47.000000 hyperglot-0.6.2/lib/hyperglot/data/acm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      263 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/acq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      351 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/acu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      583 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/acw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      200 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/acx.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      341 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/acz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      561 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ada.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      674 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ade.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      433 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ady.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      216 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aeb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      213 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aec.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      368 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aer.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      596 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/afb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      502 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/afr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      731 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/agq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/agr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/agx.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      412 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aha.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aht.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      900 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aii.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      876 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ain.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      189 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aiq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1009 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ajg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      601 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ajp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     6360 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/akk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      517 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ale.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      351 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aln.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      480 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/alq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      204 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/als.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/alt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      237 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/amc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      263 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ame.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1249 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/amh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ami.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      232 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/amr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/anc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ani.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      391 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/anw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      588 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/any.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      381 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aoz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      213 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/apc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      586 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/apd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      381 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/apn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      446 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aqc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      668 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      356 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      251 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      315 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      231 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      513 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      586 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ars.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      229 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ary.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      605 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/arz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/asa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1012 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/asm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      385 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ast.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      415 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/atv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      253 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/auc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      353 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/aud.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      421 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ava.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      517 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ave.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      216 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/avl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      564 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/avn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      847 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/awa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      367 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/awe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1439 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/awn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      430 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      211 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      197 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      205 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      216 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      235 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      356 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ayr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      673 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/azb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      822 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/azj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      743 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/azo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      755 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bak.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      634 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bal.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      592 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1164 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ban.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      781 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bas.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      527 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bax.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      392 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bba.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      957 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bbc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      638 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bbo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      266 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bci.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      408 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bdk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      491 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/beh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1031 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bel.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bem.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      729 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ben.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bez.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      516 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bfa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      472 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bfo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      310 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bhh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      968 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bho.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      679 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bib.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      405 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bik.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      354 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bin.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bis.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      515 2024-03-22 13:29:57.000000 hyperglot-0.6.2/lib/hyperglot/data/bjn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      680 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bjt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      768 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bkm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      944 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/blo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      530 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/blt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      493 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bmq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      291 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/boa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      615 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bod.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1456 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bos.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      641 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/box.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      890 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/boz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      724 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bpy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      499 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bqc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      358 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bre.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      767 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/brx.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1408 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bsc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      746 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bss.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      966 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/btd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1001 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/btm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1005 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bts.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      980 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/btx.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      362 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/buc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      990 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bug.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1051 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bul.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      514 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bwj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      367 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bwq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      708 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bxm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      702 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bxr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      703 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bxu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1937 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/byn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      686 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/byv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      722 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/bze.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      346 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cab.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      343 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cak.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      835 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cbi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      321 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cbk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      297 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cbr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cbs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      261 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cbt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      253 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cbu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      834 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ccp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ceb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      412 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ces.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      263 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cfm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cgg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      357 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cha.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      447 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/che.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/chj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/chk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      920 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/chr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      597 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/chu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/chv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      662 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cic.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      401 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cim.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cji.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      283 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cjk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      441 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cjs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      188 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cjy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      761 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ckb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      609 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cko.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      533 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ckt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      584 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cme.yaml
--rw-r--r--   0 johannes   (501) staff       (20)    10924 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cmn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cnh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cni.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      343 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cnr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cof.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      340 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/con_.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/coo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      348 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cor.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      370 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cos.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      276 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cot.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      706 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cou.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      246 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cpu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      830 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/crh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/crs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/csa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      434 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/csb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      519 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/csw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      268 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ctd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      691 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ctg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      513 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/cym.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1050 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dag.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      359 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dan.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      427 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dar.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dav.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      767 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ddn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      380 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ddo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      190 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/deh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1174 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/deu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1234 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dga.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      833 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dgi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dgl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1145 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dgo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dhv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      552 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/din.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      203 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dip.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      428 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/diq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      340 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/div.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      684 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dje.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      449 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dlg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dng.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      831 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dno.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      127 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/doi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      702 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dop.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      410 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dsb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      219 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dty.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      693 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dua.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      458 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dya.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      734 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dyo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      933 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dyu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      592 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/dzo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ebu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      542 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/efi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     5560 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/egy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      379 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ekk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      472 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/eky.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      480 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ell.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      817 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/emk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      407 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ems.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      442 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/enf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      816 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/eng.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      620 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/enh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      341 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/epo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      211 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ese.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      462 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ess.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      360 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/esu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/eus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      459 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/eve.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      490 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/evn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      890 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ewe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      751 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ewo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fao.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      252 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ffm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      235 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fia.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fij.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      331 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fil.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fin.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      333 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fkv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      768 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fmp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      706 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fod.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      502 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fon.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fra.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      408 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fry.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      557 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fub.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      634 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fuc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      570 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fue.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      618 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fuf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      223 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fuh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      556 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fui.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      551 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fuq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      456 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fur.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      280 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/fuv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      577 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gaa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      702 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gag.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      373 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gah.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      421 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gan.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gax.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gaz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      362 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gcf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      649 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gej.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1057 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gez.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      253 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gil.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      544 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gjn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      588 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gkp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      378 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gla.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      488 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gld.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      349 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gle.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      425 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/glg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/glv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1198 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gmy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      374 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gni.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      520 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gom.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      561 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gqa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1300 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/grc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gsw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/guc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      393 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gug.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      806 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/guj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      659 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gur.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/guu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      682 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gux.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/guz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/gwi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      409 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/haa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      193 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hae.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      656 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/haj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      336 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hak.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1051 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/har.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      375 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      477 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hau.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      647 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/haw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      270 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/haz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hea.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      413 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/heb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hil.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      826 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hin.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hms.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hni.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      571 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hnn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      371 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hns.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hop.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      365 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hrv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      406 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hsb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      395 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hun.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      480 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hur.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      261 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      265 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/huu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      422 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/huz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      661 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hye.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/hyw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      286 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ibb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      474 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ibo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      290 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ido.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      832 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/idu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      760 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ife.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      272 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/igs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     4865 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/iii.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      750 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ike.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      408 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ile.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ilo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      413 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ina.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1110 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ind.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      436 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/inh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/isl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      417 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ita.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      493 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/itl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      319 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1134 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jav.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      544 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jbo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      418 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jct.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      868 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jdt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      720 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jgo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      297 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jiv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)    10073 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jpn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      152 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/jpr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      703 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kaa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      411 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kab.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      745 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kal.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      325 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      745 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kan.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      488 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kap.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     2147 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      409 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kau.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      491 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kaz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      440 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kbd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      771 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kbp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      519 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kca.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      295 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kde.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      551 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kdh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      423 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kdr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      441 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kea.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kek.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      463 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ket.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      808 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/keu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      198 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kfr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      356 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kgp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kha.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      439 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/khk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      724 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/khm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      621 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/khq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      593 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kik.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kin.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      442 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kir.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kiu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kjh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      495 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kjj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      439 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kkh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1640 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kkj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      487 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kln.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      243 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kmb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1023 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kmr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      727 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/knf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/knn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      442 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/koi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      129 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kok.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kon.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/koo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)    48520 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kor.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      453 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kpt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      428 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kpv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      522 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kpy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kqn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      269 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kqs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      455 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/krc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      516 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kri.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      355 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/krl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ksb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      620 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ksf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      700 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ksh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      554 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kst.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ktu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kua.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      422 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kum.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      711 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kwi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      638 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kwk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      472 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/kyu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1841 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lab.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lad.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      352 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lag.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      614 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      663 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lao.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      415 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lbe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1261 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lee.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      427 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lez.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      618 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lia.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      428 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lij.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lin.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1191 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/linb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lit.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      657 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lkt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      440 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lld.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      405 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lmo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      522 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lns.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lob.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      541 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lot.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/loz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ltg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      439 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ltz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lua.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      388 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lub.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      549 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lug.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      384 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/luo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      320 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      417 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lvs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      543 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/lzz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      448 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mad.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      822 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mag.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      475 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mah.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      924 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mai.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      747 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mal.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      282 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1107 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mar.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      701 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mas.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      327 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/maz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      416 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mcd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      282 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mcf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      780 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mcn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      429 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mdf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/men.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mer.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      600 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mey.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      329 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mfe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1312 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mfq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      747 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mfv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mgh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      625 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mgo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      449 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mhr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      376 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mic.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      489 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/min.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/miq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      951 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mkd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      739 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mlg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      394 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mlt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      726 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mni.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      686 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mnk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      441 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mns.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1180 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mnw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      573 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/moe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/moh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      312 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mos.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      493 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mql.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      306 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mqm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mri.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mrj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      453 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mrq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      241 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mto.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      620 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mua.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      313 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      306 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mwf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      386 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mwl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1288 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mwp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mxv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      821 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mya.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      933 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/myk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      417 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/myv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      251 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/mzi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nag.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      229 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nan.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nap.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      551 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/naq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      661 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nav.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      521 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nba.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nbl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      313 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nde.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      252 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ndo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      364 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nds.yaml
--rw-r--r--   0 johannes   (501) staff       (20)       70 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nep.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      347 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nhn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      586 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nio.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      448 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/niu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      476 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/niv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      179 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/njo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      549 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nku.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      686 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nld.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      759 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nmg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      734 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nmz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      766 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nnh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      815 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nnw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nog.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      378 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/non.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      494 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nor.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      267 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/not.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nov.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1196 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/npi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nso.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      487 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ntm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      339 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nuk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      665 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      577 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nya.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nym.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nyn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      849 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nza.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      259 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/nzi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      400 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/oaa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      445 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/oci.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      283 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ojb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      704 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/oji.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/oma.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     2939 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/omn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      711 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/onw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      181 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/orc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/orh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      752 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ori.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      625 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/oss.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      998 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ota.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      332 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ote.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1742 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ozm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1106 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pan.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      339 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pap.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      283 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pau.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      312 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pbb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      554 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pbu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      401 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pcd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      596 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pes.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      232 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pga.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      677 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pil.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      302 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pis.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      214 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/piu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/plz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      387 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pms.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      298 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pnb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      877 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pnt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      364 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pol.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      245 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pon.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      599 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/por.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      385 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pot.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      288 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pov.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      254 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ppl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      388 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/prg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      255 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/prq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      206 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/prs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1078 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/pug.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      275 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/quc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      668 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/que.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      218 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/qxq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      649 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rah.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      447 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rar.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      808 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rkt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      727 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rmn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      398 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rmy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/roh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1200 2024-01-30 07:16:12.000000 hyperglot-0.6.2/lib/hyperglot/data/ron.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      238 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/roo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      688 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rue.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/run.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      396 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ruo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      369 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rup.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      488 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ruq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      915 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      433 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rut.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      245 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/rwk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1183 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ryu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      378 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sag.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      449 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sah.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1123 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/san.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/saq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      711 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sav.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      875 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sbd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      464 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sbp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      357 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/scn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      507 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sco.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      227 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sdh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      298 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/seh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      320 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sei.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      489 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sel.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      632 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ses.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sey.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      444 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sgh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1358 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sgw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/shi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      647 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/shk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      751 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/shn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      243 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/shp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      199 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/shu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      762 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/shz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      578 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sin.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      547 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sjd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      596 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sje.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      433 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sjt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      649 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sju.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sjw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      512 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/skr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      709 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sld.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      447 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/slk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      387 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/slv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sma.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      664 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sme.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      830 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/smj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      653 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/smn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      339 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/smo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      726 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sms.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sna.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1397 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/snd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      730 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/snf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      291 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/snk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      347 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/snn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/som.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sot.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      729 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/soy.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      370 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/spa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      421 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/srd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/srm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      333 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/srn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1633 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/srp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      593 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/srr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ssw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      287 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/suk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      959 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sun.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      284 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sus.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     6352 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sux.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      603 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sva.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      665 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/swb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      155 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/swc.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      389 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/swe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/swh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      625 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/sxw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      401 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/szl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      437 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tab.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      412 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tah.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/taj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1275 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tam.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tat.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      616 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tay.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      785 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tbz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      321 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tca.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      205 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tdt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      837 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tel.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      536 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tem.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1019 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/teo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      399 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tet.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      443 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tgk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      691 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tgl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      868 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tha.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/thp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1289 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tig.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      994 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tik.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1478 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tir.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      273 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tiv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tkl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      576 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tkr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      644 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/data/tlh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     5823 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tli.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      628 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tly.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      744 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tnr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      240 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tob.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      728 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tod.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/toi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/toj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      484 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ton.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      279 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/top.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tpi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      326 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tsn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tso.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tsz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1156 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ttq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ttt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      723 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tuk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tum.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      511 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tur.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      975 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tuz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      546 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tvl.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/twi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      611 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/twq.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      437 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tyv.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      267 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tzh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      380 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tzm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/tzo.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/udi.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      451 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/udm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      975 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/uig.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      811 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ukr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ulk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/umb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      366 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/umu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ura.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      647 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/urd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      398 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/uum.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      961 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/uzn.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      501 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/uzs.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1385 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vai.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vec.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      336 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ven.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      350 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vep.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1087 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vie.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vmw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      332 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vol.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      345 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/vro.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      628 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wae.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      577 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/war.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wbp.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      679 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wci.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      286 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wim.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      343 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/win.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wln.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      351 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wls.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      197 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wmw.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      631 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wol.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      284 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wrh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wss.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      193 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wuu.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1031 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wwa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/wyb.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      453 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xal.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1407 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xan.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1686 2024-03-22 13:29:57.000000 hyperglot-0.6.2/lib/hyperglot/data/xav.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xha.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      312 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xhd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xho.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      520 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xmf.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      195 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xnr.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      258 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xnz.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      288 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xog.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      311 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xqt.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      534 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xrg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xsa.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      905 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xsm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      663 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/xwe.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      337 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yad.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      456 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yai.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      257 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yao.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yap.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      724 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yav.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      404 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ydd.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      223 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yih.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      286 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yij.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      430 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ykg.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/ymk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      892 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yor.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yrk.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yua.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      223 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yue.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/yux.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      774 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zap.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      674 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zdj.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      636 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zgh.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      346 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zlm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      290 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zro.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     1230 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zsm.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zul.yaml
--rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.2/lib/hyperglot/data/zun.yaml
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.425428 hyperglot-0.6.2/lib/hyperglot/extra_data/
--rw-r--r--   0 johannes   (501) staff       (20)    18896 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/extra_data/joining-types.yaml
--rw-r--r--   0 johannes   (501) staff       (20)     9170 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/language.py
--rw-r--r--   0 johannes   (501) staff       (20)    11762 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/languages.py
--rw-r--r--   0 johannes   (501) staff       (20)     9690 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/orthography.py
--rw-r--r--   0 johannes   (501) staff       (20)    12140 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/parse.py
--rw-r--r--   0 johannes   (501) staff       (20)     8469 2024-03-22 13:29:57.000000 hyperglot-0.6.2/lib/hyperglot/shaper.py
--rw-r--r--   0 johannes   (501) staff       (20)    14974 2024-01-16 10:42:34.000000 hyperglot-0.6.2/lib/hyperglot/validate.py
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.426518 hyperglot-0.6.2/lib/hyperglot.egg-info/
--rw-r--r--   0 johannes   (501) staff       (20)    14560 2024-03-22 13:32:25.000000 hyperglot-0.6.2/lib/hyperglot.egg-info/PKG-INFO
--rw-r--r--   0 johannes   (501) staff       (20)    22493 2024-03-22 13:32:25.000000 hyperglot-0.6.2/lib/hyperglot.egg-info/SOURCES.txt
--rw-r--r--   0 johannes   (501) staff       (20)        1 2024-03-22 13:32:25.000000 hyperglot-0.6.2/lib/hyperglot.egg-info/dependency_links.txt
--rw-r--r--   0 johannes   (501) staff       (20)      260 2024-03-22 13:32:25.000000 hyperglot-0.6.2/lib/hyperglot.egg-info/entry_points.txt
--rw-r--r--   0 johannes   (501) staff       (20)       95 2024-03-22 13:32:25.000000 hyperglot-0.6.2/lib/hyperglot.egg-info/requires.txt
--rw-r--r--   0 johannes   (501) staff       (20)       10 2024-03-22 13:32:25.000000 hyperglot-0.6.2/lib/hyperglot.egg-info/top_level.txt
--rw-r--r--   0 johannes   (501) staff       (20)       38 2024-03-22 13:32:25.427091 hyperglot-0.6.2/setup.cfg
--rw-r--r--   0 johannes   (501) staff       (20)     2719 2024-01-16 10:42:34.000000 hyperglot-0.6.2/setup.py
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-03-22 13:32:25.426311 hyperglot-0.6.2/tests/
--rw-r--r--   0 johannes   (501) staff       (20)    17347 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_checker.py
--rw-r--r--   0 johannes   (501) staff       (20)    10101 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_cli.py
--rw-r--r--   0 johannes   (501) staff       (20)     2465 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_language.py
--rw-r--r--   0 johannes   (501) staff       (20)     1568 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_languages.py
--rw-r--r--   0 johannes   (501) staff       (20)     4713 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_orthography.py
--rw-r--r--   0 johannes   (501) staff       (20)     7390 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_parse.py
--rw-r--r--   0 johannes   (501) staff       (20)     3249 2024-01-16 10:42:34.000000 hyperglot-0.6.2/tests/test_shaper.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.588543 hyperglot-0.6.3/
+-rw-r--r--   0 johannes   (501) staff       (20)    35145 2022-06-21 08:09:24.000000 hyperglot-0.6.3/LICENSE.txt
+-rw-r--r--   0 johannes   (501) staff       (20)    14560 2024-04-08 12:22:08.588302 hyperglot-0.6.3/PKG-INFO
+-rw-r--r--   0 johannes   (501) staff       (20)    13584 2024-03-22 13:19:29.000000 hyperglot-0.6.3/README.md
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.470571 hyperglot-0.6.3/lib/
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.472522 hyperglot-0.6.3/lib/hyperglot/
+-rw-r--r--   0 johannes   (501) staff       (20)     2862 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/__init__.py
+-rw-r--r--   0 johannes   (501) staff       (20)    17851 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/checker.py
+-rw-r--r--   0 johannes   (501) staff       (20)    22368 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/cli.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.586743 hyperglot-0.6.3/lib/hyperglot/data/
+-rw-r--r--   0 johannes   (501) staff       (20)      215 2024-04-08 10:33:00.000000 hyperglot-0.6.3/lib/hyperglot/data/aae.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      319 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aaq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aar.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      936 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      341 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      520 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      498 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      556 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      419 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      220 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/abv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      331 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ace.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      607 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ach.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      642 2024-01-03 13:03:47.000000 hyperglot-0.6.3/lib/hyperglot/data/acm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      263 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/acq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      351 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/acu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      583 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/acw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      200 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/acx.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      341 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/acz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      561 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ada.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      674 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ade.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      433 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ady.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      216 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aeb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      213 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aec.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      368 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aer.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      596 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/afb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      502 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/afr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      731 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/agq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/agr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/agx.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      412 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aha.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aht.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      900 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aii.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      876 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ain.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      189 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aiq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1009 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ajg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      601 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ajp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     6360 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/akk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      517 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ale.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      351 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aln.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      480 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/alq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      204 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/als.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/alt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      237 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/amc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      263 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ame.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1249 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/amh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ami.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      232 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/amr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/anc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ani.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      391 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/anw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      588 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/any.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      381 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aoz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      213 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/apc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      586 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/apd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      381 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/apn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      446 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aqc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      668 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      356 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      251 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      315 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      231 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      513 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      586 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ars.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      229 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ary.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      605 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/arz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/asa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1012 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/asm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      385 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ast.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      415 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/atv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      253 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/auc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      353 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/aud.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      421 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ava.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      517 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ave.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      216 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/avl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      564 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/avn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      847 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/awa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      367 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/awe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1439 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/awn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      430 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      211 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      197 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      205 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      216 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      235 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      356 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ayr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      673 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/azb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      822 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/azj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      743 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/azo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      755 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bak.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      634 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bal.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      592 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1164 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ban.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      781 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bas.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      527 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bax.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      392 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bba.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      957 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bbc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      638 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bbo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      266 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bci.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      408 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bdk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      491 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/beh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1031 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bel.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bem.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      729 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ben.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bez.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      516 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bfa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      472 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bfo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      310 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bhh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      968 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bho.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      679 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bib.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      405 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bik.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      354 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bin.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bis.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      515 2024-03-22 13:29:57.000000 hyperglot-0.6.3/lib/hyperglot/data/bjn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      680 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bjt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      768 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bkm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      944 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/blo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      530 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/blt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      493 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bmq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      291 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/boa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      615 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bod.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1456 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bos.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      641 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/box.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      890 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/boz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      724 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bpy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      499 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bqc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      358 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bre.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      767 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/brx.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1408 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bsc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      746 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bss.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      966 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/btd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1001 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/btm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1005 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bts.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      980 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/btx.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      362 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/buc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      990 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bug.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1051 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bul.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      514 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bwj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      367 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bwq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      708 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bxm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      702 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bxr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      703 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bxu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1937 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/byn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      686 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/byv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      722 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/bze.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      346 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cab.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      343 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cak.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      835 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cbi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      321 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cbk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      297 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cbr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cbs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      261 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cbt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      253 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cbu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      834 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ccp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ceb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      412 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ces.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      263 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cfm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cgg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      357 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cha.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      447 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/che.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/chj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/chk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      920 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/chr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      597 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/chu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/chv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      662 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cic.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      401 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cim.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cji.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      283 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cjk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      441 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cjs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      188 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cjy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      761 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ckb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      609 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cko.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      533 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ckt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      584 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cme.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)    10924 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cmn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cnh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cni.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      343 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cnr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cof.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      340 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/con_.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/coo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      348 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cor.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      370 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cos.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      276 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cot.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      706 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cou.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      246 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cpu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      830 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/crh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/crs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/csa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      434 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/csb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      519 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/csw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      268 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ctd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      691 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ctg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      513 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/cym.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1050 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dag.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      359 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dan.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      427 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dar.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dav.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      767 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ddn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      380 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ddo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      190 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/deh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1174 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/deu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1234 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dga.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      833 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dgi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dgl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1145 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dgo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dhv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      552 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/din.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      203 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dip.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      428 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/diq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      340 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/div.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      684 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dje.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      449 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dlg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dng.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      831 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dno.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      127 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/doi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      702 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dop.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      410 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dsb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      219 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dty.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      693 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dua.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      458 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dya.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      734 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dyo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      933 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dyu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      592 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/dzo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ebu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      542 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/efi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     5560 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/egy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      379 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ekk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      472 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/eky.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      480 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ell.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      817 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/emk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      407 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ems.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      442 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/enf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      816 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/eng.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      620 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/enh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      341 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/epo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      211 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ese.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      462 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ess.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      360 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/esu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/eus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      459 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/eve.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      490 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/evn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      890 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ewe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      751 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ewo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fao.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      252 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ffm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      235 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fia.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fij.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      331 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fil.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fin.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      333 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fkv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      768 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fmp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      706 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fod.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      502 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fon.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fra.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      408 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fry.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      557 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fub.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      634 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fuc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      570 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fue.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      618 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fuf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      223 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fuh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      556 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fui.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      551 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fuq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      456 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fur.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      280 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/fuv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      577 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gaa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      702 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gag.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      373 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gah.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      421 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gan.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gax.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gaz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      362 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gcf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      649 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gej.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1057 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gez.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      253 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gil.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      544 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gjn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      588 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gkp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      378 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gla.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      488 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gld.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      349 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gle.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      425 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/glg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/glv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1198 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gmy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      374 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gni.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      520 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gom.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      561 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gqa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1300 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/grc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gsw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/guc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      393 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gug.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      806 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/guj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      659 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gur.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/guu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      682 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gux.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/guz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/gwi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      409 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/haa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      193 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hae.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      656 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/haj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      336 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hak.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1051 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/har.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      375 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      477 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hau.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      647 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/haw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      270 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/haz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hea.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      413 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/heb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hil.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      826 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hin.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      304 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hms.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hni.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      571 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hnn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      371 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hns.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hop.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      365 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hrv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      406 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hsb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      395 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hun.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      480 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hur.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      261 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      265 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/huu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      422 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/huz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      661 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hye.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/hyw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      286 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ibb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      474 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ibo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      290 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ido.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      832 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/idu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      760 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ife.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      272 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/igs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     4865 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/iii.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      750 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ike.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      408 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ile.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      316 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ilo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      413 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ina.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1110 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ind.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      436 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/inh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/isl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      417 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ita.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      493 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/itl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      319 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1134 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jav.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      544 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jbo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      418 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jct.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      868 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jdt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      720 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jgo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      297 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jiv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)    10073 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jpn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      152 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/jpr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      703 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kaa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      411 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kab.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      745 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kal.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      325 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      745 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kan.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      488 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kap.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     2147 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      409 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kau.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      491 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kaz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      440 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kbd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      771 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kbp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      519 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kca.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      295 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kde.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      551 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kdh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      423 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kdr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      441 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kea.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kek.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      463 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ket.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      808 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/keu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      198 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kfr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      356 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kgp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kha.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      439 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/khk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      724 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/khm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      621 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/khq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      593 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kik.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kin.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      442 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kir.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kiu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kjh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      495 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kjj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      439 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kkh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1640 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kkj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      487 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kln.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      243 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kmb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1023 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kmr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      727 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/knf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/knn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      442 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/koi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      129 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kok.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kon.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/koo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)    48520 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kor.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      453 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kpt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      428 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kpv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      522 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kpy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kqn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      269 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kqs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      455 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/krc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      516 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kri.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      355 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/krl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ksb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      620 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ksf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      700 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ksh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      554 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kst.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ktu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kua.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      422 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kum.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      711 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kwi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      638 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kwk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      472 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/kyu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1841 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lab.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lad.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      352 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lag.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      614 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      663 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lao.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      415 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lbe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1261 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lee.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      427 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lez.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      618 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lia.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      428 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lij.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lin.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1191 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/linb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lit.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      657 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lkt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      440 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lld.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      405 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lmo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      522 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lns.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lob.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      541 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lot.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/loz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ltg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      439 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ltz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lua.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      388 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lub.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      549 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lug.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      384 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/luo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      320 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      417 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lvs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      543 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/lzz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      448 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mad.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      822 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mag.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      475 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mah.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      924 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mai.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      747 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mal.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      282 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1107 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mar.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      701 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mas.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      327 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/maz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      416 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mcd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      282 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mcf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      780 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mcn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      429 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mdf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/men.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mer.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      600 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mey.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      329 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mfe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1312 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mfq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      747 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mfv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mgh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      625 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mgo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      449 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mhr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      376 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mic.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      489 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/min.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/miq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      951 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mkd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      739 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mlg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      394 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mlt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      726 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mni.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      686 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mnk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      441 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mns.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1180 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mnw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      573 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/moe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/moh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      312 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mos.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      493 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mql.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      306 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mqm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      344 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mri.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mrj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      453 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mrq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      241 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mto.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      620 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mua.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      313 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      306 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mwf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      386 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mwl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1288 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mwp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mxv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      821 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mya.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      933 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/myk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      417 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/myv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      251 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/mzi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nag.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      229 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nan.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nap.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      551 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/naq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      661 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nav.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      521 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nba.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nbl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      313 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nde.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      252 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ndo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      364 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nds.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)       70 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nep.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      347 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nhn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      586 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nio.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      448 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/niu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      476 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/niv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      179 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/njo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      549 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nku.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      686 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nld.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      759 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nmg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      734 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nmz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      766 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nnh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      815 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nnw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nog.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      378 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/non.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      494 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nor.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      267 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/not.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nov.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1196 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/npi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nso.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      487 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ntm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      339 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nuk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      665 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      577 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nya.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nym.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nyn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      849 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nza.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      259 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/nzi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      400 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/oaa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      445 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/oci.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      283 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ojb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      704 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/oji.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/oma.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     2939 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/omn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      711 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/onw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      181 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/orc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/orh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      752 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ori.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      625 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/oss.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      998 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ota.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      332 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ote.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1742 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ozm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1106 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pan.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      339 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pap.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      283 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pau.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      312 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pbb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      554 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pbu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      401 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pcd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      596 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pes.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      232 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pga.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      677 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pil.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      302 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pis.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      214 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/piu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/plz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      387 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pms.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      298 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pnb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      877 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pnt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      364 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pol.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      245 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pon.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      599 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/por.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      385 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pot.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      288 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pov.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      254 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ppl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      388 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/prg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      255 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/prq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      206 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/prs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1078 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/pug.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      275 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/quc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      668 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/que.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      218 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/qxq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      649 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rah.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      447 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rar.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      808 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rkt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      727 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rmn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      398 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rmy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/roh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1200 2024-01-30 07:16:12.000000 hyperglot-0.6.3/lib/hyperglot/data/ron.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      238 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/roo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      688 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rue.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      294 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/run.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      396 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ruo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      369 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rup.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      488 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ruq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      915 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      433 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rut.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      245 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/rwk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1183 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ryu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      378 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sag.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      449 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sah.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1123 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/san.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      289 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/saq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      711 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sav.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      875 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sbd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      464 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sbp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      357 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/scn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      507 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sco.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      227 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sdh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      298 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/seh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      320 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sei.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      489 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sel.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      632 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ses.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sey.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      444 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sgh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1358 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sgw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      431 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/shi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      647 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/shk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      751 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/shn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      243 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/shp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      199 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/shu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      762 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/shz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      578 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sin.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      547 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sjd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      596 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sje.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      433 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sjt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      649 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sju.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sjw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      512 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/skr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      709 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sld.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      447 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/slk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      387 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/slv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      372 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sma.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      664 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sme.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      830 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/smj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      653 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/smn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      339 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/smo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      726 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sms.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sna.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1397 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/snd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      730 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/snf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      291 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/snk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      347 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/snn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/som.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sot.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      729 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/soy.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      370 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/spa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      421 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/srd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/srm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      333 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/srn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1633 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/srp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      593 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/srr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      285 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ssw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      287 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/suk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      959 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sun.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      284 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sus.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     6352 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sux.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      603 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sva.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      665 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/swb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      155 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/swc.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      389 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/swe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      402 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/swh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      625 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/sxw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      401 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/szl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      437 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tab.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      412 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tah.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/taj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1275 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tam.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      454 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tat.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      616 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tay.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      785 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tbz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      321 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tca.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      205 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tdt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      837 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tel.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      536 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tem.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1019 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/teo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      399 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tet.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      443 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tgk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      691 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tgl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      868 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tha.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/thp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1289 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tig.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      994 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tik.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1478 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tir.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      273 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tiv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tkl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      576 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tkr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      644 2024-01-16 10:42:34.000000 hyperglot-0.6.3/lib/hyperglot/data/tlh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     5823 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tli.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      628 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tly.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      744 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tnr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      240 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tob.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      728 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tod.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/toi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      281 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/toj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      484 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ton.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      279 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/top.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      303 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tpi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      326 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tsn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      300 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tso.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      292 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tsz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1156 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ttq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      503 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ttt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      723 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tuk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tum.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      511 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tur.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      975 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tuz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      546 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tvl.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/twi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      611 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/twq.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      437 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tyv.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      267 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tzh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      380 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tzm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/tzo.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      420 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/udi.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      451 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/udm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      975 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/uig.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      811 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ukr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      335 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ulk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      309 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/umb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      366 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/umu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      277 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ura.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      647 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/urd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      398 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/uum.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      961 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/uzn.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      501 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/uzs.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1385 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vai.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      403 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vec.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      336 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ven.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      350 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vep.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1087 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vie.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      328 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vmw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      332 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vol.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      345 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/vro.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      628 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wae.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      577 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/war.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      296 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wbp.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      679 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wci.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      286 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wim.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      343 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/win.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      390 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wln.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      351 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wls.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      197 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wmw.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      631 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wol.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      284 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wrh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wss.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      193 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wuu.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1031 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wwa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      293 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/wyb.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      453 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xal.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1407 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xan.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1686 2024-03-22 13:29:57.000000 hyperglot-0.6.3/lib/hyperglot/data/xav.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xha.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      312 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xhd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      299 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xho.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      520 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xmf.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      195 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xnr.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      258 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xnz.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      288 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xog.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      311 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xqt.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      534 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xrg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xsa.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      905 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xsm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      663 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/xwe.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      337 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yad.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      456 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yai.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      257 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yao.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      308 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yap.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      724 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yav.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      404 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ydd.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      223 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yih.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      286 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yij.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      430 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ykg.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      278 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/ymk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      892 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yor.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yrk.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      338 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yua.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      223 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yue.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      435 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/yux.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      774 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zap.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      674 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zdj.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      636 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zgh.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      346 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zlm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      290 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zro.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     1230 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zsm.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zul.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)      305 2023-12-19 10:29:01.000000 hyperglot-0.6.3/lib/hyperglot/data/zun.yaml
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.586879 hyperglot-0.6.3/lib/hyperglot/extra_data/
+-rw-r--r--   0 johannes   (501) staff       (20)    18896 2024-01-16 10:42:34.000000 hyperglot-0.6.3/lib/hyperglot/extra_data/joining-types.yaml
+-rw-r--r--   0 johannes   (501) staff       (20)     9346 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/language.py
+-rw-r--r--   0 johannes   (501) staff       (20)    11901 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/languages.py
+-rw-r--r--   0 johannes   (501) staff       (20)     9777 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/orthography.py
+-rw-r--r--   0 johannes   (501) staff       (20)    12140 2024-01-16 10:42:34.000000 hyperglot-0.6.3/lib/hyperglot/parse.py
+-rw-r--r--   0 johannes   (501) staff       (20)     8469 2024-03-22 13:29:57.000000 hyperglot-0.6.3/lib/hyperglot/shaper.py
+-rw-r--r--   0 johannes   (501) staff       (20)    15981 2024-04-08 12:21:14.000000 hyperglot-0.6.3/lib/hyperglot/validate.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.588009 hyperglot-0.6.3/lib/hyperglot.egg-info/
+-rw-r--r--   0 johannes   (501) staff       (20)    14560 2024-04-08 12:22:08.000000 hyperglot-0.6.3/lib/hyperglot.egg-info/PKG-INFO
+-rw-r--r--   0 johannes   (501) staff       (20)    22493 2024-04-08 12:22:08.000000 hyperglot-0.6.3/lib/hyperglot.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes   (501) staff       (20)        1 2024-04-08 12:22:08.000000 hyperglot-0.6.3/lib/hyperglot.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes   (501) staff       (20)      260 2024-04-08 12:22:08.000000 hyperglot-0.6.3/lib/hyperglot.egg-info/entry_points.txt
+-rw-r--r--   0 johannes   (501) staff       (20)       95 2024-04-08 12:22:08.000000 hyperglot-0.6.3/lib/hyperglot.egg-info/requires.txt
+-rw-r--r--   0 johannes   (501) staff       (20)       10 2024-04-08 12:22:08.000000 hyperglot-0.6.3/lib/hyperglot.egg-info/top_level.txt
+-rw-r--r--   0 johannes   (501) staff       (20)       38 2024-04-08 12:22:08.588581 hyperglot-0.6.3/setup.cfg
+-rw-r--r--   0 johannes   (501) staff       (20)     2719 2024-04-08 11:59:24.000000 hyperglot-0.6.3/setup.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2024-04-08 12:22:08.587817 hyperglot-0.6.3/tests/
+-rw-r--r--   0 johannes   (501) staff       (20)    17433 2024-04-08 12:21:14.000000 hyperglot-0.6.3/tests/test_checker.py
+-rw-r--r--   0 johannes   (501) staff       (20)    10101 2024-01-16 10:42:34.000000 hyperglot-0.6.3/tests/test_cli.py
+-rw-r--r--   0 johannes   (501) staff       (20)     2906 2024-04-08 12:21:14.000000 hyperglot-0.6.3/tests/test_language.py
+-rw-r--r--   0 johannes   (501) staff       (20)     1568 2024-01-16 10:42:34.000000 hyperglot-0.6.3/tests/test_languages.py
+-rw-r--r--   0 johannes   (501) staff       (20)     5138 2024-04-08 12:21:14.000000 hyperglot-0.6.3/tests/test_orthography.py
+-rw-r--r--   0 johannes   (501) staff       (20)     7390 2024-01-16 10:42:34.000000 hyperglot-0.6.3/tests/test_parse.py
+-rw-r--r--   0 johannes   (501) staff       (20)     3249 2024-01-16 10:42:34.000000 hyperglot-0.6.3/tests/test_shaper.py
```

### Comparing `hyperglot-0.6.2/LICENSE.txt` & `hyperglot-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/PKG-INFO` & `hyperglot-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperglot
-Version: 0.6.2
+Version: 0.6.3
 Summary: Detect language support for font binaries
 Home-page: https://github.com/rosettatype/hyperglot
 Author: Johannes Neumeier - Rosetta
 Author-email: johannes@rosettatype.com
 License: GNU GPLv3
 Project-URL: Hyperglot web interface, https://hyperglot.rosettatype.com
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hyperglot-0.6.2/README.md` & `hyperglot-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/checker.py` & `hyperglot-0.6.3/lib/hyperglot/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Iterable
 
 from hyperglot.shaper import Shaper
 from hyperglot.languages import Languages
 from hyperglot.language import Language
 from hyperglot.orthography import Orthography
 from hyperglot.parse import parse_chars
-from hyperglot import SUPPORTLEVELS, VALIDITYLEVELS
+from hyperglot import SupportLevel, LanguageValidity
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.WARNING)
 
 log_missing = logging.getLogger("hyperglot.reporting.missing")
 log_missing.setLevel(logging.FATAL)
 
@@ -39,33 +39,33 @@
 
 class Checker:
     """
     A base class for CharsetChecker and FontChecker encapsulating language
     support checks.
     """
 
-    def __init__(self, fontpath=None, characters=None):
+    def __init__(self, fontpath: str = None, characters: List = None):
         self.fontpath = fontpath
         self.characters = characters
         self.font = None
         self.shaper = None
 
     def get_supported_languages(
         self,
-        supportlevel=list(SUPPORTLEVELS.keys())[0],
-        validity=VALIDITYLEVELS[1],
-        decomposed=False,
-        marks=False,
-        shaping=False,
-        include_all_orthographies=False,
-        include_historical=False,
-        include_constructed=False,
-        report_missing=-1,
-        report_marks=-1,
-        report_joining=-1,
+        supportlevel: str = SupportLevel.BASE.value,
+        validity: str = LanguageValidity.DRAFT.value,
+        decomposed: bool = False,
+        marks: bool = False,
+        shaping: bool = False,
+        include_all_orthographies: bool = False,
+        include_historical: bool = False,
+        include_constructed: bool = False,
+        report_missing: int = -1,
+        report_marks: int = -1,
+        report_joining: int = -1,
     ) -> dict:
         """
         Get all languages supported based on the passed in characters.
 
         @param supportlevel str: Check for 'base' (default) or 'aux' support.
         @param validatiy str: Filter by certainty of the database data.
             Defaults to 'weak', which ignores all but 'todo'. More stringent
@@ -98,15 +98,15 @@
             l = getattr(languages, iso)  # noqa, let's keep l short
 
             if "validity" not in l:
                 log.info("Skipping langauge '%s' which is missing " "'validity'" % iso)
                 continue
 
             # Skip languages below the currently selected validity level.
-            if VALIDITYLEVELS.index(l["validity"]) < VALIDITYLEVELS.index(validity):
+            if LanguageValidity.index(l["validity"]) < LanguageValidity.index(validity):
                 log.info("Skipping language '%s' which has lower " "'validity'" % iso)
                 continue
 
             if include_historical and l.is_historical():
                 log.info("Including historical language '%s'" % l.get_name())
             elif include_historical is False and l.is_historical():
                 log.info("Skipping historical language '%s'" % iso)
@@ -147,16 +147,16 @@
                         support[script][iso] = l
 
         return support
 
     def supports_language(
         self,
         iso: str,
-        supportlevel: str = "base",
-        validity: str = VALIDITYLEVELS[1],
+        supportlevel: str = SupportLevel.BASE.value,
+        validity: str = LanguageValidity.DRAFT.value,
         decomposed: bool = False,
         marks: bool = False,
         shaping: bool = False,
         check_all_orthographies: bool = False,
         report_missing: int = -1,
         report_marks: int = -1,
         report_joining: int = -1,
@@ -202,20 +202,21 @@
         except KeyError:
             raise ValueError(
                 "Checker.supports_language got iso code '{iso}' not found in the database."
             )
 
         # Exit if validity is not met
         if "validity" not in language or (
-            VALIDITYLEVELS.index(language["validity"]) < VALIDITYLEVELS.index(validity)
+            LanguageValidity.index(language["validity"])
+            < LanguageValidity.index(validity)
         ):
             return False
 
-        if supportlevel not in SUPPORTLEVELS.keys():
-            log.warning(
+        if supportlevel not in [s.value for s in SupportLevel]:
+            raise Exception(
                 "Provided support level '%s' not valid, "
                 "defaulting to 'base'" % supportlevel
             )
             supportlevel = "base"
 
         support = {}
         orthographies = language.get_check_orthographies(check_all_orthographies)
@@ -294,15 +295,15 @@
                 # Validation
                 if len(joining_errors) > 0 or len(mark_errors) > 0:
                     supported = False
                     logging.info(f"{language} missing base shaping for")
 
             # If an orthography has no "auxiliary" we consider it supported on
             # "auxiliary" level, too.
-            if supportlevel == "aux" and ort.auxiliary:
+            if supportlevel == SupportLevel.AUX.value and ort.auxiliary:
                 if marks:
                     req_marks_aux = ort.auxiliary_marks
                 else:
                     req_marks_aux = ort.required_auxiliary_marks
 
                 aux = set(ort.auxiliary_chars + req_marks_aux)
                 aux_missing = aux.difference(self.characters)
@@ -313,17 +314,15 @@
                         log_missing.warning(
                             "%s missing characters for 'base': %s"
                             % (language, ", ".join(aux_missing))
                         )
 
                     # Validation
                     supported = False
-                    logging.info(
-                        f"{language} missing {len(aux_missing)} 'aux'"
-                    )
+                    logging.info(f"{language} missing {len(aux_missing)} 'aux'")
 
                 if shaping:
                     joining_errors, mark_errors = self._check_shaping(
                         ort, "auxiliary", marks, decomposed
                     )
 
                     # Reporing output
```

### Comparing `hyperglot-0.6.2/lib/hyperglot/cli.py` & `hyperglot-0.6.3/lib/hyperglot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import functools
 from collections import OrderedDict
 from fontTools.ttLib import TTFont
 from hyperglot import (
     __version__,
     SORTING_DIRECTIONS,
     DB,
-    SUPPORTLEVELS,
-    VALIDITYLEVELS,
+    SupportLevel,
+    LanguageValidity,
     CHARACTER_ATTRIBUTES,
     MARK_BASE,
     SORTING,
 )
 from hyperglot.languages import Languages, find_language
 from hyperglot.language import Language
 from hyperglot.orthography import Orthography, is_mark
@@ -233,15 +233,15 @@
 
     @click.argument(
         "fonts", type=click.Path(exists=True), callback=validate_font, nargs=-1
     )
     @click.option(
         "-s",
         "--support",
-        type=click.Choice(SUPPORTLEVELS.keys(), case_sensitive=False),
+        type=click.Choice([s.value for s in SupportLevel], case_sensitive=False),
         default="base",
         show_default=True,
         help="Option to test only for the language's base charset, or to"
         " also test for presence of all auxilliary characters, if "
         "present in the database.",
     )
     @click.option(
@@ -260,16 +260,16 @@
         default=False,
         help="When this option is set all combining marks for a "
         "language are required, not just precomposed encoded "
         "characters.",
     )
     @click.option(
         "--validity",
-        type=click.Choice(VALIDITYLEVELS, case_sensitive=False),
-        default=VALIDITYLEVELS[1],
+        type=click.Choice([v.value for v in LanguageValidity], case_sensitive=False),
+        default=LanguageValidity.DRAFT.value,
         show_default=True,
         help="The level of validity for languages matched against the "
         "font. Weaker levels always include more strict levels. The "
         "default includes all languages for which the database has "
         "charset data.",
     )
     @click.option(
@@ -449,15 +449,15 @@
             include_historical=include_historical,
             include_constructed=include_constructed,
             report_missing=report_missing,
             report_marks=report_marks,
             report_joining=report_joining,
         )
 
-        level = SUPPORTLEVELS[support]
+        level = SupportLevel(support).value
 
         # Sort each script's results by the chosen sorting logic
         sorted_entries = {}
         for script, entries in supported.items():
             sorted_entries[script] = sorted(
                 entries.values(),
                 key=SORTING[sorting],
```

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/aat.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/aat.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/abi.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/abi.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/abn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/abn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ach.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ach.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/acm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/acm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/acw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/acw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ada.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ada.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ade.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ade.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/afb.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/afb.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/agq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/agq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/aii.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/aii.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ain.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ain.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ajg.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ajg.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ajp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ajp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/akk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/akk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ale.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ale.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/amh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/amh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/any.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/any.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/apd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/apd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/arb.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/arb.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/arr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/arr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ars.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ars.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/arz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/arz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/asm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/asm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ave.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ave.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/avn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/avn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/awa.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/awa.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/awn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/awn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/azb.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/azb.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/azj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/azj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/azo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/azo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bak.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bak.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bal.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bal.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bam.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bam.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ban.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ban.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bas.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bas.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bax.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bax.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bbc.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bbc.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bbo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bbo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bel.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bel.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ben.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ben.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bfa.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bfa.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bho.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bho.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bib.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bib.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bjn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bjn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bjt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bjt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bkm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bkm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/blo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/blo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/blt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/blt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bod.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bod.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bos.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bos.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/box.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/box.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/boz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/boz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bpy.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bpy.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/brx.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/brx.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bsc.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bsc.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bss.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bss.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/btd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/btd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/btm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/btm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bts.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bts.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/btx.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/btx.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bug.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bug.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bul.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bul.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bwj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bwj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bxm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bxm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bxr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bxr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bxu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bxu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/byn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/byn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/byv.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/byv.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/bze.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/bze.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cat.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cat.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ccp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ccp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/chr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/chr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/chu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/chu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cic.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cic.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ckb.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ckb.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cko.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cko.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ckt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ckt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cme.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cme.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cmn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cmn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cou.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cou.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/crh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/crh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/csw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/csw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ctg.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ctg.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/cym.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/cym.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dag.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dag.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ddn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ddn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/deu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/deu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dga.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dga.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dgi.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dgi.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dgo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dgo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/din.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/din.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dje.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dje.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dno.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dno.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dop.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dop.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dua.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dua.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dyo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dyo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dyu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dyu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/dzo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/dzo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/efi.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/efi.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/egy.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/egy.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/emk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/emk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/eng.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/eng.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/enh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/enh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ewe.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ewe.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ewo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ewo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fmp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fmp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fod.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fod.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fub.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fub.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fuc.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fuc.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fue.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fue.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fuf.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fuf.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fui.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fui.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/fuq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/fuq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gaa.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gaa.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gag.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gag.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gej.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gej.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gez.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gez.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gjn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gjn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gkp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gkp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gmy.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gmy.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gom.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gom.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gqa.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gqa.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/grc.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/grc.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/guj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/guj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gur.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gur.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/gux.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/gux.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/haj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/haj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/har.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/har.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/haw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/haw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/hin.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/hin.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/hnn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/hnn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/hye.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/hye.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/idu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/idu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ife.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ife.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/iii.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/iii.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ike.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ike.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ind.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ind.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/jav.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/jav.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/jbo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/jbo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/jdt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/jdt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/jgo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/jgo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/jpn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/jpn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kaa.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kaa.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kal.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kal.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kan.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kan.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kat.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kat.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kbp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kbp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kca.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kca.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kdh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kdh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/keu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/keu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/khm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/khm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/khq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/khq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kik.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kik.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kkj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kkj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kmr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kmr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/knf.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/knf.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kor.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kor.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kpy.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kpy.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kri.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kri.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ksf.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ksf.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ksh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ksh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kst.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kst.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kus.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kus.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/kwk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/kwk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lab.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lab.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lam.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lam.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lao.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lao.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lee.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lee.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lia.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lia.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/linb.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/linb.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lkt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lkt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lns.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lns.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lot.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lot.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lug.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lug.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/lzz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/lzz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mag.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mag.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mai.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mai.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mal.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mal.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mar.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mar.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mas.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mas.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mcn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mcn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mey.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mey.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mfq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mfq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mfv.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mfv.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mgo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mgo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mkd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mkd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mlg.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mlg.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mni.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mni.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mnk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mnk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mnw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mnw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/moe.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/moe.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mua.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mua.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mwp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mwp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/mya.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/mya.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/myk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/myk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/naq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/naq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nav.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nav.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nba.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nba.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nio.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nio.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nku.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nku.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nld.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nld.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nmg.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nmg.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nmz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nmz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nnh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nnh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nnw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nnw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/npi.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/npi.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nus.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nus.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nya.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nya.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/nza.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/nza.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/oji.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/oji.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/omn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/omn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/onw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/onw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ori.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ori.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/oss.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/oss.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ota.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ota.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ozm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ozm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/pan.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/pan.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/pbu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/pbu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/pes.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/pes.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/pil.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/pil.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/pnt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/pnt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/por.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/por.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/pug.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/pug.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/que.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/que.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/rah.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/rah.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/rkt.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/rkt.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/rmn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/rmn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ron.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ron.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/rue.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/rue.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/rus.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/rus.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ryu.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ryu.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/san.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/san.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sav.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sav.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sbd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sbd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ses.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ses.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sgw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sgw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/shk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/shk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/shn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/shn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/shz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/shz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sin.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sin.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sjd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sjd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sje.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sje.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sju.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sju.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/skr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/skr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sld.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sld.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sme.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sme.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/smj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/smj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/smn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/smn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sms.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sms.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/snd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/snd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/snf.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/snf.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/soy.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/soy.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/srp.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/srp.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/srr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/srr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sun.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sun.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sux.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sux.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sva.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sva.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/swb.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/swb.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/sxw.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/sxw.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tam.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tam.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tay.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tay.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tbz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tbz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tel.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tel.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tem.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tem.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/teo.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/teo.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tgl.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tgl.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tha.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tha.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tig.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tig.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tik.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tik.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tir.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tir.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tkr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tkr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tlh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tlh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tli.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tli.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tly.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tly.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tnr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tnr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tod.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tod.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ttq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ttq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tuk.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tuk.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tuz.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tuz.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/tvl.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/tvl.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/twq.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/twq.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/uig.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/uig.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/ukr.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/ukr.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/urd.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/urd.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/uzn.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/uzn.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/vai.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/vai.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/vie.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/vie.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/wae.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/wae.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/war.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/war.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/wci.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/wci.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/wol.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/wol.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/wwa.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/wwa.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/xan.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/xan.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/xav.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/xav.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/xmf.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/xmf.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/xrg.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/xrg.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/xsm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/xsm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/xwe.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/xwe.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/yav.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/yav.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/yor.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/yor.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/zap.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/zap.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/zdj.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/zdj.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/zgh.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/zgh.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/data/zsm.yaml` & `hyperglot-0.6.3/lib/hyperglot/data/zsm.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/extra_data/joining-types.yaml` & `hyperglot-0.6.3/lib/hyperglot/extra_data/joining-types.yaml`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/language.py` & `hyperglot-0.6.3/lib/hyperglot/language.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 """
 Helper classes to work with the lib/hyperglot/data in more pythonic way
 """
+
 import logging
 from typing import List
-from hyperglot import ORTHOGRAPHY_STATUSES, CHARACTER_ATTRIBUTES
+from hyperglot import CHARACTER_ATTRIBUTES, LanguageStatus, OrthographyStatus
 from hyperglot.languages import get_languages
 from hyperglot.orthography import Orthography
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.WARNING)
 
+
 class Language(dict):
     """
     A dict wrapper around a language data yaml entry with additional querying
     options for convenience.
     """
 
-    def __init__(self, iso, data=None):
+    defaults = {
+        # A default for unset speakers, to allow sorting
+        "speakers": 0,
+        # A default for unset status
+        "status": LanguageStatus.LIVING.value,
+    }
+
+    def __init__(self, iso, data: dict = None):
         """
         Init a single Language with the data from lib/hyperglot/data yaml.
 
         @param iso str: Iso 3 letter iso code that is the key in the yaml. Keep
             this a private attribute, not dict items, so it does not get
             printed out when converting this Language back to yaml for output
         @param data dict: The raw data as found in the yaml or extended by
@@ -29,25 +38,22 @@
         self.iso = iso
 
         if data is None:
             # Load languages from cache, return the data for this language
             languages = get_languages()
             data = languages[iso]
 
-        # A default for unset speakers, to allow sorting
-        self["speakers"] = 0
+        for key, default in self.defaults.items():
+            if key not in data:
+                data[key] = default
 
         self.update(data)
 
     def __repr__(self):
-        # return "Language object '%s'" % self.get_name()
         return f"Language ({self.iso}) {self.get_name()}"
-    
-    # @property
-    # def names(self):
 
     @property
     def presentation(self):
         tpl = """name: {name}
 autonym: {autonym}
 iso: {iso}
 orthographies:
@@ -107,38 +113,39 @@
 
         if not matches:
             raise KeyError(
                 "No orthography found for script '%s' and status "
                 "'%s' in language '%s'." % (script, status, self.iso)
             )
 
-        # Sort by status index in the ORTHOGRAPHY_STATUSES
-        matches = sorted(matches, key=lambda o: ORTHOGRAPHY_STATUSES.index(o["status"]))
+        # Sort by status index in the OrthographyStatus'es
+        matches = sorted(matches, key=lambda o: OrthographyStatus.values().index(o["status"]))
 
         # Note for multiple-orthography-primary languages (Serbian, Korean,
         # Japanese) this returns only one orthography!
         return matches[0]
-    
 
-    def get_check_orthographies(self, check_all_orthographies:bool=False) -> List:
+    def get_check_orthographies(self, check_all_orthographies: bool = False) -> List:
         """
         Get the orthographies relevant for performing support checks.
         """
         if "orthographies" not in self:
             return []
 
         # Determine which orthographies should be checked.
         if check_all_orthographies:
             orthographies = [
-                o for o in self["orthographies"]
+                o
+                for o in self["orthographies"]
                 if "status" not in o or o["status"] != "transliteration"
             ]
         else:
             orthographies = [
-                o for o in self["orthographies"]
+                o
+                for o in self["orthographies"]
                 if "status" in o and o["status"] == "primary"
             ]
 
         if not check_all_orthographies:
             # Note the .copy() here since we manipulate the attribute
             # and do not want to alter the original.
             as_group = [o.copy() for o in orthographies if "preferred_as_group" in o]
@@ -273,9 +280,7 @@
             orthography is not None
             and "status" in orthography
             and orthography["status"] == "secondary"
         ):
             return True
 
         return False
-
-
```

### Comparing `hyperglot-0.6.2/lib/hyperglot/languages.py` & `hyperglot-0.6.3/lib/hyperglot/languages.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Helper classes to work with the lib/hyperglot/data in more pythonic way
 """
 from functools import lru_cache
 import os
 import re
 import yaml
 import logging
-from hyperglot import DB, VALIDITYLEVELS
+from hyperglot import DB, LanguageValidity
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.WARNING)
 
 @lru_cache
 def get_languages(**kwargs):
     """
@@ -21,15 +21,15 @@
 
 @lru_cache
 def find_language(search):
     """
     Utility method to find a language by ISO code or language name
     """
 
-    hg = Languages(validity=VALIDITYLEVELS[0])
+    hg = Languages(validity=LanguageValidity.TODO.value)
 
     search = search.lower()
 
     # Search as 3-letter iso code, return if matched
     if search in hg.keys():
         return [getattr(hg, search)], f"Matched from iso code {search}:"
 
@@ -65,20 +65,25 @@
 
 class Languages(dict):
     """
     A dict wrapper around the language data yaml file with additional querying
     options for convenience
     """
 
-    def __init__(self, strict=False, inherit=True, validity=VALIDITYLEVELS[1]):
+    def __init__(
+        self, 
+        strict: bool = False, 
+        inherit: bool = True, 
+        validity: str = LanguageValidity.DRAFT.value,
+    ):
         """
         @param strict (Boolean): Use Rosetta macrolanguage definitions (False)
             or ISO definitions (True). Defaults to False.
         @param inherit (Boolean): Inherit orthographies. Defaults to True.
-        @param validity (Hyperglot.VALIDITYLEVEL): Minimum level of validity
+        @param validity (Hyperglot.LanguageValidity): Minimum level of validity
             which languages must have. One of "todo", "draft", "preliminary",
             "verified". Defaults to "draft" — all languages with basic
             information, but possibly unconfirmed.
         """
 
         # Load raw yaml data for all languages
         for file in os.listdir(DB):
@@ -270,23 +275,25 @@
                                   "orthographies to language '%s'"
                                   % (iso, lang))
                         # Make an explicit copy to keep the two languages
                         # separate
                         self[lang]["orthographies"] = m["orthographies"].copy()
 
     def filter_by_validity(self, validity):
-        if validity not in VALIDITYLEVELS:
-            raise ValueError("Validity level '%s' not valid, must be one of: "
-                             ", ".join(VALIDITYLEVELS) % validity)
+        if validity not in LanguageValidity.values():
+            raise ValueError(
+                "Validity level '%s' not valid, must be one of: %s" %
+                (validity, ", ".join(LanguageValidity.values()))
+            )
 
-        allowed = VALIDITYLEVELS.index(validity)
+        allowed = LanguageValidity.index(validity)
         pruned = {}
         for iso, lang in self.items():
             try:
-                if VALIDITYLEVELS.index(lang["validity"]) >= allowed:
+                if LanguageValidity.index(lang["validity"]) >= allowed:
                     pruned[iso] = lang
             except KeyError as e:
                 # Provide more context, but escalate
                 raise KeyError("Language '%s' missing attribute %s" %
                                (iso, e))
 
         self.clear()
```

### Comparing `hyperglot-0.6.2/lib/hyperglot/orthography.py` & `hyperglot-0.6.3/lib/hyperglot/orthography.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,18 @@
     """
     A orthography dict from yaml data. Inheritance has already taken place.
 
     The dict retains its original entries, but we extend it with getters that
     use the _parsed_ character lists!
     """
 
-    def __init__(self, data):
+    defaults = {"preferred_as_group": False}
+
+    def __init__(self, data: dict):
+        self.update(self.defaults)
         self.update(data)
 
     @property
     def presentation(self):
         tpl = """autonym: {autonym}
 base characters: {base_chars}
 base marks: {base_marks}
```

### Comparing `hyperglot-0.6.2/lib/hyperglot/parse.py` & `hyperglot-0.6.3/lib/hyperglot/parse.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/shaper.py` & `hyperglot-0.6.3/lib/hyperglot/shaper.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/lib/hyperglot/validate.py` & `hyperglot-0.6.3/lib/hyperglot/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 import logging
 import pprint
 import colorlog
 import unicodedata2
 from hyperglot.languages import Languages
 from hyperglot.orthography import Orthography
 from hyperglot.parse import parse_chars
-from hyperglot import (__version__, STATUSES, VALIDITYLEVELS, ORTHOGRAPHY_STATUSES)
+from hyperglot import (
+    __version__, 
+    LanguageStatus, 
+    LanguageValidity, 
+    OrthographyStatus,
+)
 
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(message)s'))
 log = colorlog.getLogger()
 log.setLevel(logging.WARNING)
 log.addHandler(handler)
 
@@ -47,15 +52,15 @@
     except Exception as e:
         log.error("Failed to get nice char list from '%s' (%s)" %
                   (str(chars), str(e)))
 
 
 def check_yaml():
     log.debug("YAML file structure ok and can be read")
-    return Languages(validity=VALIDITYLEVELS[0])
+    return Languages(validity=LanguageValidity.TODO.value)
 
 
 def check_types(Langs):
     for iso, lang in Langs.items():
         if "includes" in lang:
             if not check_is_yaml_list(lang["includes"]):
                 log.error("'%s' has invalid list 'includes'" % iso)
@@ -64,14 +69,23 @@
             if not check_is_yaml_list(lang["source"]):
                 log.error("'%s' has invalid list 'source'" % iso)
 
         if "orthographies" in lang:
             if not check_is_yaml_list(lang["orthographies"]):
                 log.error("'%s' has invalid list 'orthographies'" % iso)
 
+            preferred_as_group = [o for o in lang["orthographies"] 
+                                  if "preferred_as_group" in o and o["preferred_as_group"] is True]
+            if len(preferred_as_group) == 1:
+                log.error(
+                    "'%s': Cannot set sole orthography as 'preferred_as_group', only two or " 
+                    "more orthographies can be treated as group."
+                    % iso
+                )
+
             for o in lang["orthographies"]:
                 if "script" not in o:
                     log.error("Orthography in '%s' is missing 'script'" % iso)
 
                 if "base" in o:
                     if not check_is_valid_glyph_string(o["base"], iso):
                         log.error("'%s' has invalid 'base' glyph list: '%s'"
@@ -115,41 +129,52 @@
                     log.error("'%s' has a 'design_requirements' which is not "
                               "a list: %s" % (iso, o["design_requirements"]))
 
                 if "status" not in o:
                     log.error("'%s' has an orthography (script '%s') that is "
                               "missing 'status'" % (iso, o["script"]))
                 else:
-                    if o["status"] not in ORTHOGRAPHY_STATUSES:
+                    if o["status"] not in OrthographyStatus.values():
                         log.error("'%s' has an orthography status '%s' which "
                                   "is invalid, should be one of %s" %
                                   (iso, o["status"],
-                                   ", ".join(ORTHOGRAPHY_STATUSES)))
+                                   ", ".join(OrthographyStatus.values())))
+                
+                if "preferred_as_group" in o:
+                    if type(o["preferred_as_group"]) != bool:
+                        log.error(
+                            "'%s' has an orthography with 'preferred_as_group'"
+                            " which is not boolean: '%s'." %
+                            (iso, o["preferred_as_group"])
+                        )
 
             primary_orthography = [o for o in lang["orthographies"]
                                    if "status" in o and
                                    o["status"] == "primary"]
             if len(primary_orthography) == 0:
                 log.error("'%s' has no primary orthography" % iso)
 
         if "name" not in lang and "preferred_name" not in lang:
             log.error("'%s' has neither 'name' nor 'preferred_name'" % iso)
 
         if "name" in lang and "preferred_name" in lang \
                 and lang["name"] == lang["preferred_name"]:
             log.error("'%s' has 'name' and 'preferred_name', but they are "
                       "identical" % iso)
-
-        if "status" in lang and lang["status"] not in STATUSES:
-            log.error("'%s' has an invalid 'status'" % iso)
+                
+        if "status" in lang:
+            if lang["status"] not in [s.value for s in LanguageStatus]:
+                log.error(
+                    "'%s' has invalid 'status' '%s'" % (iso, lang["status"])
+                )
 
         if "validity" not in lang:
             log.warning("'%s' is missing 'validity'" % iso)
 
-        if "validity" in lang and lang["validity"] not in VALIDITYLEVELS:
+        if "validity" in lang and lang["validity"] not in LanguageValidity.values():
             log.error("'%s' has invalid 'validity'" % iso)
 
         if "speakers" in lang:
             if (re.search(r"[^\d]", str(lang["speakers"]))):
                 log.error("'%s' has invalid 'speakers' '%s' - only numbers "
                           "are allowed" %
                           (iso, lang["speakers"]))
```

### Comparing `hyperglot-0.6.2/lib/hyperglot.egg-info/PKG-INFO` & `hyperglot-0.6.3/lib/hyperglot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperglot
-Version: 0.6.2
+Version: 0.6.3
 Summary: Detect language support for font binaries
 Home-page: https://github.com/rosettatype/hyperglot
 Author: Johannes Neumeier - Rosetta
 Author-email: johannes@rosettatype.com
 License: GNU GPLv3
 Project-URL: Hyperglot web interface, https://hyperglot.rosettatype.com
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hyperglot-0.6.2/lib/hyperglot.egg-info/SOURCES.txt` & `hyperglot-0.6.3/lib/hyperglot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/setup.py` & `hyperglot-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/tests/test_checker.py` & `hyperglot-0.6.3/tests/test_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Basic Language support checks
 """
 import os
 import logging
 import pytest
 import unicodedata as uni
+from hyperglot import SupportLevel
 from hyperglot.parse import character_list_from_string, parse_font_chars, parse_marks
 from hyperglot.checker import CharsetChecker, FontChecker
 
 # Just a most simple placeholder charset
 ascii = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
 
 # Some test font paths
@@ -65,25 +66,25 @@
     assert "fin" in matches["Latin"].keys()
 
     # for this shorter direct check
     assert CharsetChecker(fin_base).supports_language("fin")
 
     # Just base chars input won't support aux
     assert (
-        CharsetChecker(fin_base).supports_language("fin", supportlevel="aux") is False
+        CharsetChecker(fin_base).supports_language("fin", supportlevel=SupportLevel.AUX.value) is False
     )
 
     # But aux chars input will
-    assert CharsetChecker(fin_aux).supports_language("fin", supportlevel="aux")
+    assert CharsetChecker(fin_aux).supports_language("fin", supportlevel=SupportLevel.AUX.value)
 
     # A Font without 'a' won't support this language
     assert CharsetChecker(fin_missing_a).supports_language("fin") is False
 
     # Just basic other language check
-    assert CharsetChecker(rus_base).supports_language("rus", supportlevel="base")
+    assert CharsetChecker(rus_base).supports_language("rus", supportlevel=SupportLevel.BASE.value)
 
 
 def test_language_supported_dict():
     checker = FontChecker(eczar)
 
     # Detected scripts
     assert "Latin" in checker.supports_language("deu", return_script_object=True).keys()
```

### Comparing `hyperglot-0.6.2/tests/test_cli.py` & `hyperglot-0.6.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/tests/test_language.py` & `hyperglot-0.6.3/tests/test_language.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 """
 Basic Language support checks
 """
 import pytest
+from hyperglot import LanguageStatus
 from hyperglot.languages import Languages
 from hyperglot.language import Language
 
 
 @pytest.fixture
+def language_with_omitted_defaults():
+    """
+    Return a Language with omitted default values, to test defaults being set
+    correctly. Currently there is only 'status' that is optional on Language.
+    """
+
+    return Language("tmp", {})
+
+@pytest.fixture
 def langs():
     return Languages()
 
 
 def test_language_inherit():
     langs = Languages(inherit=True)
 
@@ -79,7 +89,11 @@
     bos_cyrillic = bos.get_orthography("Cyrillic")
     assert ("Д" in bos_cyrillic["base"]) is True
 
     # However if for a specific script and status no orthography exists raise
     # exceptions
     with pytest.raises(KeyError):
         bos.get_orthography("Cyrillic", "primary")
+
+
+def test_language_defaults(language_with_omitted_defaults):
+    assert language_with_omitted_defaults["status"] == LanguageStatus.LIVING.value
```

### Comparing `hyperglot-0.6.2/tests/test_languages.py` & `hyperglot-0.6.3/tests/test_languages.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/tests/test_orthography.py` & `hyperglot-0.6.3/tests/test_orthography.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 
 
 @pytest.fixture
 def langs():
     return Languages()
 
 
+@pytest.fixture
+def orthography_with_omitted_defaults():
+    """
+    Return a Orthography with omitted default values, to test defaults being
+    set correctly. Currently there is only 'preferred_as_group' that is
+    optional on Orthography.
+    """
+
+    return Orthography({})
+
+
 def test_orthography_character_list(langs):
     deu = getattr(langs, "deu")
     ort_default = Orthography(deu["orthographies"][0])
 
     deu_base_default = ort_default._character_list("base")
 
     assert "Ä" in deu_base_default
@@ -143,7 +154,11 @@
 
 def test_yaml_escape_sequences(langs):
     # Test some particular cases where the yaml encoding has lead to confusion
 
     # Confirm the single auxiliary mark ' in Standard Malay is returned as such
     zsm = getattr(langs, "zsm")
     assert zsm.get_orthography()["auxiliary"] == "'"
+
+
+def test_orthography_defaults(orthography_with_omitted_defaults):
+    assert orthography_with_omitted_defaults["preferred_as_group"] is False
```

### Comparing `hyperglot-0.6.2/tests/test_parse.py` & `hyperglot-0.6.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.6.2/tests/test_shaper.py` & `hyperglot-0.6.3/tests/test_shaper.py`

 * *Files identical despite different names*

