# Comparing `tmp/attotree-0.1.2.tar.gz` & `tmp/attotree-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attotree-0.1.2.tar", last modified: Thu Feb  1 16:31:53 2024, max compression
+gzip compressed data, was "attotree-0.1.3.tar", last modified: Mon Apr  8 18:11:08 2024, max compression
```

## Comparing `attotree-0.1.2.tar` & `attotree-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-02-01 16:31:53.658609 attotree-0.1.2/
--rw-r--r--   0 karel      (503) staff       (20)     1071 2024-01-15 14:46:06.000000 attotree-0.1.2/LICENSE.txt
--rw-r--r--   0 karel      (503) staff       (20)     2630 2024-02-01 16:31:53.646467 attotree-0.1.2/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)     2052 2024-01-15 12:18:45.000000 attotree-0.1.2/README.rst
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-02-01 16:31:53.571889 attotree-0.1.2/attotree/
--rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 attotree-0.1.2/attotree/__init__.py
--rwxr-xr-x   0 karel      (503) staff       (20)    10806 2024-02-01 16:24:24.000000 attotree-0.1.2/attotree/attotree.py
--rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 attotree-0.1.2/attotree/increment_version.py
--rw-r--r--   0 karel      (503) staff       (20)       78 2024-02-01 16:24:24.000000 attotree-0.1.2/attotree/version.py
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-02-01 16:31:53.645525 attotree-0.1.2/attotree.egg-info/
--rw-r--r--   0 karel      (503) staff       (20)     2630 2024-02-01 16:31:53.000000 attotree-0.1.2/attotree.egg-info/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)      317 2024-02-01 16:31:53.000000 attotree-0.1.2/attotree.egg-info/SOURCES.txt
--rw-r--r--   0 karel      (503) staff       (20)        1 2024-02-01 16:31:53.000000 attotree-0.1.2/attotree.egg-info/dependency_links.txt
--rw-r--r--   0 karel      (503) staff       (20)       52 2024-02-01 16:31:53.000000 attotree-0.1.2/attotree.egg-info/entry_points.txt
--rw-r--r--   0 karel      (503) staff       (20)        6 2024-02-01 16:31:53.000000 attotree-0.1.2/attotree.egg-info/requires.txt
--rw-r--r--   0 karel      (503) staff       (20)        9 2024-02-01 16:31:53.000000 attotree-0.1.2/attotree.egg-info/top_level.txt
--rw-r--r--   0 karel      (503) staff       (20)       38 2024-02-01 16:31:53.658722 attotree-0.1.2/setup.cfg
--rw-r--r--   0 karel      (503) staff       (20)     1351 2024-01-11 15:00:05.000000 attotree-0.1.2/setup.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-08 18:11:08.562548 attotree-0.1.3/
+-rw-r--r--   0 karel      (503) staff       (20)     1071 2024-01-15 14:46:06.000000 attotree-0.1.3/LICENSE.txt
+-rw-r--r--   0 karel      (503) staff       (20)     2650 2024-04-08 18:11:08.561979 attotree-0.1.3/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     2072 2024-04-08 18:04:36.000000 attotree-0.1.3/README.rst
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-08 18:11:08.476066 attotree-0.1.3/attotree/
+-rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 attotree-0.1.3/attotree/__init__.py
+-rwxr-xr-x   0 karel      (503) staff       (20)    12878 2024-04-08 18:04:36.000000 attotree-0.1.3/attotree/attotree.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 attotree-0.1.3/attotree/increment_version.py
+-rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-08 18:04:36.000000 attotree-0.1.3/attotree/version.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-08 18:11:08.561365 attotree-0.1.3/attotree.egg-info/
+-rw-r--r--   0 karel      (503) staff       (20)     2650 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/SOURCES.txt
+-rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/dependency_links.txt
+-rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/entry_points.txt
+-rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/requires.txt
+-rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/top_level.txt
+-rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-08 18:11:08.562623 attotree-0.1.3/setup.cfg
+-rw-r--r--   0 karel      (503) staff       (20)     1351 2024-01-11 15:00:05.000000 attotree-0.1.3/setup.py
```

### Comparing `attotree-0.1.2/LICENSE.txt` & `attotree-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `attotree-0.1.2/PKG-INFO` & `attotree-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attotree
-Version: 0.1.2
+Version: 0.1.3
 Summary: description
 Home-page: https://github.com/karel-brinda/attotree
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 Requires-Dist: wheel
 
 Attotree
-==================================================================================
+========
 
 
 Introduction
 ------------
 
 Rapid estimation of phylogenetic trees directly from FASTA files in the style of
 `Mashtree <https://github.com/lskatz/mashtree>`_. With the default options,
@@ -68,33 +68,35 @@
 Command-line parameters
 -----------------------
 
 
 .. code-block::
 
     $ attotree -h
-
+ 
     Program: attotree (rapid estimation of phylogenetic trees using sketching)
-    Version: 0.1.1
+    Version: 0.1.3
     Author:  Karel Brinda <karel.brinda@inria.fr>
 
-    usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] genomes [genomes ...]
+    usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] [-D] [-V] genomes [genomes ...]
 
     positional arguments:
       genomes     input genome file (fasta / gzipped fasta / list of files when "-L")
 
     options:
       -h          show this help message and exit
       -v          show program's version number and exit
       -k INT      kmer size [21]
       -s INT      sketch size [10000]
       -t INT      number of threads [10]
       -o FILE     newick output [stdout]
       -f STR      tree inference algorithm (nj/upgma) [nj]
       -L          input files are list of files
+      -D          debugging (don't remove tmp dir)
+      -V          verbose output
 
 
 
 Issues
 ------
 
 Please use `Github issues <https://github.com/karel-brinda/attotree/issues>`_.
@@ -112,8 +114,7 @@
 `MIT <https://github.com/karel-brinda/attotree/blob/master/LICENSE.txt>`_
 
 
 Authors
 -------
 
 `Karel Brinda <http://brinda.eu>`_ <karel.brinda@inria.fr>
-
```

### Comparing `attotree-0.1.2/README.rst` & `attotree-0.1.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Attotree
-==================================================================================
+========
 
 
 Introduction
 ------------
 
 Rapid estimation of phylogenetic trees directly from FASTA files in the style of
 `Mashtree <https://github.com/lskatz/mashtree>`_. With the default options,
@@ -50,33 +50,35 @@
 Command-line parameters
 -----------------------
 
 
 .. code-block::
 
     $ attotree -h
-
+ 
     Program: attotree (rapid estimation of phylogenetic trees using sketching)
-    Version: 0.1.1
+    Version: 0.1.3
     Author:  Karel Brinda <karel.brinda@inria.fr>
 
-    usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] genomes [genomes ...]
+    usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] [-D] [-V] genomes [genomes ...]
 
     positional arguments:
       genomes     input genome file (fasta / gzipped fasta / list of files when "-L")
 
     options:
       -h          show this help message and exit
       -v          show program's version number and exit
       -k INT      kmer size [21]
       -s INT      sketch size [10000]
       -t INT      number of threads [10]
       -o FILE     newick output [stdout]
       -f STR      tree inference algorithm (nj/upgma) [nj]
       -L          input files are list of files
+      -D          debugging (don't remove tmp dir)
+      -V          verbose output
 
 
 
 Issues
 ------
 
 Please use `Github issues <https://github.com/karel-brinda/attotree/issues>`_.
@@ -94,8 +96,7 @@
 `MIT <https://github.com/karel-brinda/attotree/blob/master/LICENSE.txt>`_
 
 
 Authors
 -------
 
 `Karel Brinda <http://brinda.eu>`_ <karel.brinda@inria.fr>
-
```

### Comparing `attotree-0.1.2/attotree/attotree.py` & `attotree-0.1.3/attotree/attotree.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,29 @@
 
 DEFAULT_S = 10000
 DEFAULT_K = 21
 DEFAULT_T = os.cpu_count()
 DEFAULT_F = "nj"
 
 
+def shorten_output(s):
+    """
+    Shortens the output string if it exceeds 40 characters.
+
+    Args:
+        s (str): The input string.
+
+    Returns:
+        str: The shortened string.
+    """
+    if len(s) > 40:
+        s = s[:40] + "..."
+    return s
+
+
 def error(*msg, error_code=1):
     """
     Prints an error message to stderr and exits the program with the specified error code.
 
     Args:
         *msg: Variable number of message arguments to be printed.
         error_code (int): The error code to exit the program with. Default is 1.
@@ -55,15 +70,15 @@
     """
     dt = datetime.datetime.now()
     fdt = dt.strftime("%Y-%m-%d %H:%M:%S")
     log_line = f'[attotree] {fdt} {" ".join(msg)}'
     print(log_line, file=sys.stderr)
 
 
-def run_safe(command, output_fn=None, output_fo=None, err_msg=None, thr_exc=True, silent=False):
+def run_safe(command, output_fn=None, output_fo=None, err_msg=None, thr_exc=True, silent=False, verbose=True):
     """
     Executes a shell command safely.
 
     Args:
         command (list): The shell command to be executed, as a list of strings.
         output_fn (str, optional): The filename to redirect the command's output to. Defaults to None.
         output_fo (file object, optional): The file object to redirect the command's output to. Defaults to None.
@@ -87,17 +102,21 @@
     for part in command:
         part = str(part)
         if " " in part:
             part = '"{}"'.format(part)
         command_safe.append(part)
 
     command_str = " ".join(command_safe)
+    if verbose:
+        command_str_nice = command_str
+    else:
+        command_str_nice = shorten_output(command_str)
 
     if not silent:
-        message("Shell command:", command_str)
+        message(f"Shell command: '{command_str_nice}'")
 
     if output_fn is None:
         if output_fo is None:
             out_fo = sys.stdout
         else:
             out_fo = output_fo
     else:
@@ -116,28 +135,28 @@
     out_fo.flush()
 
     if output_fn is not None:
         out_fo.close()
 
     if error_code == 0 or error_code == 141:
         if not silent:
-            message("Finished: {}".format(command_str))
+            message(f"Finished: '{command_str_nice}'")
     else:
-        message("Unfinished, an error occurred (error code {}): {}".format(error_code, command_str))
+        message(f"Unfinished, an error occurred (error code {error_code}): '{command_str}'")
 
         if err_msg is not None:
             print('Error: {}'.format(err_msg), file=sys.stderr)
 
         if thr_exc:
             error("A command failed, see messages above.")
 
         sys.exit(1)
 
 
-def mash_triangle(inp_fns, phylip_fn, k, s, t, fof):
+def mash_triangle(inp_fns, phylip_fn, k, s, t, fof, verbose):
     """
     Runs the 'mash triangle' command with the given parameters.
 
     Args:
         inp_fns (list): List of input filenames.
         phylip_fn (str): Output filename for the phylip file.
         k (int): Value for the '-k' option.
@@ -147,20 +166,20 @@
 
     Returns:
         None
 
     Raises:
         None
     """
-    message("Running mash")
+    message("Running Mash")
     cmd = f"mash triangle -s {s} -k {k} -p {t}".split()
     if fof:
         cmd += ["-l"]
     cmd += inp_fns
-    run_safe(cmd, output_fn=phylip_fn)
+    run_safe(cmd, output_fn=phylip_fn, verbose=verbose)
 
 
 def fn_to_node_name(fn):
     """
     Converts a file name to a node name by removing the path and file extension.
 
     Args:
@@ -173,15 +192,15 @@
     if len(basename_components) == 1:
         basename_components.append("")
     # remove suffix
     nname = ".".join(basename_components[:-1])
     return nname
 
 
-def postprocess_mash_phylip(phylip_in_fn, phylip_out_fn):
+def postprocess_mash_phylip(phylip_in_fn, phylip_out_fn, verbose):
     """
     Postprocesses a PHYLIP file by copying its contents from the input file to the output file.
 
     Args:
         phylip_in_fn (str): The path to the input PHYLIP file.
         phylip_out_fn (str): The path to the output PHYLIP file.
 
@@ -189,28 +208,21 @@
         None
     """
     with open(phylip_in_fn) as f:
         with open(phylip_out_fn, "w+") as g:
             for i, x in enumerate(f):
                 x = x.strip()
                 if i != 0:
-                    print(x, file=sys.stderr)
                     l, sep, r = x.partition("\t")
                     l = fn_to_node_name(l)
                     x = l + sep + r
-                message(x)
                 print(x, file=g)
-    #basename_components = os.path.basename(p[0]).split(".")
-    #if len(basename_components) == 1:
-    #    basename_components.append("")
-    ## remove suffix
-    #p[0] = ".".join(basename_components[:-1])
 
 
-def quicktree(phylip_fn, newick_fn, algorithm):
+def quicktree(phylip_fn, newick_fn, algorithm, verbose):
     """
     Runs the quicktree algorithm to generate a phylogenetic tree.
 
     Args:
         phylip_fn (str): The filename of the input phylip file.
         newick_fn (str): The filename of the output newick file.
         algorithm (str): The algorithm to use for tree construction. Valid options are "upgma" or "nj".
@@ -220,74 +232,119 @@
     """
     message("Running quicktree")
 
     cmd = "quicktree -in m".split()
     if algorithm == "upgma":
         cmd += ["-upgma"]
     cmd += [phylip_fn]
-    run_safe(cmd, output_fn=newick_fn)
+    run_safe(cmd, output_fn=newick_fn, verbose=verbose)
 
 
-def postprocess_quicktree_nw(nw_in_fn, nw_out_fo):
+def postprocess_quicktree_nw(nw_in_fn, nw_out_fo, verbose):
     """
     Reformat newick.
 
+    This function reads an input newick file, removes any leading or trailing whitespace from each line,
+    and writes the postprocessed newick file to the specified file object.
+
     Notes:
     - assumption: node names already don't contain paths and prefixes
     - expects fo to allow both a filename or stdout
 
     Args:
         nw_in_fn (str): Path to the input newick file.
         nw_out_fo (file object): File object to write the postprocessed newick file.
+        verbose (bool): If True, print additional information during the postprocessing.
 
     Returns:
         None
     """
     message("Postprocessing tree")
     buffer = []
     with open(nw_in_fn) as fo:
         for x in fo:
             x = x.strip()
             buffer.append(x)
     print("".join(buffer), file=nw_out_fo)
 
 
-def attotree(fns, newick_fo, k, s, t, phylogeny_algorithm, fof):
+def attotree(fns, newick_fo, k, s, t, phylogeny_algorithm, fof, verbose, debug):
     """
     Generate a phylogenetic tree using the given parameters.
 
     Args:
         fns (list): List of input filenames.
         newick_fo (file object): Output file object to write the generated tree.
         k (int): Value for parameter k.
         s (int): Value for parameter s.
         t (int): Value for parameter t.
         phylogeny_algorithm (str): Name of the phylogeny algorithm to use.
         fof (bool): Flag indicating whether to use the fof parameter.
+        verbose (bool): Flag indicating whether to enable verbose output.
+        debug (bool): Flag indicating whether to retain auxiliary files.
 
     Returns:
         None
     """
-    with tempfile.TemporaryDirectory() as d:
-        message('created a temporary directory', d)
+    features = []
+    if verbose:
+        features.append("verbose")
+    if debug:
+        features.append("debuging")
+    if len(features) > 0:
+        fmsg = f" ({', '.join(features)})"
+    else:
+        fmsg = ""
+    message(f"Attotree starting{fmsg}")
+    with tempfile.TemporaryDirectory(delete=not debug) as d:
+        message('Created a temporary directory', d)
         phylip1_fn = os.path.join(d, "distances.phylip0")
         phylip2_fn = os.path.join(d, "distances.phylip")
         newick1_fn = os.path.join(d, "tree.nw")
         newick2_fo = newick_fo
-        mash_triangle(fns, phylip1_fn, k=k, s=s, t=t, fof=fof)
-        postprocess_mash_phylip(phylip1_fn, phylip2_fn)
-        quicktree(phylip2_fn, newick1_fn, algorithm=phylogeny_algorithm)
-        postprocess_quicktree_nw(newick1_fn, newick2_fo)
+        if fof:
+            #This is to make the list of file pass to Mash even with
+            #process substitutions
+            old_fof_fn = fns[0]
+            new_fof_fn = os.path.join(d, "fof.txt")
+            with open(old_fof_fn) as f, open(new_fof_fn, 'w') as g:
+                g.write(f.read())
+            fns = [new_fof_fn]
+        mash_triangle(fns, phylip1_fn, k=k, s=s, t=t, fof=fof, verbose=verbose)
+        postprocess_mash_phylip(phylip1_fn, phylip2_fn, verbose=verbose)
+        quicktree(phylip2_fn, newick1_fn, algorithm=phylogeny_algorithm, verbose=verbose)
+        postprocess_quicktree_nw(newick1_fn, newick2_fo, verbose=verbose)
+
+    if debug:
+        emsg = f" (auxiliary files retained in '{d}')"
+    else:
+        emsg = ""
+    message(f"Attotree finished{emsg}")
 
 
 def main():
+    """
+    The main function that is executed when the script is run.
+
+    Returns:
+        None
+    """
 
     class CustomArgumentParser(argparse.ArgumentParser):
 
+        def __init__(self, prog=None, **kwargs):
+            super().__init__(prog="attotree", **kwargs)
+
         def print_help(self):
+            """
+            Prints the help message.
+
+            Returns:
+                None
+            """
             msg = self.format_help()
             repl = re.compile(r'\]\s+\[')
             msg = repl.sub("] [", msg)
             msg = msg.replace(" [-h] [-v]", "")
             msg = msg.replace(", --help", "        ")
             print(msg)
 
@@ -366,22 +423,39 @@
         '-L',
         action='store_true',
         dest='L',
         help=f'input files are list of files',
     )
 
     parser.add_argument(
+        '-D',
+        action='store_true',
+        dest='D',
+        help=f'debugging (don\'t remove tmp dir)',
+    )
+
+    parser.add_argument(
+        '-V',
+        action='store_true',
+        dest='V',
+        help=f'verbose output',
+    )
+
+    parser.add_argument(
         'genomes',
         nargs="+",
         help='input genome file (fasta / gzipped fasta / list of files when "-L")',
     )
 
     args = parser.parse_args()
 
     #print(args)
-    attotree(fns=args.genomes, k=args.k, s=args.s, t=args.t, newick_fo=args.o, phylogeny_algorithm=args.f, fof=args.L)
+    attotree(
+        fns=args.genomes, k=args.k, s=args.s, t=args.t, newick_fo=args.o, phylogeny_algorithm=args.f, fof=args.L,
+        verbose=args.V, debug=args.D
+    )
 
     args = parser.parse_args()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `attotree-0.1.2/attotree.egg-info/PKG-INFO` & `attotree-0.1.3/attotree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attotree
-Version: 0.1.2
+Version: 0.1.3
 Summary: description
 Home-page: https://github.com/karel-brinda/attotree
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 Requires-Dist: wheel
 
 Attotree
-==================================================================================
+========
 
 
 Introduction
 ------------
 
 Rapid estimation of phylogenetic trees directly from FASTA files in the style of
 `Mashtree <https://github.com/lskatz/mashtree>`_. With the default options,
@@ -68,33 +68,35 @@
 Command-line parameters
 -----------------------
 
 
 .. code-block::
 
     $ attotree -h
-
+ 
     Program: attotree (rapid estimation of phylogenetic trees using sketching)
-    Version: 0.1.1
+    Version: 0.1.3
     Author:  Karel Brinda <karel.brinda@inria.fr>
 
-    usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] genomes [genomes ...]
+    usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] [-D] [-V] genomes [genomes ...]
 
     positional arguments:
       genomes     input genome file (fasta / gzipped fasta / list of files when "-L")
 
     options:
       -h          show this help message and exit
       -v          show program's version number and exit
       -k INT      kmer size [21]
       -s INT      sketch size [10000]
       -t INT      number of threads [10]
       -o FILE     newick output [stdout]
       -f STR      tree inference algorithm (nj/upgma) [nj]
       -L          input files are list of files
+      -D          debugging (don't remove tmp dir)
+      -V          verbose output
 
 
 
 Issues
 ------
 
 Please use `Github issues <https://github.com/karel-brinda/attotree/issues>`_.
@@ -112,8 +114,7 @@
 `MIT <https://github.com/karel-brinda/attotree/blob/master/LICENSE.txt>`_
 
 
 Authors
 -------
 
 `Karel Brinda <http://brinda.eu>`_ <karel.brinda@inria.fr>
-
```

### Comparing `attotree-0.1.2/setup.py` & `attotree-0.1.3/setup.py`

 * *Files identical despite different names*

