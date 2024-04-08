# Comparing `tmp/language_data-1.1.tar.gz` & `tmp/language_data-1.2.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language_data-1.1.tar", max compression
+gzip compressed data, was "language_data-1.2.0.dev3.tar", last modified: Fri Feb 23 14:34:20 2024, max compression
```

## Comparing `language_data-1.1.tar` & `language_data-1.2.0.dev3.tar`

### file list

```diff
@@ -1,693 +1,946 @@
--rw-r--r--   0        0        0      426 2021-11-10 18:13:44.311762 language_data-1.1/CHANGELOG.md
--rw-r--r--   0        0        0     2809 2021-11-10 18:21:48.860746 language_data-1.1/README.md
--rw-r--r--   0        0        0        0 2021-09-10 18:22:57.620100 language_data-1.1/language_data/__init__.py
--rw-r--r--   0        0        0    19608 2021-11-01 20:44:44.256442 language_data-1.1/language_data/build_data.py
--rw-r--r--   0        0        0     1243 2021-09-10 18:22:57.620100 language_data-1.1/language_data/data/extra_language_names.csv
--rw-r--r--   0        0        0   715867 2021-11-01 20:44:44.256442 language_data-1.1/language_data/data/language-subtag-registry.txt
--rw-r--r--   0        0        0    41382 2021-09-10 18:22:57.624101 language_data-1.1/language_data/data/languageInfo.xml
--rw-r--r--   0        0        0       69 2021-09-10 18:22:57.624101 language_data-1.1/language_data/data/override_language_names.csv
--rw-r--r--   0        0        0   381483 2021-09-10 18:22:57.624101 language_data-1.1/language_data/data/supplementalData.xml
--rw-r--r--   0        0        0     9272 2021-11-01 20:48:13.953480 language_data-1.1/language_data/data/trie/af/name_to_language.marisa
--rw-r--r--   0        0        0     4824 2021-11-01 20:48:14.325482 language_data-1.1/language_data/data/trie/af/name_to_script.marisa
--rw-r--r--   0        0        0     8128 2021-11-01 20:48:14.537483 language_data-1.1/language_data/data/trie/af/name_to_territory.marisa
--rw-r--r--   0        0        0     5224 2021-11-01 20:48:13.957480 language_data-1.1/language_data/data/trie/agq/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.945054 language_data-1.1/language_data/data/trie/agq/name_to_script.marisa
--rw-r--r--   0        0        0     7600 2021-11-01 20:48:14.541483 language_data-1.1/language_data/data/trie/agq/name_to_territory.marisa
--rw-r--r--   0        0        0     5120 2021-11-01 20:48:13.957480 language_data-1.1/language_data/data/trie/ak/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.945054 language_data-1.1/language_data/data/trie/ak/name_to_script.marisa
--rw-r--r--   0        0        0     6984 2021-11-01 20:48:14.541483 language_data-1.1/language_data/data/trie/ak/name_to_territory.marisa
--rw-r--r--   0        0        0    11640 2021-11-01 20:48:13.957480 language_data-1.1/language_data/data/trie/am/name_to_language.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/am/name_to_script.marisa
--rw-r--r--   0        0        0     9544 2021-11-01 20:48:14.541483 language_data-1.1/language_data/data/trie/am/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/ang/name_to_language.marisa
--rw-r--r--   0        0        0    11800 2021-11-01 20:48:13.961480 language_data-1.1/language_data/data/trie/ar/name_to_language.marisa
--rw-r--r--   0        0        0     6752 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/ar/name_to_script.marisa
--rw-r--r--   0        0        0     9368 2021-11-01 20:48:14.541483 language_data-1.1/language_data/data/trie/ar/name_to_territory.marisa
--rw-r--r--   0        0        0    12440 2021-11-01 20:48:13.961480 language_data-1.1/language_data/data/trie/as/name_to_language.marisa
--rw-r--r--   0        0        0     5248 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/as/name_to_script.marisa
--rw-r--r--   0        0        0    11496 2021-11-01 20:48:14.545483 language_data-1.1/language_data/data/trie/as/name_to_territory.marisa
--rw-r--r--   0        0        0     5064 2021-11-01 20:48:13.961480 language_data-1.1/language_data/data/trie/asa/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.945054 language_data-1.1/language_data/data/trie/asa/name_to_script.marisa
--rw-r--r--   0        0        0     6840 2021-11-01 20:48:14.545483 language_data-1.1/language_data/data/trie/asa/name_to_territory.marisa
--rw-r--r--   0        0        0    11512 2021-11-01 20:48:13.965480 language_data-1.1/language_data/data/trie/ast/name_to_language.marisa
--rw-r--r--   0        0        0     6808 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/ast/name_to_script.marisa
--rw-r--r--   0        0        0     8096 2021-11-01 20:48:14.545483 language_data-1.1/language_data/data/trie/ast/name_to_territory.marisa
--rw-r--r--   0        0        0    14296 2021-11-01 20:48:13.965480 language_data-1.1/language_data/data/trie/az/name_to_language.marisa
--rw-r--r--   0        0        0     5992 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/az/name_to_script.marisa
--rw-r--r--   0        0        0    12440 2021-11-01 20:48:14.549483 language_data-1.1/language_data/data/trie/az/name_to_territory.marisa
--rw-r--r--   0        0        0     5168 2021-11-01 20:48:13.965480 language_data-1.1/language_data/data/trie/bas/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.945054 language_data-1.1/language_data/data/trie/bas/name_to_script.marisa
--rw-r--r--   0        0        0     7240 2021-11-01 20:48:14.549483 language_data-1.1/language_data/data/trie/bas/name_to_territory.marisa
--rw-r--r--   0        0        0    11272 2021-11-01 20:48:13.969480 language_data-1.1/language_data/data/trie/be/name_to_language.marisa
--rw-r--r--   0        0        0     5224 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/be/name_to_script.marisa
--rw-r--r--   0        0        0     9944 2021-11-01 20:48:14.549483 language_data-1.1/language_data/data/trie/be/name_to_territory.marisa
--rw-r--r--   0        0        0     4904 2021-11-01 20:48:13.969480 language_data-1.1/language_data/data/trie/bem/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.949054 language_data-1.1/language_data/data/trie/bem/name_to_script.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.549483 language_data-1.1/language_data/data/trie/bem/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:13.969480 language_data-1.1/language_data/data/trie/bez/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.949054 language_data-1.1/language_data/data/trie/bez/name_to_script.marisa
--rw-r--r--   0        0        0     6872 2021-11-01 20:48:14.553483 language_data-1.1/language_data/data/trie/bez/name_to_territory.marisa
--rw-r--r--   0        0        0    12000 2021-11-01 20:48:13.973480 language_data-1.1/language_data/data/trie/bg/name_to_language.marisa
--rw-r--r--   0        0        0     6920 2021-11-01 20:48:14.329482 language_data-1.1/language_data/data/trie/bg/name_to_script.marisa
--rw-r--r--   0        0        0     9696 2021-11-01 20:48:14.553483 language_data-1.1/language_data/data/trie/bg/name_to_territory.marisa
--rw-r--r--   0        0        0     4112 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/bho/name_to_language.marisa
--rw-r--r--   0        0        0     5128 2021-11-01 20:48:13.973480 language_data-1.1/language_data/data/trie/bm/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.949054 language_data-1.1/language_data/data/trie/bm/name_to_script.marisa
--rw-r--r--   0        0        0     6880 2021-11-01 20:48:14.553483 language_data-1.1/language_data/data/trie/bm/name_to_territory.marisa
--rw-r--r--   0        0        0    14584 2021-11-01 20:48:13.973480 language_data-1.1/language_data/data/trie/bn/name_to_language.marisa
--rw-r--r--   0        0        0     7840 2021-11-01 20:48:14.333482 language_data-1.1/language_data/data/trie/bn/name_to_script.marisa
--rw-r--r--   0        0        0    11864 2021-11-01 20:48:14.553483 language_data-1.1/language_data/data/trie/bn/name_to_territory.marisa
--rw-r--r--   0        0        0     4600 2021-11-01 20:48:13.973480 language_data-1.1/language_data/data/trie/bo/name_to_language.marisa
--rw-r--r--   0        0        0     4312 2021-11-01 20:48:14.333482 language_data-1.1/language_data/data/trie/bo/name_to_script.marisa
--rw-r--r--   0        0        0     4504 2021-11-01 20:48:14.553483 language_data-1.1/language_data/data/trie/bo/name_to_territory.marisa
--rw-r--r--   0        0        0    10384 2021-11-01 20:48:13.977480 language_data-1.1/language_data/data/trie/br/name_to_language.marisa
--rw-r--r--   0        0        0     5496 2021-11-01 20:48:14.333482 language_data-1.1/language_data/data/trie/br/name_to_script.marisa
--rw-r--r--   0        0        0     8024 2021-11-01 20:48:14.557483 language_data-1.1/language_data/data/trie/br/name_to_territory.marisa
--rw-r--r--   0        0        0    12672 2021-11-01 20:48:13.977480 language_data-1.1/language_data/data/trie/brx/name_to_language.marisa
--rw-r--r--   0        0        0     7328 2021-11-01 20:48:14.333482 language_data-1.1/language_data/data/trie/brx/name_to_script.marisa
--rw-r--r--   0        0        0    10792 2021-11-01 20:48:14.557483 language_data-1.1/language_data/data/trie/brx/name_to_territory.marisa
--rw-r--r--   0        0        0    15632 2021-11-01 20:48:13.981480 language_data-1.1/language_data/data/trie/bs/name_to_language.marisa
--rw-r--r--   0        0        0    10328 2021-11-01 20:48:14.333482 language_data-1.1/language_data/data/trie/bs/name_to_script.marisa
--rw-r--r--   0        0        0    12392 2021-11-01 20:48:14.561483 language_data-1.1/language_data/data/trie/bs/name_to_territory.marisa
--rw-r--r--   0        0        0    10952 2021-11-01 20:48:13.981480 language_data-1.1/language_data/data/trie/ca/name_to_language.marisa
--rw-r--r--   0        0        0     6768 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/ca/name_to_script.marisa
--rw-r--r--   0        0        0     8272 2021-11-01 20:48:14.561483 language_data-1.1/language_data/data/trie/ca/name_to_territory.marisa
--rw-r--r--   0        0        0    15600 2021-11-01 20:48:13.985480 language_data-1.1/language_data/data/trie/ccp/name_to_language.marisa
--rw-r--r--   0        0        0     8480 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/ccp/name_to_script.marisa
--rw-r--r--   0        0        0    12520 2021-11-01 20:48:14.561483 language_data-1.1/language_data/data/trie/ccp/name_to_territory.marisa
--rw-r--r--   0        0        0    10792 2021-11-01 20:48:13.985480 language_data-1.1/language_data/data/trie/ce/name_to_language.marisa
--rw-r--r--   0        0        0     5120 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/ce/name_to_script.marisa
--rw-r--r--   0        0        0     9888 2021-11-01 20:48:14.565483 language_data-1.1/language_data/data/trie/ce/name_to_territory.marisa
--rw-r--r--   0        0        0     5000 2021-11-01 20:48:13.985480 language_data-1.1/language_data/data/trie/ceb/name_to_language.marisa
--rw-r--r--   0        0        0     4264 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/ceb/name_to_script.marisa
--rw-r--r--   0        0        0     8080 2021-11-01 20:48:14.565483 language_data-1.1/language_data/data/trie/ceb/name_to_territory.marisa
--rw-r--r--   0        0        0     5064 2021-11-01 20:48:13.989480 language_data-1.1/language_data/data/trie/cgg/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.953055 language_data-1.1/language_data/data/trie/cgg/name_to_script.marisa
--rw-r--r--   0        0        0     6912 2021-11-01 20:48:14.565483 language_data-1.1/language_data/data/trie/cgg/name_to_territory.marisa
--rw-r--r--   0        0        0     9784 2021-11-01 20:48:13.989480 language_data-1.1/language_data/data/trie/chr/name_to_language.marisa
--rw-r--r--   0        0        0     5056 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/chr/name_to_script.marisa
--rw-r--r--   0        0        0     9424 2021-11-01 20:48:14.569483 language_data-1.1/language_data/data/trie/chr/name_to_territory.marisa
--rw-r--r--   0        0        0    10336 2021-11-01 20:48:13.989480 language_data-1.1/language_data/data/trie/ckb/name_to_language.marisa
--rw-r--r--   0        0        0     5032 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/ckb/name_to_script.marisa
--rw-r--r--   0        0        0     9432 2021-11-01 20:48:14.569483 language_data-1.1/language_data/data/trie/ckb/name_to_territory.marisa
--rw-r--r--   0        0        0    11728 2021-11-01 20:48:13.993481 language_data-1.1/language_data/data/trie/cs/name_to_language.marisa
--rw-r--r--   0        0        0     6976 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/cs/name_to_script.marisa
--rw-r--r--   0        0        0     8352 2021-11-01 20:48:14.569483 language_data-1.1/language_data/data/trie/cs/name_to_territory.marisa
--rw-r--r--   0        0        0     4168 2021-09-10 18:22:57.632100 language_data-1.1/language_data/data/trie/cu/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-09-10 18:22:57.632100 language_data-1.1/language_data/data/trie/cu/name_to_script.marisa
--rw-r--r--   0        0        0     4168 2021-09-10 18:22:57.632100 language_data-1.1/language_data/data/trie/cu/name_to_territory.marisa
--rw-r--r--   0        0        0    10416 2021-11-01 20:48:13.993481 language_data-1.1/language_data/data/trie/cy/name_to_language.marisa
--rw-r--r--   0        0        0     4808 2021-11-01 20:48:14.337482 language_data-1.1/language_data/data/trie/cy/name_to_script.marisa
--rw-r--r--   0        0        0     8248 2021-11-01 20:48:14.569483 language_data-1.1/language_data/data/trie/cy/name_to_territory.marisa
--rw-r--r--   0        0        0    10264 2021-11-01 20:48:13.997480 language_data-1.1/language_data/data/trie/da/name_to_language.marisa
--rw-r--r--   0        0        0     6488 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/da/name_to_script.marisa
--rw-r--r--   0        0        0     8264 2021-11-01 20:48:14.573483 language_data-1.1/language_data/data/trie/da/name_to_territory.marisa
--rw-r--r--   0        0        0     5032 2021-11-01 20:48:13.997480 language_data-1.1/language_data/data/trie/dav/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.957054 language_data-1.1/language_data/data/trie/dav/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.573483 language_data-1.1/language_data/data/trie/dav/name_to_territory.marisa
--rw-r--r--   0        0        0    11432 2021-11-01 20:48:13.997480 language_data-1.1/language_data/data/trie/de/name_to_language.marisa
--rw-r--r--   0        0        0     6760 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/de/name_to_script.marisa
--rw-r--r--   0        0        0     8256 2021-11-01 20:48:14.573483 language_data-1.1/language_data/data/trie/de/name_to_territory.marisa
--rw-r--r--   0        0        0     5232 2021-11-01 20:48:13.997480 language_data-1.1/language_data/data/trie/dje/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.957054 language_data-1.1/language_data/data/trie/dje/name_to_script.marisa
--rw-r--r--   0        0        0     7040 2021-11-01 20:48:14.573483 language_data-1.1/language_data/data/trie/dje/name_to_territory.marisa
--rw-r--r--   0        0        0     5000 2021-11-01 20:48:14.001480 language_data-1.1/language_data/data/trie/doi/name_to_language.marisa
--rw-r--r--   0        0        0     4312 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/doi/name_to_script.marisa
--rw-r--r--   0        0        0     4328 2021-11-01 20:48:14.577483 language_data-1.1/language_data/data/trie/doi/name_to_territory.marisa
--rw-r--r--   0        0        0     7952 2021-11-01 20:48:14.001480 language_data-1.1/language_data/data/trie/dsb/name_to_language.marisa
--rw-r--r--   0        0        0     4840 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/dsb/name_to_script.marisa
--rw-r--r--   0        0        0     8240 2021-11-01 20:48:14.577483 language_data-1.1/language_data/data/trie/dsb/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.001480 language_data-1.1/language_data/data/trie/dua/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.957054 language_data-1.1/language_data/data/trie/dua/name_to_script.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.577483 language_data-1.1/language_data/data/trie/dua/name_to_territory.marisa
--rw-r--r--   0        0        0     4944 2021-11-01 20:48:14.001480 language_data-1.1/language_data/data/trie/dyo/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.957054 language_data-1.1/language_data/data/trie/dyo/name_to_script.marisa
--rw-r--r--   0        0        0     5304 2021-11-01 20:48:14.577483 language_data-1.1/language_data/data/trie/dyo/name_to_territory.marisa
--rw-r--r--   0        0        0     8176 2021-11-01 20:48:14.001480 language_data-1.1/language_data/data/trie/dz/name_to_language.marisa
--rw-r--r--   0        0        0     5944 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/dz/name_to_script.marisa
--rw-r--r--   0        0        0    12872 2021-11-01 20:48:14.577483 language_data-1.1/language_data/data/trie/dz/name_to_territory.marisa
--rw-r--r--   0        0        0     5056 2021-11-01 20:48:14.001480 language_data-1.1/language_data/data/trie/ebu/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.961054 language_data-1.1/language_data/data/trie/ebu/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.581483 language_data-1.1/language_data/data/trie/ebu/name_to_territory.marisa
--rw-r--r--   0        0        0     6464 2021-11-01 20:48:14.005481 language_data-1.1/language_data/data/trie/ee/name_to_language.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/ee/name_to_script.marisa
--rw-r--r--   0        0        0     8240 2021-11-01 20:48:14.581483 language_data-1.1/language_data/data/trie/ee/name_to_territory.marisa
--rw-r--r--   0        0        0    12848 2021-11-01 20:48:14.005481 language_data-1.1/language_data/data/trie/el/name_to_language.marisa
--rw-r--r--   0        0        0     7344 2021-11-01 20:48:14.341482 language_data-1.1/language_data/data/trie/el/name_to_script.marisa
--rw-r--r--   0        0        0     9888 2021-11-01 20:48:14.581483 language_data-1.1/language_data/data/trie/el/name_to_territory.marisa
--rw-r--r--   0        0        0   103352 2021-11-01 20:48:14.081481 language_data-1.1/language_data/data/trie/en/name_to_language.marisa
--rw-r--r--   0        0        0     8576 2021-11-01 20:48:14.345482 language_data-1.1/language_data/data/trie/en/name_to_script.marisa
--rw-r--r--   0        0        0     8832 2021-11-01 20:48:14.581483 language_data-1.1/language_data/data/trie/en/name_to_territory.marisa
--rw-r--r--   0        0        0     5944 2021-11-01 20:48:14.085481 language_data-1.1/language_data/data/trie/eo/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.961054 language_data-1.1/language_data/data/trie/eo/name_to_script.marisa
--rw-r--r--   0        0        0     6800 2021-11-01 20:48:14.585483 language_data-1.1/language_data/data/trie/eo/name_to_territory.marisa
--rw-r--r--   0        0        0    10440 2021-11-01 20:48:14.085481 language_data-1.1/language_data/data/trie/es/name_to_language.marisa
--rw-r--r--   0        0        0     6072 2021-11-01 20:48:14.345482 language_data-1.1/language_data/data/trie/es/name_to_script.marisa
--rw-r--r--   0        0        0     8256 2021-11-01 20:48:14.585483 language_data-1.1/language_data/data/trie/es/name_to_territory.marisa
--rw-r--r--   0        0        0    10968 2021-11-01 20:48:14.085481 language_data-1.1/language_data/data/trie/et/name_to_language.marisa
--rw-r--r--   0        0        0     6952 2021-11-01 20:48:14.345482 language_data-1.1/language_data/data/trie/et/name_to_script.marisa
--rw-r--r--   0        0        0     8136 2021-11-01 20:48:14.585483 language_data-1.1/language_data/data/trie/et/name_to_territory.marisa
--rw-r--r--   0        0        0     9160 2021-11-01 20:48:14.089481 language_data-1.1/language_data/data/trie/eu/name_to_language.marisa
--rw-r--r--   0        0        0     7136 2021-11-01 20:48:14.345482 language_data-1.1/language_data/data/trie/eu/name_to_script.marisa
--rw-r--r--   0        0        0     8112 2021-11-01 20:48:14.589483 language_data-1.1/language_data/data/trie/eu/name_to_territory.marisa
--rw-r--r--   0        0        0     5216 2021-11-01 20:48:14.089481 language_data-1.1/language_data/data/trie/ewo/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.965054 language_data-1.1/language_data/data/trie/ewo/name_to_script.marisa
--rw-r--r--   0        0        0     7368 2021-11-01 20:48:14.589483 language_data-1.1/language_data/data/trie/ewo/name_to_territory.marisa
--rw-r--r--   0        0        0    11520 2021-11-01 20:48:14.089481 language_data-1.1/language_data/data/trie/fa/name_to_language.marisa
--rw-r--r--   0        0        0     6568 2021-11-01 20:48:14.345482 language_data-1.1/language_data/data/trie/fa/name_to_script.marisa
--rw-r--r--   0        0        0     9000 2021-11-01 20:48:14.589483 language_data-1.1/language_data/data/trie/fa/name_to_territory.marisa
--rw-r--r--   0        0        0     9480 2021-11-01 20:48:14.093481 language_data-1.1/language_data/data/trie/ff/name_to_language.marisa
--rw-r--r--   0        0        0     4488 2021-11-01 20:48:14.345482 language_data-1.1/language_data/data/trie/ff/name_to_script.marisa
--rw-r--r--   0        0        0    14176 2021-11-01 20:48:14.593483 language_data-1.1/language_data/data/trie/ff/name_to_territory.marisa
--rw-r--r--   0        0        0    11272 2021-11-01 20:48:14.093481 language_data-1.1/language_data/data/trie/fi/name_to_language.marisa
--rw-r--r--   0        0        0     8072 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/fi/name_to_script.marisa
--rw-r--r--   0        0        0     8224 2021-11-01 20:48:14.593483 language_data-1.1/language_data/data/trie/fi/name_to_territory.marisa
--rw-r--r--   0        0        0     9224 2021-11-01 20:48:14.097481 language_data-1.1/language_data/data/trie/fil/name_to_language.marisa
--rw-r--r--   0        0        0     4816 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/fil/name_to_script.marisa
--rw-r--r--   0        0        0     8104 2021-11-01 20:48:14.593483 language_data-1.1/language_data/data/trie/fil/name_to_territory.marisa
--rw-r--r--   0        0        0     9232 2021-11-01 20:48:14.097481 language_data-1.1/language_data/data/trie/fo/name_to_language.marisa
--rw-r--r--   0        0        0     4776 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/fo/name_to_script.marisa
--rw-r--r--   0        0        0     7904 2021-11-01 20:48:14.593483 language_data-1.1/language_data/data/trie/fo/name_to_territory.marisa
--rw-r--r--   0        0        0    11600 2021-11-01 20:48:14.097481 language_data-1.1/language_data/data/trie/fr/name_to_language.marisa
--rw-r--r--   0        0        0     6392 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/fr/name_to_script.marisa
--rw-r--r--   0        0        0     8320 2021-11-01 20:48:14.597483 language_data-1.1/language_data/data/trie/fr/name_to_territory.marisa
--rw-r--r--   0        0        0     6536 2021-11-01 20:48:14.101481 language_data-1.1/language_data/data/trie/fur/name_to_language.marisa
--rw-r--r--   0        0        0     5152 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/fur/name_to_script.marisa
--rw-r--r--   0        0        0     7928 2021-11-01 20:48:14.597483 language_data-1.1/language_data/data/trie/fur/name_to_territory.marisa
--rw-r--r--   0        0        0    10152 2021-11-01 20:48:14.101481 language_data-1.1/language_data/data/trie/fy/name_to_language.marisa
--rw-r--r--   0        0        0     6592 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/fy/name_to_script.marisa
--rw-r--r--   0        0        0     8040 2021-11-01 20:48:14.597483 language_data-1.1/language_data/data/trie/fy/name_to_territory.marisa
--rw-r--r--   0        0        0     9160 2021-11-01 20:48:14.101481 language_data-1.1/language_data/data/trie/ga/name_to_language.marisa
--rw-r--r--   0        0        0     6032 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/ga/name_to_script.marisa
--rw-r--r--   0        0        0     8632 2021-11-01 20:48:14.601483 language_data-1.1/language_data/data/trie/ga/name_to_territory.marisa
--rw-r--r--   0        0        0    11512 2021-11-01 20:48:14.105481 language_data-1.1/language_data/data/trie/gd/name_to_language.marisa
--rw-r--r--   0        0        0     7208 2021-11-01 20:48:14.349482 language_data-1.1/language_data/data/trie/gd/name_to_script.marisa
--rw-r--r--   0        0        0     8784 2021-11-01 20:48:14.601483 language_data-1.1/language_data/data/trie/gd/name_to_territory.marisa
--rw-r--r--   0        0        0     9296 2021-11-01 20:48:14.105481 language_data-1.1/language_data/data/trie/gl/name_to_language.marisa
--rw-r--r--   0        0        0     4888 2021-11-01 20:48:14.353482 language_data-1.1/language_data/data/trie/gl/name_to_script.marisa
--rw-r--r--   0        0        0     8288 2021-11-01 20:48:14.601483 language_data-1.1/language_data/data/trie/gl/name_to_territory.marisa
--rw-r--r--   0        0        0     9688 2021-11-01 20:48:14.109481 language_data-1.1/language_data/data/trie/gsw/name_to_language.marisa
--rw-r--r--   0        0        0     6176 2021-11-01 20:48:14.353482 language_data-1.1/language_data/data/trie/gsw/name_to_script.marisa
--rw-r--r--   0        0        0     8112 2021-11-01 20:48:14.601483 language_data-1.1/language_data/data/trie/gsw/name_to_territory.marisa
--rw-r--r--   0        0        0    14408 2021-11-01 20:48:14.109481 language_data-1.1/language_data/data/trie/gu/name_to_language.marisa
--rw-r--r--   0        0        0     7712 2021-11-01 20:48:14.353482 language_data-1.1/language_data/data/trie/gu/name_to_script.marisa
--rw-r--r--   0        0        0    11408 2021-11-01 20:48:14.605483 language_data-1.1/language_data/data/trie/gu/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.109481 language_data-1.1/language_data/data/trie/guz/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.969054 language_data-1.1/language_data/data/trie/guz/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.605483 language_data-1.1/language_data/data/trie/guz/name_to_territory.marisa
--rw-r--r--   0        0        0     4120 2021-11-01 20:48:14.109481 language_data-1.1/language_data/data/trie/gv/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.973055 language_data-1.1/language_data/data/trie/gv/name_to_script.marisa
--rw-r--r--   0        0        0     4120 2021-11-01 20:48:14.605483 language_data-1.1/language_data/data/trie/gv/name_to_territory.marisa
--rw-r--r--   0        0        0     7488 2021-11-01 20:48:14.113481 language_data-1.1/language_data/data/trie/ha/name_to_language.marisa
--rw-r--r--   0        0        0     4856 2021-11-01 20:48:14.353482 language_data-1.1/language_data/data/trie/ha/name_to_script.marisa
--rw-r--r--   0        0        0     7992 2021-11-01 20:48:14.605483 language_data-1.1/language_data/data/trie/ha/name_to_territory.marisa
--rw-r--r--   0        0        0     4864 2021-11-01 20:48:14.113481 language_data-1.1/language_data/data/trie/haw/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.973055 language_data-1.1/language_data/data/trie/haw/name_to_script.marisa
--rw-r--r--   0        0        0     4384 2021-11-01 20:48:14.605483 language_data-1.1/language_data/data/trie/haw/name_to_territory.marisa
--rw-r--r--   0        0        0    10976 2021-11-01 20:48:14.113481 language_data-1.1/language_data/data/trie/he/name_to_language.marisa
--rw-r--r--   0        0        0     7488 2021-11-01 20:48:14.353482 language_data-1.1/language_data/data/trie/he/name_to_script.marisa
--rw-r--r--   0        0        0     8888 2021-11-01 20:48:14.609484 language_data-1.1/language_data/data/trie/he/name_to_territory.marisa
--rw-r--r--   0        0        0    14240 2021-11-01 20:48:14.117481 language_data-1.1/language_data/data/trie/hi/name_to_language.marisa
--rw-r--r--   0        0        0     7768 2021-11-01 20:48:14.353482 language_data-1.1/language_data/data/trie/hi/name_to_script.marisa
--rw-r--r--   0        0        0    11288 2021-11-01 20:48:14.609484 language_data-1.1/language_data/data/trie/hi/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/hil/name_to_language.marisa
--rw-r--r--   0        0        0    10496 2021-11-01 20:48:14.117481 language_data-1.1/language_data/data/trie/hr/name_to_language.marisa
--rw-r--r--   0        0        0     7328 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/hr/name_to_script.marisa
--rw-r--r--   0        0        0     8136 2021-11-01 20:48:14.609484 language_data-1.1/language_data/data/trie/hr/name_to_territory.marisa
--rw-r--r--   0        0        0     7920 2021-11-01 20:48:14.117481 language_data-1.1/language_data/data/trie/hsb/name_to_language.marisa
--rw-r--r--   0        0        0     4864 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/hsb/name_to_script.marisa
--rw-r--r--   0        0        0     8240 2021-11-01 20:48:14.609484 language_data-1.1/language_data/data/trie/hsb/name_to_territory.marisa
--rw-r--r--   0        0        0    10440 2021-11-01 20:48:14.121481 language_data-1.1/language_data/data/trie/hu/name_to_language.marisa
--rw-r--r--   0        0        0     6280 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/hu/name_to_script.marisa
--rw-r--r--   0        0        0     8392 2021-11-01 20:48:14.613484 language_data-1.1/language_data/data/trie/hu/name_to_territory.marisa
--rw-r--r--   0        0        0    11752 2021-11-01 20:48:14.121481 language_data-1.1/language_data/data/trie/hy/name_to_language.marisa
--rw-r--r--   0        0        0     5152 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/hy/name_to_script.marisa
--rw-r--r--   0        0        0     9768 2021-11-01 20:48:14.613484 language_data-1.1/language_data/data/trie/hy/name_to_territory.marisa
--rw-r--r--   0        0        0     8936 2021-11-01 20:48:14.125481 language_data-1.1/language_data/data/trie/ia/name_to_language.marisa
--rw-r--r--   0        0        0     4760 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/ia/name_to_script.marisa
--rw-r--r--   0        0        0     8096 2021-11-01 20:48:14.613484 language_data-1.1/language_data/data/trie/ia/name_to_territory.marisa
--rw-r--r--   0        0        0    10384 2021-11-01 20:48:13.953480 language_data-1.1/language_data/data/trie/id/name_to_language.marisa
--rw-r--r--   0        0        0     7104 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/id/name_to_script.marisa
--rw-r--r--   0        0        0     7872 2021-11-01 20:48:14.617483 language_data-1.1/language_data/data/trie/id/name_to_territory.marisa
--rw-r--r--   0        0        0     7512 2021-11-01 20:48:14.125481 language_data-1.1/language_data/data/trie/ig/name_to_language.marisa
--rw-r--r--   0        0        0     4840 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/ig/name_to_script.marisa
--rw-r--r--   0        0        0     8256 2021-11-01 20:48:14.617483 language_data-1.1/language_data/data/trie/ig/name_to_territory.marisa
--rw-r--r--   0        0        0     4480 2021-11-01 20:48:14.125481 language_data-1.1/language_data/data/trie/ii/name_to_language.marisa
--rw-r--r--   0        0        0     4272 2021-11-01 20:48:14.357482 language_data-1.1/language_data/data/trie/ii/name_to_script.marisa
--rw-r--r--   0        0        0     4208 2021-11-01 20:48:14.617483 language_data-1.1/language_data/data/trie/ii/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/ilo/name_to_language.marisa
--rw-r--r--   0        0        0     4088 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/io/name_to_language.marisa
--rw-r--r--   0        0        0    10288 2021-11-01 20:48:14.125481 language_data-1.1/language_data/data/trie/is/name_to_language.marisa
--rw-r--r--   0        0        0     4992 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/is/name_to_script.marisa
--rw-r--r--   0        0        0     8288 2021-11-01 20:48:14.617483 language_data-1.1/language_data/data/trie/is/name_to_territory.marisa
--rw-r--r--   0        0        0    11232 2021-11-01 20:48:14.129481 language_data-1.1/language_data/data/trie/it/name_to_language.marisa
--rw-r--r--   0        0        0     6632 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/it/name_to_script.marisa
--rw-r--r--   0        0        0     8088 2021-11-01 20:48:14.621483 language_data-1.1/language_data/data/trie/it/name_to_territory.marisa
--rw-r--r--   0        0        0    13480 2021-11-01 20:48:14.133481 language_data-1.1/language_data/data/trie/ja/name_to_language.marisa
--rw-r--r--   0        0        0     8024 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/ja/name_to_script.marisa
--rw-r--r--   0        0        0     9024 2021-11-01 20:48:14.621483 language_data-1.1/language_data/data/trie/ja/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/jbo/name_to_language.marisa
--rw-r--r--   0        0        0     4504 2021-11-01 20:48:14.133481 language_data-1.1/language_data/data/trie/jgo/name_to_language.marisa
--rw-r--r--   0        0        0     4216 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/jgo/name_to_script.marisa
--rw-r--r--   0        0        0     5296 2021-11-01 20:48:14.621483 language_data-1.1/language_data/data/trie/jgo/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.133481 language_data-1.1/language_data/data/trie/jmc/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/jmc/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.621483 language_data-1.1/language_data/data/trie/jmc/name_to_territory.marisa
--rw-r--r--   0        0        0     7272 2021-11-01 20:48:14.133481 language_data-1.1/language_data/data/trie/jv/name_to_language.marisa
--rw-r--r--   0        0        0     4720 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/jv/name_to_script.marisa
--rw-r--r--   0        0        0     8072 2021-11-01 20:48:14.625484 language_data-1.1/language_data/data/trie/jv/name_to_territory.marisa
--rw-r--r--   0        0        0    13168 2021-11-01 20:48:14.133481 language_data-1.1/language_data/data/trie/ka/name_to_language.marisa
--rw-r--r--   0        0        0     8040 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/ka/name_to_script.marisa
--rw-r--r--   0        0        0    11088 2021-11-01 20:48:14.625484 language_data-1.1/language_data/data/trie/ka/name_to_territory.marisa
--rw-r--r--   0        0        0     5064 2021-11-01 20:48:14.137481 language_data-1.1/language_data/data/trie/kab/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/kab/name_to_script.marisa
--rw-r--r--   0        0        0     6896 2021-11-01 20:48:14.625484 language_data-1.1/language_data/data/trie/kab/name_to_territory.marisa
--rw-r--r--   0        0        0     5032 2021-11-01 20:48:14.137481 language_data-1.1/language_data/data/trie/kam/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/kam/name_to_script.marisa
--rw-r--r--   0        0        0     6880 2021-11-01 20:48:14.625484 language_data-1.1/language_data/data/trie/kam/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/kcm/name_to_language.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.137481 language_data-1.1/language_data/data/trie/kde/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/kde/name_to_script.marisa
--rw-r--r--   0        0        0     6856 2021-11-01 20:48:14.629484 language_data-1.1/language_data/data/trie/kde/name_to_territory.marisa
--rw-r--r--   0        0        0     6880 2021-11-01 20:48:14.137481 language_data-1.1/language_data/data/trie/kea/name_to_language.marisa
--rw-r--r--   0        0        0     4720 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/kea/name_to_script.marisa
--rw-r--r--   0        0        0     8104 2021-11-01 20:48:14.629484 language_data-1.1/language_data/data/trie/kea/name_to_territory.marisa
--rw-r--r--   0        0        0    10440 2021-11-01 20:48:14.137481 language_data-1.1/language_data/data/trie/kgp/name_to_language.marisa
--rw-r--r--   0        0        0     6240 2021-11-01 20:48:14.361482 language_data-1.1/language_data/data/trie/kgp/name_to_script.marisa
--rw-r--r--   0        0        0     8472 2021-11-01 20:48:14.629484 language_data-1.1/language_data/data/trie/kgp/name_to_territory.marisa
--rw-r--r--   0        0        0     5256 2021-11-01 20:48:14.141481 language_data-1.1/language_data/data/trie/khq/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/khq/name_to_script.marisa
--rw-r--r--   0        0        0     7040 2021-11-01 20:48:14.629484 language_data-1.1/language_data/data/trie/khq/name_to_territory.marisa
--rw-r--r--   0        0        0     5072 2021-11-01 20:48:14.141481 language_data-1.1/language_data/data/trie/ki/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/ki/name_to_script.marisa
--rw-r--r--   0        0        0     6864 2021-11-01 20:48:14.633484 language_data-1.1/language_data/data/trie/ki/name_to_territory.marisa
--rw-r--r--   0        0        0    11264 2021-11-01 20:48:14.141481 language_data-1.1/language_data/data/trie/kk/name_to_language.marisa
--rw-r--r--   0        0        0     5432 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/kk/name_to_script.marisa
--rw-r--r--   0        0        0     9632 2021-11-01 20:48:14.633484 language_data-1.1/language_data/data/trie/kk/name_to_territory.marisa
--rw-r--r--   0        0        0     4184 2021-11-01 20:48:14.141481 language_data-1.1/language_data/data/trie/kkj/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/kkj/name_to_script.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.633484 language_data-1.1/language_data/data/trie/kkj/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.141481 language_data-1.1/language_data/data/trie/kl/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.981054 language_data-1.1/language_data/data/trie/kl/name_to_script.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:14.633484 language_data-1.1/language_data/data/trie/kl/name_to_territory.marisa
--rw-r--r--   0        0        0     5136 2021-11-01 20:48:14.141481 language_data-1.1/language_data/data/trie/kln/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.985054 language_data-1.1/language_data/data/trie/kln/name_to_script.marisa
--rw-r--r--   0        0        0     7040 2021-11-01 20:48:14.633484 language_data-1.1/language_data/data/trie/kln/name_to_territory.marisa
--rw-r--r--   0        0        0    12144 2021-11-01 20:48:14.145481 language_data-1.1/language_data/data/trie/km/name_to_language.marisa
--rw-r--r--   0        0        0     5392 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/km/name_to_script.marisa
--rw-r--r--   0        0        0    11568 2021-11-01 20:48:14.633484 language_data-1.1/language_data/data/trie/km/name_to_territory.marisa
--rw-r--r--   0        0        0    14432 2021-11-01 20:48:14.145481 language_data-1.1/language_data/data/trie/kn/name_to_language.marisa
--rw-r--r--   0        0        0     8072 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/kn/name_to_script.marisa
--rw-r--r--   0        0        0    11904 2021-11-01 20:48:14.637484 language_data-1.1/language_data/data/trie/kn/name_to_territory.marisa
--rw-r--r--   0        0        0    11944 2021-11-01 20:48:14.149481 language_data-1.1/language_data/data/trie/ko/name_to_language.marisa
--rw-r--r--   0        0        0     7800 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/ko/name_to_script.marisa
--rw-r--r--   0        0        0     8848 2021-11-01 20:48:14.637484 language_data-1.1/language_data/data/trie/ko/name_to_territory.marisa
--rw-r--r--   0        0        0    12288 2021-11-01 20:48:14.149481 language_data-1.1/language_data/data/trie/kok/name_to_language.marisa
--rw-r--r--   0        0        0     5216 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/kok/name_to_script.marisa
--rw-r--r--   0        0        0    11288 2021-11-01 20:48:14.637484 language_data-1.1/language_data/data/trie/kok/name_to_territory.marisa
--rw-r--r--   0        0        0    11176 2021-11-01 20:48:14.153481 language_data-1.1/language_data/data/trie/ks/name_to_language.marisa
--rw-r--r--   0        0        0     6816 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/ks/name_to_script.marisa
--rw-r--r--   0        0        0     9408 2021-11-01 20:48:14.641484 language_data-1.1/language_data/data/trie/ks/name_to_territory.marisa
--rw-r--r--   0        0        0     5032 2021-11-01 20:48:14.153481 language_data-1.1/language_data/data/trie/ksb/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.985054 language_data-1.1/language_data/data/trie/ksb/name_to_script.marisa
--rw-r--r--   0        0        0     6808 2021-11-01 20:48:14.641484 language_data-1.1/language_data/data/trie/ksb/name_to_territory.marisa
--rw-r--r--   0        0        0     5112 2021-11-01 20:48:14.153481 language_data-1.1/language_data/data/trie/ksf/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.985054 language_data-1.1/language_data/data/trie/ksf/name_to_script.marisa
--rw-r--r--   0        0        0     7056 2021-11-01 20:48:14.641484 language_data-1.1/language_data/data/trie/ksf/name_to_territory.marisa
--rw-r--r--   0        0        0     9048 2021-11-01 20:48:14.153481 language_data-1.1/language_data/data/trie/ksh/name_to_language.marisa
--rw-r--r--   0        0        0     5168 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/ksh/name_to_script.marisa
--rw-r--r--   0        0        0     8528 2021-11-01 20:48:14.641484 language_data-1.1/language_data/data/trie/ksh/name_to_territory.marisa
--rw-r--r--   0        0        0     7160 2021-11-01 20:48:14.153481 language_data-1.1/language_data/data/trie/ku/name_to_language.marisa
--rw-r--r--   0        0        0     4328 2021-11-01 20:48:14.365482 language_data-1.1/language_data/data/trie/ku/name_to_script.marisa
--rw-r--r--   0        0        0     7488 2021-11-01 20:48:14.645484 language_data-1.1/language_data/data/trie/ku/name_to_territory.marisa
--rw-r--r--   0        0        0     4120 2021-11-01 20:48:14.153481 language_data-1.1/language_data/data/trie/kw/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.989054 language_data-1.1/language_data/data/trie/kw/name_to_script.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:14.645484 language_data-1.1/language_data/data/trie/kw/name_to_territory.marisa
--rw-r--r--   0        0        0    10920 2021-11-01 20:48:14.157481 language_data-1.1/language_data/data/trie/ky/name_to_language.marisa
--rw-r--r--   0        0        0     5016 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/ky/name_to_script.marisa
--rw-r--r--   0        0        0     9600 2021-11-01 20:48:14.645484 language_data-1.1/language_data/data/trie/ky/name_to_territory.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/la/name_to_language.marisa
--rw-r--r--   0        0        0     5184 2021-11-01 20:48:14.157481 language_data-1.1/language_data/data/trie/lag/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.989054 language_data-1.1/language_data/data/trie/lag/name_to_script.marisa
--rw-r--r--   0        0        0     7376 2021-11-01 20:48:14.645484 language_data-1.1/language_data/data/trie/lag/name_to_territory.marisa
--rw-r--r--   0        0        0     4112 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/lah/name_to_language.marisa
--rw-r--r--   0        0        0    11616 2021-11-01 20:48:14.157481 language_data-1.1/language_data/data/trie/lb/name_to_language.marisa
--rw-r--r--   0        0        0     6088 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/lb/name_to_script.marisa
--rw-r--r--   0        0        0     8032 2021-11-01 20:48:14.645484 language_data-1.1/language_data/data/trie/lb/name_to_territory.marisa
--rw-r--r--   0        0        0     5096 2021-11-01 20:48:14.157481 language_data-1.1/language_data/data/trie/lg/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.989054 language_data-1.1/language_data/data/trie/lg/name_to_script.marisa
--rw-r--r--   0        0        0     6984 2021-11-01 20:48:14.649484 language_data-1.1/language_data/data/trie/lg/name_to_territory.marisa
--rw-r--r--   0        0        0     6552 2021-11-01 20:48:14.161481 language_data-1.1/language_data/data/trie/lkt/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.989054 language_data-1.1/language_data/data/trie/lkt/name_to_script.marisa
--rw-r--r--   0        0        0     4400 2021-11-01 20:48:14.649484 language_data-1.1/language_data/data/trie/lkt/name_to_territory.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.161481 language_data-1.1/language_data/data/trie/ln/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.989054 language_data-1.1/language_data/data/trie/ln/name_to_script.marisa
--rw-r--r--   0        0        0     7168 2021-11-01 20:48:14.649484 language_data-1.1/language_data/data/trie/ln/name_to_territory.marisa
--rw-r--r--   0        0        0    13672 2021-11-01 20:48:14.161481 language_data-1.1/language_data/data/trie/lo/name_to_language.marisa
--rw-r--r--   0        0        0     8304 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/lo/name_to_script.marisa
--rw-r--r--   0        0        0    10992 2021-11-01 20:48:14.649484 language_data-1.1/language_data/data/trie/lo/name_to_territory.marisa
--rw-r--r--   0        0        0     7976 2021-11-01 20:48:14.165481 language_data-1.1/language_data/data/trie/lrc/name_to_language.marisa
--rw-r--r--   0        0        0     4936 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/lrc/name_to_script.marisa
--rw-r--r--   0        0        0     4552 2021-11-01 20:48:14.649484 language_data-1.1/language_data/data/trie/lrc/name_to_territory.marisa
--rw-r--r--   0        0        0    11704 2021-11-01 20:48:14.165481 language_data-1.1/language_data/data/trie/lt/name_to_language.marisa
--rw-r--r--   0        0        0     6752 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/lt/name_to_script.marisa
--rw-r--r--   0        0        0     8216 2021-11-01 20:48:14.653484 language_data-1.1/language_data/data/trie/lt/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.165481 language_data-1.1/language_data/data/trie/lu/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.989054 language_data-1.1/language_data/data/trie/lu/name_to_script.marisa
--rw-r--r--   0        0        0     6784 2021-11-01 20:48:14.653484 language_data-1.1/language_data/data/trie/lu/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.165481 language_data-1.1/language_data/data/trie/luo/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/luo/name_to_script.marisa
--rw-r--r--   0        0        0     6960 2021-11-01 20:48:14.653484 language_data-1.1/language_data/data/trie/luo/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.165481 language_data-1.1/language_data/data/trie/luy/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/luy/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.653484 language_data-1.1/language_data/data/trie/luy/name_to_territory.marisa
--rw-r--r--   0        0        0    10224 2021-11-01 20:48:14.169481 language_data-1.1/language_data/data/trie/lv/name_to_language.marisa
--rw-r--r--   0        0        0     5416 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/lv/name_to_script.marisa
--rw-r--r--   0        0        0     8256 2021-11-01 20:48:14.657484 language_data-1.1/language_data/data/trie/lv/name_to_territory.marisa
--rw-r--r--   0        0        0     5072 2021-11-01 20:48:14.169481 language_data-1.1/language_data/data/trie/mai/name_to_language.marisa
--rw-r--r--   0        0        0     4312 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/mai/name_to_script.marisa
--rw-r--r--   0        0        0     4360 2021-11-01 20:48:14.657484 language_data-1.1/language_data/data/trie/mai/name_to_territory.marisa
--rw-r--r--   0        0        0     5080 2021-11-01 20:48:14.169481 language_data-1.1/language_data/data/trie/mas/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/mas/name_to_script.marisa
--rw-r--r--   0        0        0     6840 2021-11-01 20:48:14.657484 language_data-1.1/language_data/data/trie/mas/name_to_territory.marisa
--rw-r--r--   0        0        0     5064 2021-11-01 20:48:14.169481 language_data-1.1/language_data/data/trie/mer/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/mer/name_to_script.marisa
--rw-r--r--   0        0        0     6880 2021-11-01 20:48:14.657484 language_data-1.1/language_data/data/trie/mer/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.169481 language_data-1.1/language_data/data/trie/mfe/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/mfe/name_to_script.marisa
--rw-r--r--   0        0        0     6784 2021-11-01 20:48:14.657484 language_data-1.1/language_data/data/trie/mfe/name_to_territory.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.169481 language_data-1.1/language_data/data/trie/mg/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/mg/name_to_script.marisa
--rw-r--r--   0        0        0     6984 2021-11-01 20:48:14.661484 language_data-1.1/language_data/data/trie/mg/name_to_territory.marisa
--rw-r--r--   0        0        0     4920 2021-11-01 20:48:14.173481 language_data-1.1/language_data/data/trie/mgh/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.993054 language_data-1.1/language_data/data/trie/mgh/name_to_script.marisa
--rw-r--r--   0        0        0     5680 2021-11-01 20:48:14.661484 language_data-1.1/language_data/data/trie/mgh/name_to_territory.marisa
--rw-r--r--   0        0        0     4112 2021-11-01 20:48:14.173481 language_data-1.1/language_data/data/trie/mgo/name_to_language.marisa
--rw-r--r--   0        0        0     4144 2021-11-01 20:48:14.369482 language_data-1.1/language_data/data/trie/mgo/name_to_script.marisa
--rw-r--r--   0        0        0     4112 2021-11-01 20:48:14.661484 language_data-1.1/language_data/data/trie/mgo/name_to_territory.marisa
--rw-r--r--   0        0        0     4552 2021-11-01 20:48:14.173481 language_data-1.1/language_data/data/trie/mi/name_to_language.marisa
--rw-r--r--   0        0        0     4216 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/mi/name_to_script.marisa
--rw-r--r--   0        0        0     4280 2021-11-01 20:48:14.661484 language_data-1.1/language_data/data/trie/mi/name_to_territory.marisa
--rw-r--r--   0        0        0    13600 2021-11-01 20:48:14.173481 language_data-1.1/language_data/data/trie/mk/name_to_language.marisa
--rw-r--r--   0        0        0     8264 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/mk/name_to_script.marisa
--rw-r--r--   0        0        0     9728 2021-11-01 20:48:14.661484 language_data-1.1/language_data/data/trie/mk/name_to_territory.marisa
--rw-r--r--   0        0        0    14952 2021-11-01 20:48:14.177481 language_data-1.1/language_data/data/trie/ml/name_to_language.marisa
--rw-r--r--   0        0        0     7928 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/ml/name_to_script.marisa
--rw-r--r--   0        0        0    11976 2021-11-01 20:48:14.661484 language_data-1.1/language_data/data/trie/ml/name_to_territory.marisa
--rw-r--r--   0        0        0    10224 2021-11-01 20:48:14.177481 language_data-1.1/language_data/data/trie/mn/name_to_language.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/mn/name_to_script.marisa
--rw-r--r--   0        0        0     9768 2021-11-01 20:48:14.665484 language_data-1.1/language_data/data/trie/mn/name_to_territory.marisa
--rw-r--r--   0        0        0     5120 2021-11-01 20:48:14.177481 language_data-1.1/language_data/data/trie/mni/name_to_language.marisa
--rw-r--r--   0        0        0     4416 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/mni/name_to_script.marisa
--rw-r--r--   0        0        0     4368 2021-11-01 20:48:14.665484 language_data-1.1/language_data/data/trie/mni/name_to_territory.marisa
--rw-r--r--   0        0        0    14264 2021-11-01 20:48:14.181481 language_data-1.1/language_data/data/trie/mr/name_to_language.marisa
--rw-r--r--   0        0        0     7728 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/mr/name_to_script.marisa
--rw-r--r--   0        0        0    11224 2021-11-01 20:48:14.665484 language_data-1.1/language_data/data/trie/mr/name_to_territory.marisa
--rw-r--r--   0        0        0     9432 2021-11-01 20:48:13.953480 language_data-1.1/language_data/data/trie/ms/name_to_language.marisa
--rw-r--r--   0        0        0     6568 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/ms/name_to_script.marisa
--rw-r--r--   0        0        0     7936 2021-11-01 20:48:14.665484 language_data-1.1/language_data/data/trie/ms/name_to_territory.marisa
--rw-r--r--   0        0        0    10056 2021-11-01 20:48:14.181481 language_data-1.1/language_data/data/trie/mt/name_to_language.marisa
--rw-r--r--   0        0        0     4272 2021-11-01 20:48:14.373482 language_data-1.1/language_data/data/trie/mt/name_to_script.marisa
--rw-r--r--   0        0        0     8304 2021-11-01 20:48:14.669484 language_data-1.1/language_data/data/trie/mt/name_to_territory.marisa
--rw-r--r--   0        0        0     5104 2021-11-01 20:48:14.181481 language_data-1.1/language_data/data/trie/mua/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.997054 language_data-1.1/language_data/data/trie/mua/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.669484 language_data-1.1/language_data/data/trie/mua/name_to_territory.marisa
--rw-r--r--   0        0        0    12872 2021-11-01 20:48:14.185481 language_data-1.1/language_data/data/trie/my/name_to_language.marisa
--rw-r--r--   0        0        0     5552 2021-11-01 20:48:14.377482 language_data-1.1/language_data/data/trie/my/name_to_script.marisa
--rw-r--r--   0        0        0    11760 2021-11-01 20:48:14.669484 language_data-1.1/language_data/data/trie/my/name_to_territory.marisa
--rw-r--r--   0        0        0     7960 2021-11-01 20:48:14.185481 language_data-1.1/language_data/data/trie/mzn/name_to_language.marisa
--rw-r--r--   0        0        0     4496 2021-11-01 20:48:14.377482 language_data-1.1/language_data/data/trie/mzn/name_to_script.marisa
--rw-r--r--   0        0        0     8872 2021-11-01 20:48:14.673484 language_data-1.1/language_data/data/trie/mzn/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/nah/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/nan/name_to_language.marisa
--rw-r--r--   0        0        0     5280 2021-11-01 20:48:14.185481 language_data-1.1/language_data/data/trie/naq/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.997054 language_data-1.1/language_data/data/trie/naq/name_to_script.marisa
--rw-r--r--   0        0        0     7088 2021-11-01 20:48:14.673484 language_data-1.1/language_data/data/trie/naq/name_to_territory.marisa
--rw-r--r--   0        0        0    11256 2021-11-01 20:48:14.189481 language_data-1.1/language_data/data/trie/nb/name_to_language.marisa
--rw-r--r--   0        0        0     6752 2021-11-01 20:48:14.377482 language_data-1.1/language_data/data/trie/nb/name_to_script.marisa
--rw-r--r--   0        0        0     8096 2021-11-01 20:48:14.673484 language_data-1.1/language_data/data/trie/nb/name_to_territory.marisa
--rw-r--r--   0        0        0     5072 2021-11-01 20:48:14.189481 language_data-1.1/language_data/data/trie/nd/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:01.997054 language_data-1.1/language_data/data/trie/nd/name_to_script.marisa
--rw-r--r--   0        0        0     7056 2021-11-01 20:48:14.673484 language_data-1.1/language_data/data/trie/nd/name_to_territory.marisa
--rw-r--r--   0        0        0     4176 2021-11-01 20:44:44.276442 language_data-1.1/language_data/data/trie/nds/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.001054 language_data-1.1/language_data/data/trie/nds/name_to_script.marisa
--rw-r--r--   0        0        0     4168 2021-10-27 20:46:02.301054 language_data-1.1/language_data/data/trie/nds/name_to_territory.marisa
--rw-r--r--   0        0        0    15368 2021-11-01 20:48:14.193482 language_data-1.1/language_data/data/trie/ne/name_to_language.marisa
--rw-r--r--   0        0        0     7368 2021-11-01 20:48:14.377482 language_data-1.1/language_data/data/trie/ne/name_to_script.marisa
--rw-r--r--   0        0        0    11520 2021-11-01 20:48:14.677484 language_data-1.1/language_data/data/trie/ne/name_to_territory.marisa
--rw-r--r--   0        0        0    11488 2021-11-01 20:48:14.193482 language_data-1.1/language_data/data/trie/nl/name_to_language.marisa
--rw-r--r--   0        0        0     7320 2021-11-01 20:48:14.377482 language_data-1.1/language_data/data/trie/nl/name_to_script.marisa
--rw-r--r--   0        0        0     8248 2021-11-01 20:48:14.677484 language_data-1.1/language_data/data/trie/nl/name_to_territory.marisa
--rw-r--r--   0        0        0     5136 2021-11-01 20:48:14.193482 language_data-1.1/language_data/data/trie/nmg/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.001054 language_data-1.1/language_data/data/trie/nmg/name_to_script.marisa
--rw-r--r--   0        0        0     6984 2021-11-01 20:48:14.677484 language_data-1.1/language_data/data/trie/nmg/name_to_territory.marisa
--rw-r--r--   0        0        0    11280 2021-11-01 20:48:14.197481 language_data-1.1/language_data/data/trie/nn/name_to_language.marisa
--rw-r--r--   0        0        0     6736 2021-11-01 20:48:14.377482 language_data-1.1/language_data/data/trie/nn/name_to_script.marisa
--rw-r--r--   0        0        0     8072 2021-11-01 20:48:14.677484 language_data-1.1/language_data/data/trie/nn/name_to_territory.marisa
--rw-r--r--   0        0        0     4496 2021-11-01 20:48:14.197481 language_data-1.1/language_data/data/trie/nnh/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.001054 language_data-1.1/language_data/data/trie/nnh/name_to_script.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.677484 language_data-1.1/language_data/data/trie/nnh/name_to_territory.marisa
--rw-r--r--   0        0        0    11256 2021-11-01 20:48:14.197481 language_data-1.1/language_data/data/trie/no/name_to_language.marisa
--rw-r--r--   0        0        0     6752 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/no/name_to_script.marisa
--rw-r--r--   0        0        0     8096 2021-11-01 20:48:14.681484 language_data-1.1/language_data/data/trie/no/name_to_territory.marisa
--rw-r--r--   0        0        0     5032 2021-11-01 20:48:14.197481 language_data-1.1/language_data/data/trie/nus/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.001054 language_data-1.1/language_data/data/trie/nus/name_to_script.marisa
--rw-r--r--   0        0        0     4848 2021-11-01 20:48:14.681484 language_data-1.1/language_data/data/trie/nus/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/nv/name_to_language.marisa
--rw-r--r--   0        0        0     5064 2021-11-01 20:48:14.201481 language_data-1.1/language_data/data/trie/nyn/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.001054 language_data-1.1/language_data/data/trie/nyn/name_to_script.marisa
--rw-r--r--   0        0        0     6952 2021-11-01 20:48:14.681484 language_data-1.1/language_data/data/trie/nyn/name_to_territory.marisa
--rw-r--r--   0        0        0     5504 2021-11-01 20:48:14.201481 language_data-1.1/language_data/data/trie/om/name_to_language.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/om/name_to_script.marisa
--rw-r--r--   0        0        0     4232 2021-11-01 20:48:14.681484 language_data-1.1/language_data/data/trie/om/name_to_territory.marisa
--rw-r--r--   0        0        0    14272 2021-11-01 20:48:14.201481 language_data-1.1/language_data/data/trie/or/name_to_language.marisa
--rw-r--r--   0        0        0     7928 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/or/name_to_script.marisa
--rw-r--r--   0        0        0    11832 2021-11-01 20:48:14.681484 language_data-1.1/language_data/data/trie/or/name_to_territory.marisa
--rw-r--r--   0        0        0     5648 2021-11-01 20:48:14.201481 language_data-1.1/language_data/data/trie/os/name_to_language.marisa
--rw-r--r--   0        0        0     4296 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/os/name_to_script.marisa
--rw-r--r--   0        0        0     4392 2021-11-01 20:48:14.681484 language_data-1.1/language_data/data/trie/os/name_to_territory.marisa
--rw-r--r--   0        0        0    12048 2021-11-01 20:48:14.205481 language_data-1.1/language_data/data/trie/pa/name_to_language.marisa
--rw-r--r--   0        0        0     5200 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/pa/name_to_script.marisa
--rw-r--r--   0        0        0    10776 2021-11-01 20:48:14.685484 language_data-1.1/language_data/data/trie/pa/name_to_territory.marisa
--rw-r--r--   0        0        0     8336 2021-11-01 20:48:14.205481 language_data-1.1/language_data/data/trie/pcm/name_to_language.marisa
--rw-r--r--   0        0        0     4992 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/pcm/name_to_script.marisa
--rw-r--r--   0        0        0     8784 2021-11-01 20:48:14.685484 language_data-1.1/language_data/data/trie/pcm/name_to_territory.marisa
--rw-r--r--   0        0        0    11488 2021-11-01 20:48:14.205481 language_data-1.1/language_data/data/trie/pl/name_to_language.marisa
--rw-r--r--   0        0        0     6448 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/pl/name_to_script.marisa
--rw-r--r--   0        0        0     8328 2021-11-01 20:48:14.685484 language_data-1.1/language_data/data/trie/pl/name_to_territory.marisa
--rw-r--r--   0        0        0     4184 2021-09-10 18:22:57.644101 language_data-1.1/language_data/data/trie/prg/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-09-10 18:22:57.644101 language_data-1.1/language_data/data/trie/prg/name_to_script.marisa
--rw-r--r--   0        0        0     4168 2021-09-10 18:22:57.644101 language_data-1.1/language_data/data/trie/prg/name_to_territory.marisa
--rw-r--r--   0        0        0    10304 2021-11-01 20:48:14.209482 language_data-1.1/language_data/data/trie/ps/name_to_language.marisa
--rw-r--r--   0        0        0     5056 2021-11-01 20:48:14.381482 language_data-1.1/language_data/data/trie/ps/name_to_script.marisa
--rw-r--r--   0        0        0     9208 2021-11-01 20:48:14.689484 language_data-1.1/language_data/data/trie/ps/name_to_territory.marisa
--rw-r--r--   0        0        0    10520 2021-11-01 20:48:14.209482 language_data-1.1/language_data/data/trie/pt/name_to_language.marisa
--rw-r--r--   0        0        0     6152 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/pt/name_to_script.marisa
--rw-r--r--   0        0        0     8272 2021-11-01 20:48:14.689484 language_data-1.1/language_data/data/trie/pt/name_to_territory.marisa
--rw-r--r--   0        0        0     7824 2021-11-01 20:48:14.213482 language_data-1.1/language_data/data/trie/qu/name_to_language.marisa
--rw-r--r--   0        0        0     4928 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/qu/name_to_script.marisa
--rw-r--r--   0        0        0     8024 2021-11-01 20:48:14.689484 language_data-1.1/language_data/data/trie/qu/name_to_territory.marisa
--rw-r--r--   0        0        0     9880 2021-11-01 20:48:14.213482 language_data-1.1/language_data/data/trie/rm/name_to_language.marisa
--rw-r--r--   0        0        0     6280 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/rm/name_to_script.marisa
--rw-r--r--   0        0        0     8080 2021-11-01 20:48:14.693484 language_data-1.1/language_data/data/trie/rm/name_to_territory.marisa
--rw-r--r--   0        0        0     5152 2021-11-01 20:48:14.213482 language_data-1.1/language_data/data/trie/rn/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.009054 language_data-1.1/language_data/data/trie/rn/name_to_script.marisa
--rw-r--r--   0        0        0     7072 2021-11-01 20:48:14.693484 language_data-1.1/language_data/data/trie/rn/name_to_territory.marisa
--rw-r--r--   0        0        0    10448 2021-11-01 20:48:14.217481 language_data-1.1/language_data/data/trie/ro/name_to_language.marisa
--rw-r--r--   0        0        0     6696 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/ro/name_to_script.marisa
--rw-r--r--   0        0        0     8344 2021-11-01 20:48:14.693484 language_data-1.1/language_data/data/trie/ro/name_to_territory.marisa
--rw-r--r--   0        0        0     5040 2021-11-01 20:48:14.217481 language_data-1.1/language_data/data/trie/rof/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.009054 language_data-1.1/language_data/data/trie/rof/name_to_script.marisa
--rw-r--r--   0        0        0     6840 2021-11-01 20:48:14.693484 language_data-1.1/language_data/data/trie/rof/name_to_territory.marisa
--rw-r--r--   0        0        0    12584 2021-11-01 20:48:14.217481 language_data-1.1/language_data/data/trie/ru/name_to_language.marisa
--rw-r--r--   0        0        0     8088 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/ru/name_to_script.marisa
--rw-r--r--   0        0        0     9848 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/ru/name_to_territory.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/rup/name_to_language.marisa
--rw-r--r--   0        0        0     5672 2021-11-01 20:48:14.217481 language_data-1.1/language_data/data/trie/rw/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.009054 language_data-1.1/language_data/data/trie/rw/name_to_script.marisa
--rw-r--r--   0        0        0     4136 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/rw/name_to_territory.marisa
--rw-r--r--   0        0        0     5040 2021-11-01 20:48:14.217481 language_data-1.1/language_data/data/trie/rwk/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.009054 language_data-1.1/language_data/data/trie/rwk/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/rwk/name_to_territory.marisa
--rw-r--r--   0        0        0     5560 2021-11-01 20:48:14.221482 language_data-1.1/language_data/data/trie/sa/name_to_language.marisa
--rw-r--r--   0        0        0     4288 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/sa/name_to_script.marisa
--rw-r--r--   0        0        0     4368 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/sa/name_to_territory.marisa
--rw-r--r--   0        0        0     5736 2021-11-01 20:48:14.221482 language_data-1.1/language_data/data/trie/sah/name_to_language.marisa
--rw-r--r--   0        0        0     4368 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/sah/name_to_script.marisa
--rw-r--r--   0        0        0     4664 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/sah/name_to_territory.marisa
--rw-r--r--   0        0        0     5048 2021-11-01 20:48:14.221482 language_data-1.1/language_data/data/trie/saq/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.009054 language_data-1.1/language_data/data/trie/saq/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/saq/name_to_territory.marisa
--rw-r--r--   0        0        0     5096 2021-11-01 20:48:14.221482 language_data-1.1/language_data/data/trie/sat/name_to_language.marisa
--rw-r--r--   0        0        0     4376 2021-11-01 20:48:14.385482 language_data-1.1/language_data/data/trie/sat/name_to_script.marisa
--rw-r--r--   0        0        0     4360 2021-11-01 20:48:14.697484 language_data-1.1/language_data/data/trie/sat/name_to_territory.marisa
--rw-r--r--   0        0        0     5080 2021-11-01 20:48:14.221482 language_data-1.1/language_data/data/trie/sbp/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.009054 language_data-1.1/language_data/data/trie/sbp/name_to_script.marisa
--rw-r--r--   0        0        0     6928 2021-11-01 20:48:14.701484 language_data-1.1/language_data/data/trie/sbp/name_to_territory.marisa
--rw-r--r--   0        0        0     7464 2021-11-01 20:48:14.221482 language_data-1.1/language_data/data/trie/sc/name_to_language.marisa
--rw-r--r--   0        0        0     6872 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/sc/name_to_script.marisa
--rw-r--r--   0        0        0     8368 2021-11-01 20:48:14.701484 language_data-1.1/language_data/data/trie/sc/name_to_territory.marisa
--rw-r--r--   0        0        0    10680 2021-11-01 20:48:14.225482 language_data-1.1/language_data/data/trie/sd/name_to_language.marisa
--rw-r--r--   0        0        0     5952 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/sd/name_to_script.marisa
--rw-r--r--   0        0        0     9232 2021-11-01 20:48:14.701484 language_data-1.1/language_data/data/trie/sd/name_to_territory.marisa
--rw-r--r--   0        0        0     6016 2021-11-01 20:48:14.225482 language_data-1.1/language_data/data/trie/se/name_to_language.marisa
--rw-r--r--   0        0        0     4296 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/se/name_to_script.marisa
--rw-r--r--   0        0        0     7856 2021-11-01 20:48:14.701484 language_data-1.1/language_data/data/trie/se/name_to_territory.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.225482 language_data-1.1/language_data/data/trie/seh/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.013054 language_data-1.1/language_data/data/trie/seh/name_to_script.marisa
--rw-r--r--   0        0        0     7024 2021-11-01 20:48:14.705484 language_data-1.1/language_data/data/trie/seh/name_to_territory.marisa
--rw-r--r--   0        0        0     5248 2021-11-01 20:48:14.225482 language_data-1.1/language_data/data/trie/ses/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.013054 language_data-1.1/language_data/data/trie/ses/name_to_script.marisa
--rw-r--r--   0        0        0     7040 2021-11-01 20:48:14.705484 language_data-1.1/language_data/data/trie/ses/name_to_territory.marisa
--rw-r--r--   0        0        0     5224 2021-11-01 20:48:14.225482 language_data-1.1/language_data/data/trie/sg/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.013054 language_data-1.1/language_data/data/trie/sg/name_to_script.marisa
--rw-r--r--   0        0        0     7352 2021-11-01 20:48:14.705484 language_data-1.1/language_data/data/trie/sg/name_to_territory.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/sh/name_to_language.marisa
--rw-r--r--   0        0        0     6152 2021-11-01 20:48:14.225482 language_data-1.1/language_data/data/trie/shi/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.013054 language_data-1.1/language_data/data/trie/shi/name_to_script.marisa
--rw-r--r--   0        0        0    10488 2021-11-01 20:48:14.709484 language_data-1.1/language_data/data/trie/shi/name_to_territory.marisa
--rw-r--r--   0        0        0    12784 2021-11-01 20:48:14.229482 language_data-1.1/language_data/data/trie/si/name_to_language.marisa
--rw-r--r--   0        0        0     5256 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/si/name_to_script.marisa
--rw-r--r--   0        0        0    11416 2021-11-01 20:48:14.709484 language_data-1.1/language_data/data/trie/si/name_to_territory.marisa
--rw-r--r--   0        0        0    10632 2021-11-01 20:48:14.229482 language_data-1.1/language_data/data/trie/sk/name_to_language.marisa
--rw-r--r--   0        0        0     5112 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/sk/name_to_script.marisa
--rw-r--r--   0        0        0     8344 2021-11-01 20:48:14.709484 language_data-1.1/language_data/data/trie/sk/name_to_territory.marisa
--rw-r--r--   0        0        0    10280 2021-11-01 20:48:14.233482 language_data-1.1/language_data/data/trie/sl/name_to_language.marisa
--rw-r--r--   0        0        0     6336 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/sl/name_to_script.marisa
--rw-r--r--   0        0        0     8152 2021-11-01 20:48:14.709484 language_data-1.1/language_data/data/trie/sl/name_to_territory.marisa
--rw-r--r--   0        0        0     9352 2021-11-01 20:48:14.233482 language_data-1.1/language_data/data/trie/smn/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.013054 language_data-1.1/language_data/data/trie/smn/name_to_script.marisa
--rw-r--r--   0        0        0     7584 2021-11-01 20:48:14.713484 language_data-1.1/language_data/data/trie/smn/name_to_territory.marisa
--rw-r--r--   0        0        0     5072 2021-11-01 20:48:14.233482 language_data-1.1/language_data/data/trie/sn/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.013054 language_data-1.1/language_data/data/trie/sn/name_to_script.marisa
--rw-r--r--   0        0        0     6912 2021-11-01 20:48:14.713484 language_data-1.1/language_data/data/trie/sn/name_to_territory.marisa
--rw-r--r--   0        0        0     7632 2021-11-01 20:48:14.233482 language_data-1.1/language_data/data/trie/so/name_to_language.marisa
--rw-r--r--   0        0        0     7152 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/so/name_to_script.marisa
--rw-r--r--   0        0        0     8368 2021-11-01 20:48:14.713484 language_data-1.1/language_data/data/trie/so/name_to_territory.marisa
--rw-r--r--   0        0        0     9296 2021-11-01 20:48:14.237482 language_data-1.1/language_data/data/trie/sq/name_to_language.marisa
--rw-r--r--   0        0        0     6272 2021-11-01 20:48:14.389482 language_data-1.1/language_data/data/trie/sq/name_to_script.marisa
--rw-r--r--   0        0        0     8056 2021-11-01 20:48:14.713484 language_data-1.1/language_data/data/trie/sq/name_to_territory.marisa
--rw-r--r--   0        0        0    15352 2021-11-01 20:48:14.241482 language_data-1.1/language_data/data/trie/sr/name_to_language.marisa
--rw-r--r--   0        0        0     8840 2021-11-01 20:48:14.393482 language_data-1.1/language_data/data/trie/sr/name_to_script.marisa
--rw-r--r--   0        0        0    12424 2021-11-01 20:48:14.717484 language_data-1.1/language_data/data/trie/sr/name_to_territory.marisa
--rw-r--r--   0        0        0     4544 2021-11-01 20:48:14.241482 language_data-1.1/language_data/data/trie/su/name_to_language.marisa
--rw-r--r--   0        0        0     4200 2021-11-01 20:48:14.393482 language_data-1.1/language_data/data/trie/su/name_to_script.marisa
--rw-r--r--   0        0        0     4240 2021-11-01 20:48:14.717484 language_data-1.1/language_data/data/trie/su/name_to_territory.marisa
--rw-r--r--   0        0        0    11552 2021-11-01 20:48:14.241482 language_data-1.1/language_data/data/trie/sv/name_to_language.marisa
--rw-r--r--   0        0        0     7320 2021-11-01 20:48:14.393482 language_data-1.1/language_data/data/trie/sv/name_to_script.marisa
--rw-r--r--   0        0        0     8072 2021-11-01 20:48:14.717484 language_data-1.1/language_data/data/trie/sv/name_to_territory.marisa
--rw-r--r--   0        0        0     9296 2021-11-01 20:48:14.245482 language_data-1.1/language_data/data/trie/sw/name_to_language.marisa
--rw-r--r--   0        0        0     4776 2021-11-01 20:48:14.393482 language_data-1.1/language_data/data/trie/sw/name_to_script.marisa
--rw-r--r--   0        0        0     8040 2021-11-01 20:48:14.721484 language_data-1.1/language_data/data/trie/sw/name_to_territory.marisa
--rw-r--r--   0        0        0    14432 2021-11-01 20:48:14.245482 language_data-1.1/language_data/data/trie/ta/name_to_language.marisa
--rw-r--r--   0        0        0     8176 2021-11-01 20:48:14.393482 language_data-1.1/language_data/data/trie/ta/name_to_script.marisa
--rw-r--r--   0        0        0    11592 2021-11-01 20:48:14.721484 language_data-1.1/language_data/data/trie/ta/name_to_territory.marisa
--rw-r--r--   0        0        0    14280 2021-11-01 20:48:14.249482 language_data-1.1/language_data/data/trie/te/name_to_language.marisa
--rw-r--r--   0        0        0     7992 2021-11-01 20:48:14.393482 language_data-1.1/language_data/data/trie/te/name_to_script.marisa
--rw-r--r--   0        0        0    11784 2021-11-01 20:48:14.721484 language_data-1.1/language_data/data/trie/te/name_to_territory.marisa
--rw-r--r--   0        0        0     5040 2021-11-01 20:48:14.249482 language_data-1.1/language_data/data/trie/teo/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.021054 language_data-1.1/language_data/data/trie/teo/name_to_script.marisa
--rw-r--r--   0        0        0     6840 2021-11-01 20:48:14.725484 language_data-1.1/language_data/data/trie/teo/name_to_territory.marisa
--rw-r--r--   0        0        0     7056 2021-11-01 20:48:14.249482 language_data-1.1/language_data/data/trie/tg/name_to_language.marisa
--rw-r--r--   0        0        0     4264 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/tg/name_to_script.marisa
--rw-r--r--   0        0        0     8656 2021-11-01 20:48:14.725484 language_data-1.1/language_data/data/trie/tg/name_to_territory.marisa
--rw-r--r--   0        0        0    15688 2021-11-01 20:48:14.249482 language_data-1.1/language_data/data/trie/th/name_to_language.marisa
--rw-r--r--   0        0        0     8648 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/th/name_to_script.marisa
--rw-r--r--   0        0        0    11568 2021-11-01 20:48:14.725484 language_data-1.1/language_data/data/trie/th/name_to_territory.marisa
--rw-r--r--   0        0        0     8424 2021-11-01 20:48:14.253482 language_data-1.1/language_data/data/trie/ti/name_to_language.marisa
--rw-r--r--   0        0        0     4168 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/ti/name_to_script.marisa
--rw-r--r--   0        0        0     9248 2021-11-01 20:48:14.725484 language_data-1.1/language_data/data/trie/ti/name_to_territory.marisa
--rw-r--r--   0        0        0     9272 2021-11-01 20:48:14.253482 language_data-1.1/language_data/data/trie/tk/name_to_language.marisa
--rw-r--r--   0        0        0     5112 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/tk/name_to_script.marisa
--rw-r--r--   0        0        0     8192 2021-11-01 20:48:14.729484 language_data-1.1/language_data/data/trie/tk/name_to_territory.marisa
--rw-r--r--   0        0        0    11048 2021-11-01 20:48:14.257482 language_data-1.1/language_data/data/trie/to/name_to_language.marisa
--rw-r--r--   0        0        0     6720 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/to/name_to_script.marisa
--rw-r--r--   0        0        0     7944 2021-11-01 20:48:14.729484 language_data-1.1/language_data/data/trie/to/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/tpi/name_to_language.marisa
--rw-r--r--   0        0        0    12040 2021-11-01 20:48:14.257482 language_data-1.1/language_data/data/trie/tr/name_to_language.marisa
--rw-r--r--   0        0        0     6672 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/tr/name_to_script.marisa
--rw-r--r--   0        0        0     8144 2021-11-01 20:48:14.729484 language_data-1.1/language_data/data/trie/tr/name_to_territory.marisa
--rw-r--r--   0        0        0     7016 2021-11-01 20:48:14.257482 language_data-1.1/language_data/data/trie/tt/name_to_language.marisa
--rw-r--r--   0        0        0     4272 2021-11-01 20:48:14.397482 language_data-1.1/language_data/data/trie/tt/name_to_script.marisa
--rw-r--r--   0        0        0     8624 2021-11-01 20:48:14.733484 language_data-1.1/language_data/data/trie/tt/name_to_territory.marisa
--rw-r--r--   0        0        0     5256 2021-11-01 20:48:14.257482 language_data-1.1/language_data/data/trie/twq/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.025054 language_data-1.1/language_data/data/trie/twq/name_to_script.marisa
--rw-r--r--   0        0        0     7040 2021-11-01 20:48:14.733484 language_data-1.1/language_data/data/trie/twq/name_to_territory.marisa
--rw-r--r--   0        0        0     5128 2021-11-01 20:48:14.261482 language_data-1.1/language_data/data/trie/tzm/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.025054 language_data-1.1/language_data/data/trie/tzm/name_to_script.marisa
--rw-r--r--   0        0        0     7040 2021-11-01 20:48:14.733484 language_data-1.1/language_data/data/trie/tzm/name_to_territory.marisa
--rw-r--r--   0        0        0    11928 2021-11-01 20:48:14.261482 language_data-1.1/language_data/data/trie/ug/name_to_language.marisa
--rw-r--r--   0        0        0     7776 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/ug/name_to_script.marisa
--rw-r--r--   0        0        0     9744 2021-11-01 20:48:14.733484 language_data-1.1/language_data/data/trie/ug/name_to_territory.marisa
--rw-r--r--   0        0        0    13056 2021-11-01 20:48:14.261482 language_data-1.1/language_data/data/trie/uk/name_to_language.marisa
--rw-r--r--   0        0        0     7624 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/uk/name_to_script.marisa
--rw-r--r--   0        0        0    10016 2021-11-01 20:48:14.737484 language_data-1.1/language_data/data/trie/uk/name_to_territory.marisa
--rw-r--r--   0        0        0   583896 2021-11-01 20:48:13.949480 language_data-1.1/language_data/data/trie/und/name_to_language.marisa
--rw-r--r--   0        0        0   142160 2021-11-01 20:48:14.325482 language_data-1.1/language_data/data/trie/und/name_to_script.marisa
--rw-r--r--   0        0        0   405384 2021-11-01 20:48:14.537483 language_data-1.1/language_data/data/trie/und/name_to_territory.marisa
--rw-r--r--   0        0        0    10312 2021-11-01 20:48:14.265482 language_data-1.1/language_data/data/trie/ur/name_to_language.marisa
--rw-r--r--   0        0        0     5008 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/ur/name_to_script.marisa
--rw-r--r--   0        0        0     9368 2021-11-01 20:48:14.737484 language_data-1.1/language_data/data/trie/ur/name_to_territory.marisa
--rw-r--r--   0        0        0    12560 2021-11-01 20:48:14.265482 language_data-1.1/language_data/data/trie/uz/name_to_language.marisa
--rw-r--r--   0        0        0     5344 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/uz/name_to_script.marisa
--rw-r--r--   0        0        0    12480 2021-11-01 20:48:14.741484 language_data-1.1/language_data/data/trie/uz/name_to_territory.marisa
--rw-r--r--   0        0        0     5928 2021-11-01 20:48:14.269482 language_data-1.1/language_data/data/trie/vai/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.025054 language_data-1.1/language_data/data/trie/vai/name_to_script.marisa
--rw-r--r--   0        0        0    10808 2021-11-01 20:48:14.741484 language_data-1.1/language_data/data/trie/vai/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.289482 language_data-1.1/language_data/data/trie/ve/name_to_language.marisa
--rw-r--r--   0        0        0    10880 2021-11-01 20:48:14.269482 language_data-1.1/language_data/data/trie/vi/name_to_language.marisa
--rw-r--r--   0        0        0     6776 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/vi/name_to_script.marisa
--rw-r--r--   0        0        0     8352 2021-11-01 20:48:14.741484 language_data-1.1/language_data/data/trie/vi/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/vo/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-09-10 18:22:57.652101 language_data-1.1/language_data/data/trie/vo/name_to_script.marisa
--rw-r--r--   0        0        0     4168 2021-09-10 18:22:57.652101 language_data-1.1/language_data/data/trie/vo/name_to_territory.marisa
--rw-r--r--   0        0        0     5040 2021-11-01 20:48:14.269482 language_data-1.1/language_data/data/trie/vun/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.025054 language_data-1.1/language_data/data/trie/vun/name_to_script.marisa
--rw-r--r--   0        0        0     6848 2021-11-01 20:48:14.745484 language_data-1.1/language_data/data/trie/vun/name_to_territory.marisa
--rw-r--r--   0        0        0     6112 2021-11-01 20:48:14.269482 language_data-1.1/language_data/data/trie/wae/name_to_language.marisa
--rw-r--r--   0        0        0     4544 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/wae/name_to_script.marisa
--rw-r--r--   0        0        0     7920 2021-11-01 20:48:14.745484 language_data-1.1/language_data/data/trie/wae/name_to_territory.marisa
--rw-r--r--   0        0        0     6232 2021-11-01 20:48:14.273482 language_data-1.1/language_data/data/trie/wo/name_to_language.marisa
--rw-r--r--   0        0        0     4216 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/wo/name_to_script.marisa
--rw-r--r--   0        0        0     7208 2021-11-01 20:48:14.745484 language_data-1.1/language_data/data/trie/wo/name_to_territory.marisa
--rw-r--r--   0        0        0     4096 2021-11-01 20:48:14.273482 language_data-1.1/language_data/data/trie/xh/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.029054 language_data-1.1/language_data/data/trie/xh/name_to_script.marisa
--rw-r--r--   0        0        0     4120 2021-11-01 20:48:14.745484 language_data-1.1/language_data/data/trie/xh/name_to_territory.marisa
--rw-r--r--   0        0        0     5088 2021-11-01 20:48:14.273482 language_data-1.1/language_data/data/trie/xog/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.029054 language_data-1.1/language_data/data/trie/xog/name_to_script.marisa
--rw-r--r--   0        0        0     6960 2021-11-01 20:48:14.745484 language_data-1.1/language_data/data/trie/xog/name_to_territory.marisa
--rw-r--r--   0        0        0     5176 2021-11-01 20:48:14.273482 language_data-1.1/language_data/data/trie/yav/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.029054 language_data-1.1/language_data/data/trie/yav/name_to_script.marisa
--rw-r--r--   0        0        0     7176 2021-11-01 20:48:14.749484 language_data-1.1/language_data/data/trie/yav/name_to_territory.marisa
--rw-r--r--   0        0        0     7136 2021-11-01 20:48:14.273482 language_data-1.1/language_data/data/trie/yi/name_to_language.marisa
--rw-r--r--   0        0        0     4216 2021-11-01 20:48:14.401482 language_data-1.1/language_data/data/trie/yi/name_to_script.marisa
--rw-r--r--   0        0        0     8088 2021-11-01 20:48:14.749484 language_data-1.1/language_data/data/trie/yi/name_to_territory.marisa
--rw-r--r--   0        0        0     8200 2021-11-01 20:48:14.273482 language_data-1.1/language_data/data/trie/yo/name_to_language.marisa
--rw-r--r--   0        0        0     5008 2021-11-01 20:48:14.405482 language_data-1.1/language_data/data/trie/yo/name_to_script.marisa
--rw-r--r--   0        0        0     8912 2021-11-01 20:48:14.749484 language_data-1.1/language_data/data/trie/yo/name_to_territory.marisa
--rw-r--r--   0        0        0    10352 2021-11-01 20:48:14.277482 language_data-1.1/language_data/data/trie/yrl/name_to_language.marisa
--rw-r--r--   0        0        0     6320 2021-11-01 20:48:14.405482 language_data-1.1/language_data/data/trie/yrl/name_to_script.marisa
--rw-r--r--   0        0        0     8248 2021-11-01 20:48:14.749484 language_data-1.1/language_data/data/trie/yrl/name_to_territory.marisa
--rw-r--r--   0        0        0    15216 2021-11-01 20:48:14.281482 language_data-1.1/language_data/data/trie/yue/name_to_language.marisa
--rw-r--r--   0        0        0     8328 2021-11-01 20:48:14.405482 language_data-1.1/language_data/data/trie/yue/name_to_script.marisa
--rw-r--r--   0        0        0    10120 2021-11-01 20:48:14.753484 language_data-1.1/language_data/data/trie/yue/name_to_territory.marisa
--rw-r--r--   0        0        0     5704 2021-11-01 20:48:14.281482 language_data-1.1/language_data/data/trie/zgh/name_to_language.marisa
--rw-r--r--   0        0        0     4104 2021-10-27 20:46:02.029054 language_data-1.1/language_data/data/trie/zgh/name_to_script.marisa
--rw-r--r--   0        0        0     8696 2021-11-01 20:48:14.753484 language_data-1.1/language_data/data/trie/zgh/name_to_territory.marisa
--rw-r--r--   0        0        0    17520 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/zh/name_to_language.marisa
--rw-r--r--   0        0        0     9664 2021-11-01 20:48:14.405482 language_data-1.1/language_data/data/trie/zh/name_to_script.marisa
--rw-r--r--   0        0        0    10680 2021-11-01 20:48:14.757484 language_data-1.1/language_data/data/trie/zh/name_to_territory.marisa
--rw-r--r--   0        0        0     4104 2021-11-01 20:48:13.949480 language_data-1.1/language_data/data/trie/zsm/name_to_language.marisa
--rw-r--r--   0        0        0     9296 2021-11-01 20:48:14.285482 language_data-1.1/language_data/data/trie/zu/name_to_language.marisa
--rw-r--r--   0        0        0     6776 2021-11-01 20:48:14.409483 language_data-1.1/language_data/data/trie/zu/name_to_script.marisa
--rw-r--r--   0        0        0     8128 2021-11-01 20:48:14.757484 language_data-1.1/language_data/data/trie/zu/name_to_territory.marisa
--rw-r--r--   0        0        0   233291 2021-09-10 18:22:57.656101 language_data-1.1/language_data/data/wiktionary/codes-en.csv
--rw-r--r--   0        0        0     1084 2021-09-10 18:22:57.656101 language_data-1.1/language_data/language_lists.py
--rw-r--r--   0        0        0  3953875 2021-11-01 20:48:14.801484 language_data-1.1/language_data/name_data.py
--rw-r--r--   0        0        0     3848 2021-09-10 18:22:57.664101 language_data-1.1/language_data/names.py
--rw-r--r--   0        0        0   136169 2021-11-01 20:48:14.873485 language_data-1.1/language_data/population_data.py
--rw-r--r--   0        0        0     1797 2021-09-10 18:22:57.664101 language_data-1.1/language_data/registry_parser.py
--rw-r--r--   0        0        0      347 2021-09-10 18:22:57.664101 language_data-1.1/language_data/util.py
--rw-r--r--   0        0        0      589 2021-11-11 17:27:05.280191 language_data-1.1/pyproject.toml
--rw-r--r--   0        0        0    12454 2021-11-11 17:28:01.222657 language_data-1.1/setup.py
--rw-r--r--   0        0        0     3520 2021-11-11 17:28:01.223127 language_data-1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.373115 language_data-1.2.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.213116 language_data-1.2.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.245116 language_data-1.2.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-02-23 14:34:20.373115 language_data-1.2.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.253116 language_data-1.2.0.dev3/language_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19608 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/build_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.253116 language_data-1.2.0.dev3/language_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/extra_language_names.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   715867 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/language-subtag-registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    41382 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/languageInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/override_language_names.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   381483 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/supplementalData.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.245116 language_data-1.2.0.dev3/language_data/data/trie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/af/
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/af/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/af/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/af/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/agq/
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/agq/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/agq/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/agq/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/ak/
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ak/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ak/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ak/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/am/
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/am/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/am/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/am/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/ang/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ang/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ar/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ar/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ar/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/as/
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/as/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/as/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/as/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/asa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/asa/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/asa/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/asa/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.257115 language_data-1.2.0.dev3/language_data/data/trie/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ast/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ast/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ast/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/az/
+-rw-r--r--   0 runner    (1001) docker     (127)    14296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/az/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/az/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/az/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/bas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bas/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bas/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bas/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/be/
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/be/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/be/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/be/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/bem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bem/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bem/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bem/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/bez/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bez/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bez/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bez/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/bho/
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bho/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.261116 language_data-1.2.0.dev3/language_data/data/trie/bm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bm/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bm/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bm/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/bn/
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11864 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/bo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/br/
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/br/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/br/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/br/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/brx/
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/brx/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/brx/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/brx/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/bs/
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bs/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bs/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/bs/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ca/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ca/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ca/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/ccp/
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ccp/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ccp/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ccp/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.265116 language_data-1.2.0.dev3/language_data/data/trie/ce/
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ce/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ce/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ce/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/ceb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ceb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ceb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ceb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/cgg/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cgg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cgg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cgg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/chr/
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/chr/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/chr/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/chr/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/ckb/
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ckb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ckb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ckb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cs/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cs/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cs/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/cu/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/cy/
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cy/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cy/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/cy/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.269116 language_data-1.2.0.dev3/language_data/data/trie/da/
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/da/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/da/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/da/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/dav/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dav/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dav/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dav/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/de/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/de/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/de/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/dje/
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dje/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dje/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dje/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/doi/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/doi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/doi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/doi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/dsb/
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dsb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dsb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dsb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/dua/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dua/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dua/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dua/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/dyo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dyo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dyo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dyo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/dz/
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dz/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dz/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/dz/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.273115 language_data-1.2.0.dev3/language_data/data/trie/ebu/
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ebu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ebu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ebu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/ee/
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ee/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ee/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ee/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/el/
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/el/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/el/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/el/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/en/
+-rw-r--r--   0 runner    (1001) docker     (127)   103352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/en/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/en/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/en/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/eo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/eo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/eo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/es/
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/es/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/es/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/es/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/et/
+-rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/et/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/et/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/et/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.277115 language_data-1.2.0.dev3/language_data/data/trie/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/eu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/eu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/eu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/ewo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ewo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ewo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ewo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fa/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fa/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fa/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/ff/
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ff/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ff/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ff/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/fil/
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fil/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fil/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fil/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/fo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fr/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fr/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fr/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.281115 language_data-1.2.0.dev3/language_data/data/trie/fur/
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fur/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fur/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fur/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/fy/
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fy/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fy/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/fy/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/ga/
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ga/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ga/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ga/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/gd/
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gd/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gd/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gd/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/gl/
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gl/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gl/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gl/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/gsw/
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gsw/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gsw/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gsw/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/gu/
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/guz/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/guz/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/guz/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/guz/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/gv/
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gv/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gv/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/gv/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.285116 language_data-1.2.0.dev3/language_data/data/trie/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ha/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ha/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ha/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/haw/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/haw/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/haw/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/haw/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/he/
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/he/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/he/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/he/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/hi/
+-rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/hil/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hil/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hr/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hr/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hr/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/hsb/
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hsb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hsb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hsb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.289116 language_data-1.2.0.dev3/language_data/data/trie/hy/
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hy/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hy/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/hy/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/ia/
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ia/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ia/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ia/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/id/
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/id/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/id/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/id/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/ig/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ig/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ig/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ig/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/ii/
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ii/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ii/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ii/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/ilo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ilo/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/io/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/is/
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/is/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/is/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/is/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/it/
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/it/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/it/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/it/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ja/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ja/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ja/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.293115 language_data-1.2.0.dev3/language_data/data/trie/jbo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jbo/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/jgo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jgo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jgo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jgo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/jmc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jmc/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jmc/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jmc/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/jv/
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jv/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jv/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/jv/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/ka/
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ka/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ka/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ka/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/kab/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kab/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kab/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kab/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/kam/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kam/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kam/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kam/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/kcm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kcm/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/kde/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kde/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kde/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kde/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.297115 language_data-1.2.0.dev3/language_data/data/trie/kea/
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kea/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kea/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kea/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/kgp/
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kgp/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kgp/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kgp/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/khq/
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/khq/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/khq/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/khq/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/ki/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ki/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ki/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ki/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/kk/
+-rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kk/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kk/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kk/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/kkj/
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kkj/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kkj/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kkj/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/kl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kl/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kl/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kl/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.301115 language_data-1.2.0.dev3/language_data/data/trie/kln/
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kln/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kln/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kln/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/km/
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/km/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/km/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/km/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/kn/
+-rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ko/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ko/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ko/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/kok/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kok/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kok/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kok/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/ks/
+-rw-r--r--   0 runner    (1001) docker     (127)    11176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ks/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ks/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ks/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/ksb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/ksf/
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksf/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksf/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksf/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.305116 language_data-1.2.0.dev3/language_data/data/trie/ksh/
+-rw-r--r--   0 runner    (1001) docker     (127)     9048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ksh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/ku/
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ku/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ku/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ku/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/kw/
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kw/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kw/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/kw/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/ky/
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ky/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ky/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ky/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/la/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/la/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/lag/
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lag/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lag/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lag/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/lah/
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lah/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/lb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/lg/
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/lkt/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lkt/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lkt/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lkt/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.309116 language_data-1.2.0.dev3/language_data/data/trie/ln/
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ln/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ln/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ln/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/lo/
+-rw-r--r--   0 runner    (1001) docker     (127)    13672 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/lrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lrc/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lrc/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lrc/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lt/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lt/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lt/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/lu/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/luo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/luo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/luo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/luo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/luy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/luy/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/luy/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/luy/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.313115 language_data-1.2.0.dev3/language_data/data/trie/lv/
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lv/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lv/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/lv/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mai/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mai/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mai/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mai/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mas/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mas/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mas/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mer/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mer/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mer/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mfe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mfe/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mfe/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mfe/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mg/
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mgh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mgh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mgh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mgh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mgo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mgo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mgo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mgo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.317115 language_data-1.2.0.dev3/language_data/data/trie/mi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/mk/
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mk/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mk/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mk/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ml/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ml/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ml/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/mn/
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/mni/
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mni/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mni/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mni/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/mr/
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mr/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mr/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mr/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ms/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ms/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ms/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/mt/
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mt/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mt/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mt/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.321115 language_data-1.2.0.dev3/language_data/data/trie/mua/
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mua/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mua/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mua/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/my/
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/my/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/my/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/my/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/mzn/
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mzn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mzn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/mzn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/nah/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nah/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/nan/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nan/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/naq/
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/naq/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/naq/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/naq/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/nb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nb/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nb/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nb/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/nd/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nd/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nd/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nd/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/nds/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nds/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nds/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nds/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.325115 language_data-1.2.0.dev3/language_data/data/trie/ne/
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ne/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ne/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ne/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nl/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nl/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nl/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nmg/
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nmg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nmg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nmg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nnh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nnh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nnh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nnh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/no/
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/no/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/no/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/no/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nus/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nus/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nus/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nus/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nv/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nv/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/nyn/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nyn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nyn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/nyn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.329115 language_data-1.2.0.dev3/language_data/data/trie/om/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/om/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/om/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/om/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/or/
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/or/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/or/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/or/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/os/
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/os/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/os/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/os/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/pa/
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pa/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pa/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pa/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/pcm/
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pcm/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pcm/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pcm/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pl/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pl/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pl/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/prg/
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/prg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/prg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/prg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/ps/
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ps/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ps/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ps/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.333115 language_data-1.2.0.dev3/language_data/data/trie/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pt/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pt/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/pt/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/qu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/qu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/qu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/qu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/rm/
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rm/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rm/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rm/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/rn/
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ro/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ro/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ro/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/rof/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rof/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rof/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rof/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ru/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ru/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ru/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/rup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rup/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.337115 language_data-1.2.0.dev3/language_data/data/trie/rw/
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rw/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rw/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rw/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/rwk/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rwk/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rwk/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/rwk/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/sa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sa/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sa/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sa/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/sah/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sah/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sah/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sah/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/saq/
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/saq/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/saq/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/saq/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/sat/
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sat/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sat/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sat/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/sbp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sbp/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sbp/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sbp/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/sc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sc/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sc/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sc/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.341115 language_data-1.2.0.dev3/language_data/data/trie/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sd/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sd/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sd/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/se/
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/se/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/se/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/se/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/seh/
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/seh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/seh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/seh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/ses/
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ses/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ses/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ses/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/sg/
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/sh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sh/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/shi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/shi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/shi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/shi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/si/
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/si/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/si/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/si/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.345115 language_data-1.2.0.dev3/language_data/data/trie/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sk/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sk/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sk/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sl/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sl/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sl/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/smn/
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/smn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/smn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/smn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/sn/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sn/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sn/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sn/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/so/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/so/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/so/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/so/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/sq/
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sq/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sq/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sq/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sr/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sr/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sr/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/su/
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/su/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/su/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/su/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.349115 language_data-1.2.0.dev3/language_data/data/trie/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sv/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sv/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sv/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/sw/
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sw/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sw/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/sw/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ta/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ta/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ta/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/te/
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/te/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/te/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/te/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/teo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/teo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/teo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/teo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/tg/
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tg/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tg/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tg/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/th/
+-rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/th/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/th/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/th/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ti/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ti/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ti/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.353115 language_data-1.2.0.dev3/language_data/data/trie/tk/
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tk/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tk/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tk/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/to/
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/to/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/to/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/to/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/tpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tpi/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tr/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tr/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tr/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/tt/
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tt/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tt/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tt/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/twq/
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/twq/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/twq/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/twq/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/tzm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tzm/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tzm/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/tzm/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/ug/
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ug/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ug/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ug/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.357115 language_data-1.2.0.dev3/language_data/data/trie/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)    13056 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/uk/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/uk/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/uk/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.361115 language_data-1.2.0.dev3/language_data/data/trie/und/
+-rw-r--r--   0 runner    (1001) docker     (127)   583896 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/und/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)   142160 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/und/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)   405384 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/und/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.361115 language_data-1.2.0.dev3/language_data/data/trie/ur/
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ur/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ur/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ur/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.361115 language_data-1.2.0.dev3/language_data/data/trie/uz/
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/uz/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/uz/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/uz/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.361115 language_data-1.2.0.dev3/language_data/data/trie/vai/
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vai/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vai/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vai/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.361115 language_data-1.2.0.dev3/language_data/data/trie/ve/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/ve/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.361115 language_data-1.2.0.dev3/language_data/data/trie/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/vo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/vun/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vun/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vun/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/vun/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/wae/
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/wae/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/wae/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/wae/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/wo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/wo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/wo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/wo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/xh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/xh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/xh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/xh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/xog/
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/xog/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/xog/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/xog/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/yav/
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yav/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yav/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yav/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.365115 language_data-1.2.0.dev3/language_data/data/trie/yi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yi/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yi/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yi/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/yo/
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yo/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yo/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yo/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/yrl/
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yrl/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yrl/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yrl/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/yue/
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yue/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yue/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/yue/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/zgh/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zgh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zgh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zgh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zh/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zh/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zh/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/zsm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zsm/name_to_language.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/trie/zu/
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zu/name_to_language.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zu/name_to_script.marisa
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/trie/zu/name_to_territory.marisa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data/data/wiktionary/
+-rw-r--r--   0 runner    (1001) docker     (127)   233291 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/data/wiktionary/codes-en.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/language_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3953875 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/name_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136169 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/population_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/registry_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/language_data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:34:20.369115 language_data-1.2.0.dev3/language_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-02-23 14:34:20.000000 language_data-1.2.0.dev3/language_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35177 2024-02-23 14:34:20.000000 language_data-1.2.0.dev3/language_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:34:20.000000 language_data-1.2.0.dev3/language_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-23 14:34:20.000000 language_data-1.2.0.dev3/language_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-23 14:34:20.000000 language_data-1.2.0.dev3/language_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-23 14:33:56.000000 language_data-1.2.0.dev3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 14:34:20.373115 language_data-1.2.0.dev3/setup.cfg
```

### Comparing `language_data-1.1/README.md` & `language_data-1.2.0.dev3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 
 `language_data` has a dependency on the `marisa-trie` package so that it can load a compact, efficient data structure for looking up language names.
 
 ## Installation
 
 `language_data` is usually installed as a dependency of `langcodes`, and doesn't make much sense without it. You can `pip install language_data` anyway if you want.
 
-To install the `language_data` package in editable mode, run `poetry install` in the package root. (This is the equivalent of `pip install -e .`, which currently doesn't work because pip does not yet fully support PEP 621.)
+To install the `language_data` package in editable mode, run `poetry install` in the package root. (This is the equivalent of `pip install -e .`, which will hopefully become compatible again soon via PEP 660.)
```

### Comparing `language_data-1.1/language_data/build_data.py` & `language_data-1.2.0.dev3/language_data/build_data.py`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/extra_language_names.csv` & `language_data-1.2.0.dev3/language_data/data/extra_language_names.csv`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/language-subtag-registry.txt` & `language_data-1.2.0.dev3/language_data/data/language-subtag-registry.txt`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/languageInfo.xml` & `language_data-1.2.0.dev3/language_data/data/languageInfo.xml`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/supplementalData.xml` & `language_data-1.2.0.dev3/language_data/data/supplementalData.xml`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/af/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/af/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/af/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/af/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/af/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/af/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/agq/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/agq/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/agq/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/agq/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/agq/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/agq/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ak/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ak/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ak/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ak/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ak/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ak/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/am/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/am/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/am/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/am/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/am/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/am/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ang/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ang/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ar/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ar/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ar/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ar/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ar/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ar/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/as/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/as/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/as/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/as/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/as/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/as/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/asa/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/asa/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/asa/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/asa/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/asa/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/asa/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ast/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ast/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ast/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ast/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ast/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ast/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/az/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/az/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/az/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/az/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/az/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/az/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bas/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bas/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bas/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bas/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bas/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bas/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/be/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/be/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/be/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/be/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/be/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/be/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bem/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bem/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bem/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bem/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bem/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bem/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bez/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bez/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bez/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bez/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bez/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bez/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bho/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bho/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bm/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bm/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bm/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bm/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bm/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bm/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/br/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/br/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/br/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/br/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/br/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/br/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/brx/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/brx/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/brx/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/brx/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/brx/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/brx/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bs/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bs/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bs/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bs/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/bs/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/bs/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ca/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ca/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ca/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ca/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ca/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ca/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ccp/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ccp/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ccp/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ccp/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ccp/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ccp/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ce/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ce/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ce/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ce/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ce/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ce/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ceb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ceb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ceb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ceb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ceb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ceb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cgg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cgg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cgg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cgg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cgg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cgg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/chr/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/chr/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/chr/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/chr/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/chr/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/chr/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ckb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ckb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ckb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ckb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ckb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ckb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cs/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cs/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cs/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cs/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cs/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cs/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cy/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cy/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cy/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cy/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/cy/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/cy/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/da/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/da/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/da/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/da/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/da/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/da/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dav/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dav/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dav/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dav/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dav/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dav/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/de/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/de/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/de/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/de/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/de/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/de/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dje/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dje/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dje/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dje/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dje/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dje/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/doi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/doi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/doi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/doi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/doi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/doi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dsb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dsb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dsb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dsb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dsb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dsb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dua/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dua/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dua/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dua/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dua/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dua/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dyo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dyo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dyo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dyo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dyo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dyo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dz/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dz/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dz/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dz/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/dz/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/dz/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ebu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ebu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ebu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ebu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ebu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ebu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ee/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ee/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ee/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ee/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ee/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ee/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/el/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/el/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/el/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/el/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/el/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/el/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/en/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/en/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/en/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/en/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/en/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/en/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/eo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/eo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/eo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/eo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/eo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/eo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/es/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/es/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/es/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/es/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/es/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/es/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/et/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/et/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/et/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/et/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/et/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/et/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/eu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/eu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/eu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/eu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/eu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/eu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ewo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ewo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ewo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ewo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ewo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ewo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fa/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fa/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fa/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fa/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fa/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fa/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ff/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ff/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ff/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ff/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ff/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ff/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fil/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fil/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fil/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fil/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fil/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fil/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fr/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fr/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fr/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fr/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fr/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fr/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fur/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fur/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fur/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fur/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fur/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fur/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fy/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fy/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fy/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fy/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/fy/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/fy/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ga/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ga/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ga/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ga/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ga/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ga/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gd/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gd/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gd/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gd/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gd/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gd/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gl/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gl/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gl/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gl/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gl/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gl/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gsw/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gsw/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gsw/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gsw/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gsw/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gsw/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/guz/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/guz/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/guz/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/guz/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/guz/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/guz/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gv/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gv/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gv/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gv/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/gv/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/gv/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ha/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ha/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ha/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ha/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ha/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ha/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/haw/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/haw/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/haw/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/haw/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/haw/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/haw/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/he/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/he/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/he/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/he/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/he/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/he/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hil/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hil/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hr/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hr/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hr/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hr/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hr/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hr/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hsb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hsb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hsb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hsb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hsb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hsb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hy/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hy/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hy/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hy/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/hy/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/hy/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ia/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ia/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ia/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ia/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ia/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ia/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/id/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/id/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/id/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/id/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/id/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/id/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ig/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ig/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ig/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ig/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ig/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ig/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ii/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ii/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ii/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ii/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ii/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ii/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ilo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ilo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/io/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/io/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/is/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/is/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/is/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/is/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/is/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/is/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/it/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/it/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/it/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/it/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/it/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/it/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ja/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ja/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ja/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ja/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ja/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ja/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jbo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jbo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jgo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jgo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jgo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jgo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jgo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jgo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jmc/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jmc/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jmc/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jmc/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jmc/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jmc/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jv/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jv/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jv/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jv/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/jv/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/jv/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ka/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ka/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ka/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ka/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ka/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ka/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kab/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kab/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kab/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kab/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kab/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kab/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kam/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kam/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kam/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kam/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kam/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kam/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kcm/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kcm/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kde/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kde/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kde/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kde/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kde/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kde/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kea/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kea/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kea/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kea/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kea/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kea/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kgp/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kgp/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kgp/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kgp/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kgp/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kgp/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/khq/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/khq/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/khq/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/khq/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/khq/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/khq/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ki/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ki/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ki/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ki/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ki/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ki/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kk/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kk/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kk/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kk/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kk/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kk/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kkj/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kkj/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kkj/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kkj/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kkj/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kkj/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kl/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kl/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kl/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kl/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kl/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kl/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kln/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kln/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kln/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kln/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kln/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kln/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/km/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/km/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/km/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/km/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/km/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/km/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ko/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ko/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ko/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ko/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ko/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ko/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kok/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kok/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kok/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kok/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kok/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kok/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ks/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ks/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ks/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ks/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ks/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ks/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksf/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksf/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksf/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksf/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksf/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksf/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ksh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ksh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ku/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ku/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ku/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ku/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ku/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ku/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kw/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kw/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kw/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kw/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/kw/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/kw/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ky/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ky/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ky/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ky/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ky/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ky/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/la/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/la/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lag/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lag/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lag/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lag/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lag/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lag/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lah/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lah/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lkt/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lkt/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lkt/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lkt/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lkt/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lkt/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ln/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ln/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ln/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ln/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ln/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ln/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lrc/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lrc/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lrc/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lrc/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lrc/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lrc/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lt/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lt/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lt/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lt/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lt/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lt/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/luo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/luo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/luo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/luo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/luo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/luo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/luy/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/luy/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/luy/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/luy/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/luy/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/luy/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lv/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lv/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lv/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lv/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/lv/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/lv/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mai/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mai/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mai/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mai/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mai/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mai/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mas/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mas/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mas/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mas/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mas/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mas/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mer/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mer/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mer/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mer/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mer/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mer/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mfe/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mfe/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mfe/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mfe/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mfe/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mfe/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mgh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mgh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mgh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mgh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mgh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mgh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mgo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mgo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mgo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mgo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mgo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mgo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mk/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mk/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mk/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mk/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mk/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mk/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ml/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ml/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ml/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ml/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ml/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ml/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mni/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mni/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mni/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mni/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mni/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mni/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mr/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mr/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mr/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mr/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mr/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mr/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ms/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ms/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ms/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ms/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ms/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ms/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mt/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mt/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mt/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mt/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mt/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mt/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mua/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mua/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mua/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mua/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mua/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mua/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/my/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/my/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/my/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/my/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/my/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/my/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mzn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mzn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mzn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mzn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/mzn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/mzn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nah/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nah/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nan/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nan/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/naq/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/naq/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/naq/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/naq/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/naq/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/naq/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nb/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nb/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nb/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nb/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nb/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nb/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nd/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nd/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nd/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nd/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nd/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nd/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nds/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nds/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nds/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nds/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nds/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nds/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ne/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ne/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ne/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ne/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ne/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ne/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nl/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nl/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nl/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nl/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nl/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nl/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nmg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nmg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nmg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nmg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nmg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nmg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nnh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nnh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nnh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nnh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nnh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nnh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/no/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/no/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/no/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/no/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/no/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/no/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nus/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nus/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nus/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nus/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nus/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nus/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nv/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nv/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nyn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nyn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nyn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nyn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/nyn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/nyn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/om/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/om/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/om/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/om/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/om/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/om/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/or/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/or/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/or/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/or/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/or/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/or/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/os/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/os/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/os/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/os/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/os/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/os/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pa/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pa/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pa/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pa/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pa/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pa/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pcm/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pcm/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pcm/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pcm/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pcm/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pcm/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pl/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pl/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pl/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pl/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pl/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pl/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/prg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/prg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/prg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/prg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/prg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/prg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ps/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ps/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ps/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ps/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ps/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ps/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pt/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pt/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pt/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pt/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/pt/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/pt/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/qu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/qu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/qu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/qu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/qu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/qu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rm/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rm/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rm/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rm/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rm/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rm/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ro/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ro/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ro/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ro/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ro/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ro/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rof/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rof/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rof/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rof/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rof/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rof/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ru/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ru/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ru/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ru/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ru/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ru/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rup/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rup/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rw/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rw/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rw/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rw/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rw/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rw/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rwk/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rwk/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rwk/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rwk/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/rwk/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/rwk/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sa/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sa/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sa/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sa/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sa/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sa/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sah/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sah/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sah/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sah/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sah/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sah/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/saq/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/saq/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/saq/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/saq/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/saq/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/saq/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sat/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sat/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sat/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sat/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sat/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sat/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sbp/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sbp/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sbp/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sbp/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sbp/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sbp/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sc/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sc/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sc/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sc/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sc/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sc/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sd/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sd/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sd/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sd/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sd/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sd/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/se/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/se/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/se/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/se/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/se/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/se/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/seh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/seh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/seh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/seh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/seh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/seh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ses/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ses/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ses/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ses/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ses/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ses/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/shi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/shi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/shi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/shi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/shi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/shi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/si/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/si/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/si/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/si/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/si/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/si/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sk/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sk/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sk/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sk/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sk/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sk/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sl/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sl/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sl/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sl/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sl/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sl/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/smn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/smn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/smn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/smn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/smn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/smn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sn/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sn/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sn/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sn/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sn/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sn/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/so/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/so/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/so/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/so/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/so/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/so/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sq/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sq/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sq/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sq/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sq/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sq/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sr/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sr/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sr/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sr/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sr/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sr/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/su/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/su/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/su/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/su/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/su/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/su/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sv/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sv/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sv/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sv/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sv/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sv/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sw/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sw/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sw/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sw/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/sw/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/sw/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ta/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ta/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ta/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ta/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ta/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ta/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/te/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/te/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/te/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/te/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/te/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/te/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/teo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/teo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/teo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/teo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/teo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/teo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tg/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tg/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tg/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tg/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tg/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tg/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/th/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/th/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/th/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/th/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/th/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/th/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ti/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ti/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ti/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ti/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ti/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ti/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tk/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tk/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tk/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tk/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tk/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tk/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/to/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/to/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/to/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/to/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/to/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/to/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tpi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tpi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tr/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tr/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tr/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tr/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tr/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tr/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tt/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tt/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tt/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tt/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tt/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tt/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/twq/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/twq/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/twq/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/twq/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/twq/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/twq/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tzm/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tzm/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tzm/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tzm/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/tzm/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/tzm/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ug/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ug/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ug/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ug/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ug/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ug/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/uk/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/uk/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/uk/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/uk/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/uk/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/uk/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/und/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/und/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/und/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/und/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/und/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/und/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ur/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ur/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ur/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ur/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ur/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ur/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/uz/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/uz/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/uz/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/uz/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/uz/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/uz/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vai/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vai/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vai/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vai/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vai/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vai/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/ve/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/ve/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vun/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vun/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vun/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vun/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/vun/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/vun/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/wae/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/wae/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/wae/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/wae/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/wae/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/wae/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/wo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/wo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/wo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/wo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/wo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/wo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/xh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/xh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/xh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/xh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/xh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/xh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/xog/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/xog/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/xog/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/xog/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/xog/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/xog/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yav/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yav/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yav/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yav/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yav/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yav/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yi/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yi/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yi/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yi/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yi/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yi/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yo/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yo/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yo/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yo/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yo/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yo/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yrl/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yrl/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yrl/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yrl/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yrl/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yrl/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yue/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yue/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yue/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yue/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/yue/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/yue/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zgh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zgh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zgh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zgh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zgh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zgh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zh/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zh/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zh/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zh/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zh/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zh/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zsm/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zsm/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zu/name_to_language.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zu/name_to_language.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zu/name_to_script.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zu/name_to_script.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/trie/zu/name_to_territory.marisa` & `language_data-1.2.0.dev3/language_data/data/trie/zu/name_to_territory.marisa`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/data/wiktionary/codes-en.csv` & `language_data-1.2.0.dev3/language_data/data/wiktionary/codes-en.csv`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/language_lists.py` & `language_data-1.2.0.dev3/language_data/language_lists.py`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/name_data.py` & `language_data-1.2.0.dev3/language_data/name_data.py`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/names.py` & `language_data-1.2.0.dev3/language_data/names.py`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/population_data.py` & `language_data-1.2.0.dev3/language_data/population_data.py`

 * *Files identical despite different names*

### Comparing `language_data-1.1/language_data/registry_parser.py` & `language_data-1.2.0.dev3/language_data/registry_parser.py`

 * *Files identical despite different names*

### Comparing `language_data-1.1/PKG-INFO` & `language_data-1.2.0.dev3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
-Name: language-data
-Version: 1.1
+Name: language_data
+Version: 1.2.0.dev3
 Summary: Supplementary data about languages used by the langcodes module
-Home-page: https://github.com/rspeer/language_data
-License: MIT
-Author: Elia Robyn Speer
-Author-email: rspeer@arborelia.net
-Requires-Python: >=3.6
+Author-email: Elia Robyn Speer <rspeer@arborelia.net>
+Maintainer-email: Georg Krause <mail@georg-krause.net>
+Project-URL: Homepage, https://github.com/georgkrause/language_data
+Project-URL: Repository, https://github.com/georgkrause/language_data
+Project-URL: Issues, https://github.com/georgkrause/language_data/issues
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: marisa-trie (>=0.7.7,<0.8.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: marisa-trie>=0.7.7
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
 
 # language_data: a supplement to [langcodes][]
 
 [langcodes]: https://github.com/LuminosoInsight/langcodes
 
 This package is not meant to be used on its own. Please see [langcodes][] for documentation.
 
@@ -55,9 +60,8 @@
 
 `language_data` has a dependency on the `marisa-trie` package so that it can load a compact, efficient data structure for looking up language names.
 
 ## Installation
 
 `language_data` is usually installed as a dependency of `langcodes`, and doesn't make much sense without it. You can `pip install language_data` anyway if you want.
 
-To install the `language_data` package in editable mode, run `poetry install` in the package root. (This is the equivalent of `pip install -e .`, which currently doesn't work because pip does not yet fully support PEP 621.)
-
+To install the `language_data` package in editable mode, run `poetry install` in the package root. (This is the equivalent of `pip install -e .`, which will hopefully become compatible again soon via PEP 660.)
```

