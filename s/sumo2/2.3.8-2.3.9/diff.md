# Comparing `tmp/sumo2-2.3.8.tar.gz` & `tmp/sumo2-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumo2-2.3.8.tar", last modified: Mon Apr  8 10:49:09 2024, max compression
+gzip compressed data, was "sumo2-2.3.9.tar", last modified: Mon Apr  8 10:57:09 2024, max compression
```

## Comparing `sumo2-2.3.8.tar` & `sumo2-2.3.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.249929 sumo2-2.3.8/
--rw-rw-rw-   0        0        0     1068 2024-01-10 12:27:01.000000 sumo2-2.3.8/LICENSE
--rw-rw-rw-   0        0        0    10717 2024-04-08 10:49:09.247929 sumo2-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     9131 2024-01-10 12:27:01.000000 sumo2-2.3.8/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.067927 sumo2-2.3.8/examples/
--rw-rw-rw-   0        0        0      451 2024-01-10 12:27:01.000000 sumo2-2.3.8/examples/orbital_colours.conf
--rw-rw-rw-   0        0        0       42 2024-04-08 10:49:09.249929 sumo2-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2298 2024-04-08 10:47:12.000000 sumo2-2.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.072927 sumo2-2.3.8/sumo/
--rw-rw-rw-   0        0        0      201 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.130928 sumo2-2.3.8/sumo/cli/
--rw-rw-rw-   0        0        0      145 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/cli/__init__.py
--rw-rw-rw-   0        0        0    28628 2024-04-08 10:42:18.000000 sumo2-2.3.8/sumo/cli/bandplot.py
--rw-rw-rw-   0        0        0    12581 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/cli/bandstats.py
--rw-rw-rw-   0        0        0    22250 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/cli/dosplot.py
--rw-rw-rw-   0        0        0    13647 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/cli/kgen.py
--rw-rw-rw-   0        0        0    16320 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/cli/optplot.py
--rw-rw-rw-   0        0        0    24021 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/cli/phonon_bandplot.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.174928 sumo2-2.3.8/sumo/electronic_structure/
--rw-rw-rw-   0        0        0      177 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/electronic_structure/__init__.py
--rw-rw-rw-   0        0        0    11819 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/electronic_structure/bandstructure.py
--rw-rw-rw-   0        0        0    16779 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/electronic_structure/dos.py
--rw-rw-rw-   0        0        0     5711 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/electronic_structure/effective_mass.py
--rw-rw-rw-   0        0        0     9386 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/electronic_structure/optics.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.200928 sumo2-2.3.8/sumo/io/
--rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/io/__init__.py
--rw-rw-rw-   0        0        0    41648 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/io/castep.py
--rw-rw-rw-   0        0        0    43907 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/io/questaal.py
--rw-rw-rw-   0        0        0     4702 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/io/vasp.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.203929 sumo2-2.3.8/sumo/phonon/
--rw-rw-rw-   0        0        0      177 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/phonon/__init__.py
--rw-rw-rw-   0        0        0     4518 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/phonon/phonopy.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.216930 sumo2-2.3.8/sumo/plotting/
--rw-rw-rw-   0        0        0    11119 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/__init__.py
--rw-rw-rw-   0        0        0    36956 2024-04-08 10:41:06.000000 sumo2-2.3.8/sumo/plotting/bs_plotter.py
--rw-rw-rw-   0        0        0    19237 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/dos_plotter.py
--rw-rw-rw-   0        0        0    12237 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/optics_plotter.py
--rw-rw-rw-   0        0        0      276 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/orbital_colours.conf
--rw-rw-rw-   0        0        0    10511 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/phonon_bs_plotter.py
--rw-rw-rw-   0        0        0     1430 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/sumo_base.mplstyle
--rw-rw-rw-   0        0        0      385 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/sumo_bs.mplstyle
--rw-rw-rw-   0        0        0       56 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/sumo_dos.mplstyle
--rw-rw-rw-   0        0        0      315 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/sumo_optics.mplstyle
--rw-rw-rw-   0        0        0      113 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/plotting/sumo_phonon.mplstyle
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.226927 sumo2-2.3.8/sumo/symmetry/
--rw-rw-rw-   0        0        0      498 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/__init__.py
--rw-rw-rw-   0        0        0     6141 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/brad_crack_kpath.py
--rw-rw-rw-   0        0        0    14967 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/bradcrack.json
--rw-rw-rw-   0        0        0     3422 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/custom_kpath.py
--rw-rw-rw-   0        0        0    10541 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/kpath.py
--rw-rw-rw-   0        0        0     6568 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/kpoints.py
--rw-rw-rw-   0        0        0     1215 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/latimer_munro_kpath.py
--rw-rw-rw-   0        0        0     1844 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/pymatgen_kpath.py
--rw-rw-rw-   0        0        0     3594 2024-01-10 12:27:01.000000 sumo2-2.3.8/sumo/symmetry/seekpath_kpath.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.245929 sumo2-2.3.8/sumo2.egg-info/
--rw-rw-rw-   0        0        0    10717 2024-04-08 10:49:08.000000 sumo2-2.3.8/sumo2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2024-04-08 10:49:08.000000 sumo2-2.3.8/sumo2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 10:49:08.000000 sumo2-2.3.8/sumo2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      256 2024-04-08 10:49:08.000000 sumo2-2.3.8/sumo2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      197 2024-04-08 10:49:08.000000 sumo2-2.3.8/sumo2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 10:49:08.000000 sumo2-2.3.8/sumo2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.043927 sumo2-2.3.8/tests/
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.229929 sumo2-2.3.8/tests/tests_electronic_structure/
--rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_electronic_structure/__init__.py
--rw-rw-rw-   0        0        0     2455 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_electronic_structure/test_optics.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.233928 sumo2-2.3.8/tests/tests_io/
--rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_io/__init__.py
--rw-rw-rw-   0        0        0    10619 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_io/test_castep.py
--rw-rw-rw-   0        0        0     6853 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_io/test_questaal.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.235928 sumo2-2.3.8/tests/tests_phonon/
--rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_phonon/__init__.py
--rw-rw-rw-   0        0        0     1250 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_phonon/test_phonopy.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.238927 sumo2-2.3.8/tests/tests_plotting/
--rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_plotting/__init__.py
--rw-rw-rw-   0        0        0     1469 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_plotting/test_band_plotter.py
--rw-rw-rw-   0        0        0     2968 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_plotting/test_dos_plotter.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:49:09.244930 sumo2-2.3.8/tests/tests_symmetry/
--rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_symmetry/__init__.py
--rw-rw-rw-   0        0        0     2090 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_symmetry/test_bradcrack_kpath.py
--rw-rw-rw-   0        0        0     3156 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_symmetry/test_custom_kpath.py
--rw-rw-rw-   0        0        0     1707 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_symmetry/test_pymatgen_kpath.py
--rw-rw-rw-   0        0        0     2133 2024-01-10 12:27:01.000000 sumo2-2.3.8/tests/tests_symmetry/test_seekpath_kpath.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.926948 sumo2-2.3.9/
+-rw-rw-rw-   0        0        0     1068 2024-01-10 12:27:01.000000 sumo2-2.3.9/LICENSE
+-rw-rw-rw-   0        0        0    10717 2024-04-08 10:57:09.925946 sumo2-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9131 2024-01-10 12:27:01.000000 sumo2-2.3.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.848944 sumo2-2.3.9/examples/
+-rw-rw-rw-   0        0        0      451 2024-01-10 12:27:01.000000 sumo2-2.3.9/examples/orbital_colours.conf
+-rw-rw-rw-   0        0        0       42 2024-04-08 10:57:09.926948 sumo2-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2298 2024-04-08 10:47:12.000000 sumo2-2.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.849944 sumo2-2.3.9/sumo/
+-rw-rw-rw-   0        0        0      201 2024-04-08 10:57:04.000000 sumo2-2.3.9/sumo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.865944 sumo2-2.3.9/sumo/cli/
+-rw-rw-rw-   0        0        0      145 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/cli/__init__.py
+-rw-rw-rw-   0        0        0    28633 2024-04-08 10:56:43.000000 sumo2-2.3.9/sumo/cli/bandplot.py
+-rw-rw-rw-   0        0        0    12581 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/cli/bandstats.py
+-rw-rw-rw-   0        0        0    22250 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/cli/dosplot.py
+-rw-rw-rw-   0        0        0    13647 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/cli/kgen.py
+-rw-rw-rw-   0        0        0    16320 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/cli/optplot.py
+-rw-rw-rw-   0        0        0    24021 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/cli/phonon_bandplot.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.870947 sumo2-2.3.9/sumo/electronic_structure/
+-rw-rw-rw-   0        0        0      177 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/electronic_structure/__init__.py
+-rw-rw-rw-   0        0        0    11819 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/electronic_structure/bandstructure.py
+-rw-rw-rw-   0        0        0    16779 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/electronic_structure/dos.py
+-rw-rw-rw-   0        0        0     5711 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/electronic_structure/effective_mass.py
+-rw-rw-rw-   0        0        0     9386 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/electronic_structure/optics.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.874944 sumo2-2.3.9/sumo/io/
+-rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/io/__init__.py
+-rw-rw-rw-   0        0        0    41648 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/io/castep.py
+-rw-rw-rw-   0        0        0    43907 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/io/questaal.py
+-rw-rw-rw-   0        0        0     4702 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/io/vasp.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.876946 sumo2-2.3.9/sumo/phonon/
+-rw-rw-rw-   0        0        0      177 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/phonon/__init__.py
+-rw-rw-rw-   0        0        0     4518 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/phonon/phonopy.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.891945 sumo2-2.3.9/sumo/plotting/
+-rw-rw-rw-   0        0        0    11119 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/__init__.py
+-rw-rw-rw-   0        0        0    36956 2024-04-08 10:41:06.000000 sumo2-2.3.9/sumo/plotting/bs_plotter.py
+-rw-rw-rw-   0        0        0    19237 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/dos_plotter.py
+-rw-rw-rw-   0        0        0    12237 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/optics_plotter.py
+-rw-rw-rw-   0        0        0      276 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/orbital_colours.conf
+-rw-rw-rw-   0        0        0    10511 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/phonon_bs_plotter.py
+-rw-rw-rw-   0        0        0     1430 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/sumo_base.mplstyle
+-rw-rw-rw-   0        0        0      385 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/sumo_bs.mplstyle
+-rw-rw-rw-   0        0        0       56 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/sumo_dos.mplstyle
+-rw-rw-rw-   0        0        0      315 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/sumo_optics.mplstyle
+-rw-rw-rw-   0        0        0      113 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/plotting/sumo_phonon.mplstyle
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.903946 sumo2-2.3.9/sumo/symmetry/
+-rw-rw-rw-   0        0        0      498 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/__init__.py
+-rw-rw-rw-   0        0        0     6141 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/brad_crack_kpath.py
+-rw-rw-rw-   0        0        0    14967 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/bradcrack.json
+-rw-rw-rw-   0        0        0     3422 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/custom_kpath.py
+-rw-rw-rw-   0        0        0    10541 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/kpath.py
+-rw-rw-rw-   0        0        0     6568 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/kpoints.py
+-rw-rw-rw-   0        0        0     1215 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/latimer_munro_kpath.py
+-rw-rw-rw-   0        0        0     1844 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/pymatgen_kpath.py
+-rw-rw-rw-   0        0        0     3594 2024-01-10 12:27:01.000000 sumo2-2.3.9/sumo/symmetry/seekpath_kpath.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.924946 sumo2-2.3.9/sumo2.egg-info/
+-rw-rw-rw-   0        0        0    10717 2024-04-08 10:57:09.000000 sumo2-2.3.9/sumo2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2024-04-08 10:57:09.000000 sumo2-2.3.9/sumo2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 10:57:09.000000 sumo2-2.3.9/sumo2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      256 2024-04-08 10:57:09.000000 sumo2-2.3.9/sumo2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      197 2024-04-08 10:57:09.000000 sumo2-2.3.9/sumo2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 10:57:09.000000 sumo2-2.3.9/sumo2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.845945 sumo2-2.3.9/tests/
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.905949 sumo2-2.3.9/tests/tests_electronic_structure/
+-rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_electronic_structure/__init__.py
+-rw-rw-rw-   0        0        0     2455 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_electronic_structure/test_optics.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.908948 sumo2-2.3.9/tests/tests_io/
+-rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_io/__init__.py
+-rw-rw-rw-   0        0        0    10619 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_io/test_castep.py
+-rw-rw-rw-   0        0        0     6853 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_io/test_questaal.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.910948 sumo2-2.3.9/tests/tests_phonon/
+-rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_phonon/__init__.py
+-rw-rw-rw-   0        0        0     1250 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_phonon/test_phonopy.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.913948 sumo2-2.3.9/tests/tests_plotting/
+-rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_plotting/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_plotting/test_band_plotter.py
+-rw-rw-rw-   0        0        0     2968 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_plotting/test_dos_plotter.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:57:09.923946 sumo2-2.3.9/tests/tests_symmetry/
+-rw-rw-rw-   0        0        0        0 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_symmetry/__init__.py
+-rw-rw-rw-   0        0        0     2090 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_symmetry/test_bradcrack_kpath.py
+-rw-rw-rw-   0        0        0     3156 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_symmetry/test_custom_kpath.py
+-rw-rw-rw-   0        0        0     1707 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_symmetry/test_pymatgen_kpath.py
+-rw-rw-rw-   0        0        0     2133 2024-01-10 12:27:01.000000 sumo2-2.3.9/tests/tests_symmetry/test_seekpath_kpath.py
```

### Comparing `sumo2-2.3.8/LICENSE` & `sumo2-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/PKG-INFO` & `sumo2-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo2
-Version: 2.3.8
+Version: 2.3.9
 Summary: Heavy weight plotting tools for ab initio solid-state calculations
 Home-page: https://github.com/smtg-ucl/sumo
 Author: Alex Ganose, Adam J. Jackson
 Author-email: d.scanlon@ucl.ac.uk
 License: MIT
 Keywords: chemistry pymatgen dft vasp dos band
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sumo2-2.3.8/README.rst` & `sumo2-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/setup.py` & `sumo2-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/cli/bandplot.py` & `sumo2-2.3.9/sumo/cli/bandplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -755,15 +755,15 @@
         "--offset", type=int, default=0, help="band gap offset"
     )
     parser.add_argument("--font", default=None, help="font to use")
     parser.add_argument("--title", default=None, help="plot title")
     return parser
 
 
-def main(_args):
+def main(_args=None):
     args = _get_parser().parse_args(_args)
     logging.basicConfig(
         filename="sumo-bandplot.log",
         level=logging.INFO,
         filemode="w",
         format="%(message)s",
     )
```

### Comparing `sumo2-2.3.8/sumo/cli/bandstats.py` & `sumo2-2.3.9/sumo/cli/bandstats.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/cli/dosplot.py` & `sumo2-2.3.9/sumo/cli/dosplot.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/cli/kgen.py` & `sumo2-2.3.9/sumo/cli/kgen.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/cli/optplot.py` & `sumo2-2.3.9/sumo/cli/optplot.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/cli/phonon_bandplot.py` & `sumo2-2.3.9/sumo/cli/phonon_bandplot.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/electronic_structure/bandstructure.py` & `sumo2-2.3.9/sumo/electronic_structure/bandstructure.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/electronic_structure/dos.py` & `sumo2-2.3.9/sumo/electronic_structure/dos.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/electronic_structure/effective_mass.py` & `sumo2-2.3.9/sumo/electronic_structure/effective_mass.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/electronic_structure/optics.py` & `sumo2-2.3.9/sumo/electronic_structure/optics.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/io/castep.py` & `sumo2-2.3.9/sumo/io/castep.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/io/questaal.py` & `sumo2-2.3.9/sumo/io/questaal.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/io/vasp.py` & `sumo2-2.3.9/sumo/io/vasp.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/phonon/phonopy.py` & `sumo2-2.3.9/sumo/phonon/phonopy.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/plotting/__init__.py` & `sumo2-2.3.9/sumo/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/plotting/bs_plotter.py` & `sumo2-2.3.9/sumo/plotting/bs_plotter.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/plotting/dos_plotter.py` & `sumo2-2.3.9/sumo/plotting/dos_plotter.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/plotting/optics_plotter.py` & `sumo2-2.3.9/sumo/plotting/optics_plotter.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/plotting/phonon_bs_plotter.py` & `sumo2-2.3.9/sumo/plotting/phonon_bs_plotter.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/plotting/sumo_base.mplstyle` & `sumo2-2.3.9/sumo/plotting/sumo_base.mplstyle`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/brad_crack_kpath.py` & `sumo2-2.3.9/sumo/symmetry/brad_crack_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/bradcrack.json` & `sumo2-2.3.9/sumo/symmetry/bradcrack.json`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/custom_kpath.py` & `sumo2-2.3.9/sumo/symmetry/custom_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/kpath.py` & `sumo2-2.3.9/sumo/symmetry/kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/kpoints.py` & `sumo2-2.3.9/sumo/symmetry/kpoints.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/latimer_munro_kpath.py` & `sumo2-2.3.9/sumo/symmetry/latimer_munro_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/pymatgen_kpath.py` & `sumo2-2.3.9/sumo/symmetry/pymatgen_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo/symmetry/seekpath_kpath.py` & `sumo2-2.3.9/sumo/symmetry/seekpath_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/sumo2.egg-info/PKG-INFO` & `sumo2-2.3.9/sumo2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo2
-Version: 2.3.8
+Version: 2.3.9
 Summary: Heavy weight plotting tools for ab initio solid-state calculations
 Home-page: https://github.com/smtg-ucl/sumo
 Author: Alex Ganose, Adam J. Jackson
 Author-email: d.scanlon@ucl.ac.uk
 License: MIT
 Keywords: chemistry pymatgen dft vasp dos band
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sumo2-2.3.8/sumo2.egg-info/SOURCES.txt` & `sumo2-2.3.9/sumo2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_electronic_structure/test_optics.py` & `sumo2-2.3.9/tests/tests_electronic_structure/test_optics.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_io/test_castep.py` & `sumo2-2.3.9/tests/tests_io/test_castep.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_io/test_questaal.py` & `sumo2-2.3.9/tests/tests_io/test_questaal.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_phonon/test_phonopy.py` & `sumo2-2.3.9/tests/tests_phonon/test_phonopy.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_plotting/test_band_plotter.py` & `sumo2-2.3.9/tests/tests_plotting/test_band_plotter.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_plotting/test_dos_plotter.py` & `sumo2-2.3.9/tests/tests_plotting/test_dos_plotter.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_symmetry/test_bradcrack_kpath.py` & `sumo2-2.3.9/tests/tests_symmetry/test_bradcrack_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_symmetry/test_custom_kpath.py` & `sumo2-2.3.9/tests/tests_symmetry/test_custom_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_symmetry/test_pymatgen_kpath.py` & `sumo2-2.3.9/tests/tests_symmetry/test_pymatgen_kpath.py`

 * *Files identical despite different names*

### Comparing `sumo2-2.3.8/tests/tests_symmetry/test_seekpath_kpath.py` & `sumo2-2.3.9/tests/tests_symmetry/test_seekpath_kpath.py`

 * *Files identical despite different names*

