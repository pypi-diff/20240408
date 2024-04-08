# Comparing `tmp/volcano_cooking-0.9.2.tar.gz` & `tmp/volcano_cooking-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volcano_cooking-0.9.2.tar", max compression
+gzip compressed data, was "volcano_cooking-0.9.3.tar", max compression
```

## Comparing `volcano_cooking-0.9.2.tar` & `volcano_cooking-0.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/LICENSE
--rw-r--r--   0        0        0    10747 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/README.md
--rw-r--r--   0        0        0     1263 2022-10-28 18:28:44.749077 volcano_cooking-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      146 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/__init__.py
--rw-r--r--   0        0        0     5960 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/__main__.py
--rw-r--r--   0        0        0     3892 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/configurations/shift_eruption_to_date.py
--rw-r--r--   0        0        0    24143 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/createVolcEruptV3.ncl
--rw-r--r--   0        0        0     3994 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/create_cesm_frc.sh
--rw-r--r--   0        0        0      166 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/__init__.py
--rw-r--r--   0        0        0     1843 2022-10-28 18:28:21.512390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/compare_datasets.py
--rw-r--r--   0        0        0     1333 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/compare_volc_files.py
--rw-r--r--   0        0        0     2864 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/functions.py
--rw-r--r--   0        0        0     1281 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/inspect_X-vs-Y.py
--rw-r--r--   0        0        0     1196 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/inspect_year.py
--rw-r--r--   0        0        0     7118 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/view_generated_forcing.py
--rw-r--r--   0        0        0      421 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/convert/__init__.py
--rw-r--r--   0        0        0     4260 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/convert/adjust_emissions_and_heights.py
--rw-r--r--   0        0        0     3084 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/convert/convert_between_variables.py
--rw-r--r--   0        0        0      419 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/create/__init__.py
--rw-r--r--   0        0        0    15927 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/create/create_data.py
--rw-r--r--   0        0        0     9061 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/create/create_dates.py
--rw-r--r--   0        0        0     2173 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/create/create_frc.py
--rw-r--r--   0        0        0     1521 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/create/easy_fix.py
--rw-r--r--   0        0        0    10333 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/modules/create/rewrite_frc_file.py
--rw-r--r--   0        0        0     1093 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/package_last.sh
--rw-r--r--   0        0        0     1298 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/parse_stratvolc.py
--rw-r--r--   0        0        0     5663 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/plotting/figure_standards.py
--rw-r--r--   0        0        0     6800 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/sparse_to_lin.py
--rw-r--r--   0        0        0     3550 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/synthetic_volcanoes.py
--rw-r--r--   0        0        0     1571 2022-10-28 18:28:21.516390 volcano_cooking-0.9.2/src/volcano_cooking/view_force.py
--rw-r--r--   0        0        0    12497 1970-01-01 00:00:00.000000 volcano_cooking-0.9.2/setup.py
--rw-r--r--   0        0        0    11834 1970-01-01 00:00:00.000000 volcano_cooking-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-21 21:50:12.073011 volcano_cooking-0.9.3/LICENSE
+-rw-r--r--   0        0        0    12009 2022-11-21 21:50:12.073011 volcano_cooking-0.9.3/README.md
+-rw-r--r--   0        0        0     1263 2022-11-21 21:50:34.989020 volcano_cooking-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      146 2022-11-21 21:50:12.073011 volcano_cooking-0.9.3/src/volcano_cooking/__init__.py
+-rw-r--r--   0        0        0     5960 2022-11-21 21:50:12.073011 volcano_cooking-0.9.3/src/volcano_cooking/__main__.py
+-rw-r--r--   0        0        0     3892 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/configurations/shift_eruption_to_date.py
+-rw-r--r--   0        0        0    24143 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/createVolcEruptV3.ncl
+-rw-r--r--   0        0        0     3994 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/create_cesm_frc.sh
+-rw-r--r--   0        0        0      166 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/__init__.py
+-rw-r--r--   0        0        0     1843 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/compare_datasets.py
+-rw-r--r--   0        0        0     1333 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/compare_volc_files.py
+-rw-r--r--   0        0        0     2864 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/functions.py
+-rw-r--r--   0        0        0     1281 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/inspect_X-vs-Y.py
+-rw-r--r--   0        0        0     1196 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/inspect_year.py
+-rw-r--r--   0        0        0     7118 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/view_generated_forcing.py
+-rw-r--r--   0        0        0      421 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/convert/__init__.py
+-rw-r--r--   0        0        0     4260 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/convert/adjust_emissions_and_heights.py
+-rw-r--r--   0        0        0     3084 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/convert/convert_between_variables.py
+-rw-r--r--   0        0        0      419 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/create/__init__.py
+-rw-r--r--   0        0        0    15927 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/create/create_data.py
+-rw-r--r--   0        0        0     9061 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/create/create_dates.py
+-rw-r--r--   0        0        0     2173 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/create/create_frc.py
+-rw-r--r--   0        0        0     1521 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/create/easy_fix.py
+-rw-r--r--   0        0        0    10333 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/modules/create/rewrite_frc_file.py
+-rw-r--r--   0        0        0     1093 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/package_last.sh
+-rw-r--r--   0        0        0     1298 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/parse_stratvolc.py
+-rw-r--r--   0        0        0     5663 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/plotting/figure_standards.py
+-rw-r--r--   0        0        0     6763 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/sparse_to_lin.py
+-rw-r--r--   0        0        0     3550 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/synthetic_volcanoes.py
+-rw-r--r--   0        0        0     1571 2022-11-21 21:50:12.077011 volcano_cooking-0.9.3/src/volcano_cooking/view_force.py
+-rw-r--r--   0        0        0    13797 1970-01-01 00:00:00.000000 volcano_cooking-0.9.3/setup.py
+-rw-r--r--   0        0        0    13096 1970-01-01 00:00:00.000000 volcano_cooking-0.9.3/PKG-INFO
```

### Comparing `volcano_cooking-0.9.2/LICENSE` & `volcano_cooking-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/README.md` & `volcano_cooking-0.9.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,71 +21,53 @@
 
 The package is published on [PyPI] and installable via `pip`:
 
 ```bash
 pip install volcano-cooking
 ```
 
+<!-- FIXME: add reference to available classes -->
+If you only plan on using the already present generator classes and only need the CLI
+program, it is recommended to install this with [pipx][pipx-source]:
+
+```bash
+pipx install volcano-cooking
+```
+
 ## Usage
 
 ### The basics
 
-There are two CLI programs coming with this project. The main program is
+There are mainly two CLI programs coming with this project. The main program is
 `volcano-cooking`, which will create a `.nc` and `.npz` file in the `data/output`
-directory. With the `view_frc` program you can quickly view the content of the created
-files in a plot.
-
-Run from within this repository/directory via poetry:
+directory. With the `view-frc` program you can quickly view the content of the created
+files in a plot. There is also a third program called `sfrc-sparse2lin` which converts
+arrays of only non-zero events at arbitrary times to linearly spaced events where times
+between the non-zero events are filled with zeros.
 
-```sh
-poetry run volcano-cooking
-poetry run view-frc <file.nc>
-```
+### `volcano-cooking`
 
-or, if the virtual environment where the project is installed is activated:
+Once installed, run from within this directory with:
 
-```sh
+```bash
 volcano-cooking
-view-frc <file.nc>
 ```
 
-An optional flag can be sent to the `view-frc` program that will save the plot:
-`view-frc -s <file.nc>`.
-
-In either case a `data/output` directory will be created inside the current directory
-when something is saved.
+All created files are saved to a `data/output` directory that will be created inside the
+current directory from where the `volcano-cooking` command is run.
 
-For more options to either `volcano-cooking` or `view-frc`, see
+For more information, see
 
-```sh
+```bash
 volcano-cooking --help
-view-frc --help
 ```
 
-### Examples
-
-When running the command `volcano-cooking --run-ncl`, a few environment variables will
-be used, which can be controlled by setting them in a `.env` file. See
-[`.env.example`](./examples/.env.example) to see some default values. With this you can
-for example easily change the grid resolution to be `1deg` rather than `2deg` (default).
-
-The [__examples__](./examples/) directory also include an example on how to use the
-`--file` option. Cloning this repository and running `volcano-cooking --file json.json`
-from *inside* the __examples__ directory will result in some output files generated to a
-new __data__ directory inside __examples__. If you further rename `.env.example` →
-`.env` you may also run `volcano-cooking --run-ncl` and `volcano-cooking --package-last`
-(this assumes you follow option 0, see below).
-
-Finally, there is also a script [`custom_generator.py`](./examples/custom_generator.py)
-which show how you might define your own generator classes and functions. Run as `python
-custom_generator.py`.
-
-### Option 0 (default, using NCL-script)
+#### Option 0 (default, using NCL-script)
 
-#### TL;DR
+##### TL;DR
 
 ```console
 $ volcano-cooking -f 1 -s 100
 Generating with 'GenerateFPP'...
 $ volcano-cooking --run-ncl
  Copyright (C) 1995-2019 - All Rights Reserved
  University Corporation for Atmospheric Research
@@ -103,55 +85,54 @@
 $ volcano-cooking --package-last
 Successfully placed all latest source files in the 'source-files' directory.
 $ ls source-files
 20220502-140022.log                     VolcanEESMv3.11Enger_SO2_850-2016_Mscale_Zreduc_2deg_c20220502-140023.nc
 synthetic_volcanoes_20220502_135956.nc  synthetic_volcanoes_20220502_135956.npz
 ```
 
-#### Dependencies
+##### Dependencies
 
 This option needs
 
 - `volcano-cooking` installed
 - A coordinate file (~ 10 kB)
 - [`ncl`](https://www.ncl.ucar.edu/Download/) executable
 
-#### Create source file for forcing
+##### Create source file for forcing
 
 Run command `volcano-cooking` with the options you want. See `volcano-cooking --help`.
 
-#### Create forcing file for CESM2
+##### Create forcing file for CESM2
 
-> Running the [_script/create_cesm_frc.sh](_script/create_cesm_frc.sh) script depends on
-> having `ncl` installed. See installation instructions
-> [here](https://www.ncl.ucar.edu/Download/).
+> Running the `volcano-cooking --run-ncl` script depends on having `ncl` installed. See
+> installation instructions [here](https://www.ncl.ucar.edu/Download/).
 
 After having run the `volcano-cooking` command, the forcing file for CESM2 can be
 generated by running
 
 ```bash
 volcano-cooking --run-ncl
 ```
 
 If the needed coordinate files are missing, you will be asked if you want to download
 them. If you want to use different files, or change the default resolution (default is 2
-degrees), edit [.env](./.env.example) accordingly. In this case, you also need to
-manually download whatever coordinate file you want to use. See section [Setting up
-manually](#setting-up-manually).
+degrees), edit __.env__ (see [__./examples/.env.example__](./examples/.env.example))
+accordingly. In this case, you also need to manually download whatever coordinate file
+you want to use. See section [Setting up manually](#setting-up-manually).
 
-#### Wrap up
+##### Wrap up
 
 The last created files, source files, logs and final output, can be nicely collected and
 placed in a directory named `source-files` with command:
 
 ```sh
 volcano-cooking --package-last
 ```
 
-<details><summary><h4>Setting up manually</h4></summary><br>
+<details><summary><h5>Setting up manually</h5></summary><br>
 
 To be able to create forcing files used by CESM2 from the newly created synthetic file,
 we need a script from the [emissions][data_source_files] directory. These are scripts
 that use the forcing file this project generates to make a new, full forcing file that
 CESM2 accepts (examples of such files can be found [here][volc-frc-complete]). For
 example, `createVolcEruptV3.ncl` can be found in the [emissions][data_source_files]
 directory. This need a `common.ncl` file, found [here][common-ncl], in addition to other
@@ -171,41 +152,41 @@
 ```bash
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals
 ```
 
 </details>
 
-### Option 1 (directly change forcing file)
+#### Option 1 (directly change forcing file)
 
-#### TL;DR
+##### TL;DR
 
 ```console
 $ volcano-cooking -f 1 -s 100 -o
 Generating with 'GenerateFPP'...
 ```
 
-#### Dependencies
+##### Dependencies
 
 This option needs
 
 - `volcano-cooking` installed
 - A coordinate file (~ 10 kB)
 - Original CESM2 forcing file (~ 2.2 GB)
 
-#### Run library
+##### Run library
 
 Now the only thing we need to do is running `volcano-cooking` with the flag `-o`, and
 choose the type of forcing we want (see `volcano-cooking --lst`):
 
 ```bash
 volcano-cooking -f 1 -s 100 -o
 ```
 
-<details><summary><h4>Get forcing and coordinate files manually</h4></summary><br>
+<details><summary><h5>Get forcing and coordinate files manually</h5></summary><br>
 
 > Manually downloading the files and placing them in the correct directory is *not*
 > needed. Running the command as shown above will ask you if you want to download the
 > files, and place them where they need to be.
 
 This option relies on having a working forcing file and coordinate file at hand. We will
 use the forcing file that CESM2 places in the `stratvolc` directory of the `cam` model.
@@ -224,16 +205,66 @@
 ```bash
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals
 ```
 
 </details>
 
+#### Examples
+
+When running the command `volcano-cooking --run-ncl`, a few environment variables will
+be used, which can be controlled by setting them in a `.env` file. See
+[`.env.example`](./examples/.env.example) to see some default values. With this you can
+for example easily change the grid resolution to be `1deg` rather than `2deg` (default).
+
+The [__examples__](./examples/) directory also include an example on how to use the
+`--file` option. Cloning this repository and running `volcano-cooking --file json.json`
+from *inside* the __examples__ directory will result in some output files generated to a
+new __data__ directory inside __examples__. If you further rename `.env.example` →
+`.env` you may also run `volcano-cooking --run-ncl` and `volcano-cooking --package-last`
+(this assumes you follow option 0, see below).
+
+Finally, there is also a script [`custom_generator.py`](./examples/custom_generator.py)
+which show how you might define your own generator classes and functions. Run as `python
+custom_generator.py`.
+
+### `view-frc`
+
+After running the `volcano-cooking` command, files with names `synthetic_volcanoes_...`
+are created with file type `.nc` and `.npz`. These can be viewed with
+
+```bash
+view-frc <file.nc>
+```
+
+An optional flag can be sent to the `view-frc` program that will save the plot:
+`view-frc -s <file.nc>`.
+
+For more information, see
+
+```bash
+view-frc --help
+```
+
+### `sfrc-sparse2lin`
+
+This program is available as a convenience tool in the rare case when you have a forcing
+file with only the events of eruptions. The program will re-write time array to be
+linearly spaced and place the values from the forcing values into a new forcing array
+that matches the new linearly spaced time axis.
+
+It assumes the file sent to it has `yoes`(year, YYYY), `moes` (month, MM), `does`
+(days, DD) and `tes` (emissions, Tg) fields if it is a `.npz` file. If a `.nc` file is
+used, it must have a dataset with variables "Year_of_Emission", "Month_of_Emission",
+"Day_of_Emission" and "Total_Emission".
+
 ## Extra
 
+This assumes you are using the package from a python script, and not just the CLI.
+
 ### Compare created file with a similar used in a default CESM2 experiment
 
 A similar file to those that are created is needed to be able to use some scripts in the
 `helper_scripts` directory. By default, it assumes the file is named
 `volcan-eesm_global_2015_so2-emissions-database_v1.0.nc` and that it is placed inside
 the `data/originals` directory. You can find this file [here][volc-frc].
 
@@ -245,27 +276,26 @@
 ```bash
 git clone https://github.com/engeir/volcano-cooking.git
 cd volcano-cooking
 poetry install
 pre-commit install
 ```
 
-Before committing new changes to a branch you can run command
+Before committing new changes to a branch you may run the full test suite with:
 
 ```bash
 nox
 ```
 
-to run the full test suite. You will need [Poetry], [nox] and [nox-poetry] installed for
-this.
+You will need [Poetry], [nox] and [nox-poetry] installed for this.
 
-[data_source_files]: https://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission
 [common-ncl]: http://svn.code.sf.net/p/codescripts/code/trunk/ncl/lib/common.ncl
 [coord-file]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/
-[coords-repo]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/share/scripgrids/
-[volc-frc]: http://catalogue.ceda.ac.uk/uuid/bfbd5ec825fa422f9a858b14ae7b2a0d
-[volc-frc-complete]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/
-[stratvolc-forcing]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc
-[pypi]: https://pypi.org/
-[nox]: https://nox.thea.codes/en/stable/
+[data_source_files]: https://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission
 [nox-poetry]: https://nox-poetry.readthedocs.io/
+[nox]: https://nox.thea.codes/en/stable/
+[pipx-source]: https://github.com/pypa/pipx
 [poetry]: https://python-poetry.org
+[pypi]: https://pypi.org/
+[stratvolc-forcing]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc
+[volc-frc-complete]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/
+[volc-frc]: http://catalogue.ceda.ac.uk/uuid/bfbd5ec825fa422f9a858b14ae7b2a0d
```

### Comparing `volcano_cooking-0.9.2/pyproject.toml` & `volcano_cooking-0.9.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volcano-cooking"
-version = "0.9.2"
+version = "0.9.3"
 description = "Make some volcanoes and simulate them in CESM2"
 authors = ["engeir <eirroleng@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 volcano-cooking = "volcano_cooking.__main__:main"
@@ -17,32 +17,32 @@
 scipy = "^1.7.1"
 matplotlib = "^3.4.2"
 PyWavelets = "^1.1.1"
 click = "^8.0.1"
 cftime = "^1.5.0"
 netCDF4 = "^1.5.8"
 superposed-pulses = "^1.2"
-xarray = ">=0.21.1,<2022.11.0"
+xarray = ">=0.21.1,<2022.12.0"
 wget = "^3.2"
 dask = "^2022.3.0"
 cosmoplots = "^0.1.5"
 importlib-metadata = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.5"
 black = "^22.10"
 isort = "^5.9.3"
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
 pre-commit-hooks = "^4.3.0"
-pyupgrade = "^3.1.0"
+pyupgrade = "^3.2.2"
 darglint = "^1.8.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
-mypy = "^0.982"
+mypy = "^0.991"
 xdoctest = "^1.1.0"
 Pygments = "^2.13.0"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
```

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/__main__.py` & `volcano_cooking-0.9.3/src/volcano_cooking/__main__.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/configurations/shift_eruption_to_date.py` & `volcano_cooking-0.9.3/src/volcano_cooking/configurations/shift_eruption_to_date.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/createVolcEruptV3.ncl` & `volcano_cooking-0.9.3/src/volcano_cooking/createVolcEruptV3.ncl`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/create_cesm_frc.sh` & `volcano_cooking-0.9.3/src/volcano_cooking/create_cesm_frc.sh`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/compare_datasets.py` & `volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/compare_datasets.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/compare_volc_files.py` & `volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/compare_volc_files.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/functions.py` & `volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/functions.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/inspect_X-vs-Y.py` & `volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/inspect_X-vs-Y.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/inspect_year.py` & `volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/inspect_year.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/helper_scripts/view_generated_forcing.py` & `volcano_cooking-0.9.3/src/volcano_cooking/helper_scripts/view_generated_forcing.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/convert/adjust_emissions_and_heights.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/convert/adjust_emissions_and_heights.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/convert/convert_between_variables.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/convert/convert_between_variables.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/create/create_data.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/create/create_data.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/create/create_dates.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/create/create_dates.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/create/create_frc.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/create/create_frc.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/create/easy_fix.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/create/easy_fix.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/modules/create/rewrite_frc_file.py` & `volcano_cooking-0.9.3/src/volcano_cooking/modules/create/rewrite_frc_file.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/package_last.sh` & `volcano_cooking-0.9.3/src/volcano_cooking/package_last.sh`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/parse_stratvolc.py` & `volcano_cooking-0.9.3/src/volcano_cooking/parse_stratvolc.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/plotting/figure_standards.py` & `volcano_cooking-0.9.3/src/volcano_cooking/plotting/figure_standards.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/sparse_to_lin.py` & `volcano_cooking-0.9.3/src/volcano_cooking/sparse_to_lin.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     -------
     np.ndarray:
         The new linearly spaced time axis
     list:
         Masking of the original time axis that give the time stamps we want to
         keep that match best with the new time axis
     list:
-        Masking of the new new time axis that give the time stamps kept from
-        the original
+        Masking of the new time axis that give the time stamps kept from the original
 
     Examples
     --------
     >>> t = np.array(
     >>>     [
     >>>         0, 1e-3, 2e-3, 3e-3, 4e-3, 5e-3, 4, 6, 7.85, 7.91,
     >>>         7.92, 7.925, 7.93, 7.96, 7.99, 8.001, 8.002, 8.003,
@@ -69,20 +68,28 @@
         : -int(remove * samples_per_year / 12)
     ]
     # Find indices in `t_i` that are closest to `t`. If one element in `t_i` is closest
     # to two or more elements in `t`, only the one closest in `t` is kept (avoid
     # repetition of indices).
     # Make `t` a row vector (1, N) and `t_i` a column vector (M, 1), compute the
     # absolute difference -> (M, N) and pick the minimum along N -> (N,)
+    # `mask` represents which index of the new linspaced time array the given element of
+    # the original time array is closest. `mask_idx` represents unique elements of the
+    # new time array that should be used, and `mask_sections` represents the cluster of
+    # elements in the original that are closest to a given element of the new linspaced
+    # time array.
     mask = np.abs(t[None, :] - t_i[:, None]).argmin(axis=0)
     _, mask_idx = np.unique(mask, return_index=True)
-    mask_sections = [mask[m : mask_idx[i + 1]] for i, m in enumerate(mask_idx[:-1])]
-    if not mask_sections:
-        return t_i, [], []
-    mask_sections.append(mask[mask_idx[-1] :])
+    if len(t) == 1:
+        mask_sections = [mask[mask_idx[-1] :]]
+    else:
+        mask_sections = [mask[m : mask_idx[i + 1]] for i, m in enumerate(mask_idx[:-1])]
+        if not mask_sections:
+            return t_i, [], []
+        mask_sections.append(mask[mask_idx[-1] :])
     # Now we find the indices of `t` that we want to keep. `c` works as the index of the
     # first item in each array inside mask_sections
     c = 0
     t_mask: List[int] = []
     t_mask_app = t_mask.append
     ti_mask: List[int] = []
     ti_mask_app = ti_mask.append
@@ -149,33 +156,15 @@
     save: bool,
     show: bool,
     sy: int,
     ey: int,
     samples_per_year: int,
     lm: str,
 ):
-    """View a plot of `filename`.
-
-    Parameters
-    ----------
-    filename: str
-        Name of the file you want plotted
-    save: bool
-        Save the arrays to a .npz file. Defaults to False
-    show: bool
-        Show a plot of the original and new volcanic forcing arrays
-    sy: int
-        The assumed first year of the time axis
-    ey: int
-        The assumed end year of the time axis
-    samples_per_year: int
-        The number of samples per year.
-    lm: str
-        The last month of the last year
-    """
+    """View a plot of `filename`."""
     # Decide on the last month
     lm = lm.lower()
     # fmt: off
     months = {
         "jan": 1, "feb": 2, "mar": 3, "apr": 4, "may": 5, "jun": 6,
         "jul": 7, "aug": 8, "sep": 9, "oct": 10, "nov": 11, "dec": 12,
     }
```

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/synthetic_volcanoes.py` & `volcano_cooking-0.9.3/src/volcano_cooking/synthetic_volcanoes.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/src/volcano_cooking/view_force.py` & `volcano_cooking-0.9.3/src/volcano_cooking/view_force.py`

 * *Files identical despite different names*

### Comparing `volcano_cooking-0.9.2/setup.py` & `volcano_cooking-0.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,26 @@
  'importlib-metadata>=5.0.0,<6.0.0',
  'matplotlib>=3.4.2,<4.0.0',
  'netCDF4>=1.5.8,<2.0.0',
  'numpy>=1.21.1,<2.0.0',
  'scipy>=1.7.1,<2.0.0',
  'superposed-pulses>=1.2,<2.0',
  'wget>=3.2,<4.0',
- 'xarray>=0.21.1,<2022.11.0']
+ 'xarray>=0.21.1,<2022.12.0']
 
 entry_points = \
 {'console_scripts': ['sfrc-sparse2lin = volcano_cooking.sparse_to_lin:main',
                      'view-frc = volcano_cooking.view_force:main',
                      'volcano-cooking = volcano_cooking.__main__:main']}
 
 setup_kwargs = {
     'name': 'volcano-cooking',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Make some volcanoes and simulate them in CESM2',
-    'long_description': "# Volcano Cooking\n\n[![PyPI version](https://img.shields.io/pypi/v/volcano-cooking)](https://pypi.org/project/volcano-cooking/)\n[![codecov](https://codecov.io/gh/engeir/volcano-cooking/branch/main/graph/badge.svg?token=8I5VE7LYA4)](https://codecov.io/gh/engeir/volcano-cooking)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n> Let's make some volcanoes erupt!\n\n[![asciicast](https://asciinema.org/a/6eOsLnlOikscbXYLJqclxytD3.svg)](https://asciinema.org/a/6eOsLnlOikscbXYLJqclxytD3)\n\n__NOTE:__\nThe created dates *must* start before the model start. Running CESM2 from year 1850 with\nthe first eruption in 1850 will make it crash. Setting the first eruption to 1849,\nhowever, will make it run. The same goes for the end, the model must stop prior to the\nlast event, otherwise it will crash. This project will make sure one event is placed\nahead of the `init` year, but the end will vary depending on number of events created\nand their frequency.\n\n## Install\n\nThe package is published on [PyPI] and installable via `pip`:\n\n```bash\npip install volcano-cooking\n```\n\n## Usage\n\n### The basics\n\nThere are two CLI programs coming with this project. The main program is\n`volcano-cooking`, which will create a `.nc` and `.npz` file in the `data/output`\ndirectory. With the `view_frc` program you can quickly view the content of the created\nfiles in a plot.\n\nRun from within this repository/directory via poetry:\n\n```sh\npoetry run volcano-cooking\npoetry run view-frc <file.nc>\n```\n\nor, if the virtual environment where the project is installed is activated:\n\n```sh\nvolcano-cooking\nview-frc <file.nc>\n```\n\nAn optional flag can be sent to the `view-frc` program that will save the plot:\n`view-frc -s <file.nc>`.\n\nIn either case a `data/output` directory will be created inside the current directory\nwhen something is saved.\n\nFor more options to either `volcano-cooking` or `view-frc`, see\n\n```sh\nvolcano-cooking --help\nview-frc --help\n```\n\n### Examples\n\nWhen running the command `volcano-cooking --run-ncl`, a few environment variables will\nbe used, which can be controlled by setting them in a `.env` file. See\n[`.env.example`](./examples/.env.example) to see some default values. With this you can\nfor example easily change the grid resolution to be `1deg` rather than `2deg` (default).\n\nThe [__examples__](./examples/) directory also include an example on how to use the\n`--file` option. Cloning this repository and running `volcano-cooking --file json.json`\nfrom *inside* the __examples__ directory will result in some output files generated to a\nnew __data__ directory inside __examples__. If you further rename `.env.example` →\n`.env` you may also run `volcano-cooking --run-ncl` and `volcano-cooking --package-last`\n(this assumes you follow option 0, see below).\n\nFinally, there is also a script [`custom_generator.py`](./examples/custom_generator.py)\nwhich show how you might define your own generator classes and functions. Run as `python\ncustom_generator.py`.\n\n### Option 0 (default, using NCL-script)\n\n#### TL;DR\n\n```console\n$ volcano-cooking -f 1 -s 100\nGenerating with 'GenerateFPP'...\n$ volcano-cooking --run-ncl\n Copyright (C) 1995-2019 - All Rights Reserved\n University Corporation for Atmospheric Research\n NCAR Command Language Version 6.6.2\n The use of this software is governed by a License Agreement.\n See http://www.ncl.ucar.edu/ for more details.\n(0)     in data/originals/createVolcEruptV3.ncl\n...\n  long_name :   SO2 elevated emissions from explosive volcanoes\n  _FillValue :  9.96921e+36\n(0)     saving stratvolc\n(0)     File creation complete: data/cesm/VolcanEESMv3.11Enger_SO2_850-2016_Mscale_Zreduc_2deg_c20220502-140023.nc\nLog file created at data/cesm/logs/20220502-140022.log\nFixing the attributes of the altitude_int coordinate...\n$ volcano-cooking --package-last\nSuccessfully placed all latest source files in the 'source-files' directory.\n$ ls source-files\n20220502-140022.log                     VolcanEESMv3.11Enger_SO2_850-2016_Mscale_Zreduc_2deg_c20220502-140023.nc\nsynthetic_volcanoes_20220502_135956.nc  synthetic_volcanoes_20220502_135956.npz\n```\n\n#### Dependencies\n\nThis option needs\n\n- `volcano-cooking` installed\n- A coordinate file (~ 10 kB)\n- [`ncl`](https://www.ncl.ucar.edu/Download/) executable\n\n#### Create source file for forcing\n\nRun command `volcano-cooking` with the options you want. See `volcano-cooking --help`.\n\n#### Create forcing file for CESM2\n\n> Running the [_script/create_cesm_frc.sh](_script/create_cesm_frc.sh) script depends on\n> having `ncl` installed. See installation instructions\n> [here](https://www.ncl.ucar.edu/Download/).\n\nAfter having run the `volcano-cooking` command, the forcing file for CESM2 can be\ngenerated by running\n\n```bash\nvolcano-cooking --run-ncl\n```\n\nIf the needed coordinate files are missing, you will be asked if you want to download\nthem. If you want to use different files, or change the default resolution (default is 2\ndegrees), edit [.env](./.env.example) accordingly. In this case, you also need to\nmanually download whatever coordinate file you want to use. See section [Setting up\nmanually](#setting-up-manually).\n\n#### Wrap up\n\nThe last created files, source files, logs and final output, can be nicely collected and\nplaced in a directory named `source-files` with command:\n\n```sh\nvolcano-cooking --package-last\n```\n\n<details><summary><h4>Setting up manually</h4></summary><br>\n\nTo be able to create forcing files used by CESM2 from the newly created synthetic file,\nwe need a script from the [emissions][data_source_files] directory. These are scripts\nthat use the forcing file this project generates to make a new, full forcing file that\nCESM2 accepts (examples of such files can be found [here][volc-frc-complete]). For\nexample, `createVolcEruptV3.ncl` can be found in the [emissions][data_source_files]\ndirectory. This need a `common.ncl` file, found [here][common-ncl], in addition to other\nstandard `ncl` libraries. Make sure to edit `createVolcEruptV3.ncl` to read the created\nfile and that the first and last year cover those used in the created file. A working\nversion of `createVolcEruptV3.ncl` that uses input files generated by `volcano-cooking`\ncan be found in [data/originals](data/originals). To see what was changed from the\noriginal, run `diff data/originals/createVolcEruptV3.ncl.original\nsrc/volcano_cooking/createVolcEruptV3.ncl`.\n\nCoordinate files are needed when running `createVolcEruptV3.ncl` or similar scripts, and\nare located [here][coord-file]. For example `fv_1.9x2.5_L30.nc` which can be used with\ntwo degrees resolution in the atmosphere model. The following commands will download\n1 and 2 degree resolution coordinate files, respectively, to the `data/originals`\ndirectory:\n\n```bash\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals\n```\n\n</details>\n\n### Option 1 (directly change forcing file)\n\n#### TL;DR\n\n```console\n$ volcano-cooking -f 1 -s 100 -o\nGenerating with 'GenerateFPP'...\n```\n\n#### Dependencies\n\nThis option needs\n\n- `volcano-cooking` installed\n- A coordinate file (~ 10 kB)\n- Original CESM2 forcing file (~ 2.2 GB)\n\n#### Run library\n\nNow the only thing we need to do is running `volcano-cooking` with the flag `-o`, and\nchoose the type of forcing we want (see `volcano-cooking --lst`):\n\n```bash\nvolcano-cooking -f 1 -s 100 -o\n```\n\n<details><summary><h4>Get forcing and coordinate files manually</h4></summary><br>\n\n> Manually downloading the files and placing them in the correct directory is *not*\n> needed. Running the command as shown above will ask you if you want to download the\n> files, and place them where they need to be.\n\nThis option relies on having a working forcing file and coordinate file at hand. We will\nuse the forcing file that CESM2 places in the `stratvolc` directory of the `cam` model.\nDownload from [this link][stratvolc-forcing] and place it in the `data/originals`\ndirectory, or run command:\n\n```bash\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc --directory-prefix data/originals\n```\n\nIt's 2.2\xa0GB file, so it will take some time.\n\nWe will also need a coordinate file, specifically `fv_1.9x2.5_L30.nc` which is found\n[here][coord-file]. This file is small and quick to download. From the command line:\n\n```bash\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals\n```\n\n</details>\n\n## Extra\n\n### Compare created file with a similar used in a default CESM2 experiment\n\nA similar file to those that are created is needed to be able to use some scripts in the\n`helper_scripts` directory. By default, it assumes the file is named\n`volcan-eesm_global_2015_so2-emissions-database_v1.0.nc` and that it is placed inside\nthe `data/originals` directory. You can find this file [here][volc-frc].\n\n## Contributing\n\nTo contribute to the project, clone and install the full development version (uses\n[poetry] for dependencies):\n\n```bash\ngit clone https://github.com/engeir/volcano-cooking.git\ncd volcano-cooking\npoetry install\npre-commit install\n```\n\nBefore committing new changes to a branch you can run command\n\n```bash\nnox\n```\n\nto run the full test suite. You will need [Poetry], [nox] and [nox-poetry] installed for\nthis.\n\n[data_source_files]: https://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission\n[common-ncl]: http://svn.code.sf.net/p/codescripts/code/trunk/ncl/lib/common.ncl\n[coord-file]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/\n[coords-repo]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/share/scripgrids/\n[volc-frc]: http://catalogue.ceda.ac.uk/uuid/bfbd5ec825fa422f9a858b14ae7b2a0d\n[volc-frc-complete]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/\n[stratvolc-forcing]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc\n[pypi]: https://pypi.org/\n[nox]: https://nox.thea.codes/en/stable/\n[nox-poetry]: https://nox-poetry.readthedocs.io/\n[poetry]: https://python-poetry.org\n",
+    'long_description': '# Volcano Cooking\n\n[![PyPI version](https://img.shields.io/pypi/v/volcano-cooking)](https://pypi.org/project/volcano-cooking/)\n[![codecov](https://codecov.io/gh/engeir/volcano-cooking/branch/main/graph/badge.svg?token=8I5VE7LYA4)](https://codecov.io/gh/engeir/volcano-cooking)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n> Let\'s make some volcanoes erupt!\n\n[![asciicast](https://asciinema.org/a/6eOsLnlOikscbXYLJqclxytD3.svg)](https://asciinema.org/a/6eOsLnlOikscbXYLJqclxytD3)\n\n__NOTE:__\nThe created dates *must* start before the model start. Running CESM2 from year 1850 with\nthe first eruption in 1850 will make it crash. Setting the first eruption to 1849,\nhowever, will make it run. The same goes for the end, the model must stop prior to the\nlast event, otherwise it will crash. This project will make sure one event is placed\nahead of the `init` year, but the end will vary depending on number of events created\nand their frequency.\n\n## Install\n\nThe package is published on [PyPI] and installable via `pip`:\n\n```bash\npip install volcano-cooking\n```\n\n<!-- FIXME: add reference to available classes -->\nIf you only plan on using the already present generator classes and only need the CLI\nprogram, it is recommended to install this with [pipx][pipx-source]:\n\n```bash\npipx install volcano-cooking\n```\n\n## Usage\n\n### The basics\n\nThere are mainly two CLI programs coming with this project. The main program is\n`volcano-cooking`, which will create a `.nc` and `.npz` file in the `data/output`\ndirectory. With the `view-frc` program you can quickly view the content of the created\nfiles in a plot. There is also a third program called `sfrc-sparse2lin` which converts\narrays of only non-zero events at arbitrary times to linearly spaced events where times\nbetween the non-zero events are filled with zeros.\n\n### `volcano-cooking`\n\nOnce installed, run from within this directory with:\n\n```bash\nvolcano-cooking\n```\n\nAll created files are saved to a `data/output` directory that will be created inside the\ncurrent directory from where the `volcano-cooking` command is run.\n\nFor more information, see\n\n```bash\nvolcano-cooking --help\n```\n\n#### Option 0 (default, using NCL-script)\n\n##### TL;DR\n\n```console\n$ volcano-cooking -f 1 -s 100\nGenerating with \'GenerateFPP\'...\n$ volcano-cooking --run-ncl\n Copyright (C) 1995-2019 - All Rights Reserved\n University Corporation for Atmospheric Research\n NCAR Command Language Version 6.6.2\n The use of this software is governed by a License Agreement.\n See http://www.ncl.ucar.edu/ for more details.\n(0)     in data/originals/createVolcEruptV3.ncl\n...\n  long_name :   SO2 elevated emissions from explosive volcanoes\n  _FillValue :  9.96921e+36\n(0)     saving stratvolc\n(0)     File creation complete: data/cesm/VolcanEESMv3.11Enger_SO2_850-2016_Mscale_Zreduc_2deg_c20220502-140023.nc\nLog file created at data/cesm/logs/20220502-140022.log\nFixing the attributes of the altitude_int coordinate...\n$ volcano-cooking --package-last\nSuccessfully placed all latest source files in the \'source-files\' directory.\n$ ls source-files\n20220502-140022.log                     VolcanEESMv3.11Enger_SO2_850-2016_Mscale_Zreduc_2deg_c20220502-140023.nc\nsynthetic_volcanoes_20220502_135956.nc  synthetic_volcanoes_20220502_135956.npz\n```\n\n##### Dependencies\n\nThis option needs\n\n- `volcano-cooking` installed\n- A coordinate file (~ 10 kB)\n- [`ncl`](https://www.ncl.ucar.edu/Download/) executable\n\n##### Create source file for forcing\n\nRun command `volcano-cooking` with the options you want. See `volcano-cooking --help`.\n\n##### Create forcing file for CESM2\n\n> Running the `volcano-cooking --run-ncl` script depends on having `ncl` installed. See\n> installation instructions [here](https://www.ncl.ucar.edu/Download/).\n\nAfter having run the `volcano-cooking` command, the forcing file for CESM2 can be\ngenerated by running\n\n```bash\nvolcano-cooking --run-ncl\n```\n\nIf the needed coordinate files are missing, you will be asked if you want to download\nthem. If you want to use different files, or change the default resolution (default is 2\ndegrees), edit __.env__ (see [__./examples/.env.example__](./examples/.env.example))\naccordingly. In this case, you also need to manually download whatever coordinate file\nyou want to use. See section [Setting up manually](#setting-up-manually).\n\n##### Wrap up\n\nThe last created files, source files, logs and final output, can be nicely collected and\nplaced in a directory named `source-files` with command:\n\n```sh\nvolcano-cooking --package-last\n```\n\n<details><summary><h5>Setting up manually</h5></summary><br>\n\nTo be able to create forcing files used by CESM2 from the newly created synthetic file,\nwe need a script from the [emissions][data_source_files] directory. These are scripts\nthat use the forcing file this project generates to make a new, full forcing file that\nCESM2 accepts (examples of such files can be found [here][volc-frc-complete]). For\nexample, `createVolcEruptV3.ncl` can be found in the [emissions][data_source_files]\ndirectory. This need a `common.ncl` file, found [here][common-ncl], in addition to other\nstandard `ncl` libraries. Make sure to edit `createVolcEruptV3.ncl` to read the created\nfile and that the first and last year cover those used in the created file. A working\nversion of `createVolcEruptV3.ncl` that uses input files generated by `volcano-cooking`\ncan be found in [data/originals](data/originals). To see what was changed from the\noriginal, run `diff data/originals/createVolcEruptV3.ncl.original\nsrc/volcano_cooking/createVolcEruptV3.ncl`.\n\nCoordinate files are needed when running `createVolcEruptV3.ncl` or similar scripts, and\nare located [here][coord-file]. For example `fv_1.9x2.5_L30.nc` which can be used with\ntwo degrees resolution in the atmosphere model. The following commands will download\n1 and 2 degree resolution coordinate files, respectively, to the `data/originals`\ndirectory:\n\n```bash\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals\n```\n\n</details>\n\n#### Option 1 (directly change forcing file)\n\n##### TL;DR\n\n```console\n$ volcano-cooking -f 1 -s 100 -o\nGenerating with \'GenerateFPP\'...\n```\n\n##### Dependencies\n\nThis option needs\n\n- `volcano-cooking` installed\n- A coordinate file (~ 10 kB)\n- Original CESM2 forcing file (~ 2.2 GB)\n\n##### Run library\n\nNow the only thing we need to do is running `volcano-cooking` with the flag `-o`, and\nchoose the type of forcing we want (see `volcano-cooking --lst`):\n\n```bash\nvolcano-cooking -f 1 -s 100 -o\n```\n\n<details><summary><h5>Get forcing and coordinate files manually</h5></summary><br>\n\n> Manually downloading the files and placing them in the correct directory is *not*\n> needed. Running the command as shown above will ask you if you want to download the\n> files, and place them where they need to be.\n\nThis option relies on having a working forcing file and coordinate file at hand. We will\nuse the forcing file that CESM2 places in the `stratvolc` directory of the `cam` model.\nDownload from [this link][stratvolc-forcing] and place it in the `data/originals`\ndirectory, or run command:\n\n```bash\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc --directory-prefix data/originals\n```\n\nIt\'s 2.2\xa0GB file, so it will take some time.\n\nWe will also need a coordinate file, specifically `fv_1.9x2.5_L30.nc` which is found\n[here][coord-file]. This file is small and quick to download. From the command line:\n\n```bash\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals\nwget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals\n```\n\n</details>\n\n#### Examples\n\nWhen running the command `volcano-cooking --run-ncl`, a few environment variables will\nbe used, which can be controlled by setting them in a `.env` file. See\n[`.env.example`](./examples/.env.example) to see some default values. With this you can\nfor example easily change the grid resolution to be `1deg` rather than `2deg` (default).\n\nThe [__examples__](./examples/) directory also include an example on how to use the\n`--file` option. Cloning this repository and running `volcano-cooking --file json.json`\nfrom *inside* the __examples__ directory will result in some output files generated to a\nnew __data__ directory inside __examples__. If you further rename `.env.example` →\n`.env` you may also run `volcano-cooking --run-ncl` and `volcano-cooking --package-last`\n(this assumes you follow option 0, see below).\n\nFinally, there is also a script [`custom_generator.py`](./examples/custom_generator.py)\nwhich show how you might define your own generator classes and functions. Run as `python\ncustom_generator.py`.\n\n### `view-frc`\n\nAfter running the `volcano-cooking` command, files with names `synthetic_volcanoes_...`\nare created with file type `.nc` and `.npz`. These can be viewed with\n\n```bash\nview-frc <file.nc>\n```\n\nAn optional flag can be sent to the `view-frc` program that will save the plot:\n`view-frc -s <file.nc>`.\n\nFor more information, see\n\n```bash\nview-frc --help\n```\n\n### `sfrc-sparse2lin`\n\nThis program is available as a convenience tool in the rare case when you have a forcing\nfile with only the events of eruptions. The program will re-write time array to be\nlinearly spaced and place the values from the forcing values into a new forcing array\nthat matches the new linearly spaced time axis.\n\nIt assumes the file sent to it has `yoes`(year, YYYY), `moes` (month, MM), `does`\n(days, DD) and `tes` (emissions, Tg) fields if it is a `.npz` file. If a `.nc` file is\nused, it must have a dataset with variables "Year_of_Emission", "Month_of_Emission",\n"Day_of_Emission" and "Total_Emission".\n\n## Extra\n\nThis assumes you are using the package from a python script, and not just the CLI.\n\n### Compare created file with a similar used in a default CESM2 experiment\n\nA similar file to those that are created is needed to be able to use some scripts in the\n`helper_scripts` directory. By default, it assumes the file is named\n`volcan-eesm_global_2015_so2-emissions-database_v1.0.nc` and that it is placed inside\nthe `data/originals` directory. You can find this file [here][volc-frc].\n\n## Contributing\n\nTo contribute to the project, clone and install the full development version (uses\n[poetry] for dependencies):\n\n```bash\ngit clone https://github.com/engeir/volcano-cooking.git\ncd volcano-cooking\npoetry install\npre-commit install\n```\n\nBefore committing new changes to a branch you may run the full test suite with:\n\n```bash\nnox\n```\n\nYou will need [Poetry], [nox] and [nox-poetry] installed for this.\n\n[common-ncl]: http://svn.code.sf.net/p/codescripts/code/trunk/ncl/lib/common.ncl\n[coord-file]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/\n[data_source_files]: https://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission\n[nox-poetry]: https://nox-poetry.readthedocs.io/\n[nox]: https://nox.thea.codes/en/stable/\n[pipx-source]: https://github.com/pypa/pipx\n[poetry]: https://python-poetry.org\n[pypi]: https://pypi.org/\n[stratvolc-forcing]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc\n[volc-frc-complete]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/\n[volc-frc]: http://catalogue.ceda.ac.uk/uuid/bfbd5ec825fa422f9a858b14ae7b2a0d\n',
     'author': 'engeir',
     'author_email': 'eirroleng@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `volcano_cooking-0.9.2/PKG-INFO` & `volcano_cooking-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volcano-cooking
-Version: 0.9.2
+Version: 0.9.3
 Summary: Make some volcanoes and simulate them in CESM2
 License: GPL-3.0-or-later
 Author: engeir
 Author-email: eirroleng@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: importlib-metadata (>=5.0.0,<6.0.0)
 Requires-Dist: matplotlib (>=3.4.2,<4.0.0)
 Requires-Dist: netCDF4 (>=1.5.8,<2.0.0)
 Requires-Dist: numpy (>=1.21.1,<2.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: superposed-pulses (>=1.2,<2.0)
 Requires-Dist: wget (>=3.2,<4.0)
-Requires-Dist: xarray (>=0.21.1,<2022.11.0)
+Requires-Dist: xarray (>=0.21.1,<2022.12.0)
 Description-Content-Type: text/markdown
 
 # Volcano Cooking
 
 [![PyPI version](https://img.shields.io/pypi/v/volcano-cooking)](https://pypi.org/project/volcano-cooking/)
 [![codecov](https://codecov.io/gh/engeir/volcano-cooking/branch/main/graph/badge.svg?token=8I5VE7LYA4)](https://codecov.io/gh/engeir/volcano-cooking)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
@@ -49,71 +49,53 @@
 
 The package is published on [PyPI] and installable via `pip`:
 
 ```bash
 pip install volcano-cooking
 ```
 
+<!-- FIXME: add reference to available classes -->
+If you only plan on using the already present generator classes and only need the CLI
+program, it is recommended to install this with [pipx][pipx-source]:
+
+```bash
+pipx install volcano-cooking
+```
+
 ## Usage
 
 ### The basics
 
-There are two CLI programs coming with this project. The main program is
+There are mainly two CLI programs coming with this project. The main program is
 `volcano-cooking`, which will create a `.nc` and `.npz` file in the `data/output`
-directory. With the `view_frc` program you can quickly view the content of the created
-files in a plot.
-
-Run from within this repository/directory via poetry:
+directory. With the `view-frc` program you can quickly view the content of the created
+files in a plot. There is also a third program called `sfrc-sparse2lin` which converts
+arrays of only non-zero events at arbitrary times to linearly spaced events where times
+between the non-zero events are filled with zeros.
 
-```sh
-poetry run volcano-cooking
-poetry run view-frc <file.nc>
-```
+### `volcano-cooking`
 
-or, if the virtual environment where the project is installed is activated:
+Once installed, run from within this directory with:
 
-```sh
+```bash
 volcano-cooking
-view-frc <file.nc>
 ```
 
-An optional flag can be sent to the `view-frc` program that will save the plot:
-`view-frc -s <file.nc>`.
-
-In either case a `data/output` directory will be created inside the current directory
-when something is saved.
+All created files are saved to a `data/output` directory that will be created inside the
+current directory from where the `volcano-cooking` command is run.
 
-For more options to either `volcano-cooking` or `view-frc`, see
+For more information, see
 
-```sh
+```bash
 volcano-cooking --help
-view-frc --help
 ```
 
-### Examples
-
-When running the command `volcano-cooking --run-ncl`, a few environment variables will
-be used, which can be controlled by setting them in a `.env` file. See
-[`.env.example`](./examples/.env.example) to see some default values. With this you can
-for example easily change the grid resolution to be `1deg` rather than `2deg` (default).
-
-The [__examples__](./examples/) directory also include an example on how to use the
-`--file` option. Cloning this repository and running `volcano-cooking --file json.json`
-from *inside* the __examples__ directory will result in some output files generated to a
-new __data__ directory inside __examples__. If you further rename `.env.example` →
-`.env` you may also run `volcano-cooking --run-ncl` and `volcano-cooking --package-last`
-(this assumes you follow option 0, see below).
-
-Finally, there is also a script [`custom_generator.py`](./examples/custom_generator.py)
-which show how you might define your own generator classes and functions. Run as `python
-custom_generator.py`.
-
-### Option 0 (default, using NCL-script)
+#### Option 0 (default, using NCL-script)
 
-#### TL;DR
+##### TL;DR
 
 ```console
 $ volcano-cooking -f 1 -s 100
 Generating with 'GenerateFPP'...
 $ volcano-cooking --run-ncl
  Copyright (C) 1995-2019 - All Rights Reserved
  University Corporation for Atmospheric Research
@@ -131,55 +113,54 @@
 $ volcano-cooking --package-last
 Successfully placed all latest source files in the 'source-files' directory.
 $ ls source-files
 20220502-140022.log                     VolcanEESMv3.11Enger_SO2_850-2016_Mscale_Zreduc_2deg_c20220502-140023.nc
 synthetic_volcanoes_20220502_135956.nc  synthetic_volcanoes_20220502_135956.npz
 ```
 
-#### Dependencies
+##### Dependencies
 
 This option needs
 
 - `volcano-cooking` installed
 - A coordinate file (~ 10 kB)
 - [`ncl`](https://www.ncl.ucar.edu/Download/) executable
 
-#### Create source file for forcing
+##### Create source file for forcing
 
 Run command `volcano-cooking` with the options you want. See `volcano-cooking --help`.
 
-#### Create forcing file for CESM2
+##### Create forcing file for CESM2
 
-> Running the [_script/create_cesm_frc.sh](_script/create_cesm_frc.sh) script depends on
-> having `ncl` installed. See installation instructions
-> [here](https://www.ncl.ucar.edu/Download/).
+> Running the `volcano-cooking --run-ncl` script depends on having `ncl` installed. See
+> installation instructions [here](https://www.ncl.ucar.edu/Download/).
 
 After having run the `volcano-cooking` command, the forcing file for CESM2 can be
 generated by running
 
 ```bash
 volcano-cooking --run-ncl
 ```
 
 If the needed coordinate files are missing, you will be asked if you want to download
 them. If you want to use different files, or change the default resolution (default is 2
-degrees), edit [.env](./.env.example) accordingly. In this case, you also need to
-manually download whatever coordinate file you want to use. See section [Setting up
-manually](#setting-up-manually).
+degrees), edit __.env__ (see [__./examples/.env.example__](./examples/.env.example))
+accordingly. In this case, you also need to manually download whatever coordinate file
+you want to use. See section [Setting up manually](#setting-up-manually).
 
-#### Wrap up
+##### Wrap up
 
 The last created files, source files, logs and final output, can be nicely collected and
 placed in a directory named `source-files` with command:
 
 ```sh
 volcano-cooking --package-last
 ```
 
-<details><summary><h4>Setting up manually</h4></summary><br>
+<details><summary><h5>Setting up manually</h5></summary><br>
 
 To be able to create forcing files used by CESM2 from the newly created synthetic file,
 we need a script from the [emissions][data_source_files] directory. These are scripts
 that use the forcing file this project generates to make a new, full forcing file that
 CESM2 accepts (examples of such files can be found [here][volc-frc-complete]). For
 example, `createVolcEruptV3.ncl` can be found in the [emissions][data_source_files]
 directory. This need a `common.ncl` file, found [here][common-ncl], in addition to other
@@ -199,41 +180,41 @@
 ```bash
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals
 ```
 
 </details>
 
-### Option 1 (directly change forcing file)
+#### Option 1 (directly change forcing file)
 
-#### TL;DR
+##### TL;DR
 
 ```console
 $ volcano-cooking -f 1 -s 100 -o
 Generating with 'GenerateFPP'...
 ```
 
-#### Dependencies
+##### Dependencies
 
 This option needs
 
 - `volcano-cooking` installed
 - A coordinate file (~ 10 kB)
 - Original CESM2 forcing file (~ 2.2 GB)
 
-#### Run library
+##### Run library
 
 Now the only thing we need to do is running `volcano-cooking` with the flag `-o`, and
 choose the type of forcing we want (see `volcano-cooking --lst`):
 
 ```bash
 volcano-cooking -f 1 -s 100 -o
 ```
 
-<details><summary><h4>Get forcing and coordinate files manually</h4></summary><br>
+<details><summary><h5>Get forcing and coordinate files manually</h5></summary><br>
 
 > Manually downloading the files and placing them in the correct directory is *not*
 > needed. Running the command as shown above will ask you if you want to download the
 > files, and place them where they need to be.
 
 This option relies on having a working forcing file and coordinate file at hand. We will
 use the forcing file that CESM2 places in the `stratvolc` directory of the `cam` model.
@@ -252,16 +233,66 @@
 ```bash
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_0.9x1.25_L30.nc --directory-prefix data/originals
 wget --no-check-certificate https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/fv_1.9x2.5_L30.nc --directory-prefix data/originals
 ```
 
 </details>
 
+#### Examples
+
+When running the command `volcano-cooking --run-ncl`, a few environment variables will
+be used, which can be controlled by setting them in a `.env` file. See
+[`.env.example`](./examples/.env.example) to see some default values. With this you can
+for example easily change the grid resolution to be `1deg` rather than `2deg` (default).
+
+The [__examples__](./examples/) directory also include an example on how to use the
+`--file` option. Cloning this repository and running `volcano-cooking --file json.json`
+from *inside* the __examples__ directory will result in some output files generated to a
+new __data__ directory inside __examples__. If you further rename `.env.example` →
+`.env` you may also run `volcano-cooking --run-ncl` and `volcano-cooking --package-last`
+(this assumes you follow option 0, see below).
+
+Finally, there is also a script [`custom_generator.py`](./examples/custom_generator.py)
+which show how you might define your own generator classes and functions. Run as `python
+custom_generator.py`.
+
+### `view-frc`
+
+After running the `volcano-cooking` command, files with names `synthetic_volcanoes_...`
+are created with file type `.nc` and `.npz`. These can be viewed with
+
+```bash
+view-frc <file.nc>
+```
+
+An optional flag can be sent to the `view-frc` program that will save the plot:
+`view-frc -s <file.nc>`.
+
+For more information, see
+
+```bash
+view-frc --help
+```
+
+### `sfrc-sparse2lin`
+
+This program is available as a convenience tool in the rare case when you have a forcing
+file with only the events of eruptions. The program will re-write time array to be
+linearly spaced and place the values from the forcing values into a new forcing array
+that matches the new linearly spaced time axis.
+
+It assumes the file sent to it has `yoes`(year, YYYY), `moes` (month, MM), `does`
+(days, DD) and `tes` (emissions, Tg) fields if it is a `.npz` file. If a `.nc` file is
+used, it must have a dataset with variables "Year_of_Emission", "Month_of_Emission",
+"Day_of_Emission" and "Total_Emission".
+
 ## Extra
 
+This assumes you are using the package from a python script, and not just the CLI.
+
 ### Compare created file with a similar used in a default CESM2 experiment
 
 A similar file to those that are created is needed to be able to use some scripts in the
 `helper_scripts` directory. By default, it assumes the file is named
 `volcan-eesm_global_2015_so2-emissions-database_v1.0.nc` and that it is placed inside
 the `data/originals` directory. You can find this file [here][volc-frc].
 
@@ -273,28 +304,27 @@
 ```bash
 git clone https://github.com/engeir/volcano-cooking.git
 cd volcano-cooking
 poetry install
 pre-commit install
 ```
 
-Before committing new changes to a branch you can run command
+Before committing new changes to a branch you may run the full test suite with:
 
 ```bash
 nox
 ```
 
-to run the full test suite. You will need [Poetry], [nox] and [nox-poetry] installed for
-this.
+You will need [Poetry], [nox] and [nox-poetry] installed for this.
 
-[data_source_files]: https://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission
 [common-ncl]: http://svn.code.sf.net/p/codescripts/code/trunk/ncl/lib/common.ncl
 [coord-file]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/coords/
-[coords-repo]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/share/scripgrids/
-[volc-frc]: http://catalogue.ceda.ac.uk/uuid/bfbd5ec825fa422f9a858b14ae7b2a0d
-[volc-frc-complete]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/
-[stratvolc-forcing]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc
-[pypi]: https://pypi.org/
-[nox]: https://nox.thea.codes/en/stable/
+[data_source_files]: https://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission
 [nox-poetry]: https://nox-poetry.readthedocs.io/
+[nox]: https://nox.thea.codes/en/stable/
+[pipx-source]: https://github.com/pypa/pipx
 [poetry]: https://python-poetry.org
+[pypi]: https://pypi.org/
+[stratvolc-forcing]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/VolcanEESMv3.11_SO2_850-2016_Mscale_Zreduc_2deg_c191125.nc
+[volc-frc-complete]: https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/chem/stratvolc/
+[volc-frc]: http://catalogue.ceda.ac.uk/uuid/bfbd5ec825fa422f9a858b14ae7b2a0d
```

