# Comparing `tmp/janus_core-0.2.0b1.tar.gz` & `tmp/janus_core-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.2.0b1.tar", max compression
+gzip compressed data, was "janus_core-0.2.0b2.tar", max compression
```

## Comparing `janus_core-0.2.0b1.tar` & `janus_core-0.2.0b2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1533 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/LICENSE
--rw-r--r--   0        0        0     6606 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/README.md
--rw-r--r--   0        0        0       80 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/janus_core/__init__.py
--rw-r--r--   0        0        0    28141 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/janus_core/cli.py
--rw-r--r--   0        0        0     4790 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/janus_core/geom_opt.py
--rw-r--r--   0        0        0     1664 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/janus_core/janus_types.py
--rw-r--r--   0        0        0     4045 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/janus_core/log.py
--rw-r--r--   0        0        0    29064 2024-04-05 08:14:54.043906 janus_core-0.2.0b1/janus_core/md.py
--rw-r--r--   0        0        0     3514 2024-04-05 08:14:54.047906 janus_core-0.2.0b1/janus_core/mlip_calculators.py
--rw-r--r--   0        0        0    12111 2024-04-05 08:14:54.047906 janus_core-0.2.0b1/janus_core/single_point.py
--rw-r--r--   0        0        0     3293 2024-04-05 08:14:54.047906 janus_core-0.2.0b1/janus_core/stats.py
--rw-r--r--   0        0        0      545 2024-04-05 08:14:54.047906 janus_core-0.2.0b1/janus_core/utils.py
--rw-r--r--   0        0        0     2529 2024-04-05 08:14:54.047906 janus_core-0.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 janus_core-0.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/LICENSE
+-rw-r--r--   0        0        0     8011 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/README.md
+-rw-r--r--   0        0        0       80 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/__init__.py
+-rw-r--r--   0        0        0    28266 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/cli.py
+-rw-r--r--   0        0        0     4790 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/geom_opt.py
+-rw-r--r--   0        0        0     1664 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/janus_types.py
+-rw-r--r--   0        0        0     4045 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/log.py
+-rw-r--r--   0        0        0    29064 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/md.py
+-rw-r--r--   0        0        0     3514 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/mlip_calculators.py
+-rw-r--r--   0        0        0    12111 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/single_point.py
+-rw-r--r--   0        0        0     3293 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/stats.py
+-rw-r--r--   0        0        0      545 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/utils.py
+-rw-r--r--   0        0        0     2553 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     9072 1970-01-01 00:00:00.000000 janus_core-0.2.0b2/PKG-INFO
```

### Comparing `janus_core-0.2.0b1/LICENSE` & `janus_core-0.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/README.md` & `janus_core-0.2.0b2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 - [x] Support for multiple MLIPs
   - MACE
   - M3GNET
   - CHGNET
 - [x] Single point calculations
 - [x] Geometry optimisation
-- [ ] Molecular Dynamics
+- [x] Molecular Dynamics
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
 - [ ] Nudge Elastic Band
 - [ ] Phonons
   - vibroscopy
 - [ ] Training ML potentials
@@ -65,38 +65,38 @@
 ### Single Point Calculations
 
 Perform a single point calcuation (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
 ```shell
 janus singlepoint --struct tests/data/NaCl.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}"
 ```
 
-This will calculate the energy, stress and forces and save this in `NaCl-results.xyz`, in addition to generating a log file, `singlepoint.log`.
+This will calculate the energy, stress and forces and save this in `NaCl-results.xyz`, in addition to generating a log file, `singlepoint.log`, and summary of inputs, `singlepoint_summary.yml`.
 
 Additional options may be specified. For example:
 
 ```shell
-janus singlepoint --struct tests/data/NaCl.cif --arch mace --calc-kwargs "{'model' : '/path/to/your/ml.model'}" --property energy --log './example.log' --write-kwargs "{'filename': './example.xyz'}"
+janus singlepoint --struct tests/data/NaCl.cif --arch mace --calc-kwargs "{'model' : '/path/to/your/ml.model'}" --properties energy --properties forces --log ./example.log --out ./example.xyz
 ```
 
-This defines the MLIP architecture and path to your locally saved model, as well as changing where the log and results files are saved.
+This calculates both forces and energies, defines the MLIP architecture and path to your locally saved model, and changes where the log and results files are saved.
 
 Note: the MACE calculator currently returns energy, forces and stress together, so in this case the choice of property will not change the output.
 
 For all options, run `janus singlepoint --help`.
 
 
 ### Geometry optimization
 
 Perform geometry optimization (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
 
 ```shell
 janus geomopt --struct tests/data/H2O.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}"
 ```
 
-This will optimize the atomic positions and save the resulting structure in `H2O-opt.xyz`, in addition to generating a log file, `geomopt.log`.
+This will optimize the atomic positions and save the resulting structure in `H2O-opt.xyz`, in addition to generating a log file, `geomopt.log`, and summary of inputs, `geomopt_summary.yml`.
 
 Additional options may be specified. This shares most options with `singlepoint`, as well as a few additional options, such as:
 
 ```shell
 janus geomopt --struct tests/data/NaCl.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}" --vectors-only --traj 'NaCl-traj.xyz'
 ```
 
@@ -115,15 +115,15 @@
 
 This will generate several output files:
 
 - Thermodynamical statistics every 100 steps, written to `NaCl-npt-T300.0-p1.0-stats.dat`
 - The structure trajectory every 100 steps, written to `NaCl-npt-T300.0-p1.0-traj.xyz`
 - The structure to be able to restart the dynamics every 1000 steps, written to `NaCl-npt-T300.0-p1.0-res-1000.xyz`
 - A log of the processes carried out, written to `md.log`
-
+- A summary of the inputs and start/end time, written to `md_summary.yml`.
 
 Additional options may be specified. For example:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --steps 1000 --timestep 0.5 --temp 300 --minimize --minimize-every 100 --rescale-velocities --remove-rot --rescale-every 100 --equil-steps 200
 ```
 
@@ -136,14 +136,49 @@
 
 This performs an NVE molecular dynamics simulation at 300K for 200 steps (0.2 ps), saving the trajectory every 10 steps after the first 100, and the thermodynamical statistics every 10 steps, as well as changing the output file names for both.
 
 
 For all options, run `janus md --help`.
 
 
+### Using configuration files
+
+Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
+
+For example, with the following configuration file and command:
+
+```yaml
+struct: "NaCl.cif"
+properties:
+  - "energy"
+out: "NaCl-results.xyz"
+arch: mace_mp
+calc_kwargs:
+  model: medium
+```
+
+```shell
+janus singlepoint --struct KCl.cif --out KCl-results.cif --config config.yml
+```
+
+This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
+
+
+> [!NOTE]
+> `properties` must be passed as a Yaml list, as above, not as a string.
+
+> [!WARNING]
+> Options in the Yaml file must use `_` instead of `-`.
+> For example, `calc_kwargs` should be used in the configuration file for the `--calc-kwargs` option.
+
+> [!WARNING]
+> If an option in the configuration file does not match any variable names, an error will **not** be raised.
+> Please check the summary file to ensure the configuration has been read correctly.
+
+
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
 
 Contributors to this project were funded by
```

### Comparing `janus_core-0.2.0b1/janus_core/cli.py` & `janus_core-0.2.0b2/janus_core/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Set up commandline interface."""
 
 import ast
 import datetime
 import logging
 from pathlib import Path
-from typing import Annotated, Optional, get_args
+from typing import Annotated, Optional, Union, get_args
 
 from ase import Atoms
 import typer
+from typer_config import use_yaml_config
 import yaml
 
 from janus_core.geom_opt import optimize
-from janus_core.janus_types import Ensembles
+from janus_core.janus_types import ASEReadArgs, Ensembles
 from janus_core.md import NPH, NPT, NVE, NVT, NVT_NH
 from janus_core.single_point import SinglePoint
 
 app = typer.Typer()
 
 
 class TyperDict:  #  pylint: disable=too-few-public-methods
@@ -47,28 +48,30 @@
         -------
         str
             Class name and value of string representing a dictionary.
         """
         return f"<TyperDict: value={self.value}>"
 
 
-def _parse_dict_class(value: str):
+def _parse_dict_class(value: Union[str, ASEReadArgs]):
     """
     Convert string input into a dictionary.
 
     Parameters
     ----------
     value : str
         String representing dictionary to be parsed.
 
     Returns
     -------
     TyperDict
         Parsed string as a dictionary.
     """
+    if isinstance(value, dict):
+        return TyperDict(value)
     return TyperDict(ast.literal_eval(value))
 
 
 def _parse_typer_dicts(typer_dicts: list[TyperDict]) -> list[dict]:
     """
     Convert list of TyperDict objects to list of dictionaries.
 
@@ -86,15 +89,18 @@
     ------
     ValueError
         If items in list are not converted to dicts.
     """
     for i, typer_dict in enumerate(typer_dicts):
         typer_dicts[i] = typer_dict.value if typer_dict else {}
         if not isinstance(typer_dicts[i], dict):
-            raise ValueError(f"{typer_dicts[i]} must be passed as a dictionary")
+            raise ValueError(
+                f"""{typer_dicts[i]} must be passed as a dictionary wrapped in quotes.\
+ For example, "{{'key' : value}}" """
+            )
     return typer_dicts
 
 
 def _dict_paths_to_strs(dictionary: dict) -> None:
     """
     Recursively iterate over dictionary, converting Path values to strings.
 
@@ -107,19 +113,17 @@
         if isinstance(value, dict):
             _dict_paths_to_strs(value)
         elif isinstance(value, Path):
             dictionary[key] = str(value)
 
 
 # Shared type aliases
-StructPath = Annotated[
-    Path, typer.Option("--struct", help="Path of structure to simulate.")
-]
+StructPath = Annotated[Path, typer.Option(help="Path of structure to simulate.")]
 Architecture = Annotated[
-    str, typer.Option("--arch", help="MLIP architecture to use for calculations.")
+    str, typer.Option(help="MLIP architecture to use for calculations.")
 ]
 Device = Annotated[str, typer.Option(help="Device to run calculations on.")]
 ReadKwargs = Annotated[
     TyperDict,
     typer.Option(
         parser=_parse_dict_class,
         help=(
@@ -155,122 +159,125 @@
             passed as a dictionary wrapped in quotes, e.g. "{'key' : value}".
              [default: "{}"]
             """
         ),
         metavar="DICT",
     ),
 ]
-LogFile = Annotated[Path, typer.Option("--log", help="Path to save logs to.")]
+LogPath = Annotated[Path, typer.Option(help="Path to save logs to.")]
 Summary = Annotated[
     Path, typer.Option(help="Path to save summary of inputs and start/end time.")
 ]
 
 
 @app.command(help="Perform single point calculations and save to file.")
-def singlepoint(  # pylint: disable=too-many-locals
-    struct_path: StructPath,
-    architecture: Architecture = "mace_mp",
+@use_yaml_config()
+def singlepoint(
+    # pylint: disable=too-many-locals
+    # numpydoc ignore=PR02
+    struct: StructPath,
+    arch: Architecture = "mace_mp",
     device: Device = "cpu",
     properties: Annotated[
         list[str],
         typer.Option(
-            "--property",
             help=(
                 "Properties to calculate. If not specified, 'energy', 'forces' "
                 "and 'stress' will be returned."
             ),
         ),
     ] = None,
-    out_file: Annotated[
+    out: Annotated[
         Path,
         typer.Option(
-            "--out",
             help=(
                 "Path to save structure with calculated results. Default is inferred "
                 "from name of structure file."
             ),
         ),
     ] = None,
     read_kwargs: ReadKwargs = None,
     calc_kwargs: CalcKwargs = None,
     write_kwargs: WriteKwargs = None,
-    log_file: LogFile = "singlepoint.log",
+    log: LogPath = "singlepoint.log",
     summary: Summary = "singlepoint_summary.yml",
 ):
     """
     Perform single point calculations and save to file.
 
     Parameters
     ----------
-    struct_path : Path
+    struct : Path
         Path of structure to simulate.
-    architecture : Optional[str]
+    arch : Optional[str]
         MLIP architecture to use for single point calculations.
         Default is "mace_mp".
     device : Optional[str]
         Device to run model on. Default is "cpu".
     properties : Optional[str]
         Physical properties to calculate. Default is "energy".
-    out_file : Optional[Path]
+    out : Optional[Path]
         Path to save structure with calculated results. Default is inferred from name
         of the structure file.
     read_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to ase.io.read. Default is {}.
     calc_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to the selected calculator. Default is {}.
     write_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to ase.io.write when saving results. Default is {}.
-    log_file : Optional[Path]
+    log : Optional[Path]
         Path to write logs to. Default is "singlepoint.log".
     summary : Path
         Path to save summary of inputs and start/end time. Default is
         singlepoint_summary.yml.
+    config : Path
+        Path to yaml configuration file to define the above options. Default is None.
     """
     [read_kwargs, calc_kwargs, write_kwargs] = _parse_typer_dicts(
         [read_kwargs, calc_kwargs, write_kwargs]
     )
 
     # Check filename for results not duplicated
     if "filename" in write_kwargs:
         raise ValueError("'filename' must be passed through the --out option")
 
     # Default filname for saving results determined in SinglePoint if not specified
-    if out_file:
-        write_kwargs["filename"] = out_file
+    if out:
+        write_kwargs["filename"] = out
 
     singlepoint_kwargs = {
-        "struct_path": struct_path,
-        "architecture": architecture,
+        "struct_path": struct,
+        "architecture": arch,
         "device": device,
         "read_kwargs": read_kwargs,
         "calc_kwargs": calc_kwargs,
-        "log_kwargs": {"filename": log_file, "filemode": "w"},
+        "log_kwargs": {"filename": log, "filemode": "w"},
     }
 
     # Initialise singlepoint structure and calculator
     s_point = SinglePoint(**singlepoint_kwargs)
 
     # Store inputs for yaml summary
     inputs = singlepoint_kwargs.copy()
 
     # Store only filename as filemode is not set by user
     del inputs["log_kwargs"]
-    inputs["log"] = log_file
+    inputs["log"] = log
 
     if isinstance(s_point.struct, Atoms):
         inputs["struct"] = {
             "n_atoms": len(s_point.struct),
-            "struct_path": struct_path,
+            "struct_path": struct,
             "struct_name": s_point.struct_name,
             "formula": s_point.struct.get_chemical_formula(),
         }
     else:
         inputs["traj"] = {
             "length": len(s_point.struct),
-            "struct_path": struct_path,
+            "struct_path": struct,
             "struct_name": s_point.struct_name,
             "struct": {
                 "n_atoms": len(s_point.struct[0]),
                 "formula": s_point.struct[0].get_chemical_formula(),
             },
         }
 
@@ -303,53 +310,47 @@
         )
     logging.shutdown()
 
 
 @app.command(
     help="Perform geometry optimization and save optimized structure to file.",
 )
-def geomopt(  # pylint: disable=too-many-arguments,too-many-locals
-    struct_path: StructPath,
-    fmax: Annotated[
-        float, typer.Option("--max-force", help="Maximum force for convergence.")
-    ] = 0.1,
+@use_yaml_config()
+def geomopt(
+    # pylint: disable=too-many-arguments,too-many-locals
+    # numpydoc ignore=PR02
+    struct: StructPath,
+    fmax: Annotated[float, typer.Option(help="Maximum force for convergence.")] = 0.1,
     steps: Annotated[
-        int, typer.Option("--steps", help="Maximum number of optimization steps.")
+        int, typer.Option(help="Maximum number of optimization steps.")
     ] = 1000,
-    architecture: Architecture = "mace_mp",
+    arch: Architecture = "mace_mp",
     device: Device = "cpu",
     vectors_only: Annotated[
         bool,
-        typer.Option(
-            "--vectors-only",
-            help=("Optimize cell vectors, as well as atomic positions."),
-        ),
+        typer.Option(help="Optimize cell vectors, as well as atomic positions."),
     ] = False,
     fully_opt: Annotated[
         bool,
         typer.Option(
-            "--fully-opt",
             help="Fully optimize the cell vectors, angles, and atomic positions.",
         ),
     ] = False,
-    out_file: Annotated[
+    out: Annotated[
         Path,
         typer.Option(
-            "--out",
             help=(
                 "Path to save optimized structure. Default is inferred from name "
                 "of structure file."
             ),
         ),
     ] = None,
-    traj_file: Annotated[
+    traj: Annotated[
         str,
-        typer.Option(
-            "--traj", help="Path if saving optimization frames.  [default: None]"
-        ),
+        typer.Option(help="Path if saving optimization frames.  [default: None]"),
     ] = None,
     read_kwargs: ReadKwargs = None,
     calc_kwargs: CalcKwargs = None,
     opt_kwargs: Annotated[
         TyperDict,
         typer.Option(
             parser=_parse_dict_class,
@@ -359,91 +360,93 @@
                 wrapped in quotes, e.g. "{'key' : value}".  [default: "{}"]
                 """
             ),
             metavar="DICT",
         ),
     ] = None,
     write_kwargs: WriteKwargs = None,
-    log_file: LogFile = "geomopt.log",
+    log: LogPath = "geomopt.log",
     summary: Summary = "geomopt_summary.yml",
 ):
     """
     Perform geometry optimization and save optimized structure to file.
 
     Parameters
     ----------
-    struct_path : Path
+    struct : Path
         Path of structure to simulate.
     fmax : float
         Set force convergence criteria for optimizer in units eV/Å.
         Default is 0.1.
     steps : int
         Set maximum number of optimization steps to run. Default is 1000.
-    architecture : Optional[str]
+    arch : Optional[str]
         MLIP architecture to use for geometry optimization.
         Default is "mace_mp".
     device : Optional[str]
         Device to run model on. Default is "cpu".
     vectors_only : bool
         Whether to optimize cell vectors, as well as atomic positions, by setting
         `hydrostatic_strain` in the filter function. Default is False.
     fully_opt : bool
         Whether to fully optimize the cell vectors, angles, and atomic positions.
         Default is False.
-    out_file : Optional[Path]
+    out : Optional[Path]
         Path to save optimized structure, or last structure if optimization did not
         converge. Default is inferred from name of structure file.
-    traj_file : Optional[str]
+    traj : Optional[str]
         Path if saving optimization frames. Default is None.
     read_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to ase.io.read. Default is {}.
     calc_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to the selected calculator. Default is {}.
     opt_kwargs : Optional[ASEOptArgs]
         Keyword arguments to pass to optimizer. Default is {}.
     write_kwargs : Optional[ASEWriteArgs]
         Keyword arguments to pass to ase.io.write when saving optimized structure.
         Default is {}.
-    log_file : Optional[Path]
+    log : Optional[Path]
         Path to write logs to. Default is "geomopt.log".
     summary : Path
         Path to save summary of inputs and start/end time. Default is
         geomopt_summary.yml.
+    config : Path
+        Path to yaml configuration file to define the above options. Default is None.
     """
     [read_kwargs, calc_kwargs, opt_kwargs, write_kwargs] = _parse_typer_dicts(
         [read_kwargs, calc_kwargs, opt_kwargs, write_kwargs]
     )
 
     # Set up single point calculator
     s_point = SinglePoint(
-        struct_path=struct_path,
-        architecture=architecture,
+        struct_path=struct,
+        architecture=arch,
         device=device,
         read_kwargs=read_kwargs,
         calc_kwargs=calc_kwargs,
-        log_kwargs={"filename": log_file, "filemode": "w"},
+        log_kwargs={"filename": log, "filemode": "w"},
     )
 
     # Check optimized structure path not duplicated
     if "filename" in write_kwargs:
         raise ValueError("'filename' must be passed through the --out option")
 
     # Check trajectory path not duplicated
     if "trajectory" in opt_kwargs:
         raise ValueError("'trajectory' must be passed through the --traj option")
 
     # Set default filname for writing optimized structure if not specified
-    if out_file:
-        write_kwargs["filename"] = out_file
+    if out:
+        write_kwargs["filename"] = out
     else:
         write_kwargs["filename"] = f"{s_point.struct_name}-opt.xyz"
 
     # Set same trajectory filenames to overwrite saved binary with xyz
-    opt_kwargs["trajectory"] = traj_file if traj_file else None
-    traj_kwargs = {"filename": traj_file} if traj_file else None
+    opt_kwargs["trajectory"] = traj if traj else None
+    traj_kwargs = {"filename": traj} if traj else None
 
     # Set hydrostatic_strain
     # If not passed --fully-opt or --vectors-only, will be unused
     filter_kwargs = {"hydrostatic_strain": vectors_only}
 
     # Use default filter if passed --fully-opt or --vectors-only
     # Otherwise override with None
@@ -456,33 +459,33 @@
         "steps": steps,
         "filter_kwargs": filter_kwargs,
         **fully_opt_dict,
         "opt_kwargs": opt_kwargs,
         "write_results": True,
         "write_kwargs": write_kwargs,
         "traj_kwargs": traj_kwargs,
-        "log_kwargs": {"filename": log_file, "filemode": "a"},
+        "log_kwargs": {"filename": log, "filemode": "a"},
     }
 
     # Store inputs for yaml summary
     inputs = optimize_kwargs.copy()
 
     # Store only filename as filemode is not set by user
     del inputs["log_kwargs"]
-    inputs["log"] = log_file
+    inputs["log"] = log
 
     inputs["struct"] = {
         "n_atoms": len(s_point.struct),
-        "struct_path": struct_path,
+        "struct_path": struct,
         "struct_name": s_point.struct_name,
         "formula": s_point.struct.get_chemical_formula(),
     }
 
     inputs["calc"] = {
-        "architecture": architecture,
+        "arch": arch,
         "device": device,
         "read_kwargs": read_kwargs,
         "calc_kwargs": calc_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
     _dict_paths_to_strs(inputs)
@@ -508,17 +511,20 @@
         )
     logging.shutdown()
 
 
 @app.command(
     help="Run molecular dynamics simulation, and save trajectory and statistics.",
 )
-def md(  # pylint: disable=too-many-arguments,too-many-locals,invalid-name
+@use_yaml_config()
+def md(
+    # pylint: disable=too-many-arguments,too-many-locals,invalid-name
+    # numpydoc ignore=PR02
     ensemble: Annotated[str, typer.Option(help="Name of thermodynamic ensemble.")],
-    struct_path: StructPath,
+    struct: StructPath,
     steps: Annotated[int, typer.Option(help="Number of steps in simulation.")] = 0,
     timestep: Annotated[
         float, typer.Option(help="Timestep for integrator, in fs.")
     ] = 1.0,
     temp: Annotated[float, typer.Option(help="Temperature, in K.")] = 300.0,
     thermostat_time: Annotated[
         float,
@@ -534,15 +540,15 @@
     ] = 2.0,
     pressure: Annotated[
         float, typer.Option(help="Pressure fpr NPT or NPH simulation, in bar.")
     ] = 0.0,
     friction: Annotated[
         float, typer.Option(help="Friction coefficient for NVT simulation, in fs^-1.")
     ] = 0.005,
-    architecture: Architecture = "mace_mp",
+    arch: Architecture = "mace_mp",
     device: Device = "cpu",
     read_kwargs: ReadKwargs = None,
     calc_kwargs: CalcKwargs = None,
     equil_steps: Annotated[
         int,
         typer.Option(
             help=("Maximum number of steps at which to perform optimization and reset")
@@ -636,29 +642,29 @@
     ] = False,
     traj_start: Annotated[
         int, typer.Option(help="Step to start saving trajectory.")
     ] = 0,
     traj_every: Annotated[
         int, typer.Option(help="Frequency of steps to save trajectory.")
     ] = 100,
-    log_file: LogFile = "md.log",
+    log: LogPath = "md.log",
     seed: Annotated[
         Optional[int],
         typer.Option(help="Random seed for numpy.random and random functions."),
     ] = None,
     summary: Summary = "md_summary.yml",
 ):
     """
     Run molecular dynamics simulation, and save trajectory and statistics.
 
     Parameters
     ----------
     ensemble : str
         Name of thermodynamic ensemble.
-    struct_path : Path
+    struct : Path
         Path of structure to simulate.
     steps : int
         Number of steps in simulation. Default is 0.
     timestep : float
         Timestep for integrator, in fs. Default is 1.0.
     temp : float
         Temperature, in K. Default is 300.
@@ -668,15 +674,15 @@
         Barostat time, in fs. Default is 75.0.
     bulk_modulus : float
         Bulk modulus, in GPa. Default is 2.0.
     pressure : float
         Pressure, in bar. Default is 0.0.
     friction : float
         Friction coefficient in fs^-1. Default is 0.005.
-    architecture : Optional[str]
+    arch : Optional[str]
         MLIP architecture to use for molecular dynamics.
         Default is "mace_mp".
     device : Optional[str]
         Device to run model on. Default is "cpu".
     read_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to ase.io.read. Default is {}.
     calc_kwargs : Optional[dict[str, Any]]
@@ -718,40 +724,42 @@
         Trajectory file to save. Default inferred from `file_prefix`.
     traj_append : bool
         Whether to append trajectory. Default is False.
     traj_start : int
         Step to start saving trajectory. Default is 0.
     traj_every : int
         Frequency of steps to save trajectory. Default is 100.
-    log_file : Optional[Path]
+    log : Optional[Path]
         Path to write logs to. Default is "md.log".
     seed : Optional[int]
         Random seed used by numpy.random and random functions, such as in Langevin.
         Default is None.
     summary : Path
         Path to save summary of inputs and start/end time. Default is md_summary.yml.
+    config : Path
+        Path to yaml configuration file to define the above options. Default is None.
     """
     [read_kwargs, calc_kwargs, minimize_kwargs] = _parse_typer_dicts(
         [read_kwargs, calc_kwargs, minimize_kwargs]
     )
 
     if not ensemble in get_args(Ensembles):
         raise ValueError(f"ensemble must be in {get_args(Ensembles)}")
 
     # Set up single point calculator
     s_point = SinglePoint(
-        struct_path=struct_path,
-        architecture=architecture,
+        struct_path=struct,
+        architecture=arch,
         device=device,
         read_kwargs=read_kwargs,
         calc_kwargs=calc_kwargs,
-        log_kwargs={"filename": log_file, "filemode": "w"},
+        log_kwargs={"filename": log, "filemode": "w"},
     )
 
-    log_kwargs = {"filename": log_file, "filemode": "a"}
+    log_kwargs = {"filename": log, "filemode": "a"}
 
     dyn_kwargs = {
         "struct": s_point.struct,
         "struct_name": s_point.struct_name,
         "timestep": timestep,
         "steps": steps,
         "temp": temp,
@@ -815,25 +823,25 @@
         dyn = NVT_NH(**dyn_kwargs)
 
     # Store inputs for yaml summary
     inputs = dyn_kwargs | {"ensemble": ensemble}
 
     # Store only filename as filemode is not set by user
     del inputs["log_kwargs"]
-    inputs["log"] = log_file
+    inputs["log"] = log
 
     inputs["struct"] = {
         "n_atoms": len(s_point.struct),
-        "struct_path": struct_path,
+        "struct_path": struct,
         "struct_name": s_point.struct_name,
         "formula": s_point.struct.get_chemical_formula(),
     }
 
     inputs["calc"] = {
-        "architecture": architecture,
+        "arch": arch,
         "device": device,
         "read_kwargs": read_kwargs,
         "calc_kwargs": calc_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
     _dict_paths_to_strs(inputs)
```

### Comparing `janus_core-0.2.0b1/janus_core/geom_opt.py` & `janus_core-0.2.0b2/janus_core/geom_opt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/janus_types.py` & `janus_core-0.2.0b2/janus_core/janus_types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/log.py` & `janus_core-0.2.0b2/janus_core/log.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/md.py` & `janus_core-0.2.0b2/janus_core/md.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/mlip_calculators.py` & `janus_core-0.2.0b2/janus_core/mlip_calculators.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/single_point.py` & `janus_core-0.2.0b2/janus_core/single_point.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/stats.py` & `janus_core-0.2.0b2/janus_core/stats.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/janus_core/utils.py` & `janus_core-0.2.0b2/janus_core/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b1/pyproject.toml` & `janus_core-0.2.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.2.0b1"
+version = "0.2.0b2"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
@@ -25,16 +25,17 @@
 [tool.poetry.scripts]
 janus = "janus_core.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ase = "^3.22.1"
 mace-torch = "^0.3.4"
-typer = "^0.9.0"
 pyaml = "^23.12.0"
+typer = "^0.9.0"
+typer-config = "^1.4.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^7.4.1"}
 pgtest = "^1.3.2"
 pytest = "^8.0"
 pytest-cov = "^4.1.0"
 tox = "^4.12.1"
```

### Comparing `janus_core-0.2.0b1/PKG-INFO` & `janus_core-0.2.0b2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: mace-torch (>=0.3.4,<0.4.0)
 Requires-Dist: pyaml (>=23.12.0,<24.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer-config (>=1.4.0,<2.0.0)
 Project-URL: Documentation, https://stfc.github.io/janus-core/
 Project-URL: Repository, https://github.com/stfc/janus-core/
 Description-Content-Type: text/markdown
 
 [![Build Status][ci-badge]][ci-link]
 [![Coverage Status][cov-badge]][cov-link]
 [![Docs status][docs-badge]][docs-link]
@@ -38,15 +39,15 @@
 
 - [x] Support for multiple MLIPs
   - MACE
   - M3GNET
   - CHGNET
 - [x] Single point calculations
 - [x] Geometry optimisation
-- [ ] Molecular Dynamics
+- [x] Molecular Dynamics
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
 - [ ] Nudge Elastic Band
 - [ ] Phonons
   - vibroscopy
 - [ ] Training ML potentials
@@ -90,38 +91,38 @@
 ### Single Point Calculations
 
 Perform a single point calcuation (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
 ```shell
 janus singlepoint --struct tests/data/NaCl.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}"
 ```
 
-This will calculate the energy, stress and forces and save this in `NaCl-results.xyz`, in addition to generating a log file, `singlepoint.log`.
+This will calculate the energy, stress and forces and save this in `NaCl-results.xyz`, in addition to generating a log file, `singlepoint.log`, and summary of inputs, `singlepoint_summary.yml`.
 
 Additional options may be specified. For example:
 
 ```shell
-janus singlepoint --struct tests/data/NaCl.cif --arch mace --calc-kwargs "{'model' : '/path/to/your/ml.model'}" --property energy --log './example.log' --write-kwargs "{'filename': './example.xyz'}"
+janus singlepoint --struct tests/data/NaCl.cif --arch mace --calc-kwargs "{'model' : '/path/to/your/ml.model'}" --properties energy --properties forces --log ./example.log --out ./example.xyz
 ```
 
-This defines the MLIP architecture and path to your locally saved model, as well as changing where the log and results files are saved.
+This calculates both forces and energies, defines the MLIP architecture and path to your locally saved model, and changes where the log and results files are saved.
 
 Note: the MACE calculator currently returns energy, forces and stress together, so in this case the choice of property will not change the output.
 
 For all options, run `janus singlepoint --help`.
 
 
 ### Geometry optimization
 
 Perform geometry optimization (using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "small" force-field):
 
 ```shell
 janus geomopt --struct tests/data/H2O.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}"
 ```
 
-This will optimize the atomic positions and save the resulting structure in `H2O-opt.xyz`, in addition to generating a log file, `geomopt.log`.
+This will optimize the atomic positions and save the resulting structure in `H2O-opt.xyz`, in addition to generating a log file, `geomopt.log`, and summary of inputs, `geomopt_summary.yml`.
 
 Additional options may be specified. This shares most options with `singlepoint`, as well as a few additional options, such as:
 
 ```shell
 janus geomopt --struct tests/data/NaCl.cif --arch mace_mp --calc-kwargs "{'model' : 'small'}" --vectors-only --traj 'NaCl-traj.xyz'
 ```
 
@@ -140,15 +141,15 @@
 
 This will generate several output files:
 
 - Thermodynamical statistics every 100 steps, written to `NaCl-npt-T300.0-p1.0-stats.dat`
 - The structure trajectory every 100 steps, written to `NaCl-npt-T300.0-p1.0-traj.xyz`
 - The structure to be able to restart the dynamics every 1000 steps, written to `NaCl-npt-T300.0-p1.0-res-1000.xyz`
 - A log of the processes carried out, written to `md.log`
-
+- A summary of the inputs and start/end time, written to `md_summary.yml`.
 
 Additional options may be specified. For example:
 
 ```shell
 janus md --ensemble nvt --struct tests/data/NaCl.cif --steps 1000 --timestep 0.5 --temp 300 --minimize --minimize-every 100 --rescale-velocities --remove-rot --rescale-every 100 --equil-steps 200
 ```
 
@@ -161,14 +162,49 @@
 
 This performs an NVE molecular dynamics simulation at 300K for 200 steps (0.2 ps), saving the trajectory every 10 steps after the first 100, and the thermodynamical statistics every 10 steps, as well as changing the output file names for both.
 
 
 For all options, run `janus md --help`.
 
 
+### Using configuration files
+
+Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
+
+For example, with the following configuration file and command:
+
+```yaml
+struct: "NaCl.cif"
+properties:
+  - "energy"
+out: "NaCl-results.xyz"
+arch: mace_mp
+calc_kwargs:
+  model: medium
+```
+
+```shell
+janus singlepoint --struct KCl.cif --out KCl-results.cif --config config.yml
+```
+
+This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
+
+
+> [!NOTE]
+> `properties` must be passed as a Yaml list, as above, not as a string.
+
+> [!WARNING]
+> Options in the Yaml file must use `_` instead of `-`.
+> For example, `calc_kwargs` should be used in the configuration file for the `--calc-kwargs` option.
+
+> [!WARNING]
+> If an option in the configuration file does not match any variable names, an error will **not** be raised.
+> Please check the summary file to ensure the configuration has been read correctly.
+
+
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
 
 Contributors to this project were funded by
```

