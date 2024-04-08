# Comparing `tmp/CCMetagen-1.4.2.tar.gz` & `tmp/CCMetagen-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/scratch/projects/punim1293/vini/software/CCMetagen/dist/tmpw_rh19b6/CCMetagen-1.4.2.tar", last modified: Mon Dec 11 08:40:43 2023, max compression
+gzip compressed data, was "CCMetagen-1.5.0.tar", last modified: Mon Apr  8 05:32:04 2024, max compression
```

## Comparing `CCMetagen-1.4.2.tar` & `CCMetagen-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-sr-x   0 viniws   (13695) punim1293 (11358)        0 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/
--rw-r--r--   0 viniws   (13695) punim1293 (11358)       38 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/setup.py
--rw-r--r--   0 viniws   (13695) punim1293 (11358)    22507 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/PKG-INFO
--rw-r--r--   0 viniws   (13695) punim1293 (11358)    35147 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/LICENSE
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)     2499 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/CCMetagen_extract_seqs.py
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)     5035 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/CCMetagen_merge.py
--rw-r--r--   0 viniws   (13695) punim1293 (11358)     1105 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/setup.cfg
--rw-r--r--   0 viniws   (13695) punim1293 (11358)    21535 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/README.md
-drwxr-sr-x   0 viniws   (13695) punim1293 (11358)        0 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/ccmetagen/
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)     1762 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/ccmetagen/cTaxInfo.py
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)     5812 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/ccmetagen/fParseKMA.py
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)        0 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/ccmetagen/__init__.py
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)     2649 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/ccmetagen/fNCBItax.py
-drwxr-sr-x   0 viniws   (13695) punim1293 (11358)        0 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/CCMetagen.egg-info/
--rw-r--r--   0 viniws   (13695) punim1293 (11358)      347 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/CCMetagen.egg-info/SOURCES.txt
--rw-r--r--   0 viniws   (13695) punim1293 (11358)    22507 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/CCMetagen.egg-info/PKG-INFO
--rw-r--r--   0 viniws   (13695) punim1293 (11358)        1 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/CCMetagen.egg-info/dependency_links.txt
--rw-r--r--   0 viniws   (13695) punim1293 (11358)       10 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/CCMetagen.egg-info/top_level.txt
--rw-r--r--   0 viniws   (13695) punim1293 (11358)       12 2023-12-11 08:40:43.000000 CCMetagen-1.4.2/CCMetagen.egg-info/requires.txt
--rwxr-xr-x   0 viniws   (13695) punim1293 (11358)    15394 2023-12-11 08:21:21.000000 CCMetagen-1.4.2/CCMetagen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:32:04.788916 CCMetagen-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/AUTHORS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:32:04.788916 CCMetagen-1.5.0/CCMetagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-08 05:32:04.000000 CCMetagen-1.5.0/CCMetagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 05:32:04.000000 CCMetagen-1.5.0/CCMetagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:32:04.000000 CCMetagen-1.5.0/CCMetagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 05:32:04.000000 CCMetagen-1.5.0/CCMetagen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 05:32:04.000000 CCMetagen-1.5.0/CCMetagen.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18681 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/CCMetagen.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2580 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/CCMetagen_extract_seqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5058 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/CCMetagen_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-08 05:32:04.788916 CCMetagen-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20731 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:32:04.788916 CCMetagen-1.5.0/ccmetagen/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/ccmetagen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1803 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/ccmetagen/cTaxInfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1338 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/ccmetagen/fNCBItax.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4858 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/ccmetagen/fParseKMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 05:32:04.788916 CCMetagen-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:32:04.788916 CCMetagen-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 05:32:00.000000 CCMetagen-1.5.0/tests/test_ccmetagen.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `CCMetagen-1.4.2/PKG-INFO` & `CCMetagen-1.5.0/CCMetagen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,124 +1,100 @@
 Metadata-Version: 2.1
 Name: CCMetagen
-Version: 1.4.2
+Version: 1.5.0
 Summary: Microbiome classification pipeline
 Home-page: https://github.com/vrmarcelino/CCMetagen.git
 Author: Vanessa R. Marcelino Jan P. Buchmann Andreas Sjödin Philip T.L.C. Clausen
 Author-email: vrmarcelino@gmail.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/vrmarcelino/CCMetagen.git
 Project-URL: Preprint, https://www.biorxiv.org/content/10.1101/641332v2
 Keywords: bioinformatics taxonomy metagenomic classifier KMA
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: pandas
+Requires-Dist: ete3
 
 # CCMetagen
 
 CCMetagen processes sequence alignments produced with [KMA](https://bitbucket.org/genomicepidemiology/kma), which implements the ConClave sorting scheme to achieve highly accurate read mappings. The pipeline is fast enough to use the whole NCBI nt collection as reference, facilitating the inclusion of understudied organisms, such as microbial eukaryotes, in metagenome surveys. CCMetagen produces ranked taxonomic results in user-friendly formats that are ready for publication or downstream statistical analyses.
 
 If you this tool, please cite CCMetagen and KMA:
 
   * [Marcelino VR, Clausen PT, Buchman J, Wille M, Iredell JR, Meyer W, Lund O, Sorrell T, Holmes EC. 2019. CCMetagen: comprehensive and accurate identification of eukaryotes and prokaryotes in metagenomic data. Genome Biology. 2020 Dec;21(1):1-5.](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02014-2)
 
   * [Clausen PT, Aarestrup FM, Lund O. 2018. Rapid and precise alignment of raw reads against redundant databases with KMA. BMC bioinformatics. 2018 Dec;19(1):307.](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-018-2336-6)
 
-Besides the guidelines below, we also provide a tutorial to reproduce our metagenome clasisfication analyses of the microbiome of wild birds [here](https://github.com/vrmarcelino/CCMetagen/tree/master/tutorial).
+Besides the guidelines below, we also provide a tutorial to reproduce our metagenome clasisfication analyses of the microbiome of wild birds [here](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/tutorial).
 
 The guidelines below will guide you in using the command-line version of the CCMetagen pipeline.
 
 CCMetagen is also available as a web service at https://cge.food.dtu.dk/services/CCMetagen/.
 Note that we recommend using this command-line version to analyze data exceeding 1.5Gb.
 
-## Requirements and Installation
 
-Make sure you have the dependencies below installed and accessible in your $PATH.
-The guidelines below are for Unix systems.
+## Installation
 
-  * If you do not have it already, download and install [Python 3.6](https://www.python.org/downloads/)
-CCMetagen requires the Python modules [pandas (>0.23)](https://pandas.pydata.org/) and [ETE3](http://etetoolkit.org/).
-The easiest way to install these modules is via conda or pip:
+We recommend installing CCMetagen through [conda](https://docs.conda.io/en/latest/). This will install CCMetagen along with all of its required dependencies.
 
-`conda install pandas`
+After installing conda, you can create a new environment with CCMetagen through the following command:
 
-  * You need a C-compiler and zlib development files to install KMA:
-
-`sudo apt-get install libz-dev`
-
-  * Download and install [KMA](https://bitbucket.org/genomicepidemiology/kma):
-```
-git clone https://bitbucket.org/genomicepidemiology/kma.git
-cd kma && make
-```
-**Note - a new version of KMA - v1.3.0 – has been released, featuring higher speed and precision. We recommend that you update KMA to v.1.3.0**
-
-
-  * [Krona](https://github.com/marbl/Krona) is required for graphs. To install Krona it in the local folder:
 ```
-wget https://github.com/marbl/Krona/releases/download/v2.7/KronaTools-2.7.tar
-tar xvf KronaTools-2.7.tar 
-cd  KronaTools-2.7
-./install.pl --prefix . 
+conda create -n ccmetagen ccmetagen -c bioconda -c conda-forge
 ```
 
-  * Then download CCMetagen and add it to your path. You have two options:
+You can then activate your environment with:
 
-**Install CCMetagen via git:**
 ```
-git clone https://github.com/vrmarcelino/CCMetagen
+conda activate ccmetagen
 ```
-This will download CCMetagen and the tutorial files.
-You can also just download the python files from this github directory (CCMetagen.py, CCMetagen_merge.py) and the ones in the ccmetagen folder if you rather avoid downloading all other files.
 
-Then add the CCMetagen python scripts to the path, temporarily or permanently. For example:
-`PATH=$PATH<your_folder>/CCMetagen`
+The `-n ccmetagen` flag will name the environment as `ccmetagen`, but you can choose any different name that you'd like. The `ccmetagen` after that specifies that you'd like the CCMetagen package installed into that environment.
+Finally, the `-c bioconda -c conda-forge` specifies that you'd like to use the Bioconda and Conda-Forge channels, which host CCMetagen and its dependencies.
 
-To update CCMetagen, go to the CCMetagen folder and type: `git pull`
-
-**Or install CCMetagen via pip:**
-```
-pip install CCMetagen
-```
-This will automatically install the necessary python packages (pandas and ete3), so you can skip that step if you use pip.
+You can also install CCMetagen from source, or using pip, the Python package manager. For that, follow the installation instructions in the deprecated README file in the [docs](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/old_repository_README.md).
 
+Check your CCMetagen installation by running `CCMetagen.py --version` on your command-line.
 
 
 ## Databases
 
-**Option 1** Download the indexed (ready-to-go) nt or RefSeq database [here](http://dx.doi.org/10.25910/5cc7cd40fca8e).
-Download the ncbi_nt_kma.zip file (96GB zipped file, 165GB uncompressed) or the RefSeq_bf.zip (90GB zipped file)
+After installing CCMetagen, you will need a reference database to perform taxonomic classification. There are two ways to obtain this:
+
+**Option 1** Download the indexed (ready-to-go) nt from [here](https://melbourne.figshare.com/projects/CCMetagen_databases/195755).
+Download the ncbi_nt_kma file (103GB zipped file) or the RefSeq_bf.zip (90GB zipped file)
 Unzip the database, e.g.: `unzip ncbi_nt_kma`.
-The nt database contains the whole in NCBI nucleotide collection (of of Jan 2018), and therefore is suitable to identify a range of microorganisms, including prokaryotes and eukaryotes.
-The RefSeq_bf database contains complete reference bacterial and fungal genomes, suitable for better known habitats such as the human gut or when trying to detect well known species.
+The nt database contains the whole in NCBI nucleotide collection (from 2019, updated database to be released soon!), and therefore is suitable to identify a range of microorganisms, including prokaryotes and eukaryotes.
 
-**Option 2** We have indexed a more recent version of the ncbi nucleotide collection (June 2019) that does not contain environemntal or artificial sequences. The file ncbi_nt_no_env_11jun2019.zip can be found [here](http://dx.doi.org/10.25910/5cc7cd40fca8e) and contains all ncbi nt entries excluding the descendants of environmental eukaryotes (taxid 61964), environmental prokaryotes (48479), unclassified sequences (12908) and artificial sequences (28384).
+There are two versions of the nt database, the one previously mentioned, and another one that does not contain environemntal or artificial sequences. The file ncbi_nt_no_env_11jun2019.zip contains all ncbi nt entries excluding the descendants of environmental eukaryotes (taxid 61964), environmental prokaryotes (48479), unclassified sequences (12908) and artificial sequences (28384).
 
-**Option 3:** Build your own reference database (recommended!)
+**Option 2:** Build your own reference database (recommended!)
 Follow the instructions in the [KMA website](https://bitbucket.org/genomicepidemiology/kma) to index the database.
 It is important that taxids are incorporated in sequence headers for processing with CCMetagen. Sequence headers should look like 
 `>1234|sequence_description`, where 1234 is the taxid. 
-We provide scripts to rename sequences in the nt database [here](https://github.com/vrmarcelino/CCMetagen/tree/master/benchmarking/rename_nt).
+We provide scripts to rename sequences in the nt database [here](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/benchmarking/rename_nt).
 
 If you want to use the RefSeq database, the format is similar to the one required for Kraken. The [Opiniomics blog](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/) describes how to download sequences in an adequate format. Note that you still need to build the index with KMA: `kma_index -i refseq.fna -o refseq_indexed -NI -Sparse -` or `kma_index -i refseq.fna -o refseq_indexed -NI -Sparse TG` for faster analysis.
 
 
 ## Quick Start
 
   * First map sequence reads (or contigs) to the database with **KMA**.
 
 For paired-end files:
+
 ```
 kma -ipe $SAMPLE_R1 $SAMPLE_R2 -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and -apm f
 ```
 
 For single-end files:
 ```
 kma -i $SAMPLE -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and
@@ -127,40 +103,46 @@
 If you want to calculate abundance in reads per million (RPM) or in number of reads (fragments), or if you want to calculate the proportion of mapped reads, add the flag -ef (extended features):
 ```
 kma -ipe $SAMPLE_R1 $SAMPLE_R2 -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and -apm f -ef
 ```
 
 Where:
 
-$db is the path to the reference database
-$th is the number of threads
-$SAMPLE_R1 is the path to the mate1 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
-$SAMPLE_R2 is the path to the mate2 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
-$SAMPLE is the path to a single-end metagenome/metatranscriptome file (reads or contigs)
+- `$db` is the path to the reference database
+- `$th` is the number of threads
+- `$SAMPLE_R1` is the path to the mate1 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
+- `$SAMPLE_R2` is the path to the mate2 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
+- `$SAMPLE` is the path to a single-end metagenome/metatranscriptome file (reads or contigs)
 
+Then run `CCMetagen.py`:
 
-  * Then run **CCMetagen**:
 ```
 CCMetagen.py -i $sample_out_kma.res -o results
 ```
+
 Where $sample_out_kma.res is alignment results produced by KMA.
 
 Note that if you are running CCMetagen from the local folder (instead of adding it to your path), you may need to add 'python' before CCMetagen: `python CCMetagen.py -i $sample_out_kma.res -o results`
 
 Done! This will make an additional quality filter and output a text file with ranked taxonomic classifications and a krona graph file for interactive visualization.
 
-An example of the CCMetagen output can be found [here (.csv file)](https://github.com/vrmarcelino/CCMetagen/blob/master/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.csv) and [here (.html file)](https://htmlpreview.github.io/?https://github.com/vrmarcelino/CCMetagen/blob/master/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.html).
+An example of the CCMetagen output can be found [here (.csv file)](https://github.com/vrmarcelino/CCMetagen/blob/master/docs/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.csv) and [here (.html file)](https://htmlpreview.github.io/?https://github.com/vrmarcelino/CCMetagen/blob/master/docs/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.html).
 
-<img src=tutorial/figs_tutorial/krona_photo.png width="500" height="419.64">
+<img src=docs/tutorial/figs_tutorial/krona_photo.png width="500" height="419.64">
 
 In the .csv file, you will find the depth (abundance) of each match.
 
 ## Abundance units
 
-**Depth can be estimated in four ways:** by counting the number of nucleotides matching the reference sequence (use flag --depth_unit nc), by applying an additional correction for template length (default in KMA and CCMetagen), by calculating depth in Reads Per Million (RPM, use flag --depth_unit rpm), or by counting the number of fragments (i.e. number of PE reads matching to teh reference sequence, use flag --depth_unit fr). If you want RPM or fragment units, you will need to suply the .mapstats file generated with KMA (which you get when running kma with the flag '-ef').
+**Depth can be estimated in four ways:** 
+
+1. By applying an additional correction for template length (default in KMA and CCMetagen);
+2. By counting the number of nucleotides matching the reference sequence (use flag --depth_unit nc);
+3. By calculating depth in Reads Per Million (RPM, use flag --depth_unit rpm); or
+4. By counting the number of fragments (i.e. number of PE reads matching to teh reference sequence, use flag --depth_unit fr). If you want RPM or fragment units, you will need to suply the .mapstats file generated with KMA (which you get when running kma with the flag '-ef').
 
 
 ## Balancing sensitivity and specificity
 
 You can **adjust the stringency of the taxonomic assignments** by adjusting the minimum coverage (--coverage), the minimum abundance (--depth), and the minimum level of sequence similarity (--query_identity). Coverage is the percentage of bases in the reference sequence that is covered by the consensus sequence (your query), it can be over 100% when the consensus sequence is larger than the reference (due to insertions for example). You can also adjust the KMA settings to facilitate the identification of more distant-related taxa (see below)
 
 If you change the default depth unit, we recommend adjusting the minimum abundance (--depth) to remove taxa found in low abundance accordingly. For example, you can use -d 200 (200 nucleotides) when using --depth_unit nc, which is similar to -d 0.2 when using the default '--depth_unit kma' option. If you choose to calculate abundances in RPM, you may want to adjust the minimum abundance according to your sequence depth.
@@ -190,15 +172,15 @@
 ```
 
   * **To get the abundance of each taxon, and/or summarize results for multiple samples, use CCMetagen_merge**:
 ```
 CCMetagen_merge.py -i $CCMetagen_out
 ```
 
-Where $CCMetagen_out is the folder containing the CCMetagen taxonomic classifications.
+Where `$CCMetagen_out` is the folder containing the CCMetagen taxonomic classifications.
 The results must be in .csv format (default or '--mode text' output of CCMetagen), and these files **must end in ".ccm.csv"**.
 
 The flag '-t' define the taxonomic level to merge the results. The default is species-level.
 
 You can also filter out specific taxa, at any taxonomic level:
 
 Use flag -kr to keep (k) or remove (r) taxa.
@@ -233,24 +215,24 @@
 
 This script will produce a fasta file containing all reads assigned to a taxon of interest. 
 Ex: Generate a fasta file containing all sequences that mapped to the genus Eschericha:
 ```
 CCMetagen_extract_seqs.py -iccm $CCMetagen_out -ifrag $sample_out_kma.frag -l Genus -t Eschericha
 ```
 
-Where $CCMetagen_out is the .csv file generated with CCMetagen and $sample_out_kma.frag is the .frag file generated with KMA. The frag file needs to be decompressed: `gunzip *.frag.gz`
+Where `$CCMetagen_out` is the .csv file generated with CCMetagen and `$sample_out_kma.frag` is the .frag file generated with KMA. The frag file needs to be decompressed: `gunzip *.frag.gz`
 
 For species-level filtering (where there is a space in taxon names), use quotation marks.
 Ex: Generate a fasta file containing all sequences that mapped to _E. coli_:
 ```
 CCMetagen_extract_seqs.py -iccm $CCMetagen_out -ifrag $sample_out_kma.frag -l Species -t "Escherichia coli"
 ```
 
 
-**Check out our [tutorial](https://github.com/vrmarcelino/CCMetagen/tree/master/tutorial) for an applied example of the CCMetagen pipeline.**
+**Check out our [tutorial](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/tutorial) for an applied example of the CCMetagen pipeline.**
 
 
 
 ## FAQs
 
 * Error taxid not found.
   You probably need to update your local ETE3 database, which contains the taxids and lineage information:
@@ -360,9 +342,7 @@
                         applied
   -off TURN_OFF_SIM_THRESHOLDS, --turn_off_sim_thresholds TURN_OFF_SIM_THRESHOLDS
                         Turns simularity-based filtering off. Options = y or
                         n. Default = n
   --version             show program's version number and exit
  ```
 
-
-
```

### Comparing `CCMetagen-1.4.2/LICENSE` & `CCMetagen-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CCMetagen-1.4.2/CCMetagen_merge.py` & `CCMetagen-1.5.0/CCMetagen_merge.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+
 """
 CCMetagen_merge.py
 
 Merge the abundance results of CCMetagen for several samples into a single table.
 The results must be in .csv format (default CCMetagen or ---mode text).
 The files must end in ".ccm.csv".
 
@@ -11,143 +12,181 @@
 USAGE example 1: Merge table at family level:
 CCMetagen_merge.py -i CCMetagen_folder -t Family
 
 USAGE example 2: Merge table by species (default) and keep only Cryptococcus and Candida:
 CCMetagen_merge.py -i CCMetagen_folder -kr k -l Genus -tlist Candida,Cryptococcus
 
 @ V.R.Marcelino
-Created on Tue Dec 18 10:00:48 2018
+Created on Tue Dec 18 10:00:48 2018.
 """
 
 import sys
-import pandas as pd 
+import pandas as pd
 from argparse import ArgumentParser
 import os
 
 
 parser = ArgumentParser()
-parser.add_argument('-i', '--input_fp', help="""Path to the folder containing CCMetagen text results.
+parser.add_argument(
+    "-i",
+    "--input_fp",
+    help="""Path to the folder containing CCMetagen text results.
                     Note that files must end with ".csv"
-                    and the folder should not contain other .csv files""", required=True)
-parser.add_argument('-t', '--tax_level', default = 'Species',
-                    help="""Taxonomic level to merge the results. Options:
+                    and the folder should not contain other .csv files""",
+    required=True,
+)
+parser.add_argument(
+    "-t",
+    "--tax_level",
+    default="Species",
+    help="""Taxonomic level to merge the results. Options:
                     Closest_match (includes different genes for the same species),
                     Species (Default), Genus, Family, Order, Class, Phylum, Kingdom and Superkingdom
-                    """, required=False)
-parser.add_argument('-o', '--output_fp', default = 'merged_samples', 
-                    help='Path to the output file. Default = merged_samples', required=False)
+                    """,
+    required=False,
+)
+parser.add_argument(
+    "-o",
+    "--output_fp",
+    default="merged_samples",
+    help="Path to the output file. Default = merged_samples",
+    required=False,
+)
 
 # arguments to filter by taxonomy:
-parser.add_argument('-kr', '--keep_or_remove', default = 'n', 
-                    help='keep or remove taxa. Options = k (keep), r (remove) and n (none, default)', required=False)
-
-parser.add_argument('-l', '--filtering_tax_level', default = 'none', 
-                    help='level to perform taxonomic filtering, default = none', required=False)
-
-parser.add_argument('-tlist', '--taxa_list', default = [], type=str, 
-                    help='list taxon names (comma-separated) that you want to keep or exclude', required=False)
+parser.add_argument(
+    "-kr",
+    "--keep_or_remove",
+    default="n",
+    help="keep or remove taxa. Options = k (keep), r (remove) and n (none, default)",
+    required=False,
+)
+
+parser.add_argument(
+    "-l",
+    "--filtering_tax_level",
+    default="none",
+    help="level to perform taxonomic filtering, default = none",
+    required=False,
+)
+
+parser.add_argument(
+    "-tlist",
+    "--taxa_list",
+    default=[],
+    type=str,
+    help="list taxon names (comma-separated) that you want to keep or exclude",
+    required=False,
+)
 
 args = parser.parse_args()
 in_folder = args.input_fp
 tax_level = args.tax_level
 output = args.output_fp
 kr = args.keep_or_remove
 
 
 # debugging:
-#in_folder = "/Users/vmar0011/Documents/Programs_dev/03_CCM_nt"
-#tax_level = "Species"
-#output = "merged_samples_depth_species_no_ecoli"
-#kr = "r" # k for keep, r for remove, and n for none
-#level = "Species"
-#taxa = ["Escherichia coli"]
+# in_folder = "/Users/vmar0011/Documents/Programs_dev/03_CCM_nt"
+# tax_level = "Species"
+# output = "merged_samples_depth_species_no_ecoli"
+# kr = "r" # k for keep, r for remove, and n for none
+# level = "Species"
+# taxa = ["Escherichia coli"]
 
 
 # Set the taxonomic levels to retain info:
-l = ['Superkingdom','Kingdom','Phylum','Class','Order','Family','Genus','Species','Closest_match']
+l = [
+    "Superkingdom",
+    "Kingdom",
+    "Phylum",
+    "Class",
+    "Order",
+    "Family",
+    "Genus",
+    "Species",
+    "Closest_match",
+]
 
 f4agg = {}
 
-f4agg['Depth']= 'sum'
+f4agg["Depth"] = "sum"
 for i in l:
     if i == tax_level:
-        f4agg[i] = 'first'
+        f4agg[i] = "first"
         break
     else:
-        f4agg[i] = 'first'
-    
+        f4agg[i] = "first"
+
 # list of wanted taxa (no depth):
 wanted_taxa = list(f4agg.keys())
-wanted_taxa.remove('Depth')
+wanted_taxa.remove("Depth")
 
 # create new dataframe:
 all_samples = pd.DataFrame()
 
 
 # read input files and merge results
 for file in os.listdir(in_folder):
     if file.endswith(".ccm.csv"):
-        
         sample_name = file.split(".res.ccm.csv")[0]
         result_fp = os.path.join(in_folder, file)
 
-        df = pd.read_csv(result_fp, sep=',', index_col=0)
+        df = pd.read_csv(result_fp, sep=",", index_col=0)
 
-        # this is needed because groupby excludes rows with NAs 
+        # this is needed because groupby excludes rows with NAs
         df = df.fillna("NA")
-        
+
         # keep or remove taxa:
         if kr == "k":
             level = args.filtering_tax_level
             taxa = args.taxa_list.split(",")
-            filt_df_str = "df[df['{}'].isin({})]".format(level,taxa)
+            filt_df_str = "df[df['{}'].isin({})]".format(level, taxa)
             df = eval(filt_df_str)
-            
+
         elif kr == "r":
             level = args.filtering_tax_level
             taxa = args.taxa_list.split(",")
-            filt_df_str = "df[~df['{}'].isin({})]".format(level,taxa)
+            filt_df_str = "df[~df['{}'].isin({})]".format(level, taxa)
             df = eval(filt_df_str)
         elif kr == "n":
-            pass        
+            pass
         else:
-            print ("kr must be k (keep), r (remove) or n (none).")
+            print("kr must be k (keep), r (remove) or n (none).")
             sys.exit("Try again.")
- 
+
         # if tax_level = closest_match, we need an extra column:
-        
-        if tax_level == 'Closest_match':
-            df['Closest_match'] = df.index
-            df.index.name = None # This is needed in modern versions of Pandas (1.0.1)
+
+        if tax_level == "Closest_match":
+            df["Closest_match"] = df.index
+            df.index.name = None  # This is needed in modern versions of Pandas (1.0.1)
 
         depth_by_tax = df.groupby(by=wanted_taxa).agg(f4agg)
-        depth_by_tax.rename(columns={'Depth':sample_name}, inplace=True)
+        depth_by_tax.rename(columns={"Depth": sample_name}, inplace=True)
 
         all_samples = pd.concat([all_samples, depth_by_tax], sort=True, axis=1)
-    
 
-# Group taxon ranks 
-all_samples = all_samples.groupby(by=all_samples.columns, axis = 1).first()
+
+# Group taxon ranks
+all_samples = all_samples.groupby(by=all_samples.columns, axis=1).first()
 
 # add taxon info at the end of the table:
 tax_cols_l = list(f4agg.keys())
-tax_cols_l.remove('Depth')
+tax_cols_l.remove("Depth")
 
 tax_cols = all_samples[tax_cols_l]
 sample_cols = all_samples.drop(columns=tax_cols_l)
 
-all_samples = pd.merge(sample_cols,tax_cols,left_index=True,right_index=True)
+all_samples = pd.merge(sample_cols, tax_cols, left_index=True, right_index=True)
 
 # Fill NaN with zeros:
 all_samples = all_samples.fillna(0)
 
 # Remove the artificially added NAs:
-all_samples = all_samples.replace(["NA"], value = "")
+all_samples = all_samples.replace(["NA"], value="")
 
 
 ### Save
 out = output + ".csv"
 pd.DataFrame.to_csv(all_samples, out, index=False)
 
-print ("Done. Abundance estimates for all samples saved as %s" %(out))
-
-
+print("Done. Abundance estimates for all samples saved as %s" % (out))
```

### Comparing `CCMetagen-1.4.2/setup.cfg` & `CCMetagen-1.5.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [metadata]
 name = CCMetagen
-version = 1.4.2
+version = attr: ccmetagen.__version__
 author = Vanessa R. Marcelino Jan P. Buchmann Andreas Sjödin Philip T.L.C. Clausen
 author_email = vrmarcelino@gmail.com
 description = Microbiome classification pipeline
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = bioinformatics taxonomy metagenomic classifier KMA
 url = https://github.com/vrmarcelino/CCMetagen.git
 project_urls = 
 	Source = https://github.com/vrmarcelino/CCMetagen.git
 	Preprint = https://www.biorxiv.org/content/10.1101/641332v2
 license = GPL-3.0
 classifiers = 
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.9
 	Operating System :: POSIX :: Linux
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.9
 packages = 
 	ccmetagen
 install_requires = 
 	pandas
 	ete3
 scripts = 
 	CCMetagen.py
```

### Comparing `CCMetagen-1.4.2/README.md` & `CCMetagen-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,100 @@
+Metadata-Version: 2.1
+Name: CCMetagen
+Version: 1.5.0
+Summary: Microbiome classification pipeline
+Home-page: https://github.com/vrmarcelino/CCMetagen.git
+Author: Vanessa R. Marcelino Jan P. Buchmann Andreas Sjödin Philip T.L.C. Clausen
+Author-email: vrmarcelino@gmail.com
+License: GPL-3.0
+Project-URL: Source, https://github.com/vrmarcelino/CCMetagen.git
+Project-URL: Preprint, https://www.biorxiv.org/content/10.1101/641332v2
+Keywords: bioinformatics taxonomy metagenomic classifier KMA
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: pandas
+Requires-Dist: ete3
+
 # CCMetagen
 
 CCMetagen processes sequence alignments produced with [KMA](https://bitbucket.org/genomicepidemiology/kma), which implements the ConClave sorting scheme to achieve highly accurate read mappings. The pipeline is fast enough to use the whole NCBI nt collection as reference, facilitating the inclusion of understudied organisms, such as microbial eukaryotes, in metagenome surveys. CCMetagen produces ranked taxonomic results in user-friendly formats that are ready for publication or downstream statistical analyses.
 
 If you this tool, please cite CCMetagen and KMA:
 
   * [Marcelino VR, Clausen PT, Buchman J, Wille M, Iredell JR, Meyer W, Lund O, Sorrell T, Holmes EC. 2019. CCMetagen: comprehensive and accurate identification of eukaryotes and prokaryotes in metagenomic data. Genome Biology. 2020 Dec;21(1):1-5.](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02014-2)
 
   * [Clausen PT, Aarestrup FM, Lund O. 2018. Rapid and precise alignment of raw reads against redundant databases with KMA. BMC bioinformatics. 2018 Dec;19(1):307.](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-018-2336-6)
 
-Besides the guidelines below, we also provide a tutorial to reproduce our metagenome clasisfication analyses of the microbiome of wild birds [here](https://github.com/vrmarcelino/CCMetagen/tree/master/tutorial).
+Besides the guidelines below, we also provide a tutorial to reproduce our metagenome clasisfication analyses of the microbiome of wild birds [here](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/tutorial).
 
 The guidelines below will guide you in using the command-line version of the CCMetagen pipeline.
 
 CCMetagen is also available as a web service at https://cge.food.dtu.dk/services/CCMetagen/.
 Note that we recommend using this command-line version to analyze data exceeding 1.5Gb.
 
-## Requirements and Installation
-
-Make sure you have the dependencies below installed and accessible in your $PATH.
-The guidelines below are for Unix systems.
-
-  * If you do not have it already, download and install [Python 3.6](https://www.python.org/downloads/)
-CCMetagen requires the Python modules [pandas (>0.23)](https://pandas.pydata.org/) and [ETE3](http://etetoolkit.org/).
-The easiest way to install these modules is via conda or pip:
-
-`conda install pandas`
 
-  * You need a C-compiler and zlib development files to install KMA:
+## Installation
 
-`sudo apt-get install libz-dev`
-
-  * Download and install [KMA](https://bitbucket.org/genomicepidemiology/kma):
-```
-git clone https://bitbucket.org/genomicepidemiology/kma.git
-cd kma && make
-```
-**Note - a new version of KMA - v1.3.0 – has been released, featuring higher speed and precision. We recommend that you update KMA to v.1.3.0**
+We recommend installing CCMetagen through [conda](https://docs.conda.io/en/latest/). This will install CCMetagen along with all of its required dependencies.
 
+After installing conda, you can create a new environment with CCMetagen through the following command:
 
-  * [Krona](https://github.com/marbl/Krona) is required for graphs. To install Krona it in the local folder:
 ```
-wget https://github.com/marbl/Krona/releases/download/v2.7/KronaTools-2.7.tar
-tar xvf KronaTools-2.7.tar 
-cd  KronaTools-2.7
-./install.pl --prefix . 
+conda create -n ccmetagen ccmetagen -c bioconda -c conda-forge
 ```
 
-  * Then download CCMetagen and add it to your path. You have two options:
+You can then activate your environment with:
 
-**Install CCMetagen via git:**
 ```
-git clone https://github.com/vrmarcelino/CCMetagen
+conda activate ccmetagen
 ```
-This will download CCMetagen and the tutorial files.
-You can also just download the python files from this github directory (CCMetagen.py, CCMetagen_merge.py) and the ones in the ccmetagen folder if you rather avoid downloading all other files.
 
-Then add the CCMetagen python scripts to the path, temporarily or permanently. For example:
-`PATH=$PATH<your_folder>/CCMetagen`
+The `-n ccmetagen` flag will name the environment as `ccmetagen`, but you can choose any different name that you'd like. The `ccmetagen` after that specifies that you'd like the CCMetagen package installed into that environment.
+Finally, the `-c bioconda -c conda-forge` specifies that you'd like to use the Bioconda and Conda-Forge channels, which host CCMetagen and its dependencies.
 
-To update CCMetagen, go to the CCMetagen folder and type: `git pull`
-
-**Or install CCMetagen via pip:**
-```
-pip install CCMetagen
-```
-This will automatically install the necessary python packages (pandas and ete3), so you can skip that step if you use pip.
+You can also install CCMetagen from source, or using pip, the Python package manager. For that, follow the installation instructions in the deprecated README file in the [docs](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/old_repository_README.md).
 
+Check your CCMetagen installation by running `CCMetagen.py --version` on your command-line.
 
 
 ## Databases
 
-**Option 1** Download the indexed (ready-to-go) nt or RefSeq database [here](http://dx.doi.org/10.25910/5cc7cd40fca8e).
-Download the ncbi_nt_kma.zip file (96GB zipped file, 165GB uncompressed) or the RefSeq_bf.zip (90GB zipped file)
+After installing CCMetagen, you will need a reference database to perform taxonomic classification. There are two ways to obtain this:
+
+**Option 1** Download the indexed (ready-to-go) nt from [here](https://melbourne.figshare.com/projects/CCMetagen_databases/195755).
+Download the ncbi_nt_kma file (103GB zipped file) or the RefSeq_bf.zip (90GB zipped file)
 Unzip the database, e.g.: `unzip ncbi_nt_kma`.
-The nt database contains the whole in NCBI nucleotide collection (of of Jan 2018), and therefore is suitable to identify a range of microorganisms, including prokaryotes and eukaryotes.
-The RefSeq_bf database contains complete reference bacterial and fungal genomes, suitable for better known habitats such as the human gut or when trying to detect well known species.
+The nt database contains the whole in NCBI nucleotide collection (from 2019, updated database to be released soon!), and therefore is suitable to identify a range of microorganisms, including prokaryotes and eukaryotes.
 
-**Option 2** We have indexed a more recent version of the ncbi nucleotide collection (June 2019) that does not contain environemntal or artificial sequences. The file ncbi_nt_no_env_11jun2019.zip can be found [here](http://dx.doi.org/10.25910/5cc7cd40fca8e) and contains all ncbi nt entries excluding the descendants of environmental eukaryotes (taxid 61964), environmental prokaryotes (48479), unclassified sequences (12908) and artificial sequences (28384).
+There are two versions of the nt database, the one previously mentioned, and another one that does not contain environemntal or artificial sequences. The file ncbi_nt_no_env_11jun2019.zip contains all ncbi nt entries excluding the descendants of environmental eukaryotes (taxid 61964), environmental prokaryotes (48479), unclassified sequences (12908) and artificial sequences (28384).
 
-**Option 3:** Build your own reference database (recommended!)
+**Option 2:** Build your own reference database (recommended!)
 Follow the instructions in the [KMA website](https://bitbucket.org/genomicepidemiology/kma) to index the database.
 It is important that taxids are incorporated in sequence headers for processing with CCMetagen. Sequence headers should look like 
 `>1234|sequence_description`, where 1234 is the taxid. 
-We provide scripts to rename sequences in the nt database [here](https://github.com/vrmarcelino/CCMetagen/tree/master/benchmarking/rename_nt).
+We provide scripts to rename sequences in the nt database [here](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/benchmarking/rename_nt).
 
 If you want to use the RefSeq database, the format is similar to the one required for Kraken. The [Opiniomics blog](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/) describes how to download sequences in an adequate format. Note that you still need to build the index with KMA: `kma_index -i refseq.fna -o refseq_indexed -NI -Sparse -` or `kma_index -i refseq.fna -o refseq_indexed -NI -Sparse TG` for faster analysis.
 
 
 ## Quick Start
 
   * First map sequence reads (or contigs) to the database with **KMA**.
 
 For paired-end files:
+
 ```
 kma -ipe $SAMPLE_R1 $SAMPLE_R2 -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and -apm f
 ```
 
 For single-end files:
 ```
 kma -i $SAMPLE -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and
@@ -104,40 +103,46 @@
 If you want to calculate abundance in reads per million (RPM) or in number of reads (fragments), or if you want to calculate the proportion of mapped reads, add the flag -ef (extended features):
 ```
 kma -ipe $SAMPLE_R1 $SAMPLE_R2 -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and -apm f -ef
 ```
 
 Where:
 
-$db is the path to the reference database
-$th is the number of threads
-$SAMPLE_R1 is the path to the mate1 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
-$SAMPLE_R2 is the path to the mate2 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
-$SAMPLE is the path to a single-end metagenome/metatranscriptome file (reads or contigs)
+- `$db` is the path to the reference database
+- `$th` is the number of threads
+- `$SAMPLE_R1` is the path to the mate1 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
+- `$SAMPLE_R2` is the path to the mate2 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
+- `$SAMPLE` is the path to a single-end metagenome/metatranscriptome file (reads or contigs)
 
+Then run `CCMetagen.py`:
 
-  * Then run **CCMetagen**:
 ```
 CCMetagen.py -i $sample_out_kma.res -o results
 ```
+
 Where $sample_out_kma.res is alignment results produced by KMA.
 
 Note that if you are running CCMetagen from the local folder (instead of adding it to your path), you may need to add 'python' before CCMetagen: `python CCMetagen.py -i $sample_out_kma.res -o results`
 
 Done! This will make an additional quality filter and output a text file with ranked taxonomic classifications and a krona graph file for interactive visualization.
 
-An example of the CCMetagen output can be found [here (.csv file)](https://github.com/vrmarcelino/CCMetagen/blob/master/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.csv) and [here (.html file)](https://htmlpreview.github.io/?https://github.com/vrmarcelino/CCMetagen/blob/master/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.html).
+An example of the CCMetagen output can be found [here (.csv file)](https://github.com/vrmarcelino/CCMetagen/blob/master/docs/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.csv) and [here (.html file)](https://htmlpreview.github.io/?https://github.com/vrmarcelino/CCMetagen/blob/master/docs/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.html).
 
-<img src=tutorial/figs_tutorial/krona_photo.png width="500" height="419.64">
+<img src=docs/tutorial/figs_tutorial/krona_photo.png width="500" height="419.64">
 
 In the .csv file, you will find the depth (abundance) of each match.
 
 ## Abundance units
 
-**Depth can be estimated in four ways:** by counting the number of nucleotides matching the reference sequence (use flag --depth_unit nc), by applying an additional correction for template length (default in KMA and CCMetagen), by calculating depth in Reads Per Million (RPM, use flag --depth_unit rpm), or by counting the number of fragments (i.e. number of PE reads matching to teh reference sequence, use flag --depth_unit fr). If you want RPM or fragment units, you will need to suply the .mapstats file generated with KMA (which you get when running kma with the flag '-ef').
+**Depth can be estimated in four ways:** 
+
+1. By applying an additional correction for template length (default in KMA and CCMetagen);
+2. By counting the number of nucleotides matching the reference sequence (use flag --depth_unit nc);
+3. By calculating depth in Reads Per Million (RPM, use flag --depth_unit rpm); or
+4. By counting the number of fragments (i.e. number of PE reads matching to teh reference sequence, use flag --depth_unit fr). If you want RPM or fragment units, you will need to suply the .mapstats file generated with KMA (which you get when running kma with the flag '-ef').
 
 
 ## Balancing sensitivity and specificity
 
 You can **adjust the stringency of the taxonomic assignments** by adjusting the minimum coverage (--coverage), the minimum abundance (--depth), and the minimum level of sequence similarity (--query_identity). Coverage is the percentage of bases in the reference sequence that is covered by the consensus sequence (your query), it can be over 100% when the consensus sequence is larger than the reference (due to insertions for example). You can also adjust the KMA settings to facilitate the identification of more distant-related taxa (see below)
 
 If you change the default depth unit, we recommend adjusting the minimum abundance (--depth) to remove taxa found in low abundance accordingly. For example, you can use -d 200 (200 nucleotides) when using --depth_unit nc, which is similar to -d 0.2 when using the default '--depth_unit kma' option. If you choose to calculate abundances in RPM, you may want to adjust the minimum abundance according to your sequence depth.
@@ -167,15 +172,15 @@
 ```
 
   * **To get the abundance of each taxon, and/or summarize results for multiple samples, use CCMetagen_merge**:
 ```
 CCMetagen_merge.py -i $CCMetagen_out
 ```
 
-Where $CCMetagen_out is the folder containing the CCMetagen taxonomic classifications.
+Where `$CCMetagen_out` is the folder containing the CCMetagen taxonomic classifications.
 The results must be in .csv format (default or '--mode text' output of CCMetagen), and these files **must end in ".ccm.csv"**.
 
 The flag '-t' define the taxonomic level to merge the results. The default is species-level.
 
 You can also filter out specific taxa, at any taxonomic level:
 
 Use flag -kr to keep (k) or remove (r) taxa.
@@ -210,24 +215,24 @@
 
 This script will produce a fasta file containing all reads assigned to a taxon of interest. 
 Ex: Generate a fasta file containing all sequences that mapped to the genus Eschericha:
 ```
 CCMetagen_extract_seqs.py -iccm $CCMetagen_out -ifrag $sample_out_kma.frag -l Genus -t Eschericha
 ```
 
-Where $CCMetagen_out is the .csv file generated with CCMetagen and $sample_out_kma.frag is the .frag file generated with KMA. The frag file needs to be decompressed: `gunzip *.frag.gz`
+Where `$CCMetagen_out` is the .csv file generated with CCMetagen and `$sample_out_kma.frag` is the .frag file generated with KMA. The frag file needs to be decompressed: `gunzip *.frag.gz`
 
 For species-level filtering (where there is a space in taxon names), use quotation marks.
 Ex: Generate a fasta file containing all sequences that mapped to _E. coli_:
 ```
 CCMetagen_extract_seqs.py -iccm $CCMetagen_out -ifrag $sample_out_kma.frag -l Species -t "Escherichia coli"
 ```
 
 
-**Check out our [tutorial](https://github.com/vrmarcelino/CCMetagen/tree/master/tutorial) for an applied example of the CCMetagen pipeline.**
+**Check out our [tutorial](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/tutorial) for an applied example of the CCMetagen pipeline.**
 
 
 
 ## FAQs
 
 * Error taxid not found.
   You probably need to update your local ETE3 database, which contains the taxids and lineage information:
```

### Comparing `CCMetagen-1.4.2/ccmetagen/cTaxInfo.py` & `CCMetagen-1.5.0/ccmetagen/cTaxInfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+
 """
 Classes that store taxonomic info from matches and NCBI lineage
 
 @ V.R.Marcelino
-Created on 12 Jul 2018
-Last update on 27 March 2019
-
+Created on 12 Jul 2018.
 """
 
+
 ### Stores taxid and other info
-class TaxInfo(): 
-    
-    def __init__(self, TaxId=None, Lineage=None, Sample=None, RefDatabase=None, 
-                 Abundance=None, Superkingdom = None, Superkingdom_TaxId = None, 
-                 Kingdom=None, Kingdom_TaxId=None, Phylum=None, 
-                 Phylum_TaxId=None, Class=None, Class_TaxId=None,
-                 Order=None, Order_TaxId=None, Family=None, Family_TaxId=None,
-                 Genus=None, Genus_TaxId=None, Species=None, Species_TaxId=None,
-                 LCA_TaxId=None, Coverage=None):
-        
+class TaxInfo:
+    def __init__(
+        self,
+        TaxId=None,
+        Lineage=None,
+        Sample=None,
+        RefDatabase=None,
+        Abundance=None,
+        Superkingdom=None,
+        Superkingdom_TaxId=None,
+        Kingdom=None,
+        Kingdom_TaxId=None,
+        Phylum=None,
+        Phylum_TaxId=None,
+        Class=None,
+        Class_TaxId=None,
+        Order=None,
+        Order_TaxId=None,
+        Family=None,
+        Family_TaxId=None,
+        Genus=None,
+        Genus_TaxId=None,
+        Species=None,
+        Species_TaxId=None,
+        LCA_TaxId=None,
+        Coverage=None,
+    ):
         # info from matches
         self.TaxId = TaxId
-        self.Lineage = Lineage # the results of the match, not considering taxIDs
+        self.Lineage = Lineage  # the results of the match, not considering taxIDs
         self.Sample = Sample
         self.RefDatabase = RefDatabase
         self.Abundance = Abundance
 
         # info from NCBI
         self.Superkingdom = Superkingdom
         self.Superkingdom_TaxId = Superkingdom_TaxId
@@ -34,19 +51,19 @@
         self.Kingdom_TaxId = Kingdom_TaxId
         self.Phylum = Phylum
         self.Phylum_TaxId = Phylum_TaxId
         self.Class = Class
         self.Class_TaxId = Class_TaxId
         self.Order = Order
         self.Order_TaxId = Order_TaxId
-        self.Family = Order
-        self.Family_TaxId = Order_TaxId
+        self.Family = Family
+        self.Family_TaxId = Family_TaxId
         self.Genus = Genus
         self.Genus_TaxId = Genus_TaxId
         self.Species = Species
         self.Species_TaxId = Species_TaxId
-        
+
         # Taxid of the Lowest Common Ancestor
         self.LCA_TaxId = LCA_TaxId
 
         # info from Fungi Table only
         self.Coverage = Coverage
```

### Comparing `CCMetagen-1.4.2/ccmetagen/fParseKMA.py` & `CCMetagen-1.5.0/ccmetagen/fParseKMA.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,156 +1,155 @@
 #!/usr/bin/env ipython
 # -*- coding: utf-8 -*-
+
 """
 Functions to parse KMA results
 
 @ V.R.Marcelino
-Created on 1 Aug 2018
-
-
+Created on 1 Aug 2018.
 """
+
 import re
 
 # local imports
-from ccmetagen import cTaxInfo
-from ccmetagen import fNCBItax
-
-import subprocess
+from ccmetagen import cTaxInfo, fNCBItax
 
 # function to filter a res file in pandas df format:
-def res_filter(df,ref_database, cov,Iden,Depth,p):
+def res_filter(df, cov, Iden, Depth, p):
     df = df.drop(df[df.Template_Coverage < cov].index)
 
-    # filter based on identity      
+    # filter based on identity
     df = df.drop(df[df.Query_Identity < Iden].index)
-    
+
     # filter based on depth
     df = df.drop(df[df.Depth < Depth].index)
 
     # filter based on p-values
     df = df.drop(df[df.p_value > p].index)
-     
-    return df
 
+    return df
 
-# function that takes as input a pandas dataframe with KMA results 
-# and add tax information to results 
-def populate_w_tax(in_df, ref_database,species_threshold,genus_threshold,
-                   family_threshold,order_threshold,class_threshold,phylum_threshold, taxfile=None):
-    #defaults:
-    #species_threshold = 98.41 # Yeast - Vu et al 2016
-    #genus_threshold = 96.31 # Yeast - Vu et al 2016
-    #family_threshold = 88.51 # Filamentous fungi - Vu et al 2019
-    #order_threshold = 81.21 # Filamentous fungi - Vu et al 2019
-    #class_threshold = 80.91 # Filamentous fungi - Vu et al 2019
-    #phylum, kingdom and superkingdom = 0  # no data, no filtering
 
+# function that takes as input a pandas dataframe with KMA results
+# and add tax information to results
+def populate_w_tax(
+    in_df,
+    ref_database,
+    species_threshold,
+    genus_threshold,
+    family_threshold,
+    order_threshold,
+    class_threshold,
+    phylum_threshold,
+    taxfile=None,
+):
+    # For default thresholds, see ccmetagen/__init__.py
 
     # Make sure all taxa columns are strings (doesn't automatically happen if the first one is None)
-    in_df = in_df.assign(LCA_TaxId="",Superkingdom="",Kingdom="",Phylum="",Class="",Order="",Family="",Genus="",Species="")
-
+    in_df = in_df.assign(
+        LCA_TaxId="",
+        Superkingdom="",
+        Kingdom="",
+        Phylum="",
+        Class="",
+        Order="",
+        Family="",
+        Genus="",
+        Species="",
+    )
 
     # index == the #template (fungal match)
     for index, row in in_df.iterrows():
         match_info = cTaxInfo.TaxInfo()
 
         # define the tax. rank based on similarity:
         if ref_database == "UNITE":
-            split_match = re.split (r'(\|| )', index)
-            qiden = row['Query_Identity']
+            split_match = re.split(r"(\|| )", index)
+            qiden = row["Query_Identity"]
             match_info.Lineage = split_match[12]
 
             # if taxid is knwon:
-            if split_match[4] != 'unk_taxid':
-                
+            if split_match[4] != "unk_taxid":
                 match_info.TaxId = int(split_match[4])
-                match_info = fNCBItax.lineage_extractor(match_info.TaxId , match_info, taxfile)
-                
-                # Warning about unknown taxids: 
-            else:
-                print ("")
-                print ("WARNING: based on accession number, no taxonomic information was found in NCBI for %s" %(match_info.Lineage))
-                print ("This match will not get NCBItax taxonomic ranks")
-                print ("")
-                match_info.TaxId = split_match[4] # 'unk_taxid'
+                match_info = fNCBItax.lineage_extractor(
+                    match_info.TaxId, match_info, taxfile
+                )
 
+                # Warning about unknown taxids:
+            else:
+                print("")
+                print(
+                    "WARNING: based on accession number, no taxonomic information was found in NCBI for %s"
+                    % (match_info.Lineage)
+                )
+                print("This match will not get NCBItax taxonomic ranks")
+                print("")
+                match_info.TaxId = split_match[4]  # 'unk_taxid'
 
         elif ref_database == "RefSeq":
-            split_match = re.split (r'(\|| )', index)
-            qiden = row['Query_Identity']
+            split_match = re.split(r"(\|| )", index)
+            qiden = row["Query_Identity"]
             match_info.TaxId = int(split_match[4])
             species = split_match[6] + " " + split_match[8]
             match_info.Lineage = species
             # include info from NCBI:
-            match_info = fNCBItax.lineage_extractor(match_info.TaxId, match_info, taxfile)
-
+            match_info = fNCBItax.lineage_extractor(
+                match_info.TaxId, match_info, taxfile
+            )
 
         elif ref_database == "nt":
-            split_match = re.split (r'(\|| )', index)
-            qiden = row['Query_Identity']
+            split_match = re.split(r"(\|| )", index)
+            qiden = row["Query_Identity"]
             match_info.Lineage = split_match[2]
-            
-            #get taxid from accession number
+
+            # get taxid from accession number
             taxid = split_match[0]
 
-            if taxid == 'unk_taxid':
-                # Warning about unknown taxids: 
-                print ("")
-                print ("WARNING: no NCBI's taxid found for accession %s" %(match_info.Lineage))
-                print ("This match will not get taxonomic ranks")
-                print ("")
-                
+            if taxid == "unk_taxid":
+                # Warning about unknown taxids:
+                print("")
+                print(
+                    "WARNING: no NCBI's taxid found for accession %s"
+                    % (match_info.Lineage)
+                )
+                print("This match will not get taxonomic ranks")
+                print("")
+
             else:
-                match_info.TaxId = int(taxid)            
-                match_info = fNCBItax.lineage_extractor(match_info.TaxId, match_info, taxfile)
-   
-            
-        # Populate the df with lineage info and the LCA taxid: 
-        
-        in_df.at[index, 'Superkingdom'] = match_info.Superkingdom
-        in_df.at[index, 'Kingdom'] = match_info.Kingdom
-        
+                match_info.TaxId = int(taxid)
+                match_info = fNCBItax.lineage_extractor(
+                    match_info.TaxId, match_info, taxfile
+                )
+
+        # Populate the df with lineage info and the LCA taxid:
+        in_df.at[index, "Superkingdom"] = match_info.Superkingdom
+        in_df.at[index, "Kingdom"] = match_info.Kingdom
+
         # Assign LCA_taxid. Go to Kingdom if possible:
-        in_df.at[index, 'LCA_TaxId'] = match_info.Superkingdom_TaxId
-        
+        in_df.at[index, "LCA_TaxId"] = match_info.Superkingdom_TaxId
+
         if match_info.Kingdom_TaxId is not None:
-            in_df.at[index, 'LCA_TaxId'] = match_info.Kingdom_TaxId
-        
+            in_df.at[index, "LCA_TaxId"] = match_info.Kingdom_TaxId
+
         # if it matches to uncultured or unclassified fungus, use the Fungi LCA itaxid:
-        if match_info.Kingdom == 'Fungi':
-            in_df.at[index, 'LCA_TaxId'] = 4751
+        if match_info.Kingdom == "Fungi":
+            in_df.at[index, "LCA_TaxId"] = 4751
 
-        # fill in the rest of the table according to similarity threshold:
-        if qiden >= phylum_threshold:
-            in_df.at[index, 'Phylum'] = match_info.Phylum
-            if match_info.Phylum_TaxId != None:
-                in_df.at[index, 'LCA_TaxId'] = match_info.Phylum_TaxId
-
-        if qiden >= class_threshold:
-            in_df.at[index, 'Class'] = match_info.Class
-            if match_info.Class_TaxId != None:
-                in_df.at[index, 'LCA_TaxId'] = match_info.Class_TaxId
-    
-        if qiden >= order_threshold:
-            in_df.at[index, 'Order'] = match_info.Order
-            if match_info.Order_TaxId != None:
-                in_df.at[index, 'LCA_TaxId'] = match_info.Order_TaxId
-
-        if qiden >= family_threshold:
-            in_df.at[index, 'Family'] = match_info.Family
-            if match_info.Family_TaxId != None:
-                in_df.at[index, 'LCA_TaxId'] = match_info.Family_TaxId
-    
-        if qiden >= genus_threshold:
-            in_df.at[index, 'Genus'] = match_info.Genus
-            if match_info.Genus_TaxId != None:
-                in_df.at[index, 'LCA_TaxId'] = match_info.Genus_TaxId
-    
-        if qiden >= species_threshold:
-            in_df.at[index, 'Species'] = match_info.Species
-            if match_info.Species_TaxId != None:
-                in_df.at[index, 'LCA_TaxId'] = match_info.Species_TaxId
-    
-    return in_df
+        thresholds = {
+            "Phylum": phylum_threshold,
+            "Class": class_threshold,
+            "Order": order_threshold,
+            "Family": family_threshold,
+            "Genus": genus_threshold,
+            "Species": species_threshold
+        }
+
+        for rank, threshold in thresholds.items():
+            if qiden >= threshold:
+                tax_info_attr = f"{rank}_TaxId"
 
+                in_df.at[index, rank] = getattr(match_info, rank)
 
+                if getattr(match_info, tax_info_attr) is not None:
+                    in_df.at[index, "LCA_TaxId"] = getattr(match_info, tax_info_attr)
 
+    return in_df
```

### Comparing `CCMetagen-1.4.2/CCMetagen.egg-info/PKG-INFO` & `CCMetagen-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,124 +1,75 @@
-Metadata-Version: 2.1
-Name: CCMetagen
-Version: 1.4.2
-Summary: Microbiome classification pipeline
-Home-page: https://github.com/vrmarcelino/CCMetagen.git
-Author: Vanessa R. Marcelino Jan P. Buchmann Andreas Sjödin Philip T.L.C. Clausen
-Author-email: vrmarcelino@gmail.com
-License: GPL-3.0
-Project-URL: Source, https://github.com/vrmarcelino/CCMetagen.git
-Project-URL: Preprint, https://www.biorxiv.org/content/10.1101/641332v2
-Keywords: bioinformatics taxonomy metagenomic classifier KMA
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CCMetagen
 
 CCMetagen processes sequence alignments produced with [KMA](https://bitbucket.org/genomicepidemiology/kma), which implements the ConClave sorting scheme to achieve highly accurate read mappings. The pipeline is fast enough to use the whole NCBI nt collection as reference, facilitating the inclusion of understudied organisms, such as microbial eukaryotes, in metagenome surveys. CCMetagen produces ranked taxonomic results in user-friendly formats that are ready for publication or downstream statistical analyses.
 
 If you this tool, please cite CCMetagen and KMA:
 
   * [Marcelino VR, Clausen PT, Buchman J, Wille M, Iredell JR, Meyer W, Lund O, Sorrell T, Holmes EC. 2019. CCMetagen: comprehensive and accurate identification of eukaryotes and prokaryotes in metagenomic data. Genome Biology. 2020 Dec;21(1):1-5.](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02014-2)
 
   * [Clausen PT, Aarestrup FM, Lund O. 2018. Rapid and precise alignment of raw reads against redundant databases with KMA. BMC bioinformatics. 2018 Dec;19(1):307.](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-018-2336-6)
 
-Besides the guidelines below, we also provide a tutorial to reproduce our metagenome clasisfication analyses of the microbiome of wild birds [here](https://github.com/vrmarcelino/CCMetagen/tree/master/tutorial).
+Besides the guidelines below, we also provide a tutorial to reproduce our metagenome clasisfication analyses of the microbiome of wild birds [here](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/tutorial).
 
 The guidelines below will guide you in using the command-line version of the CCMetagen pipeline.
 
 CCMetagen is also available as a web service at https://cge.food.dtu.dk/services/CCMetagen/.
 Note that we recommend using this command-line version to analyze data exceeding 1.5Gb.
 
-## Requirements and Installation
-
-Make sure you have the dependencies below installed and accessible in your $PATH.
-The guidelines below are for Unix systems.
-
-  * If you do not have it already, download and install [Python 3.6](https://www.python.org/downloads/)
-CCMetagen requires the Python modules [pandas (>0.23)](https://pandas.pydata.org/) and [ETE3](http://etetoolkit.org/).
-The easiest way to install these modules is via conda or pip:
-
-`conda install pandas`
 
-  * You need a C-compiler and zlib development files to install KMA:
+## Installation
 
-`sudo apt-get install libz-dev`
+We recommend installing CCMetagen through [conda](https://docs.conda.io/en/latest/). This will install CCMetagen along with all of its required dependencies.
 
-  * Download and install [KMA](https://bitbucket.org/genomicepidemiology/kma):
-```
-git clone https://bitbucket.org/genomicepidemiology/kma.git
-cd kma && make
-```
-**Note - a new version of KMA - v1.3.0 – has been released, featuring higher speed and precision. We recommend that you update KMA to v.1.3.0**
+After installing conda, you can create a new environment with CCMetagen through the following command:
 
-
-  * [Krona](https://github.com/marbl/Krona) is required for graphs. To install Krona it in the local folder:
 ```
-wget https://github.com/marbl/Krona/releases/download/v2.7/KronaTools-2.7.tar
-tar xvf KronaTools-2.7.tar 
-cd  KronaTools-2.7
-./install.pl --prefix . 
+conda create -n ccmetagen ccmetagen -c bioconda -c conda-forge
 ```
 
-  * Then download CCMetagen and add it to your path. You have two options:
+You can then activate your environment with:
 
-**Install CCMetagen via git:**
 ```
-git clone https://github.com/vrmarcelino/CCMetagen
+conda activate ccmetagen
 ```
-This will download CCMetagen and the tutorial files.
-You can also just download the python files from this github directory (CCMetagen.py, CCMetagen_merge.py) and the ones in the ccmetagen folder if you rather avoid downloading all other files.
-
-Then add the CCMetagen python scripts to the path, temporarily or permanently. For example:
-`PATH=$PATH<your_folder>/CCMetagen`
 
-To update CCMetagen, go to the CCMetagen folder and type: `git pull`
+The `-n ccmetagen` flag will name the environment as `ccmetagen`, but you can choose any different name that you'd like. The `ccmetagen` after that specifies that you'd like the CCMetagen package installed into that environment.
+Finally, the `-c bioconda -c conda-forge` specifies that you'd like to use the Bioconda and Conda-Forge channels, which host CCMetagen and its dependencies.
 
-**Or install CCMetagen via pip:**
-```
-pip install CCMetagen
-```
-This will automatically install the necessary python packages (pandas and ete3), so you can skip that step if you use pip.
+You can also install CCMetagen from source, or using pip, the Python package manager. For that, follow the installation instructions in the deprecated README file in the [docs](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/old_repository_README.md).
 
+Check your CCMetagen installation by running `CCMetagen.py --version` on your command-line.
 
 
 ## Databases
 
-**Option 1** Download the indexed (ready-to-go) nt or RefSeq database [here](http://dx.doi.org/10.25910/5cc7cd40fca8e).
-Download the ncbi_nt_kma.zip file (96GB zipped file, 165GB uncompressed) or the RefSeq_bf.zip (90GB zipped file)
+After installing CCMetagen, you will need a reference database to perform taxonomic classification. There are two ways to obtain this:
+
+**Option 1** Download the indexed (ready-to-go) nt from [here](https://melbourne.figshare.com/projects/CCMetagen_databases/195755).
+Download the ncbi_nt_kma file (103GB zipped file) or the RefSeq_bf.zip (90GB zipped file)
 Unzip the database, e.g.: `unzip ncbi_nt_kma`.
-The nt database contains the whole in NCBI nucleotide collection (of of Jan 2018), and therefore is suitable to identify a range of microorganisms, including prokaryotes and eukaryotes.
-The RefSeq_bf database contains complete reference bacterial and fungal genomes, suitable for better known habitats such as the human gut or when trying to detect well known species.
+The nt database contains the whole in NCBI nucleotide collection (from 2019, updated database to be released soon!), and therefore is suitable to identify a range of microorganisms, including prokaryotes and eukaryotes.
 
-**Option 2** We have indexed a more recent version of the ncbi nucleotide collection (June 2019) that does not contain environemntal or artificial sequences. The file ncbi_nt_no_env_11jun2019.zip can be found [here](http://dx.doi.org/10.25910/5cc7cd40fca8e) and contains all ncbi nt entries excluding the descendants of environmental eukaryotes (taxid 61964), environmental prokaryotes (48479), unclassified sequences (12908) and artificial sequences (28384).
+There are two versions of the nt database, the one previously mentioned, and another one that does not contain environemntal or artificial sequences. The file ncbi_nt_no_env_11jun2019.zip contains all ncbi nt entries excluding the descendants of environmental eukaryotes (taxid 61964), environmental prokaryotes (48479), unclassified sequences (12908) and artificial sequences (28384).
 
-**Option 3:** Build your own reference database (recommended!)
+**Option 2:** Build your own reference database (recommended!)
 Follow the instructions in the [KMA website](https://bitbucket.org/genomicepidemiology/kma) to index the database.
 It is important that taxids are incorporated in sequence headers for processing with CCMetagen. Sequence headers should look like 
 `>1234|sequence_description`, where 1234 is the taxid. 
-We provide scripts to rename sequences in the nt database [here](https://github.com/vrmarcelino/CCMetagen/tree/master/benchmarking/rename_nt).
+We provide scripts to rename sequences in the nt database [here](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/benchmarking/rename_nt).
 
 If you want to use the RefSeq database, the format is similar to the one required for Kraken. The [Opiniomics blog](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/) describes how to download sequences in an adequate format. Note that you still need to build the index with KMA: `kma_index -i refseq.fna -o refseq_indexed -NI -Sparse -` or `kma_index -i refseq.fna -o refseq_indexed -NI -Sparse TG` for faster analysis.
 
 
 ## Quick Start
 
   * First map sequence reads (or contigs) to the database with **KMA**.
 
 For paired-end files:
+
 ```
 kma -ipe $SAMPLE_R1 $SAMPLE_R2 -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and -apm f
 ```
 
 For single-end files:
 ```
 kma -i $SAMPLE -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and
@@ -127,40 +78,46 @@
 If you want to calculate abundance in reads per million (RPM) or in number of reads (fragments), or if you want to calculate the proportion of mapped reads, add the flag -ef (extended features):
 ```
 kma -ipe $SAMPLE_R1 $SAMPLE_R2 -o sample_out_kma -t_db $db -t $th -1t1 -mem_mode -and -apm f -ef
 ```
 
 Where:
 
-$db is the path to the reference database
-$th is the number of threads
-$SAMPLE_R1 is the path to the mate1 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
-$SAMPLE_R2 is the path to the mate2 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
-$SAMPLE is the path to a single-end metagenome/metatranscriptome file (reads or contigs)
+- `$db` is the path to the reference database
+- `$th` is the number of threads
+- `$SAMPLE_R1` is the path to the mate1 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
+- `$SAMPLE_R2` is the path to the mate2 of a paired-end metagenome/metatranscriptome sample (fastq or fasta)
+- `$SAMPLE` is the path to a single-end metagenome/metatranscriptome file (reads or contigs)
 
+Then run `CCMetagen.py`:
 
-  * Then run **CCMetagen**:
 ```
 CCMetagen.py -i $sample_out_kma.res -o results
 ```
+
 Where $sample_out_kma.res is alignment results produced by KMA.
 
 Note that if you are running CCMetagen from the local folder (instead of adding it to your path), you may need to add 'python' before CCMetagen: `python CCMetagen.py -i $sample_out_kma.res -o results`
 
 Done! This will make an additional quality filter and output a text file with ranked taxonomic classifications and a krona graph file for interactive visualization.
 
-An example of the CCMetagen output can be found [here (.csv file)](https://github.com/vrmarcelino/CCMetagen/blob/master/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.csv) and [here (.html file)](https://htmlpreview.github.io/?https://github.com/vrmarcelino/CCMetagen/blob/master/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.html).
+An example of the CCMetagen output can be found [here (.csv file)](https://github.com/vrmarcelino/CCMetagen/blob/master/docs/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.csv) and [here (.html file)](https://htmlpreview.github.io/?https://github.com/vrmarcelino/CCMetagen/blob/master/docs/tutorial/figs_tutorial/Turnstone_Temperate_Flu_Ng.res.html).
 
-<img src=tutorial/figs_tutorial/krona_photo.png width="500" height="419.64">
+<img src=docs/tutorial/figs_tutorial/krona_photo.png width="500" height="419.64">
 
 In the .csv file, you will find the depth (abundance) of each match.
 
 ## Abundance units
 
-**Depth can be estimated in four ways:** by counting the number of nucleotides matching the reference sequence (use flag --depth_unit nc), by applying an additional correction for template length (default in KMA and CCMetagen), by calculating depth in Reads Per Million (RPM, use flag --depth_unit rpm), or by counting the number of fragments (i.e. number of PE reads matching to teh reference sequence, use flag --depth_unit fr). If you want RPM or fragment units, you will need to suply the .mapstats file generated with KMA (which you get when running kma with the flag '-ef').
+**Depth can be estimated in four ways:** 
+
+1. By applying an additional correction for template length (default in KMA and CCMetagen);
+2. By counting the number of nucleotides matching the reference sequence (use flag --depth_unit nc);
+3. By calculating depth in Reads Per Million (RPM, use flag --depth_unit rpm); or
+4. By counting the number of fragments (i.e. number of PE reads matching to teh reference sequence, use flag --depth_unit fr). If you want RPM or fragment units, you will need to suply the .mapstats file generated with KMA (which you get when running kma with the flag '-ef').
 
 
 ## Balancing sensitivity and specificity
 
 You can **adjust the stringency of the taxonomic assignments** by adjusting the minimum coverage (--coverage), the minimum abundance (--depth), and the minimum level of sequence similarity (--query_identity). Coverage is the percentage of bases in the reference sequence that is covered by the consensus sequence (your query), it can be over 100% when the consensus sequence is larger than the reference (due to insertions for example). You can also adjust the KMA settings to facilitate the identification of more distant-related taxa (see below)
 
 If you change the default depth unit, we recommend adjusting the minimum abundance (--depth) to remove taxa found in low abundance accordingly. For example, you can use -d 200 (200 nucleotides) when using --depth_unit nc, which is similar to -d 0.2 when using the default '--depth_unit kma' option. If you choose to calculate abundances in RPM, you may want to adjust the minimum abundance according to your sequence depth.
@@ -190,15 +147,15 @@
 ```
 
   * **To get the abundance of each taxon, and/or summarize results for multiple samples, use CCMetagen_merge**:
 ```
 CCMetagen_merge.py -i $CCMetagen_out
 ```
 
-Where $CCMetagen_out is the folder containing the CCMetagen taxonomic classifications.
+Where `$CCMetagen_out` is the folder containing the CCMetagen taxonomic classifications.
 The results must be in .csv format (default or '--mode text' output of CCMetagen), and these files **must end in ".ccm.csv"**.
 
 The flag '-t' define the taxonomic level to merge the results. The default is species-level.
 
 You can also filter out specific taxa, at any taxonomic level:
 
 Use flag -kr to keep (k) or remove (r) taxa.
@@ -233,24 +190,24 @@
 
 This script will produce a fasta file containing all reads assigned to a taxon of interest. 
 Ex: Generate a fasta file containing all sequences that mapped to the genus Eschericha:
 ```
 CCMetagen_extract_seqs.py -iccm $CCMetagen_out -ifrag $sample_out_kma.frag -l Genus -t Eschericha
 ```
 
-Where $CCMetagen_out is the .csv file generated with CCMetagen and $sample_out_kma.frag is the .frag file generated with KMA. The frag file needs to be decompressed: `gunzip *.frag.gz`
+Where `$CCMetagen_out` is the .csv file generated with CCMetagen and `$sample_out_kma.frag` is the .frag file generated with KMA. The frag file needs to be decompressed: `gunzip *.frag.gz`
 
 For species-level filtering (where there is a space in taxon names), use quotation marks.
 Ex: Generate a fasta file containing all sequences that mapped to _E. coli_:
 ```
 CCMetagen_extract_seqs.py -iccm $CCMetagen_out -ifrag $sample_out_kma.frag -l Species -t "Escherichia coli"
 ```
 
 
-**Check out our [tutorial](https://github.com/vrmarcelino/CCMetagen/tree/master/tutorial) for an applied example of the CCMetagen pipeline.**
+**Check out our [tutorial](https://github.com/vrmarcelino/CCMetagen/tree/master/docs/tutorial) for an applied example of the CCMetagen pipeline.**
 
 
 
 ## FAQs
 
 * Error taxid not found.
   You probably need to update your local ETE3 database, which contains the taxids and lineage information:
@@ -360,9 +317,7 @@
                         applied
   -off TURN_OFF_SIM_THRESHOLDS, --turn_off_sim_thresholds TURN_OFF_SIM_THRESHOLDS
                         Turns simularity-based filtering off. Options = y or
                         n. Default = n
   --version             show program's version number and exit
  ```
 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

