# Comparing `tmp/socialgene-0.6.5.tar.gz` & `tmp/socialgene-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialgene-0.6.5.tar", last modified: Mon Apr  8 17:08:34 2024, max compression
+gzip compressed data, was "socialgene-0.6.6.tar", last modified: Mon Apr  8 17:14:01 2024, max compression
```

## Comparing `socialgene-0.6.5.tar` & `socialgene-0.6.6.tar`

### file list

```diff
@@ -1,175 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.293557 socialgene-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-08 17:08:25.000000 socialgene-0.6.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 17:08:34.293557 socialgene-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-08 17:08:25.000000 socialgene-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-08 17:08:25.000000 socialgene-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 17:08:34.293557 socialgene-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 17:08:25.000000 socialgene-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.273557 socialgene-0.6.5/socialgene/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.273557 socialgene-0.6.5/socialgene/addons/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.273557 socialgene-0.6.5/socialgene/addons/chebi/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chebi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chebi/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.273557 socialgene-0.6.5/socialgene/addons/chembl/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chembl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chembl/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.273557 socialgene-0.6.5/socialgene/addons/chemistry/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chemistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chemistry/cli_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/chemistry/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.273557 socialgene-0.6.5/socialgene/addons/classyfire/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/classyfire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/classyfire/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/classyfire/nr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/classyfire/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/gene_cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gene_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gene_cluster/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/gnps_library/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_library/nr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_library/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/gnps_networking/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_networking/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_networking/nr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/gnps_networking/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/mibig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/mibig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/mibig/link_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/mibig/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/npatlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npatlas/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npatlas/nr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npatlas/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/npclassifier/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npclassifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npclassifier/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/npmrd/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npmrd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/npmrd/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.277557 socialgene-0.6.5/socialgene/addons/publication/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/publication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/addons/publication/nr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/base/chem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/base/compare_protein.py
--rw-r--r--   0 runner    (1001) docker     (127)    37922 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/base/molbio.py
--rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/base/socialgene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/cli/external_mods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/external_mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/external_mods/gnps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/cli/neo4j/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/neo4j/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/neo4j/massage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/cli/nextflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/clean_hmms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/create_neo4j_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/export_neo4j_header_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/export_protein_loci_assembly_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/parameter_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/parse_ncbi_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/parse_ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/process_domtblout.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/cli/nextflow/socialgene_hmm_tsv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/clustermap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/clustermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/clustermap/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/common_parameters.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.281557 socialgene-0.6.5/socialgene/compare_gene_clusters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_gene_clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_gene_clusters/compare_gene_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/compare_proteins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_proteins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_proteins/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_proteins/diamond.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_proteins/hmm_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_proteins/hmmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/compare_proteins/mmseqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/data/biosample_attributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/dbmodifiers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/dbmodifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/dbmodifiers/massage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/dbmodifiers/massage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/dbmodifiers/massage/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/dbmodifiers/massage/massage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/hashing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/hashing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/hashing/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/hmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/hmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/hmm/hmmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/hmm/hmminfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/neo4j/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)    21961 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/neo4j_element.py
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/queries.cypher
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/neo4j/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/schema/graph_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/schema/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/schema/socialgene_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.285557 socialgene-0.6.5/socialgene/neo4j/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/search/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.289557 socialgene-0.6.5/socialgene/neo4j/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/utils/admin_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/neo4j/utils/ingest_from_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.289557 socialgene-0.6.5/socialgene/nextflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/nextflow/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/nextflow/relationships.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.289557 socialgene-0.6.5/socialgene/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/datasets_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/genbank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/hmmer_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/hmmmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/ncbi_feature_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/parsers/sequence_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.289557 socialgene-0.6.5/socialgene/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31054 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/search/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24639 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/search/hmmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.293557 socialgene-0.6.5/socialgene/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/chunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/get_ncbi_biosample_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/goterms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/lists_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/ncbi_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/nextflow_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/np_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/prep_ncbi_biosample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/run_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/simple_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/untargz.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 17:08:25.000000 socialgene-0.6.5/socialgene/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:08:34.293557 socialgene-0.6.5/socialgene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 17:08:34.000000 socialgene-0.6.5/socialgene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-08 17:08:34.000000 socialgene-0.6.5/socialgene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:08:34.000000 socialgene-0.6.5/socialgene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 17:08:34.000000 socialgene-0.6.5/socialgene.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 17:08:34.000000 socialgene-0.6.5/socialgene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:08:34.000000 socialgene-0.6.5/socialgene.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.166015 socialgene-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-08 17:13:47.000000 socialgene-0.6.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 17:14:01.166015 socialgene-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-08 17:13:47.000000 socialgene-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-08 17:13:47.000000 socialgene-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 17:14:01.166015 socialgene-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 17:13:47.000000 socialgene-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.146016 socialgene-0.6.6/socialgene/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.146016 socialgene-0.6.6/socialgene/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.146016 socialgene-0.6.6/socialgene/addons/chebi/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chebi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chebi/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.146016 socialgene-0.6.6/socialgene/addons/chembl/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chembl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chembl/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/chemistry/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chemistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chemistry/cli_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/chemistry/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/classyfire/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/classyfire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/classyfire/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/classyfire/nr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/classyfire/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/gene_cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gene_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gene_cluster/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/gnps_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_library/nr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_library/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/gnps_networking/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_networking/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_networking/nr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/gnps_networking/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/mibig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/mibig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/mibig/link_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/mibig/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/npatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npatlas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npatlas/nr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npatlas/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/npclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npclassifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npclassifier/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/npmrd/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npmrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/npmrd/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.150015 socialgene-0.6.6/socialgene/addons/publication/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/publication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/addons/publication/nr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/base/chem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/base/compare_protein.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37922 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/base/molbio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/base/socialgene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/cli/external_mods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/external_mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/external_mods/gnps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/cli/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/neo4j/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/neo4j/massage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/cli/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/clean_hmms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/create_neo4j_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/export_neo4j_header_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/export_protein_loci_assembly_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/parameter_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/parse_ncbi_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/parse_ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/process_domtblout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/nextflow/socialgene_hmm_tsv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/cli/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/search/gene_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/search/runalot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/cli/search/sea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.154015 socialgene-0.6.6/socialgene/clustermap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/clustermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/clustermap/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/common_parameters.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/compare_gene_clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_gene_clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_gene_clusters/compare_gene_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/compare_proteins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_proteins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_proteins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_proteins/diamond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_proteins/hmm_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_proteins/hmmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/compare_proteins/mmseqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/data/biosample_attributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/dbmodifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/dbmodifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/dbmodifiers/massage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/dbmodifiers/massage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/dbmodifiers/massage/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/dbmodifiers/massage/massage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/hashing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/hashing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/hashing/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/hmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/hmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/hmm/hmmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/hmm/hmminfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21961 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/neo4j_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/queries.cypher
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.158016 socialgene-0.6.6/socialgene/neo4j/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/schema/graph_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/schema/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/schema/socialgene_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.162016 socialgene-0.6.6/socialgene/neo4j/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/search/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.162016 socialgene-0.6.6/socialgene/neo4j/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/utils/admin_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/neo4j/utils/ingest_from_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.162016 socialgene-0.6.6/socialgene/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/nextflow/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/nextflow/relationships.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.162016 socialgene-0.6.6/socialgene/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/datasets_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/hmmer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/hmmmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/ncbi_feature_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/parsers/sequence_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.162016 socialgene-0.6.6/socialgene/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31054 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24639 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/search/hmmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.166015 socialgene-0.6.6/socialgene/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/chunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/get_ncbi_biosample_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/goterms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/lists_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/ncbi_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/nextflow_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/np_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/prep_ncbi_biosample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/run_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/simple_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/untargz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 17:13:47.000000 socialgene-0.6.6/socialgene/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:01.166015 socialgene-0.6.6/socialgene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 17:14:01.000000 socialgene-0.6.6/socialgene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-08 17:14:01.000000 socialgene-0.6.6/socialgene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:14:01.000000 socialgene-0.6.6/socialgene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 17:14:01.000000 socialgene-0.6.6/socialgene.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 17:14:01.000000 socialgene-0.6.6/socialgene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:14:01.000000 socialgene-0.6.6/socialgene.egg-info/top_level.txt
```

### Comparing `socialgene-0.6.5/LICENSE.md` & `socialgene-0.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/PKG-INFO` & `socialgene-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.6.5
+Version: 0.6.6
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `socialgene-0.6.5/README.md` & `socialgene-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/pyproject.toml` & `socialgene-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socialgene"
-version = "0.6.5"
+version = "0.6.6"
 description = "Creating and interacting with graph databases of protein domains and their genome coordinates"
 readme = "README.md"
 authors =  [
     {name = "Chase M. Clark", email = "chasingmicrobes@gmail.com"},
 ]
 keywords = []  #! TODO
 requires-python = ">=3.12"
```

### Comparing `socialgene-0.6.5/setup.cfg` & `socialgene-0.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/setup.py` & `socialgene-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/chemistry/cli_similarity.py` & `socialgene-0.6.6/socialgene/addons/chemistry/cli_similarity.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/chemistry/nr.py` & `socialgene-0.6.6/socialgene/addons/chemistry/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/classyfire/nr.py` & `socialgene-0.6.6/socialgene/addons/classyfire/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/classyfire/parse.py` & `socialgene-0.6.6/socialgene/addons/classyfire/parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/gene_cluster/nr.py` & `socialgene-0.6.6/socialgene/addons/gene_cluster/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/gnps_library/nr.py` & `socialgene-0.6.6/socialgene/addons/gnps_library/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/gnps_library/parse.py` & `socialgene-0.6.6/socialgene/addons/gnps_library/parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/gnps_networking/cli.py` & `socialgene-0.6.6/socialgene/addons/gnps_networking/cli.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/gnps_networking/nr.py` & `socialgene-0.6.6/socialgene/addons/gnps_networking/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/gnps_networking/parse.py` & `socialgene-0.6.6/socialgene/addons/gnps_networking/parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/mibig/link_cli.py` & `socialgene-0.6.6/socialgene/addons/mibig/link_cli.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/mibig/nr.py` & `socialgene-0.6.6/socialgene/addons/mibig/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/npatlas/cli.py` & `socialgene-0.6.6/socialgene/addons/npatlas/cli.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/npatlas/nr.py` & `socialgene-0.6.6/socialgene/addons/npatlas/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/npatlas/parse.py` & `socialgene-0.6.6/socialgene/addons/npatlas/parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/npclassifier/nr.py` & `socialgene-0.6.6/socialgene/addons/npclassifier/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/addons/publication/nr.py` & `socialgene-0.6.6/socialgene/addons/publication/nr.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/base/chem.py` & `socialgene-0.6.6/socialgene/base/chem.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/base/compare_protein.py` & `socialgene-0.6.6/socialgene/base/compare_protein.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/base/molbio.py` & `socialgene-0.6.6/socialgene/base/molbio.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/base/socialgene.py` & `socialgene-0.6.6/socialgene/base/socialgene.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/external_mods/gnps.py` & `socialgene-0.6.6/socialgene/cli/external_mods/gnps.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/neo4j/indices.py` & `socialgene-0.6.6/socialgene/cli/neo4j/indices.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/neo4j/massage.py` & `socialgene-0.6.6/socialgene/cli/neo4j/massage.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/clean_hmms.py` & `socialgene-0.6.6/socialgene/cli/nextflow/clean_hmms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/create_neo4j_db.py` & `socialgene-0.6.6/socialgene/cli/nextflow/create_neo4j_db.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/export_neo4j_header_files.py` & `socialgene-0.6.6/socialgene/cli/nextflow/export_neo4j_header_files.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/export_protein_loci_assembly_tables.py` & `socialgene-0.6.6/socialgene/cli/nextflow/export_protein_loci_assembly_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/parameter_export.py` & `socialgene-0.6.6/socialgene/cli/nextflow/parameter_export.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/parse_ncbi_feature_tables.py` & `socialgene-0.6.6/socialgene/cli/nextflow/parse_ncbi_feature_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/parse_ncbi_taxonomy.py` & `socialgene-0.6.6/socialgene/cli/nextflow/parse_ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/process_domtblout.py` & `socialgene-0.6.6/socialgene/cli/nextflow/process_domtblout.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/cli/nextflow/socialgene_hmm_tsv_parser.py` & `socialgene-0.6.6/socialgene/cli/nextflow/socialgene_hmm_tsv_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/clustermap/serialize.py` & `socialgene-0.6.6/socialgene/clustermap/serialize.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/common_parameters.env` & `socialgene-0.6.6/socialgene/common_parameters.env`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/compare_gene_clusters/compare_gene_clusters.py` & `socialgene-0.6.6/socialgene/compare_gene_clusters/compare_gene_clusters.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/compare_proteins/base.py` & `socialgene-0.6.6/socialgene/compare_proteins/base.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/compare_proteins/diamond.py` & `socialgene-0.6.6/socialgene/compare_proteins/diamond.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/compare_proteins/hmm_scoring.py` & `socialgene-0.6.6/socialgene/compare_proteins/hmm_scoring.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/compare_proteins/hmmer.py` & `socialgene-0.6.6/socialgene/compare_proteins/hmmer.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/compare_proteins/mmseqs.py` & `socialgene-0.6.6/socialgene/compare_proteins/mmseqs.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/config.py` & `socialgene-0.6.6/socialgene/config.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/data/biosample_attributes` & `socialgene-0.6.6/socialgene/data/biosample_attributes`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/dbmodifiers/massage/indices.py` & `socialgene-0.6.6/socialgene/dbmodifiers/massage/indices.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/dbmodifiers/massage/massage.py` & `socialgene-0.6.6/socialgene/dbmodifiers/massage/massage.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/hashing/hashing.py` & `socialgene-0.6.6/socialgene/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/hmm/hmmer.py` & `socialgene-0.6.6/socialgene/hmm/hmmer.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/hmm/hmminfo.py` & `socialgene-0.6.6/socialgene/hmm/hmminfo.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/neo4j.py` & `socialgene-0.6.6/socialgene/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/neo4j_element.py` & `socialgene-0.6.6/socialgene/neo4j/neo4j_element.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/queries.cypher` & `socialgene-0.6.6/socialgene/neo4j/queries.cypher`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/schema/graph_schema.py` & `socialgene-0.6.6/socialgene/neo4j/schema/graph_schema.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/schema/modules.py` & `socialgene-0.6.6/socialgene/neo4j/schema/modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/schema/socialgene_modules.py` & `socialgene-0.6.6/socialgene/neo4j/schema/socialgene_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/search/basic.py` & `socialgene-0.6.6/socialgene/neo4j/search/basic.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/utils/admin_import.py` & `socialgene-0.6.6/socialgene/neo4j/utils/admin_import.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/neo4j/utils/ingest_from_neo4j.py` & `socialgene-0.6.6/socialgene/neo4j/utils/ingest_from_neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/nextflow/nodes.py` & `socialgene-0.6.6/socialgene/nextflow/nodes.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/nextflow/relationships.py` & `socialgene-0.6.6/socialgene/nextflow/relationships.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/datasets_parse.py` & `socialgene-0.6.6/socialgene/parsers/datasets_parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/fasta.py` & `socialgene-0.6.6/socialgene/parsers/fasta.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/genbank.py` & `socialgene-0.6.6/socialgene/parsers/genbank.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/hmmer_parser.py` & `socialgene-0.6.6/socialgene/parsers/hmmer_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/hmmmodel.py` & `socialgene-0.6.6/socialgene/parsers/hmmmodel.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/ncbi_feature_table.py` & `socialgene-0.6.6/socialgene/parsers/ncbi_feature_table.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/ncbi_taxonomy.py` & `socialgene-0.6.6/socialgene/parsers/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/parsers/sequence_parser.py` & `socialgene-0.6.6/socialgene/parsers/sequence_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/search/base.py` & `socialgene-0.6.6/socialgene/search/base.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/search/hmmer.py` & `socialgene-0.6.6/socialgene/search/hmmer.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/chunker.py` & `socialgene-0.6.6/socialgene/utils/chunker.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/download.py` & `socialgene-0.6.6/socialgene/utils/download.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/file_handling.py` & `socialgene-0.6.6/socialgene/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/get_ncbi_biosample_attributes.py` & `socialgene-0.6.6/socialgene/utils/get_ncbi_biosample_attributes.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/goterms.py` & `socialgene-0.6.6/socialgene/utils/goterms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/lists_to_markdown.py` & `socialgene-0.6.6/socialgene/utils/lists_to_markdown.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/logging.py` & `socialgene-0.6.6/socialgene/utils/logging.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/ncbi_ftp.py` & `socialgene-0.6.6/socialgene/utils/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/nextflow_test_utils.py` & `socialgene-0.6.6/socialgene/utils/nextflow_test_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/prep_ncbi_biosample_data.py` & `socialgene-0.6.6/socialgene/utils/prep_ncbi_biosample_data.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/protein_sqlite.py` & `socialgene-0.6.6/socialgene/utils/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/run_subprocess.py` & `socialgene-0.6.6/socialgene/utils/run_subprocess.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene/utils/untargz.py` & `socialgene-0.6.6/socialgene/utils/untargz.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.6.5/socialgene.egg-info/PKG-INFO` & `socialgene-0.6.6/socialgene.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.6.5
+Version: 0.6.6
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `socialgene-0.6.5/socialgene.egg-info/SOURCES.txt` & `socialgene-0.6.6/socialgene.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,18 @@
 socialgene/cli/nextflow/export_neo4j_header_files.py
 socialgene/cli/nextflow/export_protein_loci_assembly_tables.py
 socialgene/cli/nextflow/parameter_export.py
 socialgene/cli/nextflow/parse_ncbi_feature_tables.py
 socialgene/cli/nextflow/parse_ncbi_taxonomy.py
 socialgene/cli/nextflow/process_domtblout.py
 socialgene/cli/nextflow/socialgene_hmm_tsv_parser.py
+socialgene/cli/search/__init__.py
+socialgene/cli/search/gene_cluster.py
+socialgene/cli/search/runalot.py
+socialgene/cli/search/sea.py
 socialgene/clustermap/__init__.py
 socialgene/clustermap/serialize.py
 socialgene/compare_gene_clusters/__init__.py
 socialgene/compare_gene_clusters/compare_gene_clusters.py
 socialgene/compare_proteins/__init__.py
 socialgene/compare_proteins/base.py
 socialgene/compare_proteins/diamond.py
```

### Comparing `socialgene-0.6.5/socialgene.egg-info/entry_points.txt` & `socialgene-0.6.6/socialgene.egg-info/entry_points.txt`

 * *Files identical despite different names*

