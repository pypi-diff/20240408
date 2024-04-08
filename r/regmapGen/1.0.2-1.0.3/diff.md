# Comparing `tmp/regmapGen-1.0.2.tar.gz` & `tmp/regmapGen-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regmapGen-1.0.2.tar", last modified: Wed Apr  3 19:40:34 2024, max compression
+gzip compressed data, was "regmapGen-1.0.3.tar", last modified: Mon Apr  8 18:00:52 2024, max compression
```

## Comparing `regmapGen-1.0.2.tar` & `regmapGen-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/
--rw-r--r--   0 paul      (1000) paul      (1000)     1081 2024-03-19 12:13:26.000000 regmapGen-1.0.2/LICENSE
--rw-r--r--   0 paul      (1000) paul      (1000)     7687 2024-04-03 19:40:34.009918 regmapGen-1.0.2/PKG-INFO
--rwxr-xr-x   0 paul      (1000) paul      (1000)     7145 2024-04-03 19:40:02.000000 regmapGen-1.0.2/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/regmapGen/
--rwxr-xr-x   0 paul      (1000) paul      (1000)      684 2024-03-19 12:32:41.000000 regmapGen-1.0.2/regmapGen/__init__.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     8438 2024-04-02 20:34:28.000000 regmapGen-1.0.2/regmapGen/__main__.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)    11204 2024-03-19 12:30:11.000000 regmapGen-1.0.2/regmapGen/bitfield.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     5087 2024-04-01 19:31:56.000000 regmapGen-1.0.2/regmapGen/config.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2877 2024-03-19 12:30:11.000000 regmapGen-1.0.2/regmapGen/enum.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)    37017 2024-04-03 19:33:06.000000 regmapGen-1.0.2/regmapGen/generators.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     7975 2024-03-19 12:45:29.000000 regmapGen-1.0.2/regmapGen/reg.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     9242 2024-04-03 19:33:51.000000 regmapGen-1.0.2/regmapGen/regmap.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/regmapGen/templates/
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2085 2024-03-23 10:32:06.000000 regmapGen-1.0.2/regmapGen/templates/amm2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     1618 2024-03-23 10:30:08.000000 regmapGen-1.0.2/regmapGen/templates/apb2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     5259 2024-03-23 10:30:44.000000 regmapGen-1.0.2/regmapGen/templates/axil2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     3764 2024-03-23 10:18:16.000000 regmapGen-1.0.2/regmapGen/templates/c_header.j2
--rw-r--r--   0 paul      (1000) paul      (1000)     3267 2024-04-02 18:39:12.000000 regmapGen-1.0.2/regmapGen/templates/cmsis_svd.j2
--rw-r--r--   0 paul      (1000) paul      (1000)     3526 2024-04-02 19:39:18.000000 regmapGen-1.0.2/regmapGen/templates/ipxact_xml.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2943 2024-03-26 19:41:45.000000 regmapGen-1.0.2/regmapGen/templates/regmap_asciidoc.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     3227 2024-03-26 19:42:25.000000 regmapGen-1.0.2/regmapGen/templates/regmap_md.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2544 2024-03-19 12:51:37.000000 regmapGen-1.0.2/regmapGen/templates/regmap_py.j2
--rw-r--r--   0 paul      (1000) paul      (1000)     3637 2024-04-02 20:53:31.000000 regmapGen-1.0.2/regmapGen/templates/regmap_rst.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)    15879 2024-03-26 19:10:36.000000 regmapGen-1.0.2/regmapGen/templates/regmap_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     9730 2024-03-23 10:33:02.000000 regmapGen-1.0.2/regmapGen/templates/spi2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     1656 2024-03-26 16:16:54.000000 regmapGen-1.0.2/regmapGen/templates/sv_header.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     1900 2024-03-23 10:10:08.000000 regmapGen-1.0.2/regmapGen/templates/sv_package.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     5878 2024-03-19 12:30:11.000000 regmapGen-1.0.2/regmapGen/utils.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/regmapGen.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     7687 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)      881 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       55 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/entry_points.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      124 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       10 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/top_level.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2024-04-03 19:40:34.009918 regmapGen-1.0.2/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1251 2024-04-02 20:23:34.000000 regmapGen-1.0.2/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-08 18:00:52.182325 regmapGen-1.0.3/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1061 2024-04-07 19:53:03.000000 regmapGen-1.0.3/LICENSE
+-rw-r--r--   0 paul      (1000) paul      (1000)     7687 2024-04-08 18:00:52.182325 regmapGen-1.0.3/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7145 2024-04-07 19:53:03.000000 regmapGen-1.0.3/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-08 18:00:52.182325 regmapGen-1.0.3/regmapGen/
+-rw-r--r--   0 paul      (1000) paul      (1000)      572 2024-04-08 17:19:43.000000 regmapGen-1.0.3/regmapGen/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8332 2024-04-08 17:36:38.000000 regmapGen-1.0.3/regmapGen/__main__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    11204 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/bitfield.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5087 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/config.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2877 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/enum.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    37862 2024-04-08 17:28:02.000000 regmapGen-1.0.3/regmapGen/generators.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7975 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/reg.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9012 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/regmap.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-08 18:00:52.182325 regmapGen-1.0.3/regmapGen/templates/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2085 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/amm2lb_sv.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     1556 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/apb2lb_sv.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     5095 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/axil2lb_sv.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3764 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/c_header.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3177 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/cmsis_svd.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3442 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/ipxact_xml.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     2837 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/regmap_asciidoc.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3227 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/regmap_md.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     2544 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/regmap_py.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3490 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/regmap_rst.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)    15879 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/regmap_sv.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     9422 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/spi2lb_sv.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     1656 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/sv_header.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     1900 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/templates/sv_package.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     5959 2024-04-08 17:48:09.000000 regmapGen-1.0.3/regmapGen/templates/sv_wrapper.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     5878 2024-04-07 19:53:03.000000 regmapGen-1.0.3/regmapGen/utils.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-08 18:00:52.182325 regmapGen-1.0.3/regmapGen.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     7687 2024-04-08 18:00:52.000000 regmapGen-1.0.3/regmapGen.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)      915 2024-04-08 18:00:52.000000 regmapGen-1.0.3/regmapGen.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-04-08 18:00:52.000000 regmapGen-1.0.3/regmapGen.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       55 2024-04-08 18:00:52.000000 regmapGen-1.0.3/regmapGen.egg-info/entry_points.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      124 2024-04-08 18:00:52.000000 regmapGen-1.0.3/regmapGen.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       10 2024-04-08 18:00:52.000000 regmapGen-1.0.3/regmapGen.egg-info/top_level.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2024-04-08 18:00:52.182325 regmapGen-1.0.3/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1251 2024-04-08 17:55:21.000000 regmapGen-1.0.3/setup.py
```

### Comparing `regmapGen-1.0.2/PKG-INFO` & `regmapGen-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regmapGen
-Version: 1.0.2
+Version: 1.0.3
 Summary: Генератор Регистровой Карты
 Home-page: https://github.com/paulmsv/regmapGen
 Author: paulmsv
 Author-email: bobkovpg@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://regmapGen.readthedocs.io
 Platform: UNKNOWN
```

### Comparing `regmapGen-1.0.2/README.md` & `regmapGen-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/__init__.py` & `regmapGen-1.0.3/regmapGen/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 
 """regmapGen это Генератор Регистровой Карты.
 Он позволяет автоматически создавать пригодный для синтеза SystemVerilog код и документацию.
 """
 
 __title__ = "regmapGen"
 __description__ = "Генератор Регистровой Карты."
-
-try:
-    from ._version import version as __version__
-except (ImportError, ModuleNotFoundError) as e:
-    __version__ = 'git-latest'
+__version__ = '1.0.3'
 
 from . import config
 from .enum import EnumValue
 from .bitfield import BitField
 from .reg import Register
 from .regmap import RegisterMap
 from . import generators
```

### Comparing `regmapGen-1.0.2/regmapGen/__main__.py` & `regmapGen-1.0.3/regmapGen/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,222 +1,223 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-"""Run regmapGen from command line with arguments.
-"""
-
-import sys
-import os
-import argparse
-from pathlib import Path
-import regmapGen
-from . import utils
-from contextlib import contextmanager
-import importlib.util
-
-__all__ = ['main']
-
-
-@contextmanager
-def cwd(path):
-    oldpwd = os.getcwd()
-    os.chdir(path)
-    try:
-        yield
-    finally:
-        os.chdir(oldpwd)
-
-
-class ArgumentParser(argparse.ArgumentParser):
-    """Inherit ArgumentParser to override the behaviour of error method."""
-
-    def error(self, message):
-        self.print_help(sys.stderr)
-        self.exit(2, '\n%s: error: %s\n' % (self.prog, message))
-
-
-def parse_arguments():
-    """Parse and validate arguments."""
-    parser = ArgumentParser(prog=regmapGen.__title__,
-                            description=regmapGen.__description__)
-    parser.add_argument('-v', '--version',
-                        action='version',
-                        version='%(prog)s v' + regmapGen.__version__)
-    parser.add_argument(metavar='WORKDIR',
-                        nargs='?',
-                        dest='workdir_path',
-                        default=os.getcwd(),
-                        help='working directory (default is the current directory)')
-    parser.add_argument('-r',
-                        metavar='REGMAP',
-                        dest='regmap_path',
-                        help='read register map from file')
-    parser.add_argument('-c',
-                        metavar='CONFIG',
-                        dest='config_path',
-                        help='read configuration from file')
-    template_choices = ['json', 'yaml', 'txt']
-    parser.add_argument('-t',
-                        metavar='FORMAT',
-                        choices=template_choices,
-                        dest='template_format',
-                        help='create templates (choose from %s)' % ', '.join(template_choices))
-    return parser.parse_args()
-
-
-def generate_templates(format):
-    print("... templates format: '%s'" % format)
-    # global configuration
-    globcfg = regmapGen.config.default_globcfg()
-    globcfg['data_width'] = 32
-    globcfg['address_width'] = 16
-    globcfg['register_reset'] = 'sync_pos'
-    regmapGen.config.set_globcfg(globcfg)
-
-    # targets
-    targets = {}
-    targets.update(regmapGen.generators.SystemVerilog(path="hw/regs.sv").make_target('sv_module'))
-    targets.update(regmapGen.generators.SystemVerilogHeader(path="hw/regs.svh").make_target('sv_header'))
-    targets.update(regmapGen.generators.SystemVerilogPackage(path="hw/regs_pkg.sv").make_target('sv_pkg'))
-    targets.update(regmapGen.generators.Python(path="sw/regs.py").make_target('py'))
-    targets.update(regmapGen.generators.CHeader(path="sw/regs.h").make_target('c_header'))
-    targets.update(regmapGen.generators.CmsisSvd(path="sw/regs.svd").make_target('cmsis_svd'))
-    targets.update(regmapGen.generators.IpxactXml(path="sw/regs.xml").make_target('ipxact_xml'))
-    targets.update(regmapGen.generators.Markdown(path="doc/regs.md", image_dir="md_img").make_target('md_doc'))
-    targets.update(regmapGen.generators.Asciidoc(path="doc/regs.adoc", image_dir="adoc_img").make_target('asciidoc_doc'))
-    targets.update(regmapGen.generators.Rst(path="doc/regs.rst", image_dir="rst_img").make_target('rst_doc'))
-    targets.update(regmapGen.generators.Docx(path="doc/regs.docx").make_target('docx_doc'))
-
-    # create templates
-    if format == 'txt':
-        rmap = regmapGen.utils.create_template_simple()
-    else:
-        rmap = regmapGen.utils.create_template()
-    # register map template
-    if format == 'json':
-        gen = regmapGen.generators.Json(rmap)
-        regmap_path = 'regs.json'
-    elif format == 'yaml':
-        gen = regmapGen.generators.Yaml(rmap)
-        regmap_path = 'regs.yaml'
-    elif format == 'txt':
-        gen = regmapGen.generators.Txt(rmap)
-        regmap_path = 'regs.txt'
-    print("... generate register map file '%s'" % regmap_path)
-    gen.generate()
-    # configuration file template
-    config_path = 'config'
-    globcfg['regmap_path'] = regmap_path
-    print("... generate configuration file '%s'" % config_path)
-    regmapGen.config.write_config(config_path, globcfg, targets)
-
-
-def die(msg):
-    print("Error: %s" % msg)
-    exit(1)
-
-
-def finish():
-    print('Success!')
-    exit(0)
-
-
-def app(args):
-    print("... set working directory '%s'" % args.workdir_path)
-
-    # check if teplates are needed
-    if args.template_format:
-        generate_templates(args.template_format)
-        finish()
-
-    # check if configuration file path was provided
-    if args.config_path:
-        config_path = Path(args.config_path)
-    else:
-        config_path = Path('config')
-    # check it existance
-    if not config_path.is_file():
-        die("Can't find configuration file '%s'!" % config_path)
-    # try to read it
-    print("... read configuration file '%s'" % config_path)
-    globcfg, targets = regmapGen.config.read_config(config_path)
-
-    # Execute Xls2Yaml target if present, before anything else
-    pre_target = next((target for target in targets.values() if target.get('generator') == 'Xls2Yaml'), None)
-    pre_target_name = next((key for key, value in targets.items() if value.get('generator') == 'Xls2Yaml'), None)
-    if pre_target:
-        # Generate YAML from Excel before reading regmap
-        print("... make '%s': Xls2Yaml -> '%s':" % (pre_target_name, pre_target.get('path')))
-        regmapGen.generators.Xls2Yaml(path=pre_target.get('path'), input_xls=pre_target.get('input_xls')).generate()
-        # Remove Xls2Yaml target from targets to avoid its re-execution in make targets section
-        targets.pop(pre_target_name, None)
-
-    # check if regiter map file path was provided
-    if args.regmap_path:
-        regmap_path = Path(args.regmap_path)
-        globcfg['regmap_path'] = regmap_path
-    elif 'regmap_path' in globcfg.keys():
-        regmap_path = Path(globcfg['regmap_path'])
-    else:
-        regmap_path = None
-        print("Warning: No register map file was specified!")
-    regmapGen.config.set_globcfg(globcfg)
-
-    if regmap_path:
-        # check it existance
-        if not regmap_path.is_file():
-            die("Can't find register map file '%s'!" % regmap_path)
-
-        # try to read it
-        print("... read register map file '%s'" % regmap_path)
-        rmap = regmapGen.RegisterMap()
-        rmap.read_file(regmap_path)
-        print("... validate register map")
-        rmap.validate()
-    else:
-        rmap = None
-
-    # make targets
-    if not targets:
-        die("No targets were specified! Nothing to do!")
-    for t in targets:
-        print("... make '%s': " % t, end='')
-        if 'generator' not in targets[t].keys():
-            die("No generator was specified for the target!")
-
-        if '.py::' in targets[t]['generator']:
-            custom_module_path, custom_generator_name = targets[t]['generator'].split('::')
-            custom_module_name = utils.get_file_name(custom_module_path)
-            spec = importlib.util.spec_from_file_location(custom_module_name, custom_module_path)
-            custom_module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(custom_module)
-            try:
-                gen_obj = getattr(custom_module, custom_generator_name)
-                gen_name = custom_generator_name
-            except AttributeError:
-                die("Generator '%s' from module '%s' does not exist!" % (custom_generator_name, custom_module_path))
-        else:
-            gen_name = targets[t]['generator']
-            try:
-                gen_obj = getattr(regmapGen.generators, gen_name)
-            except AttributeError:
-                die("Generator '%s' does not exist!" % gen_name)
-
-        gen_args = targets[t]
-        print("%s -> '%s': " % (gen_name, gen_args['path']))
-        gen_obj(rmap, **gen_args).generate()
-
-
-def main():
-    """Program main"""
-    # parse arguments
-    args = parse_arguments()
-
-    # do all the things inside working directory
-    args.workdir_path = str(Path(args.workdir_path).absolute())
-    with cwd(args.workdir_path):
-        app(args)
-    finish()
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""Run regmapGen from command line with arguments.
+"""
+
+import sys
+import os
+import argparse
+from pathlib import Path
+import regmapGen
+from . import utils
+from contextlib import contextmanager
+import importlib.util
+
+__all__ = ['main']
+
+
+@contextmanager
+def cwd(path):
+    oldpwd = os.getcwd()
+    os.chdir(path)
+    try:
+        yield
+    finally:
+        os.chdir(oldpwd)
+
+
+class ArgumentParser(argparse.ArgumentParser):
+    """Inherit ArgumentParser to override the behaviour of error method."""
+
+    def error(self, message):
+        self.print_help(sys.stderr)
+        self.exit(2, '\n%s: error: %s\n' % (self.prog, message))
+
+
+def parse_arguments():
+    """Parse and validate arguments."""
+    parser = ArgumentParser(prog=regmapGen.__title__,
+                            description=regmapGen.__description__)
+    parser.add_argument('-v', '--version',
+                        action='version',
+                        version='%(prog)s v' + regmapGen.__version__)
+    parser.add_argument(metavar='WORKDIR',
+                        nargs='?',
+                        dest='workdir_path',
+                        default=os.getcwd(),
+                        help='working directory (default is the current directory)')
+    parser.add_argument('-r',
+                        metavar='REGMAP',
+                        dest='regmap_path',
+                        help='read register map from file')
+    parser.add_argument('-c',
+                        metavar='CONFIG',
+                        dest='config_path',
+                        help='read configuration from file')
+    template_choices = ['json', 'yaml', 'txt']
+    parser.add_argument('-t',
+                        metavar='FORMAT',
+                        choices=template_choices,
+                        dest='template_format',
+                        help='create templates (choose from %s)' % ', '.join(template_choices))
+    return parser.parse_args()
+
+
+def generate_templates(format):
+    print("... templates format: '%s'" % format)
+    # global configuration
+    globcfg = regmapGen.config.default_globcfg()
+    globcfg['data_width'] = 32
+    globcfg['address_width'] = 16
+    globcfg['register_reset'] = 'sync_pos'
+    regmapGen.config.set_globcfg(globcfg)
+
+    # targets
+    targets = {}
+    targets.update(regmapGen.generators.SystemVerilog(path="hw/regs.sv").make_target('sv_module'))
+    targets.update(regmapGen.generators.SystemVerilogWrapper(path="hw/regs_wrapper.svh").make_target('sv_wrapper'))
+    targets.update(regmapGen.generators.SystemVerilogHeader(path="hw/regs.svh").make_target('sv_header'))
+    targets.update(regmapGen.generators.SystemVerilogPackage(path="hw/regs_pkg.sv").make_target('sv_pkg'))
+    targets.update(regmapGen.generators.Python(path="sw/regs.py").make_target('py'))
+    targets.update(regmapGen.generators.CHeader(path="sw/regs.h").make_target('c_header'))
+    targets.update(regmapGen.generators.CmsisSvd(path="sw/regs.svd").make_target('cmsis_svd'))
+    targets.update(regmapGen.generators.IpxactXml(path="sw/regs.xml").make_target('ipxact_xml'))
+    targets.update(regmapGen.generators.Markdown(path="doc/regs.md", image_dir="md_img").make_target('md_doc'))
+    targets.update(regmapGen.generators.Asciidoc(path="doc/regs.adoc", image_dir="adoc_img").make_target('asciidoc_doc'))
+    targets.update(regmapGen.generators.Rst(path="doc/regs.rst", image_dir="rst_img").make_target('rst_doc'))
+    targets.update(regmapGen.generators.Docx(path="doc/regs.docx").make_target('docx_doc'))
+
+    # create templates
+    if format == 'txt':
+        rmap = regmapGen.utils.create_template_simple()
+    else:
+        rmap = regmapGen.utils.create_template()
+    # register map template
+    if format == 'json':
+        gen = regmapGen.generators.Json(rmap)
+        regmap_path = 'regs.json'
+    elif format == 'yaml':
+        gen = regmapGen.generators.Yaml(rmap)
+        regmap_path = 'regs.yaml'
+    elif format == 'txt':
+        gen = regmapGen.generators.Txt(rmap)
+        regmap_path = 'regs.txt'
+    print("... generate register map file '%s'" % regmap_path)
+    gen.generate()
+    # configuration file template
+    config_path = 'config'
+    globcfg['regmap_path'] = regmap_path
+    print("... generate configuration file '%s'" % config_path)
+    regmapGen.config.write_config(config_path, globcfg, targets)
+
+
+def die(msg):
+    print("Error: %s" % msg)
+    exit(1)
+
+
+def finish():
+    print('Success!')
+    exit(0)
+
+
+def app(args):
+    print("... set working directory '%s'" % args.workdir_path)
+
+    # check if teplates are needed
+    if args.template_format:
+        generate_templates(args.template_format)
+        finish()
+
+    # check if configuration file path was provided
+    if args.config_path:
+        config_path = Path(args.config_path)
+    else:
+        config_path = Path('config')
+    # check it existance
+    if not config_path.is_file():
+        die("Can't find configuration file '%s'!" % config_path)
+    # try to read it
+    print("... read configuration file '%s'" % config_path)
+    globcfg, targets = regmapGen.config.read_config(config_path)
+
+    # Execute Xls2Yaml target if present, before anything else
+    pre_target = next((target for target in targets.values() if target.get('generator') == 'Xls2Yaml'), None)
+    pre_target_name = next((key for key, value in targets.items() if value.get('generator') == 'Xls2Yaml'), None)
+    if pre_target:
+        # Generate YAML from Excel before reading regmap
+        print("... make '%s': Xls2Yaml -> '%s':" % (pre_target_name, pre_target.get('path')))
+        regmapGen.generators.Xls2Yaml(path=pre_target.get('path'), input_xls=pre_target.get('input_xls')).generate()
+        # Remove Xls2Yaml target from targets to avoid its re-execution in make targets section
+        targets.pop(pre_target_name, None)
+
+    # check if regiter map file path was provided
+    if args.regmap_path:
+        regmap_path = Path(args.regmap_path)
+        globcfg['regmap_path'] = regmap_path
+    elif 'regmap_path' in globcfg.keys():
+        regmap_path = Path(globcfg['regmap_path'])
+    else:
+        regmap_path = None
+        print("Warning: No register map file was specified!")
+    regmapGen.config.set_globcfg(globcfg)
+
+    if regmap_path:
+        # check it existance
+        if not regmap_path.is_file():
+            die("Can't find register map file '%s'!" % regmap_path)
+
+        # try to read it
+        print("... read register map file '%s'" % regmap_path)
+        rmap = regmapGen.RegisterMap()
+        rmap.read_file(regmap_path)
+        print("... validate register map")
+        rmap.validate()
+    else:
+        rmap = None
+
+    # make targets
+    if not targets:
+        die("No targets were specified! Nothing to do!")
+    for t in targets:
+        print("... make '%s': " % t, end='')
+        if 'generator' not in targets[t].keys():
+            die("No generator was specified for the target!")
+
+        if '.py::' in targets[t]['generator']:
+            custom_module_path, custom_generator_name = targets[t]['generator'].split('::')
+            custom_module_name = utils.get_file_name(custom_module_path)
+            spec = importlib.util.spec_from_file_location(custom_module_name, custom_module_path)
+            custom_module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(custom_module)
+            try:
+                gen_obj = getattr(custom_module, custom_generator_name)
+                gen_name = custom_generator_name
+            except AttributeError:
+                die("Generator '%s' from module '%s' does not exist!" % (custom_generator_name, custom_module_path))
+        else:
+            gen_name = targets[t]['generator']
+            try:
+                gen_obj = getattr(regmapGen.generators, gen_name)
+            except AttributeError:
+                die("Generator '%s' does not exist!" % gen_name)
+
+        gen_args = targets[t]
+        print("%s -> '%s': " % (gen_name, gen_args['path']))
+        gen_obj(rmap, **gen_args).generate()
+
+
+def main():
+    """Program main"""
+    # parse arguments
+    args = parse_arguments()
+
+    # do all the things inside working directory
+    args.workdir_path = str(Path(args.workdir_path).absolute())
+    with cwd(args.workdir_path):
+        app(args)
+    finish()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `regmapGen-1.0.2/regmapGen/bitfield.py` & `regmapGen-1.0.3/regmapGen/bitfield.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/config.py` & `regmapGen-1.0.3/regmapGen/config.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/enum.py` & `regmapGen-1.0.3/regmapGen/enum.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/generators.py` & `regmapGen-1.0.3/regmapGen/generators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,922 +1,968 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-"""Output file generators
-"""
-
-import os
-import json
-import yaml
-import jinja2
-from regmapGen import __version__
-from . import utils
-from . import config
-from .regmap import RegisterMap
-from pathlib import Path
-import wavedrom
-import subprocess
-import pandas as pd
-from ruamel.yaml.scalarstring import PreservedScalarString as pss
-from ruamel.yaml import YAML
-import numpy as np
-
-class Generator():
-    """Base generator class.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    """
-
-    def __init__(self, rmap, **args):
-        self.rmap = rmap
-        self.etc = args
-
-    def _name(self):
-        return self.__class__.__name__
-
-    def generate(self):
-        """Do file generation."""
-        pass
-
-    def validate(self):
-        """Validate generator parameters."""
-        # config
-        config.validate_globcfg(config.globcfg)
-        # rmap
-        assert isinstance(self.rmap, RegisterMap), \
-            "Register map has to be '%s', but '%s' was provided for '%s' generator!" % (
-                repr(RegisterMap()), repr(self.rmap), self._name())
-        self.rmap.validate()
-
-    def make_target(self, name):
-        """Dump class attributes to dictionary that can be used as target for `config` generation.
-
-        :param name: Name of the target
-        :return: Target dictionary
-        """
-        params = vars(self)
-        params.pop('etc')
-        params.pop('rmap')
-        params['generator'] = self._name()
-        return {name: params}
-
-
-class Jinja2():
-    """Basic class for rendering Jinja2 templates"""
-
-    def render(self, template, vars, templates_path=None):
-        """Render text with Jinja2.
-
-        :param template: Jinja2 template filename
-        :param vars: Dictionary with variables for Jinja2 rendering
-        :param templates_path: Path to search templates. If no path provided, then internal templates will be used
-        :return: String with rendered text
-        """
-        # prepare template
-        if not templates_path:
-            templates_path = str(Path(__file__).parent / 'templates')
-        j2_env = jinja2.Environment(loader=jinja2.FileSystemLoader(searchpath=templates_path),
-                                    trim_blocks=True, lstrip_blocks=True)
-        j2_env.globals.update(zip=zip)
-        j2_template = j2_env.get_template(template)
-        # render
-        return j2_template.render(vars)
-
-    def render_to_file(self, template, vars, path, templates_path=None):
-        """Render text with Jinja2 and save it to the file.
-
-        :param template: Jinja2 template filename
-        :param vars: Dictionary with variables for Jinja2 rendering
-        :param path: Path to the output file
-        :param templates_path: Path to search templates. If no path provided, then internal templates will be used
-        """
-        # render
-        rendered_text = self.render(template, vars, templates_path)
-        # save
-        utils.create_dirs(self.path)
-        with open(path, "w", encoding="utf-8") as f:
-            f.write(rendered_text)
-
-
-class Wavedrom():
-    """Basic class for rendering register images with wavedrom"""
-
-    def draw_regs(self, imgdir, rmap):
-        imgdir.mkdir(exist_ok=True)
-
-        bits = config.globcfg['data_width']
-        lanes = bits // 8 if bits > 8 else 1
-        for reg in rmap:
-            reg_wd = {"reg": [],
-                      "config": {"bits": bits, "lanes": lanes, "fontsize": 14, "vspace": 100, "fontfamily": 'Arial'}}
-            bit_pos = -1
-            for bf in reg:
-                if bit_pos == -1 and bf.lsb > 0:
-                    reg_wd["reg"].append({"bits": bf.lsb})
-                elif bf.lsb - bit_pos > 1:
-                    reg_wd["reg"].append({"bits": bf.lsb - bit_pos - 1})
-                name = bf.name
-                #name_max_len = 5 * bf.width
-                #if len(bf.name) > name_max_len:  # to prevent labels overlapping
-                #    name = bf.name[:name_max_len - 1] + '..'
-                reg_wd["reg"].append({"name": name, "attr": bf.access, "bits": bf.width})
-                bit_pos = bf.msb
-            if (bits - 1) > bit_pos:
-                reg_wd["reg"].append({"bits": bits - bit_pos - 1})
-            wavedrom.render(json.dumps(reg_wd)).saveas(str(imgdir / ("%s.svg" % reg.name.lower())))
-
-
-class Json(Generator):
-    """Dump register map to a JSON file.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.json', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-
-    def generate(self):
-        # validate register map
-        self.rmap.validate()
-        # prepare data
-        data = {'regmap': list(self.rmap.as_dict().values())}
-        # dump
-        utils.create_dirs(self.path)
-        with open(self.path, 'w', encoding="utf-8") as f:
-            json.dump(data, f, indent=4)
-
-
-class Yaml(Generator):
-    """Dump register map to a YAML file.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.yaml', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare data
-        data = {'regmap': list(self.rmap.as_dict().values())}
-        # dump
-        utils.create_dirs(self.path)
-        with open(self.path, 'w', encoding="utf-8") as f:
-            yaml.Dumper.ignore_aliases = lambda *args: True  # hack to disable aliases
-            yaml.dump(data, f, indent=4, default_flow_style=False, sort_keys=False)
-
-
-class Txt(Generator):
-    """Dump register map to a text table.
-
-    Note: only registers with single bitfield are allowed.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.txt', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        for reg in self.rmap:
-            if len(reg) > 1:
-                raise ValueError("Only registers with single bitfield are allowed for %s generator." % self._name())
-        # prepare template strings
-        data_w = config.globcfg['data_width']
-        address_w = config.globcfg['address_width']
-        address_digits = address_w // 4 + (1 if address_w % 4 else 0)
-        address_str = "0x%0{0}x".format(address_digits)
-        reset_digits = data_w // 4 + (1 if data_w % 4 else 0)
-        reset_str = "0x%0{0}x".format(reset_digits)
-        row_template = "| %-{0}s | %-{1}s | %-{2}s | %-{3}s | %-{4}s | %-{5}s | %-{6}s |\n"
-        # prepare table data
-        row_top = ["Address", "Name", "Width", "Access", "Hardware", "Reset", "Description"]
-        col_address = [address_str % reg.address for reg in self.rmap]
-        col_names = self.rmap.reg_names
-        col_width = ["%d" % reg.bitfields[0].width for reg in self.rmap]
-        col_access = [reg.bitfields[0].access for reg in self.rmap]
-        col_hardware = [reg.bitfields[0].hardware for reg in self.rmap]
-        col_reset = [reset_str % reg.reset for reg in self.rmap]
-        col_description = [reg.description for reg in self.rmap]
-        # calculate width of the columns for pretty printing
-        cols_w = [max(address_digits + 2, len(row_top[0])),
-                  max(max([len(s) for s in col_names]), len(row_top[1])),
-                  max(max([len(s) for s in col_width]), len(row_top[2])),
-                  max(max([len(s) for s in col_access]), len(row_top[3])),
-                  max(max([len(s) for s in col_hardware]), len(row_top[4])),
-                  max(reset_digits + 2, len(row_top[5])),
-                  max(max([len(s) for s in col_description]), len(row_top[6]))]
-        row_template = row_template.format(*cols_w)
-        # render
-        out_lines = [row_template % tuple(row_top)]
-        out_lines.append(row_template % tuple(["-" * w for w in cols_w]))
-        for i in range(len(col_names)):
-            out_lines.append(row_template % (col_address[i], col_names[i],
-                             col_width[i], col_access[i], col_hardware[i], col_reset[i], col_description[i]))
-        # save to file
-        utils.create_dirs(self.path)
-        with open(self.path, 'w', encoding="utf-8") as f:
-            f.writelines(out_lines)
-
-
-class SystemVerilog(Generator, Jinja2):
-    """Create SystemVerilog file with register map.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param read_filler: Numeric value to return if wrong address was read
-    :type read_filler: int
-    :param interface: Register map bus protocol. Use one of: `axil`, `apb`, `amm`, `spi`, `lb`
-    :type interface: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.sv', read_filler=0, interface='axil', template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.read_filler = read_filler
-        self.interface = interface
-        self.template_path = template_path
-
-    def validate(self):
-        super().validate()
-        assert self.interface in ['axil', 'apb', 'amm', 'spi', 'lb'], \
-            "Unknown '%s' interface!" % (self.interface)
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'regmap_sv.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['module_name'] = utils.get_file_name(self.path)
-        j2_vars['read_filler'] = utils.str2int(self.read_filler)
-        j2_vars['interface'] = self.interface
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class SystemVerilogHeader(Generator, Jinja2):
-    """Create SystemVerilog header file with register map defines.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param prefix: Prefix for the all defines. Empty is allowed.
-    :type prefix: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.svh', prefix="", template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.prefix = prefix
-        self.template_path = template_path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'sv_header.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['prefix'] = self.prefix.upper()
-        j2_vars['file_name'] = utils.get_file_name(self.path)
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class CHeader(Generator, Jinja2):
-    """Create C header file with register map defines.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param prefix: Prefix for the all defines and types. Empty is allowed.
-    :type prefix: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.h', prefix="", template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.prefix = prefix
-        self.template_path = template_path
-
-    def validate(self):
-        super().validate()
-        data_width_allowed = [8, 16, 32, 64]
-        assert config.globcfg['data_width'] in [8, 16, 32, 64], \
-            "For %s generator, global 'data_width' must be one of '%s', but current is %d" % \
-            (self._name(), data_width_allowed, config.globcfg['data_width'])
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'c_header.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['prefix'] = self.prefix.upper()
-        j2_vars['file_name'] = utils.get_file_name(self.path)
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class SystemVerilogPackage(Generator, Jinja2):
-    """Create SystemVerilog package with register map parameters.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param prefix: Prefix for the all parameters and types. Empty is allowed.
-    :type prefix: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs_pkg.sv', prefix="", template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.prefix = prefix
-        self.template_path = template_path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'sv_package.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['prefix'] = self.prefix.upper()
-        j2_vars['file_name'] = utils.get_file_name(self.path)
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class LbBridgeSystemVerilog(Generator, Jinja2):
-    """Create SystemVerilog file with bridge to Local Bus.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param bridge_type: Bridge protocol. Use one of `axil`, `apb`, `amm`, `spi`.
-    :type bridge_type: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='axil2lb.sv', bridge_type='axil', template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.bridge_type = bridge_type
-        self.template_path = template_path
-
-    def validate(self):
-        assert self.bridge_type in ['axil', 'apb', 'amm', 'spi'], \
-            "Unknown '%s' bridge type!" % (self.bridge_type)
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_templates = {
-            'axil' : 'axil2lb_sv.j2',
-            'apb' : 'apb2lb_sv.j2',
-            'amm' : 'amm2lb_sv.j2',
-            'spi' : 'spi2lb_sv.j2'
-        }
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', default_templates[self.bridge_type]
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['module_name'] = utils.get_file_name(self.path)
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class Markdown(Generator, Jinja2, Wavedrom):
-    """Create documentation for a register map in Markdown.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param title: Document title
-    :type title: str
-    :param print_images: Enable generating images for bit fields of a register
-    :type print_images: bool
-    :param image_dir: Path to directory where all images will be saved
-    :type image_dir: str
-    :param print_conventions: Enable generating table with register access modes explained
-    :type print_conventions: bool
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.md', title='Register map',
-                 print_images=True, image_dir="regs_img", print_conventions=True, template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.title = title
-        self.print_images = print_images
-        self.image_dir = image_dir
-        self.print_conventions = print_conventions
-        self.template_path = template_path
-
-    def generate(self):
-        filename = utils.get_file_name(self.path)
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'regmap_md.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['print_images'] = utils.str2bool(self.print_images)
-        j2_vars['print_conventions'] = utils.str2bool(self.print_conventions)
-        j2_vars['image_dir'] = self.image_dir
-        j2_vars['filename'] = filename
-        j2_vars['title'] = self.title
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-        # draw register images
-        if self.print_images:
-            self.draw_regs(Path(self.path).parent / self.image_dir, self.rmap)
-
-
-class Asciidoc(Generator, Jinja2, Wavedrom):
-    """Create documentation for a register map in AsciiDoc.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param title: Document title
-    :type title: str
-    :param print_images: Enable generating images for bit fields of a register
-    :type print_images: bool
-    :param image_dir: Path to directory where all images will be saved
-    :type image_dir: str
-    :param print_conventions: Enable generating table with register access modes explained
-    :type print_conventions: bool
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.adoc', title='Register map',
-                 print_images=True, image_dir="regs_img", print_conventions=True, template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.title = title
-        self.print_images = print_images
-        self.image_dir = image_dir
-        self.print_conventions = print_conventions
-        self.template_path = template_path
-
-    def generate(self):
-        filename = utils.get_file_name(self.path)
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'regmap_asciidoc.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['print_images'] = utils.str2bool(self.print_images)
-        j2_vars['print_conventions'] = utils.str2bool(self.print_conventions)
-        j2_vars['image_dir'] = self.image_dir
-        j2_vars['filename'] = filename
-        j2_vars['title'] = self.title
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-        # draw register images
-        if self.print_images:
-            self.draw_regs(Path(self.path).parent / self.image_dir, self.rmap)
-
-
-class Rst(Generator, Jinja2, Wavedrom):
-    """Create documentation for a register map in reStructuredText.
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param title: Document title
-    :type title: str
-    :param print_images: Enable generating images for bit fields of a register
-    :type print_images: bool
-    :param image_dir: Path to directory where all images will be saved
-    :type image_dir: str
-    :param print_conventions: Enable generating table with register access modes explained
-    :type print_conventions: bool
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.rst', title='Register map',
-                 print_images=True, image_dir="regs_img", print_conventions=True, template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.title = title
-        self.print_images = print_images
-        self.image_dir = image_dir
-        self.print_conventions = print_conventions
-        self.template_path = template_path
-
-    def generate(self):
-        filename = utils.get_file_name(self.path)
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'regmap_rst.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['print_images'] = utils.str2bool(self.print_images)
-        j2_vars['print_conventions'] = utils.str2bool(self.print_conventions)
-        j2_vars['image_dir'] = self.image_dir
-        j2_vars['filename'] = filename
-        j2_vars['title'] = self.title
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-        # draw register images
-        if self.print_images:
-            self.draw_regs(Path(self.path).parent / self.image_dir, self.rmap)
-
-
-class Docx(Generator):
-    """Create documentation in Docx from Markdown using Pandoc.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param input_md: Path to the input Markdown file
-    :type input_md: str
-    :param path: Path to the output DOCX file
-    :type path: str
-    :param pandoc_args: Additional arguments for Pandoc command-line tool
-    :type pandoc_args: str or list
-    """
-
-    def __init__(self, rmap=None, path='regs.docx', input_md='regs.md', pandoc_args=None, **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.input_md = input_md
-        self.pandoc_args = pandoc_args if pandoc_args else ''
-
-    def generate(self):
-        # Validate parameters
-        self.validate()
-
-        # Save current directory
-        current_dir = os.getcwd()
-        
-        try:
-            # Change directory to the specified path
-            os.chdir(os.path.dirname(self.path))
-            
-            # Convert Markdown to Docx using Pandoc
-            command = ['pandoc', '-s', '-o', os.path.basename(self.path), self.input_md]
-            if self.pandoc_args:
-                if isinstance(self.pandoc_args, str):
-                    command.extend(self.pandoc_args.split())  # If pandoc_args is a string, split it by spaces
-                else:
-                    command.extend(self.pandoc_args)  # Otherwise, add the arguments as they are
-            subprocess.run(command, check=True)
-            print("... docx document generated successfully!")
-        except subprocess.CalledProcessError as e:
-            print(f"... docx document error generating: {e}")
-        finally:
-            # Change back to the original directory
-            os.chdir(current_dir)
-
-
-class CmsisSvd(Generator, Jinja2):
-    """ Create the CMSIS SVD file.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param peripheral_name: Header SVD info - peripheral name
-    :type peripheral_name: str
-    :param description: Header SVD info - description
-    :type description: str
-    :param part_version: Header SVD info - version
-    :type part_version: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.svd', peripheral_name='CSR',
-                 description='no description', part_version='1.0.0', template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.peripheral_name = peripheral_name
-        self.description = description
-        self.part_version = part_version
-        self.template_path = template_path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'cmsis_svd.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['peripheral_name'] = self.peripheral_name
-        j2_vars['description'] = self.description
-        j2_vars['part_version'] = self.part_version
-        j2_vars['config'] = config.globcfg
-        j2_vars['part_name'] = utils.get_file_name(self.path)
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class IpxactXml(Generator, Jinja2):
-    """ Create the IP-XACT XML file.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param vendor: Header XML info - Vendor
-    :type vendor: str
-    :param library: Header XML info - library
-    :type library: str
-    :param component_name: Header XML info - component name
-    :type component_name: str
-    :param version: Header XML info - version
-    :type version: str
-    :param memorymap_name: Header XML info - memorymap name
-    :type memorymap_name: str
-    :param addressblock_name: Header XML info - addressblock name
-    :type addressblock_name: str
-    :param description: Header XML info - description
-    :type description: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.xml', vendor='NM-Tech',
-                 library='No library', component_name='No component_name', version='No version', 
-                 memorymap_name='No memorymap_name', addressblock_name='No addressblock_name', description='No description', 
-                 template_path='',  **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.vendor = vendor
-        self.library = library
-        self.component_name = component_name
-        self.version = version
-        self.memorymap_name = memorymap_name
-        self.addressblock_name = addressblock_name
-        self.description = description
-        self.template_path = template_path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'ipxact_xml.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['vendor'] = self.vendor
-        j2_vars['library'] =self.library
-        j2_vars['component_name'] =self.component_name
-        j2_vars['version'] =self.version
-        j2_vars['memorymap_name'] =self.memorymap_name
-        j2_vars['addressblock_name'] =self.addressblock_name
-        j2_vars['description'] =self.description
-        j2_vars['config'] = config.globcfg
-        j2_vars['part_name'] = utils.get_file_name(self.path)
-
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
-
-
-class Xls2Yaml(Generator):
-    """Convert Excel table to YAML format.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param input_xls: Path to the input Excel file
-    :type input_xls: str
-    :param path: Path to the output YAML file
-    :type path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.yaml', input_xls="regs.xls", **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.input_xls = input_xls
-        self.regmap = []
-
-    def replace_nan_to_empty(self, value):
-        """Replace .NaN to empty field rows recursivly."""
-        if isinstance(value, dict):
-            return {k: self.replace_nan_to_empty(v) for k, v in value.items()}
-        elif isinstance(value, list):
-            return [self.replace_nan_to_empty(v) for v in value]
-        elif isinstance(value, float) and np.isnan(value):
-            return ''
-        else:
-            return value
-
-    def preserve_multiline_strings(self, data):
-        """Turn multiline strings into PreservedScalarString objects recursivly."""
-        if isinstance(data, dict):
-            return {k: self.preserve_multiline_strings(v) for k, v in data.items()}
-        elif isinstance(data, list):
-            return [self.preserve_multiline_strings(v) for v in data]
-        elif isinstance(data, str) and '\n' in data:
-            return pss(data)
-        else:
-            return data
-
-    def flatten_multiline_strings(self, data):
-        """Convert multiline strings into single line strings recursively."""
-        if isinstance(data, dict):
-            return {k: self.flatten_multiline_strings(v) for k, v in data.items()}
-        elif isinstance(data, list):
-            return [self.flatten_multiline_strings(v) for v in data]
-        elif isinstance(data, str) and '\n' in data:
-            return data.replace('\n', ' ')
-        else:
-            return data
-
-    def load_excel_data(self):
-        """Load data from the input Excel file."""
-        self.df = pd.read_excel(self.input_xls)
-
-    def process_excel_data(self):
-        """Process the loaded Excel data and convert it to YAML format."""
-        current_register = None
-        for index, row in self.df.iterrows():
-            register_name = str(row["Register Name"]).lower() if pd.notnull(row["Register Name"]) else None
-            field_name = str(row["Field Name"]).lower() if pd.notnull(row["Field Name"]) else None
-
-            if register_name and any(keyword in register_name for keyword in ["-", "reserved", "unused", "not_used"]) or \
-                    field_name and any(keyword in field_name for keyword in ["-", "reserved", "unused", "not_used"]):
-                continue
-
-            if pd.notnull(row["Register Name"]):
-                if current_register:
-                    self.regmap.append(current_register)
-                current_register = {
-                    "name": row["Register Name"],
-                    "description": row["Description"],
-                    "address": int(row["Offset"], 16),
-                    "bitfields": []
-                }
-            elif pd.notnull(row["Field Name"]):
-                current_bitfield = {
-                    "name": row["Field Name"],
-                    "description": row["Description"],
-                    "reset": int(row["Value"], 16) if isinstance(row["Value"], str) and row["Value"].startswith("0x") else row["Value"],
-                    "width": int(row["Width"]),
-                    "lsb": int(str(row["Offset"]), 16),
-                    "access": row["Access"],
-                    "hardware": row["_hwAccess_"] if "_hwAccess_" in row else None,
-                    "enums": [] if pd.isnull(row["Enum Name"]) else [{
-                        "name": row["Enum Name"],
-                        "description": row["Description"],
-                        "value": row["Value"]
-                    }]
-                }
-                current_register["bitfields"].append(current_bitfield)
-            elif pd.isnull(row["Field Name"]):
-                if pd.notnull(row["Enum Name"]):
-                    current_bitfield["enums"].append({
-                        "name": row["Enum Name"],
-                        "description": row["Description"],
-                        "value": row["Value"]
-                    })
-        if current_register:
-            self.regmap.append(current_register)
-
-    def write_to_yaml(self):
-        """Write the processed data to the output YAML file."""
-        yaml = YAML()
-        yaml.explicit_start = False
-        regmap_cleaned = self.flatten_multiline_strings(self.replace_nan_to_empty(self.regmap))
-        with open(self.path, "w", encoding="utf-8") as f:
-            yaml.dump({"regmap": regmap_cleaned}, f)
-        print("... yaml file from Excel table generated successfully!")
-
-    def generate(self):
-        """Generate YAML file from the Excel input."""
-        self.load_excel_data()
-        self.process_excel_data()
-        self.write_to_yaml()
-
-
-class Python(Generator, Jinja2):
-    """Create Python file to access register map via some interface.
-
-    :param rmap: Register map object
-    :type rmap: :class:`regmapGen.RegisterMap`
-    :param path: Path to the output file
-    :type path: str
-    :param template_path: A path to the template to use instead of the default template.
-    :type template_path: str
-    """
-
-    def __init__(self, rmap=None, path='regs.py', template_path='', **args):
-        super().__init__(rmap, **args)
-        self.path = path
-        self.template_path = template_path
-
-    def generate(self):
-        # validate parameters
-        self.validate()
-        # prepare jinja2
-        default_template = os.path.join(
-            Path(__file__).parent, 'templates', 'regmap_py.j2'
-        )
-        template_path = self.template_path if self.template_path != '' else default_template
-        j2_template = Path(template_path).name
-        j2_vars = {}
-        j2_vars['regmapGen_ver'] = __version__
-        j2_vars['rmap'] = self.rmap
-        j2_vars['config'] = config.globcfg
-        # render
-        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""Output file generators
+"""
+
+import os
+import json
+import yaml
+import jinja2
+from regmapGen import __version__
+from . import utils
+from . import config
+from .regmap import RegisterMap
+from pathlib import Path
+import wavedrom
+import subprocess
+import pandas as pd
+from ruamel.yaml.scalarstring import PreservedScalarString as pss
+from ruamel.yaml import YAML
+import numpy as np
+
+class Generator():
+    """Base generator class.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    """
+
+    def __init__(self, rmap, **args):
+        self.rmap = rmap
+        self.etc = args
+
+    def _name(self):
+        return self.__class__.__name__
+
+    def generate(self):
+        """Do file generation."""
+        pass
+
+    def validate(self):
+        """Validate generator parameters."""
+        # config
+        config.validate_globcfg(config.globcfg)
+        # rmap
+        assert isinstance(self.rmap, RegisterMap), \
+            "Register map has to be '%s', but '%s' was provided for '%s' generator!" % (
+                repr(RegisterMap()), repr(self.rmap), self._name())
+        self.rmap.validate()
+
+    def make_target(self, name):
+        """Dump class attributes to dictionary that can be used as target for `config` generation.
+
+        :param name: Name of the target
+        :return: Target dictionary
+        """
+        params = vars(self)
+        params.pop('etc')
+        params.pop('rmap')
+        params['generator'] = self._name()
+        return {name: params}
+
+
+class Jinja2():
+    """Basic class for rendering Jinja2 templates"""
+
+    def render(self, template, vars, templates_path=None):
+        """Render text with Jinja2.
+
+        :param template: Jinja2 template filename
+        :param vars: Dictionary with variables for Jinja2 rendering
+        :param templates_path: Path to search templates. If no path provided, then internal templates will be used
+        :return: String with rendered text
+        """
+        # prepare template
+        if not templates_path:
+            templates_path = str(Path(__file__).parent / 'templates')
+        j2_env = jinja2.Environment(loader=jinja2.FileSystemLoader(searchpath=templates_path),
+                                    trim_blocks=True, lstrip_blocks=True)
+        j2_env.globals.update(zip=zip)
+        j2_template = j2_env.get_template(template)
+        # render
+        return j2_template.render(vars)
+
+    def render_to_file(self, template, vars, path, templates_path=None):
+        """Render text with Jinja2 and save it to the file.
+
+        :param template: Jinja2 template filename
+        :param vars: Dictionary with variables for Jinja2 rendering
+        :param path: Path to the output file
+        :param templates_path: Path to search templates. If no path provided, then internal templates will be used
+        """
+        # render
+        rendered_text = self.render(template, vars, templates_path)
+        # save
+        utils.create_dirs(self.path)
+        with open(path, "w", encoding="utf-8") as f:
+            f.write(rendered_text)
+
+
+class Wavedrom():
+    """Basic class for rendering register images with wavedrom"""
+
+    def draw_regs(self, imgdir, rmap):
+        imgdir.mkdir(exist_ok=True)
+
+        bits = config.globcfg['data_width']
+        lanes = bits // 8 if bits > 8 else 1
+        for reg in rmap:
+            reg_wd = {"reg": [],
+                      "config": {"bits": bits, "lanes": lanes, "fontsize": 14, "vspace": 100, "fontfamily": 'Arial'}}
+            bit_pos = -1
+            for bf in reg:
+                if bit_pos == -1 and bf.lsb > 0:
+                    reg_wd["reg"].append({"bits": bf.lsb})
+                elif bf.lsb - bit_pos > 1:
+                    reg_wd["reg"].append({"bits": bf.lsb - bit_pos - 1})
+                name = bf.name
+                #name_max_len = 5 * bf.width
+                #if len(bf.name) > name_max_len:  # to prevent labels overlapping
+                #    name = bf.name[:name_max_len - 1] + '..'
+                reg_wd["reg"].append({"name": name, "attr": bf.access, "bits": bf.width})
+                bit_pos = bf.msb
+            if (bits - 1) > bit_pos:
+                reg_wd["reg"].append({"bits": bits - bit_pos - 1})
+            wavedrom.render(json.dumps(reg_wd)).saveas(str(imgdir / ("%s.svg" % reg.name.lower())))
+
+
+class Json(Generator):
+    """Dump register map to a JSON file.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.json', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+
+    def generate(self):
+        # validate register map
+        self.rmap.validate()
+        # prepare data
+        data = {'regmap': list(self.rmap.as_dict().values())}
+        # dump
+        utils.create_dirs(self.path)
+        with open(self.path, 'w', encoding="utf-8") as f:
+            json.dump(data, f, indent=4)
+
+
+class Yaml(Generator):
+    """Dump register map to a YAML file.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.yaml', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare data
+        data = {'regmap': list(self.rmap.as_dict().values())}
+        # dump
+        utils.create_dirs(self.path)
+        with open(self.path, 'w', encoding="utf-8") as f:
+            yaml.Dumper.ignore_aliases = lambda *args: True  # hack to disable aliases
+            yaml.dump(data, f, indent=4, default_flow_style=False, sort_keys=False)
+
+
+class Txt(Generator):
+    """Dump register map to a text table.
+
+    Note: only registers with single bitfield are allowed.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.txt', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        for reg in self.rmap:
+            if len(reg) > 1:
+                raise ValueError("Only registers with single bitfield are allowed for %s generator." % self._name())
+        # prepare template strings
+        data_w = config.globcfg['data_width']
+        address_w = config.globcfg['address_width']
+        address_digits = address_w // 4 + (1 if address_w % 4 else 0)
+        address_str = "0x%0{0}x".format(address_digits)
+        reset_digits = data_w // 4 + (1 if data_w % 4 else 0)
+        reset_str = "0x%0{0}x".format(reset_digits)
+        row_template = "| %-{0}s | %-{1}s | %-{2}s | %-{3}s | %-{4}s | %-{5}s | %-{6}s |\n"
+        # prepare table data
+        row_top = ["Address", "Name", "Width", "Access", "Hardware", "Reset", "Description"]
+        col_address = [address_str % reg.address for reg in self.rmap]
+        col_names = self.rmap.reg_names
+        col_width = ["%d" % reg.bitfields[0].width for reg in self.rmap]
+        col_access = [reg.bitfields[0].access for reg in self.rmap]
+        col_hardware = [reg.bitfields[0].hardware for reg in self.rmap]
+        col_reset = [reset_str % reg.reset for reg in self.rmap]
+        col_description = [reg.description for reg in self.rmap]
+        # calculate width of the columns for pretty printing
+        cols_w = [max(address_digits + 2, len(row_top[0])),
+                  max(max([len(s) for s in col_names]), len(row_top[1])),
+                  max(max([len(s) for s in col_width]), len(row_top[2])),
+                  max(max([len(s) for s in col_access]), len(row_top[3])),
+                  max(max([len(s) for s in col_hardware]), len(row_top[4])),
+                  max(reset_digits + 2, len(row_top[5])),
+                  max(max([len(s) for s in col_description]), len(row_top[6]))]
+        row_template = row_template.format(*cols_w)
+        # render
+        out_lines = [row_template % tuple(row_top)]
+        out_lines.append(row_template % tuple(["-" * w for w in cols_w]))
+        for i in range(len(col_names)):
+            out_lines.append(row_template % (col_address[i], col_names[i],
+                             col_width[i], col_access[i], col_hardware[i], col_reset[i], col_description[i]))
+        # save to file
+        utils.create_dirs(self.path)
+        with open(self.path, 'w', encoding="utf-8") as f:
+            f.writelines(out_lines)
+
+
+class SystemVerilog(Generator, Jinja2):
+    """Create SystemVerilog file with register map.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param read_filler: Numeric value to return if wrong address was read
+    :type read_filler: int
+    :param interface: Register map bus protocol. Use one of: `axil`, `apb`, `amm`, `spi`, `lb`
+    :type interface: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.sv', read_filler=0, interface='axil', template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.read_filler = read_filler
+        self.interface = interface
+        self.template_path = template_path
+
+    def validate(self):
+        super().validate()
+        assert self.interface in ['axil', 'apb', 'amm', 'spi', 'lb'], \
+            "Unknown '%s' interface!" % (self.interface)
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'regmap_sv.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['module_name'] = utils.get_file_name(self.path)
+        j2_vars['read_filler'] = utils.str2int(self.read_filler)
+        j2_vars['interface'] = self.interface
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class SystemVerilogWrapper(Generator, Jinja2):
+    """Create SystemVerilog file with register map.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param module_name: Module name of register map
+    :type module_name: str
+    :param interface: Register map bus protocol. Use one of: `axil`, `apb`, `amm`, `spi`, `lb`
+    :type interface: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs_wrapper.svh', module_name='regs', interface='axil', template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.module_name = module_name
+        self.interface = interface
+        self.template_path = template_path
+
+    def validate(self):
+        super().validate()
+        assert self.interface in ['axil', 'apb', 'amm', 'spi', 'lb'], \
+            "Unknown '%s' interface!" % (self.interface)
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'sv_wrapper.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['module_name'] = self.module_name
+        j2_vars['interface'] = self.interface
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class SystemVerilogHeader(Generator, Jinja2):
+    """Create SystemVerilog header file with register map defines.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param prefix: Prefix for the all defines. Empty is allowed.
+    :type prefix: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.svh', prefix="", template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.prefix = prefix
+        self.template_path = template_path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'sv_header.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['prefix'] = self.prefix.upper()
+        j2_vars['file_name'] = utils.get_file_name(self.path)
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class CHeader(Generator, Jinja2):
+    """Create C header file with register map defines.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param prefix: Prefix for the all defines and types. Empty is allowed.
+    :type prefix: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.h', prefix="", template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.prefix = prefix
+        self.template_path = template_path
+
+    def validate(self):
+        super().validate()
+        data_width_allowed = [8, 16, 32, 64]
+        assert config.globcfg['data_width'] in [8, 16, 32, 64], \
+            "For %s generator, global 'data_width' must be one of '%s', but current is %d" % \
+            (self._name(), data_width_allowed, config.globcfg['data_width'])
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'c_header.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['prefix'] = self.prefix.upper()
+        j2_vars['file_name'] = utils.get_file_name(self.path)
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class SystemVerilogPackage(Generator, Jinja2):
+    """Create SystemVerilog package with register map parameters.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param prefix: Prefix for the all parameters and types. Empty is allowed.
+    :type prefix: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs_pkg.sv', prefix="", template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.prefix = prefix
+        self.template_path = template_path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'sv_package.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['prefix'] = self.prefix.upper()
+        j2_vars['file_name'] = utils.get_file_name(self.path)
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class LbBridgeSystemVerilog(Generator, Jinja2):
+    """Create SystemVerilog file with bridge to Local Bus.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param bridge_type: Bridge protocol. Use one of `axil`, `apb`, `amm`, `spi`.
+    :type bridge_type: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='axil2lb.sv', bridge_type='axil', template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.bridge_type = bridge_type
+        self.template_path = template_path
+
+    def validate(self):
+        assert self.bridge_type in ['axil', 'apb', 'amm', 'spi'], \
+            "Unknown '%s' bridge type!" % (self.bridge_type)
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_templates = {
+            'axil' : 'axil2lb_sv.j2',
+            'apb' : 'apb2lb_sv.j2',
+            'amm' : 'amm2lb_sv.j2',
+            'spi' : 'spi2lb_sv.j2'
+        }
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', default_templates[self.bridge_type]
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['module_name'] = utils.get_file_name(self.path)
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class Markdown(Generator, Jinja2, Wavedrom):
+    """Create documentation for a register map in Markdown.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param title: Document title
+    :type title: str
+    :param print_images: Enable generating images for bit fields of a register
+    :type print_images: bool
+    :param image_dir: Path to directory where all images will be saved
+    :type image_dir: str
+    :param print_conventions: Enable generating table with register access modes explained
+    :type print_conventions: bool
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.md', title='Register map',
+                 print_images=True, image_dir="regs_img", print_conventions=True, template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.title = title
+        self.print_images = print_images
+        self.image_dir = image_dir
+        self.print_conventions = print_conventions
+        self.template_path = template_path
+
+    def generate(self):
+        filename = utils.get_file_name(self.path)
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'regmap_md.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['print_images'] = utils.str2bool(self.print_images)
+        j2_vars['print_conventions'] = utils.str2bool(self.print_conventions)
+        j2_vars['image_dir'] = self.image_dir
+        j2_vars['filename'] = filename
+        j2_vars['title'] = self.title
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+        # draw register images
+        if self.print_images:
+            self.draw_regs(Path(self.path).parent / self.image_dir, self.rmap)
+
+
+class Asciidoc(Generator, Jinja2, Wavedrom):
+    """Create documentation for a register map in AsciiDoc.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param title: Document title
+    :type title: str
+    :param print_images: Enable generating images for bit fields of a register
+    :type print_images: bool
+    :param image_dir: Path to directory where all images will be saved
+    :type image_dir: str
+    :param print_conventions: Enable generating table with register access modes explained
+    :type print_conventions: bool
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.adoc', title='Register map',
+                 print_images=True, image_dir="regs_img", print_conventions=True, template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.title = title
+        self.print_images = print_images
+        self.image_dir = image_dir
+        self.print_conventions = print_conventions
+        self.template_path = template_path
+
+    def generate(self):
+        filename = utils.get_file_name(self.path)
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'regmap_asciidoc.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['print_images'] = utils.str2bool(self.print_images)
+        j2_vars['print_conventions'] = utils.str2bool(self.print_conventions)
+        j2_vars['image_dir'] = self.image_dir
+        j2_vars['filename'] = filename
+        j2_vars['title'] = self.title
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+        # draw register images
+        if self.print_images:
+            self.draw_regs(Path(self.path).parent / self.image_dir, self.rmap)
+
+
+class Rst(Generator, Jinja2, Wavedrom):
+    """Create documentation for a register map in reStructuredText.
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param title: Document title
+    :type title: str
+    :param print_images: Enable generating images for bit fields of a register
+    :type print_images: bool
+    :param image_dir: Path to directory where all images will be saved
+    :type image_dir: str
+    :param print_conventions: Enable generating table with register access modes explained
+    :type print_conventions: bool
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.rst', title='Register map',
+                 print_images=True, image_dir="regs_img", print_conventions=True, template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.title = title
+        self.print_images = print_images
+        self.image_dir = image_dir
+        self.print_conventions = print_conventions
+        self.template_path = template_path
+
+    def generate(self):
+        filename = utils.get_file_name(self.path)
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'regmap_rst.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['print_images'] = utils.str2bool(self.print_images)
+        j2_vars['print_conventions'] = utils.str2bool(self.print_conventions)
+        j2_vars['image_dir'] = self.image_dir
+        j2_vars['filename'] = filename
+        j2_vars['title'] = self.title
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+        # draw register images
+        if self.print_images:
+            self.draw_regs(Path(self.path).parent / self.image_dir, self.rmap)
+
+
+class Docx(Generator):
+    """Create documentation in Docx from Markdown using Pandoc.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param input_md: Path to the input Markdown file
+    :type input_md: str
+    :param path: Path to the output DOCX file
+    :type path: str
+    :param pandoc_args: Additional arguments for Pandoc command-line tool
+    :type pandoc_args: str or list
+    """
+
+    def __init__(self, rmap=None, path='regs.docx', input_md='regs.md', pandoc_args=None, **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.input_md = input_md
+        self.pandoc_args = pandoc_args if pandoc_args else ''
+
+    def generate(self):
+        # Validate parameters
+        self.validate()
+
+        # Save current directory
+        current_dir = os.getcwd()
+        
+        try:
+            # Change directory to the specified path
+            os.chdir(os.path.dirname(self.path))
+            
+            # Convert Markdown to Docx using Pandoc
+            command = ['pandoc', '-s', '-o', os.path.basename(self.path), self.input_md]
+            if self.pandoc_args:
+                if isinstance(self.pandoc_args, str):
+                    command.extend(self.pandoc_args.split())  # If pandoc_args is a string, split it by spaces
+                else:
+                    command.extend(self.pandoc_args)  # Otherwise, add the arguments as they are
+            subprocess.run(command, check=True)
+            print("... docx document generated successfully!")
+        except subprocess.CalledProcessError as e:
+            print(f"... docx document error generating: {e}")
+        finally:
+            # Change back to the original directory
+            os.chdir(current_dir)
+
+
+class CmsisSvd(Generator, Jinja2):
+    """ Create the CMSIS SVD file.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param peripheral_name: Header SVD info - peripheral name
+    :type peripheral_name: str
+    :param description: Header SVD info - description
+    :type description: str
+    :param part_version: Header SVD info - version
+    :type part_version: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.svd', peripheral_name='CSR',
+                 description='no description', part_version='1.0.0', template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.peripheral_name = peripheral_name
+        self.description = description
+        self.part_version = part_version
+        self.template_path = template_path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'cmsis_svd.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['peripheral_name'] = self.peripheral_name
+        j2_vars['description'] = self.description
+        j2_vars['part_version'] = self.part_version
+        j2_vars['config'] = config.globcfg
+        j2_vars['part_name'] = utils.get_file_name(self.path)
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class IpxactXml(Generator, Jinja2):
+    """ Create the IP-XACT XML file.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param vendor: Header XML info - Vendor
+    :type vendor: str
+    :param library: Header XML info - library
+    :type library: str
+    :param component_name: Header XML info - component name
+    :type component_name: str
+    :param version: Header XML info - version
+    :type version: str
+    :param memorymap_name: Header XML info - memorymap name
+    :type memorymap_name: str
+    :param addressblock_name: Header XML info - addressblock name
+    :type addressblock_name: str
+    :param description: Header XML info - description
+    :type description: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.xml', vendor='NM-Tech',
+                 library='No library', component_name='No component_name', version='No version', 
+                 memorymap_name='No memorymap_name', addressblock_name='No addressblock_name', description='No description', 
+                 template_path='',  **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.vendor = vendor
+        self.library = library
+        self.component_name = component_name
+        self.version = version
+        self.memorymap_name = memorymap_name
+        self.addressblock_name = addressblock_name
+        self.description = description
+        self.template_path = template_path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'ipxact_xml.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['vendor'] = self.vendor
+        j2_vars['library'] =self.library
+        j2_vars['component_name'] =self.component_name
+        j2_vars['version'] =self.version
+        j2_vars['memorymap_name'] =self.memorymap_name
+        j2_vars['addressblock_name'] =self.addressblock_name
+        j2_vars['description'] =self.description
+        j2_vars['config'] = config.globcfg
+        j2_vars['part_name'] = utils.get_file_name(self.path)
+
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
+
+
+class Xls2Yaml(Generator):
+    """Convert Excel table to YAML format.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param input_xls: Path to the input Excel file
+    :type input_xls: str
+    :param path: Path to the output YAML file
+    :type path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.yaml', input_xls="regs.xls", **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.input_xls = input_xls
+        self.regmap = []
+
+    def replace_nan_to_empty(self, value):
+        """Replace .NaN to empty field rows recursivly."""
+        if isinstance(value, dict):
+            return {k: self.replace_nan_to_empty(v) for k, v in value.items()}
+        elif isinstance(value, list):
+            return [self.replace_nan_to_empty(v) for v in value]
+        elif isinstance(value, float) and np.isnan(value):
+            return ''
+        else:
+            return value
+
+    def preserve_multiline_strings(self, data):
+        """Turn multiline strings into PreservedScalarString objects recursivly."""
+        if isinstance(data, dict):
+            return {k: self.preserve_multiline_strings(v) for k, v in data.items()}
+        elif isinstance(data, list):
+            return [self.preserve_multiline_strings(v) for v in data]
+        elif isinstance(data, str) and '\n' in data:
+            return pss(data)
+        else:
+            return data
+
+    def flatten_multiline_strings(self, data):
+        """Convert multiline strings into single line strings recursively."""
+        if isinstance(data, dict):
+            return {k: self.flatten_multiline_strings(v) for k, v in data.items()}
+        elif isinstance(data, list):
+            return [self.flatten_multiline_strings(v) for v in data]
+        elif isinstance(data, str) and '\n' in data:
+            return data.replace('\n', ' ')
+        else:
+            return data
+
+    def load_excel_data(self):
+        """Load data from the input Excel file."""
+        self.df = pd.read_excel(self.input_xls)
+
+    def process_excel_data(self):
+        """Process the loaded Excel data and convert it to YAML format."""
+        current_register = None
+        for index, row in self.df.iterrows():
+            register_name = str(row["Register Name"]).lower() if pd.notnull(row["Register Name"]) else None
+            field_name = str(row["Field Name"]).lower() if pd.notnull(row["Field Name"]) else None
+
+            if register_name and any(keyword in register_name for keyword in ["-", "reserved", "unused", "not_used"]) or \
+                    field_name and any(keyword in field_name for keyword in ["-", "reserved", "unused", "not_used"]):
+                continue
+
+            if pd.notnull(row["Register Name"]):
+                if current_register:
+                    self.regmap.append(current_register)
+                current_register = {
+                    "name": row["Register Name"],
+                    "description": row["Description"],
+                    "address": int(row["Offset"], 16),
+                    "bitfields": []
+                }
+            elif pd.notnull(row["Field Name"]):
+                current_bitfield = {
+                    "name": row["Field Name"],
+                    "description": row["Description"],
+                    "reset": int(row["Value"], 16) if isinstance(row["Value"], str) and row["Value"].startswith("0x") else row["Value"],
+                    "width": int(row["Width"]),
+                    "lsb": int(str(row["Offset"]), 16),
+                    "access": row["Access"],
+                    "hardware": row["_hwAccess_"] if "_hwAccess_" in row else None,
+                    "enums": [] if pd.isnull(row["Enum Name"]) else [{
+                        "name": row["Enum Name"],
+                        "description": row["Description"],
+                        "value": row["Value"]
+                    }]
+                }
+                current_register["bitfields"].append(current_bitfield)
+            elif pd.isnull(row["Field Name"]):
+                if pd.notnull(row["Enum Name"]):
+                    current_bitfield["enums"].append({
+                        "name": row["Enum Name"],
+                        "description": row["Description"],
+                        "value": row["Value"]
+                    })
+        if current_register:
+            self.regmap.append(current_register)
+
+    def write_to_yaml(self):
+        """Write the processed data to the output YAML file."""
+        yaml = YAML()
+        yaml.explicit_start = False
+        regmap_cleaned = self.flatten_multiline_strings(self.replace_nan_to_empty(self.regmap))
+        with open(self.path, "w", encoding="utf-8") as f:
+            yaml.dump({"regmap": regmap_cleaned}, f)
+        print("... yaml file from Excel table generated successfully!")
+
+    def generate(self):
+        """Generate YAML file from the Excel input."""
+        self.load_excel_data()
+        self.process_excel_data()
+        self.write_to_yaml()
+
+
+class Python(Generator, Jinja2):
+    """Create Python file to access register map via some interface.
+
+    :param rmap: Register map object
+    :type rmap: :class:`regmapGen.RegisterMap`
+    :param path: Path to the output file
+    :type path: str
+    :param template_path: A path to the template to use instead of the default template.
+    :type template_path: str
+    """
+
+    def __init__(self, rmap=None, path='regs.py', template_path='', **args):
+        super().__init__(rmap, **args)
+        self.path = path
+        self.template_path = template_path
+
+    def generate(self):
+        # validate parameters
+        self.validate()
+        # prepare jinja2
+        default_template = os.path.join(
+            Path(__file__).parent, 'templates', 'regmap_py.j2'
+        )
+        template_path = self.template_path if self.template_path != '' else default_template
+        j2_template = Path(template_path).name
+        j2_vars = {}
+        j2_vars['regmapGen_ver'] = __version__
+        j2_vars['rmap'] = self.rmap
+        j2_vars['config'] = config.globcfg
+        # render
+        self.render_to_file(j2_template, j2_vars, self.path, Path(template_path).parent)
```

### Comparing `regmapGen-1.0.2/regmapGen/reg.py` & `regmapGen-1.0.3/regmapGen/reg.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/amm2lb_sv.j2` & `regmapGen-1.0.3/regmapGen/templates/amm2lb_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/axil2lb_sv.j2` & `regmapGen-1.0.3/regmapGen/templates/axil2lb_sv.j2`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-// Created with regmapGen v{{ regmapGen_ver }}
-//
-// AXI-Lite to Local Bus bridge
-//
-
-module  {{ module_name }} #(
-    parameter ADDR_W = {{ config['address_width'] }},
-    parameter DATA_W = {{ config['data_width'] }},
-    parameter STRB_W = DATA_W / 8
-)(
-    input               clk,
-    input               rst,
-    // Local Bus
-    input               wready,
-    output [ADDR_W-1:0] waddr,
-    output [DATA_W-1:0] wdata,
-    output              wen,
-    output [STRB_W-1:0] wstrb,
-    input  [DATA_W-1:0] rdata,
-    input               rvalid,
-    output [ADDR_W-1:0] raddr,
-    output              ren,
-{% macro axil_core(regmap_embed=False) %}
-    // AXI
-    input  [ADDR_W-1:0] axil_awaddr,
-    input  [2:0]        axil_awprot,
-    input               axil_awvalid,
-    output              axil_awready,
-    input  [DATA_W-1:0] axil_wdata,
-    input  [STRB_W-1:0] axil_wstrb,
-    input               axil_wvalid,
-    output              axil_wready,
-    output [1:0]        axil_bresp,
-    output              axil_bvalid,
-    input               axil_bready,
-
-    input  [ADDR_W-1:0] axil_araddr,
-    input  [2:0]        axil_arprot,
-    input               axil_arvalid,
-    output              axil_arready,
-    output [DATA_W-1:0] axil_rdata,
-    output [1:0]        axil_rresp,
-    output              axil_rvalid,
-    input               axil_rready
-);
-
-{% if regmap_embed %}
-wire              wready;
-wire [ADDR_W-1:0] waddr;
-wire [DATA_W-1:0] wdata;
-wire              wen;
-wire [STRB_W-1:0] wstrb;
-wire [DATA_W-1:0] rdata;
-wire              rvalid;
-wire [ADDR_W-1:0] raddr;
-wire              ren;
-{% endif %}
-
-reg [ADDR_W-1:0] waddr_int;
-reg [ADDR_W-1:0] raddr_int;
-reg [DATA_W-1:0] wdata_int;
-reg [STRB_W-1:0] strb_int;
-reg              awflag;
-reg              wflag;
-reg              arflag;
-reg              rflag;
-
-reg              axil_bvalid_int;
-reg [DATA_W-1:0] axil_rdata_int;
-reg              axil_rvalid_int;
-
-assign axil_awready = ~awflag;
-assign axil_wready  = ~wflag;
-assign axil_bvalid  = axil_bvalid_int;
-assign waddr        = waddr_int;
-assign wdata        = wdata_int;
-assign wstrb        = strb_int;
-assign wen          = awflag && wflag;
-assign axil_bresp   = 'd0; // always okay
-
-{% set rst_type = config['register_reset'] %}
-{%- if rst_type == 'async_pos' or rst_type == 'sync_pos' %}
-    {% set rst_active = 1%}
-{%- elif rst_type == 'async_neg' or rst_type == 'sync_neg' %}
-    {% set rst_active = 0%}
-{%- endif %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        waddr_int       <= 'd0;
-        wdata_int       <= 'd0;
-        strb_int        <= 'd0;
-        awflag          <= 1'b0;
-        wflag           <= 1'b0;
-        axil_bvalid_int <= 1'b0;
-    end else begin
-        if (axil_awvalid == 1'b1 && awflag == 1'b0) begin
-            awflag    <= 1'b1;
-            waddr_int <= axil_awaddr;
-        end else if (wen == 1'b1 && wready == 1'b1) begin
-            awflag    <= 1'b0;
-        end
-
-        if (axil_wvalid == 1'b1 && wflag == 1'b0) begin
-            wflag     <= 1'b1;
-            wdata_int <= axil_wdata;
-            strb_int  <= axil_wstrb;
-        end else if (wen == 1'b1 && wready == 1'b1) begin
-            wflag     <= 1'b0;
-        end
-
-        if (axil_bvalid_int == 1'b1 && axil_bready == 1'b1) begin
-            axil_bvalid_int <= 1'b0;
-        end else if ((axil_wvalid == 1'b1 && awflag == 1'b1) || (axil_awvalid == 1'b1 && wflag == 1'b1) || (wflag == 1'b1 && awflag == 1'b1)) begin
-            axil_bvalid_int <= wready;
-        end
-    end
-end
-
-assign axil_arready = ~arflag;
-assign axil_rdata   = axil_rdata_int;
-assign axil_rvalid  = axil_rvalid_int;
-assign raddr        = raddr_int;
-assign ren          = arflag && ~rflag;
-assign axil_rresp   = 'd0; // always okay
-
-{% set rst_type = config['register_reset'] %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        raddr_int       <= 'd0;
-        arflag          <= 1'b0;
-        rflag           <= 1'b0;
-        axil_rdata_int  <= 'd0;
-        axil_rvalid_int <= 1'b0;
-    end else begin
-        if (axil_arvalid == 1'b1 && arflag == 1'b0) begin
-            arflag    <= 1'b1;
-            raddr_int <= axil_araddr;
-        end else if (axil_rvalid_int == 1'b1 && axil_rready == 1'b1) begin
-            arflag    <= 1'b0;
-        end
-
-        if (rvalid == 1'b1 && ren == 1'b1 && rflag == 1'b0) begin
-            rflag <= 1'b1;
-        end else if (axil_rvalid_int == 1'b1 && axil_rready == 1'b1) begin
-            rflag <= 1'b0;
-        end
-
-        if (rvalid == 1'b1 && axil_rvalid_int == 1'b0) begin
-            axil_rdata_int  <= rdata;
-            axil_rvalid_int <= 1'b1;
-        end else if (axil_rvalid_int == 1'b1 && axil_rready == 1'b1) begin
-            axil_rvalid_int <= 1'b0;
-        end
-    end
-end
-{% endmacro %}
-{{ axil_core() }}
-endmodule
+// Created with regmapGen v{{ regmapGen_ver }}
+//
+// AXI-Lite to Local Bus bridge
+//
+
+module  {{ module_name }} #(
+    parameter ADDR_W = {{ config['address_width'] }},
+    parameter DATA_W = {{ config['data_width'] }},
+    parameter STRB_W = DATA_W / 8
+)(
+    input               clk,
+    input               rst,
+    // Local Bus
+    input               wready,
+    output [ADDR_W-1:0] waddr,
+    output [DATA_W-1:0] wdata,
+    output              wen,
+    output [STRB_W-1:0] wstrb,
+    input  [DATA_W-1:0] rdata,
+    input               rvalid,
+    output [ADDR_W-1:0] raddr,
+    output              ren,
+{% macro axil_core(regmap_embed=False) %}
+    // AXI
+    input  [ADDR_W-1:0] axil_awaddr,
+    input  [2:0]        axil_awprot,
+    input               axil_awvalid,
+    output              axil_awready,
+    input  [DATA_W-1:0] axil_wdata,
+    input  [STRB_W-1:0] axil_wstrb,
+    input               axil_wvalid,
+    output              axil_wready,
+    output [1:0]        axil_bresp,
+    output              axil_bvalid,
+    input               axil_bready,
+
+    input  [ADDR_W-1:0] axil_araddr,
+    input  [2:0]        axil_arprot,
+    input               axil_arvalid,
+    output              axil_arready,
+    output [DATA_W-1:0] axil_rdata,
+    output [1:0]        axil_rresp,
+    output              axil_rvalid,
+    input               axil_rready
+);
+
+{% if regmap_embed %}
+wire              wready;
+wire [ADDR_W-1:0] waddr;
+wire [DATA_W-1:0] wdata;
+wire              wen;
+wire [STRB_W-1:0] wstrb;
+wire [DATA_W-1:0] rdata;
+wire              rvalid;
+wire [ADDR_W-1:0] raddr;
+wire              ren;
+{% endif %}
+
+reg [ADDR_W-1:0] waddr_int;
+reg [ADDR_W-1:0] raddr_int;
+reg [DATA_W-1:0] wdata_int;
+reg [STRB_W-1:0] strb_int;
+reg              awflag;
+reg              wflag;
+reg              arflag;
+reg              rflag;
+
+reg              axil_bvalid_int;
+reg [DATA_W-1:0] axil_rdata_int;
+reg              axil_rvalid_int;
+
+assign axil_awready = ~awflag;
+assign axil_wready  = ~wflag;
+assign axil_bvalid  = axil_bvalid_int;
+assign waddr        = waddr_int;
+assign wdata        = wdata_int;
+assign wstrb        = strb_int;
+assign wen          = awflag && wflag;
+assign axil_bresp   = 'd0; // always okay
+
+{% set rst_type = config['register_reset'] %}
+{%- if rst_type == 'async_pos' or rst_type == 'sync_pos' %}
+    {% set rst_active = 1%}
+{%- elif rst_type == 'async_neg' or rst_type == 'sync_neg' %}
+    {% set rst_active = 0%}
+{%- endif %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        waddr_int       <= 'd0;
+        wdata_int       <= 'd0;
+        strb_int        <= 'd0;
+        awflag          <= 1'b0;
+        wflag           <= 1'b0;
+        axil_bvalid_int <= 1'b0;
+    end else begin
+        if (axil_awvalid == 1'b1 && awflag == 1'b0) begin
+            awflag    <= 1'b1;
+            waddr_int <= axil_awaddr;
+        end else if (wen == 1'b1 && wready == 1'b1) begin
+            awflag    <= 1'b0;
+        end
+
+        if (axil_wvalid == 1'b1 && wflag == 1'b0) begin
+            wflag     <= 1'b1;
+            wdata_int <= axil_wdata;
+            strb_int  <= axil_wstrb;
+        end else if (wen == 1'b1 && wready == 1'b1) begin
+            wflag     <= 1'b0;
+        end
+
+        if (axil_bvalid_int == 1'b1 && axil_bready == 1'b1) begin
+            axil_bvalid_int <= 1'b0;
+        end else if ((axil_wvalid == 1'b1 && awflag == 1'b1) || (axil_awvalid == 1'b1 && wflag == 1'b1) || (wflag == 1'b1 && awflag == 1'b1)) begin
+            axil_bvalid_int <= wready;
+        end
+    end
+end
+
+assign axil_arready = ~arflag;
+assign axil_rdata   = axil_rdata_int;
+assign axil_rvalid  = axil_rvalid_int;
+assign raddr        = raddr_int;
+assign ren          = arflag && ~rflag;
+assign axil_rresp   = 'd0; // always okay
+
+{% set rst_type = config['register_reset'] %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        raddr_int       <= 'd0;
+        arflag          <= 1'b0;
+        rflag           <= 1'b0;
+        axil_rdata_int  <= 'd0;
+        axil_rvalid_int <= 1'b0;
+    end else begin
+        if (axil_arvalid == 1'b1 && arflag == 1'b0) begin
+            arflag    <= 1'b1;
+            raddr_int <= axil_araddr;
+        end else if (axil_rvalid_int == 1'b1 && axil_rready == 1'b1) begin
+            arflag    <= 1'b0;
+        end
+
+        if (rvalid == 1'b1 && ren == 1'b1 && rflag == 1'b0) begin
+            rflag <= 1'b1;
+        end else if (axil_rvalid_int == 1'b1 && axil_rready == 1'b1) begin
+            rflag <= 1'b0;
+        end
+
+        if (rvalid == 1'b1 && axil_rvalid_int == 1'b0) begin
+            axil_rdata_int  <= rdata;
+            axil_rvalid_int <= 1'b1;
+        end else if (axil_rvalid_int == 1'b1 && axil_rready == 1'b1) begin
+            axil_rvalid_int <= 1'b0;
+        end
+    end
+end
+{% endmacro %}
+{{ axil_core() }}
+endmodule
```

### Comparing `regmapGen-1.0.2/regmapGen/templates/c_header.j2` & `regmapGen-1.0.3/regmapGen/templates/c_header.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/cmsis_svd.j2` & `regmapGen-1.0.3/regmapGen/templates/cmsis_svd.j2`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-{#- value in hex format #}
-{% macro literal(reset, width) %}
-{{ "0x%0{w}x".format(w=width // 4) % reset }}
-{%- endmacro %}
-{#- sw access #}
-{% macro access(bf) %}
-<access>{%- if bf.access.startswith('ro') %}
-read-only
-{%- elif bf.access.startswith('wo') %}
-write-only
-{%- else %}
-read-write
-{%- endif %}</access>
-{%- endmacro %}
-{#- read / write modify #}
-{% macro rw_mod(bf) %}
-{% if bf.access == 'rw1c' %}
-              <modifiedWriteValues>oneToClear</modifiedWriteValues>
-{% elif bf.access == '1s' %}
-              <modifiedWriteValues>oneToSet</modifiedWriteValues>
-{% elif bf.access in ['roc', 'rolh'] %}
-              <readAction>clear</readAction>
-{% elif bf.access == 'roll' %}
-              <readAction>set</readAction>
-{% endif -%}
-{% endmacro %}
-<?xml version="1.0" encoding="utf-8"?>
-<device schemaVersion="1.1" xmlns:xs="http://www.w3.org/2001/XMLSchema-instance" xs:noNamespaceSchemaLocation="https://raw.githubusercontent.com/ARM-software/CMSIS_5/develop/CMSIS/Utilities/CMSIS-SVD.xsd" >
-  <name>{{ part_name }}</name>
-  <version>{{ part_version }}</version>
-  <description>{{ description }}</description>
-  <addressUnitBits>{{ config.address_width }}</addressUnitBits>
-  <width>{{ config.data_width }}</width>
-  <size>{{ config.data_width }}</size>
-
-  <peripherals>
-    {% set min_offset = (rmap | map(attribute='address') | sort)[0] %}
-    {% set max_offset = (rmap | map(attribute='address') | sort)[-1] %}
-    <!-- {{ peripheral_name }} -->
-    <peripheral>
-      <name>{{ peripheral_name }}</name>
-      <baseAddress>{{ literal(config.base_address, config.address_width) }}</baseAddress>
-      <addressBlock>
-        <offset>{{ literal(min_offset, config.address_width) }}</offset>
-        <size>{{ '0x%x' % (max_offset - min_offset + config.data_width / config.address_width) | int }}</size>
-        <usage>registers</usage>
-      </addressBlock>
-      <registers>
-{% for reg in rmap %}
-        <!-- {{ reg.name }} -->
-        <register>
-          <name>{{ reg.name }}</name>
-{% if reg.description %}
-          <description>{{ reg.description }}</description>
-{% endif %}
-          <addressOffset>{{ literal(reg.address, config.address_width) }}</addressOffset>
-          <resetValue>{{ literal(reg.reset, config.data_width) }}</resetValue>
-
-          <fields>
-{% for bf in reg.bitfields %}
-            <!-- {{ bf.name }} -->
-            <field>
-              <name>{{ bf.name }}</name>
-{% if bf.description %}
-              <description>{{ bf.description }}</description>
-{% endif %}
-              <bitRange>[{{ bf.msb }}:{{ bf.lsb }}]</bitRange>
-              {{ access(bf) }}
-{{ rw_mod(bf) }}
-{% if bf.enums %}
-              <enumeratedValues>
-{% for enum in bf.enums %}
-                <enumeratedValue>
-                  <name>{{ enum.name }}</name>
-{% if enum.description %}
-                  <description>{{ enum.description }}</description>
-{% endif %}
-                  <value>{{ enum.value }}</value>
-                </enumeratedValue>
-{% endfor %}
-              </enumeratedValues>
-{% endif %}
-            </field>
-{% endfor %}
-          </fields>
-        </register>
-{% endfor %}
-      </registers>
-    </peripheral>
-  </peripherals>
+{#- value in hex format #}
+{% macro literal(reset, width) %}
+{{ "0x%0{w}x".format(w=width // 4) % reset }}
+{%- endmacro %}
+{#- sw access #}
+{% macro access(bf) %}
+<access>{%- if bf.access.startswith('ro') %}
+read-only
+{%- elif bf.access.startswith('wo') %}
+write-only
+{%- else %}
+read-write
+{%- endif %}</access>
+{%- endmacro %}
+{#- read / write modify #}
+{% macro rw_mod(bf) %}
+{% if bf.access == 'rw1c' %}
+              <modifiedWriteValues>oneToClear</modifiedWriteValues>
+{% elif bf.access == '1s' %}
+              <modifiedWriteValues>oneToSet</modifiedWriteValues>
+{% elif bf.access in ['roc', 'rolh'] %}
+              <readAction>clear</readAction>
+{% elif bf.access == 'roll' %}
+              <readAction>set</readAction>
+{% endif -%}
+{% endmacro %}
+<?xml version="1.0" encoding="utf-8"?>
+<device schemaVersion="1.1" xmlns:xs="http://www.w3.org/2001/XMLSchema-instance" xs:noNamespaceSchemaLocation="https://raw.githubusercontent.com/ARM-software/CMSIS_5/develop/CMSIS/Utilities/CMSIS-SVD.xsd" >
+  <name>{{ part_name }}</name>
+  <version>{{ part_version }}</version>
+  <description>{{ description }}</description>
+  <addressUnitBits>{{ config.address_width }}</addressUnitBits>
+  <width>{{ config.data_width }}</width>
+  <size>{{ config.data_width }}</size>
+
+  <peripherals>
+    {% set min_offset = (rmap | map(attribute='address') | sort)[0] %}
+    {% set max_offset = (rmap | map(attribute='address') | sort)[-1] %}
+    <!-- {{ peripheral_name }} -->
+    <peripheral>
+      <name>{{ peripheral_name }}</name>
+      <baseAddress>{{ literal(config.base_address, config.address_width) }}</baseAddress>
+      <addressBlock>
+        <offset>{{ literal(min_offset, config.address_width) }}</offset>
+        <size>{{ '0x%x' % (max_offset - min_offset + config.data_width / config.address_width) | int }}</size>
+        <usage>registers</usage>
+      </addressBlock>
+      <registers>
+{% for reg in rmap %}
+        <!-- {{ reg.name }} -->
+        <register>
+          <name>{{ reg.name }}</name>
+{% if reg.description %}
+          <description>{{ reg.description }}</description>
+{% endif %}
+          <addressOffset>{{ literal(reg.address, config.address_width) }}</addressOffset>
+          <resetValue>{{ literal(reg.reset, config.data_width) }}</resetValue>
+
+          <fields>
+{% for bf in reg.bitfields %}
+            <!-- {{ bf.name }} -->
+            <field>
+              <name>{{ bf.name }}</name>
+{% if bf.description %}
+              <description>{{ bf.description }}</description>
+{% endif %}
+              <bitRange>[{{ bf.msb }}:{{ bf.lsb }}]</bitRange>
+              {{ access(bf) }}
+{{ rw_mod(bf) }}
+{% if bf.enums %}
+              <enumeratedValues>
+{% for enum in bf.enums %}
+                <enumeratedValue>
+                  <name>{{ enum.name }}</name>
+{% if enum.description %}
+                  <description>{{ enum.description }}</description>
+{% endif %}
+                  <value>{{ enum.value }}</value>
+                </enumeratedValue>
+{% endfor %}
+              </enumeratedValues>
+{% endif %}
+            </field>
+{% endfor %}
+          </fields>
+        </register>
+{% endfor %}
+      </registers>
+    </peripheral>
+  </peripherals>
 </device>
```

### Comparing `regmapGen-1.0.2/regmapGen/templates/ipxact_xml.j2` & `regmapGen-1.0.3/regmapGen/templates/ipxact_xml.j2`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-{#- value in hex format #}
-{% macro literal(reset, width) %}
-{{ "0x%0{w}x".format(w=width // 4) % reset }}
-{%- endmacro %}
-{#- sw access #}
-{% macro access(bf) %}
-<spirit:access>{%- if bf.access.startswith('ro') %}
-read-only
-{%- elif bf.access.startswith('wo') %}
-write-only
-{%- else %}
-read-write
-{%- endif %}</spirit:access>
-{%- endmacro %}
-{#- read / write modify #}
-{% macro rw_mod(bf) %}
-{% if bf.access == 'rw1c' %}
-            <spirit:modifiedWriteValues>oneToClear</spirit:modifiedWriteValues>
-{% elif bf.access == '1s' %}
-            <spirit:modifiedWriteValues>oneToSet</spirit:modifiedWriteValues>
-{% elif bf.access in ['roc', 'rolh'] %}
-            <spirit:readAction>clear</spirit:readAction>
-{% elif bf.access == 'roll' %}
-            <spirit:readAction>set</spirit:readAction>
-{% endif -%}
-{% endmacro %}
-<?xml version="1.0" encoding="utf-8"?>
-<spirit:component xmlns:spirit="http://www.spiritconsortium.org/XMLSchema/SPIRIT/1.5" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
-  <spirit:vendor>{{ vendor }}</spirit:vendor>
-  <spirit:library>{{ library }}</spirit:library>
-  <spirit:name>{{ component_name }}</spirit:name>
-  <spirit:version>{{ version }}</spirit:version>
-  <spirit:memoryMaps>
-    <spirit:memoryMap>
-      <spirit:name>{{ memorymap_name }}</spirit:name>
-      <spirit:addressBlock>
-        {% set min_offset = (rmap | map(attribute='address') | sort)[0] %}
-        {% set max_offset = (rmap | map(attribute='address') | sort)[-1] %}
-        <spirit:name>{{ addressblock_name }}</spirit:name>
-        <spirit:description>{{ description }}</spirit:description>
-        <spirit:baseAddress>{{ literal(config.base_address, config.address_width) }}</spirit:baseAddress>
-        <spirit:range>{{ '0x%x' % (max_offset - min_offset + config.data_width / config.address_width) | int }}</spirit:range>
-        <spirit:width>{{ config.data_width }}</spirit:width>
-{% for reg in rmap %}
-        <spirit:register>
-          <spirit:name>{{ reg.name }}</spirit:name>
-{% if reg.description %}
-          <spirit:description>{{ reg.description }}</spirit:description>
-{% endif %}
-          <spirit:addressOffset>{{ literal(reg.address, config.address_width) }}</spirit:addressOffset>
-          <spirit:size>{{ config.data_width }}</spirit:size>
-          <spirit:reset>
-            <spirit:value>{{ literal(reg.reset, config.data_width) }}</spirit:value>
-          </spirit:reset>
-{% for bf in reg.bitfields %}
-          <spirit:field>
-            <spirit:name>{{ bf.name }}</spirit:name>
-{% if bf.description %}
-            <spirit:description>{{ bf.description }}</spirit:description>
-{% endif %}
-            <spirit:bitOffset>{{ bf.lsb }}</spirit:bitOffset>
-            <spirit:bitWidth>{{ bf.msb - bf.lsb + 1 }}</spirit:bitWidth>
-            {{ access(bf) -}}
-{{ rw_mod(bf) }}
-{% if bf.enums %}
-            <spirit:enumeratedValues>
-{% for enum in bf.enums %}
-              <spirit:enumeratedValue>
-                <spirit:name>{{ enum.name }}</spirit:name>
-{% if enum.description %}
-                <spirit:description>{{ enum.description }}</spirit:description>
-{% endif %}
-                <spirit:value>{{ enum.value }}</spirit:value>
-              </spirit:enumeratedValue>
-{% endfor %}
-            </spirit:enumeratedValues>
-{% endif %}
-          </spirit:field>
-{% endfor %}
-        </spirit:register>
-{% endfor %}
-      </spirit:addressBlock>
-    </spirit:memoryMap>
-  </spirit:memoryMaps>
+{#- value in hex format #}
+{% macro literal(reset, width) %}
+{{ "0x%0{w}x".format(w=width // 4) % reset }}
+{%- endmacro %}
+{#- sw access #}
+{% macro access(bf) %}
+<spirit:access>{%- if bf.access.startswith('ro') %}
+read-only
+{%- elif bf.access.startswith('wo') %}
+write-only
+{%- else %}
+read-write
+{%- endif %}</spirit:access>
+{%- endmacro %}
+{#- read / write modify #}
+{% macro rw_mod(bf) %}
+{% if bf.access == 'rw1c' %}
+            <spirit:modifiedWriteValues>oneToClear</spirit:modifiedWriteValues>
+{% elif bf.access == '1s' %}
+            <spirit:modifiedWriteValues>oneToSet</spirit:modifiedWriteValues>
+{% elif bf.access in ['roc', 'rolh'] %}
+            <spirit:readAction>clear</spirit:readAction>
+{% elif bf.access == 'roll' %}
+            <spirit:readAction>set</spirit:readAction>
+{% endif -%}
+{% endmacro %}
+<?xml version="1.0" encoding="utf-8"?>
+<spirit:component xmlns:spirit="http://www.spiritconsortium.org/XMLSchema/SPIRIT/1.5" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
+  <spirit:vendor>{{ vendor }}</spirit:vendor>
+  <spirit:library>{{ library }}</spirit:library>
+  <spirit:name>{{ component_name }}</spirit:name>
+  <spirit:version>{{ version }}</spirit:version>
+  <spirit:memoryMaps>
+    <spirit:memoryMap>
+      <spirit:name>{{ memorymap_name }}</spirit:name>
+      <spirit:addressBlock>
+        {% set min_offset = (rmap | map(attribute='address') | sort)[0] %}
+        {% set max_offset = (rmap | map(attribute='address') | sort)[-1] %}
+        <spirit:name>{{ addressblock_name }}</spirit:name>
+        <spirit:description>{{ description }}</spirit:description>
+        <spirit:baseAddress>{{ literal(config.base_address, config.address_width) }}</spirit:baseAddress>
+        <spirit:range>{{ '0x%x' % (max_offset - min_offset + config.data_width / config.address_width) | int }}</spirit:range>
+        <spirit:width>{{ config.data_width }}</spirit:width>
+{% for reg in rmap %}
+        <spirit:register>
+          <spirit:name>{{ reg.name }}</spirit:name>
+{% if reg.description %}
+          <spirit:description>{{ reg.description }}</spirit:description>
+{% endif %}
+          <spirit:addressOffset>{{ literal(reg.address, config.address_width) }}</spirit:addressOffset>
+          <spirit:size>{{ config.data_width }}</spirit:size>
+          <spirit:reset>
+            <spirit:value>{{ literal(reg.reset, config.data_width) }}</spirit:value>
+          </spirit:reset>
+{% for bf in reg.bitfields %}
+          <spirit:field>
+            <spirit:name>{{ bf.name }}</spirit:name>
+{% if bf.description %}
+            <spirit:description>{{ bf.description }}</spirit:description>
+{% endif %}
+            <spirit:bitOffset>{{ bf.lsb }}</spirit:bitOffset>
+            <spirit:bitWidth>{{ bf.msb - bf.lsb + 1 }}</spirit:bitWidth>
+            {{ access(bf) -}}
+{{ rw_mod(bf) }}
+{% if bf.enums %}
+            <spirit:enumeratedValues>
+{% for enum in bf.enums %}
+              <spirit:enumeratedValue>
+                <spirit:name>{{ enum.name }}</spirit:name>
+{% if enum.description %}
+                <spirit:description>{{ enum.description }}</spirit:description>
+{% endif %}
+                <spirit:value>{{ enum.value }}</spirit:value>
+              </spirit:enumeratedValue>
+{% endfor %}
+            </spirit:enumeratedValues>
+{% endif %}
+          </spirit:field>
+{% endfor %}
+        </spirit:register>
+{% endfor %}
+      </spirit:addressBlock>
+    </spirit:memoryMap>
+  </spirit:memoryMaps>
 </spirit:component>
```

### Comparing `regmapGen-1.0.2/regmapGen/templates/regmap_asciidoc.j2` & `regmapGen-1.0.3/regmapGen/templates/regmap_asciidoc.j2`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-{#- MACRO #}
-{#- bit field range #}
-{% macro range(bf) %}
-    {% if bf.width == 1 %}
-{{ bf.msb }}
-    {%- else %}
-{{ bf.msb }}:{{ bf.lsb }}
-    {%- endif %}
-{%- endmacro %}
-
-{#- bit field mode #}
-{% macro mode(bf) %}
-{{ bf.access }}
-{%- endmacro %}
-
-{#- value in hex format #}
-{% macro literal(initial, width) %}
-{{ "0x%0{w}x".format(w=width // 4) % initial }}
-{%- endmacro %}
-
-{#- TEMPLATE NAMESPACE #}
-{% set tmp = namespace() %}
-
-{#- TEMPLATE #}
-= {{ title }}
-
-Автоматически сгенерировано с помощью программы regmapGen.
-
-{% if print_conventions %}
-[#table-Register_access_modes,cols="1,1", options="header"]
-|==========================
-| Тип доступа | Описание
-| rw          | Read and Write
-| rw1c        | Read and Write 1 to Clear
-| rw1s        | Read and Write 1 to Set
-| ro          | Read Only
-| roc         | Read Only to Clear
-| roll        | Read Only / Latch Low
-| rolh        | Read Only / Latch High
-| wo          | Write only
-| wosc        | Write Only / Self Clear
-|==========================
-{% endif %}
-
-[[register_map_summary]]
-== Регистры и команды
-
-**Базовый адрес**
-
-{{ "0x%08x" % config['base_address'] }}
-
-[#table-Register_map,cols="1,1,1", options="header"]
-|==========================
-| Регистр | Адрес | Описание
-{% for reg in rmap %}
-{{ "| %-24s | %-10s | %s" % ("<<%s>>" % (reg.name), literal(reg.address, config['address_width']), reg.description) }}
-{% endfor %}
-|==========================
-
-{% for reg in rmap %}
-
-\newpage
-
-[[{{ reg.name }}]]
-=== {{ reg.name }}
-
-**Описание**
-
-{{ reg.description }}
-
-**Смещение адреса**
-
-{{ literal(reg.address, config['address_width']) }}
-
-**Значение при сбросе**
-
-{{ literal(reg.reset, config['data_width']) }}
-
-{% if print_images %}
-image::{{ image_dir }}/{{ reg.name.lower() }}.svg[]
-{% endif %}
-
-[#table-{{ reg.name }},cols="1,1,1,1,1", options="header"]
-|==========================
-| Поле | Биты | Тип | Значение | Описание
-{% for bf in reg.bitfields[::-1] %}
-{{ "| %-16s | %-6s | %-15s | %-10s | %s" % (bf.name, range(bf), mode(bf), literal(bf.reset, bf.width), bf.description) }}
-{% endfor %}
-|==========================
-
-{% for bf in reg %}
-    {% if bf.enums %}
-
-Enumerated значения для {{ reg.name }}.{{ bf.name }}.
-
-[#table-{{ reg.name }}_{{ bf.name }}_enums,cols="1,1,1", options="header"]
-|==========================
-| Enum | Биты | Описание
-            {% for enum in bf %}
-{{ "| %-16s | %-6s | %s" % (enum.name, literal(enum.value, bf.width), enum.description) }}
-            {% endfor %}
-|==========================
-    {% endif %}
-{% endfor %}
-: *Таблица {{ loop.index }}* - Описание полей регистра {{ reg.name }}
-
+{#- MACRO #}
+{#- bit field range #}
+{% macro range(bf) %}
+    {% if bf.width == 1 %}
+{{ bf.msb }}
+    {%- else %}
+{{ bf.msb }}:{{ bf.lsb }}
+    {%- endif %}
+{%- endmacro %}
+
+{#- bit field mode #}
+{% macro mode(bf) %}
+{{ bf.access }}
+{%- endmacro %}
+
+{#- value in hex format #}
+{% macro literal(initial, width) %}
+{{ "0x%0{w}x".format(w=width // 4) % initial }}
+{%- endmacro %}
+
+{#- TEMPLATE NAMESPACE #}
+{% set tmp = namespace() %}
+
+{#- TEMPLATE #}
+= {{ title }}
+
+Автоматически сгенерировано с помощью программы regmapGen.
+
+{% if print_conventions %}
+[#table-Register_access_modes,cols="1,1", options="header"]
+|==========================
+| Тип доступа | Описание
+| rw          | Read and Write
+| rw1c        | Read and Write 1 to Clear
+| rw1s        | Read and Write 1 to Set
+| ro          | Read Only
+| roc         | Read Only to Clear
+| roll        | Read Only / Latch Low
+| rolh        | Read Only / Latch High
+| wo          | Write only
+| wosc        | Write Only / Self Clear
+|==========================
+{% endif %}
+
+[[register_map_summary]]
+== Регистры и команды
+
+**Базовый адрес**
+
+{{ "0x%08x" % config['base_address'] }}
+
+[#table-Register_map,cols="1,1,1", options="header"]
+|==========================
+| Регистр | Адрес | Описание
+{% for reg in rmap %}
+{{ "| %-24s | %-10s | %s" % ("<<%s>>" % (reg.name), literal(reg.address, config['address_width']), reg.description) }}
+{% endfor %}
+|==========================
+
+{% for reg in rmap %}
+
+\newpage
+
+[[{{ reg.name }}]]
+=== {{ reg.name }}
+
+**Описание**
+
+{{ reg.description }}
+
+**Смещение адреса**
+
+{{ literal(reg.address, config['address_width']) }}
+
+**Значение при сбросе**
+
+{{ literal(reg.reset, config['data_width']) }}
+
+{% if print_images %}
+image::{{ image_dir }}/{{ reg.name.lower() }}.svg[]
+{% endif %}
+
+[#table-{{ reg.name }},cols="1,1,1,1,1", options="header"]
+|==========================
+| Поле | Биты | Тип | Значение | Описание
+{% for bf in reg.bitfields[::-1] %}
+{{ "| %-16s | %-6s | %-15s | %-10s | %s" % (bf.name, range(bf), mode(bf), literal(bf.reset, bf.width), bf.description) }}
+{% endfor %}
+|==========================
+
+{% for bf in reg %}
+    {% if bf.enums %}
+
+Enumerated значения для {{ reg.name }}.{{ bf.name }}.
+
+[#table-{{ reg.name }}_{{ bf.name }}_enums,cols="1,1,1", options="header"]
+|==========================
+| Enum | Биты | Описание
+            {% for enum in bf %}
+{{ "| %-16s | %-6s | %s" % (enum.name, literal(enum.value, bf.width), enum.description) }}
+            {% endfor %}
+|==========================
+    {% endif %}
+{% endfor %}
+: *Таблица {{ loop.index }}* - Описание полей регистра {{ reg.name }}
+
 {% endfor %}
```

### Comparing `regmapGen-1.0.2/regmapGen/templates/regmap_md.j2` & `regmapGen-1.0.3/regmapGen/templates/regmap_md.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/regmap_py.j2` & `regmapGen-1.0.3/regmapGen/templates/regmap_py.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/regmap_rst.j2` & `regmapGen-1.0.3/regmapGen/templates/regmap_rst.j2`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-{# MACRO #}
-{#- generic range #}
-{% from "regmap_md.j2" import range with context %}
-{#- bit field mode #}
-{% from "regmap_md.j2" import mode with context %}
-{#- value in hex format #}
-{% from "regmap_md.j2" import literal with context %}
-{#- linkify title #}
-{% macro linkify(title) %}
-{{ title | lower | replace('_', '-') }}
-{%- endmacro %}
-{#- title with underline #}
-{% macro make_title(title, symbol) %}
-{{ title }}
-{{ symbol * title | length }}
-{%- endmacro %}
-{#- replace newlines #}
-{% macro rnl(string) %}
-{{ string | replace('\r', '') | replace('\n', ' |br| ') }}
-{%- endmacro %}
-
-{#- TEMPLATE NAMESPACE #}
-{% set tmp = namespace() %}
-
-{#- TEMPLATE #}
-.. |br| raw:: html
-
-   <br/>
-
-{{ make_title(title , '=') }}
-
-Автоматически сгенерировано с помощью программы regmapGen.
-
-{% if print_conventions %}
-{{ make_title("Сокращения", '-') }}
-
-.. list-table::
-   :header-rows: 1
-
-   * - Тип доступа
-     - Описание
-   * - rw
-     - Read and Write
-   * - rw1c
-     - Read and Write 1 to Clear
-   * - rw1s
-     - Read and Write 1 to Set
-   * - ro
-     - Read Only
-   * - roc
-     - Read Only to Clear
-   * - roll
-     - Read Only / Latch Low
-   * - rolh
-     - Read Only / Latch High
-   * - wo
-     - Write only
-   * - wosc
-     - Write Only / Self Clear
-{% endif %}
-
-{{ make_title("Регистры и команды", '-') }}
-
-Base address: {{ "0x%08x" % config['base_address'] }}
-
-.. list-table::
-   :header-rows: 1
-   :widths: auto
-
-   * - Регистр
-     - Адрес
-     - Описание
-{% for reg in rmap %}
-   * - `{{ reg.name }} <#{{ linkify(reg.name) }}>`__
-     - {{ literal(reg.address, config['address_width']) }}
-     - {{ rnl(reg.description) }}
-{% endfor %}
-{% for reg in rmap %}
-
-
-{{ make_title(reg.name, '-') }}
-
-Описание
-
-{{ reg.description }}
-
-Смещение адреса
-
-{{ literal(reg.address, config['address_width']) }}
-
-Значение при сбросе
-
-{{ literal(reg.reset, config['data_width']) }}
-
-{% if print_images %}
-.. image:: {{ image_dir }}/{{ reg.name.lower()}}.svg
-   :alt: {{ reg.name.lower()}}
-{% endif %}
-
-.. list-table::
-   :header-rows: 1
-   :widths: auto
-
-   * - Поле
-     - Биты
-     - Тип
-     - Значение
-     - Описание
-    {% set tmp.reserved_msb = config['data_width'] - 1 %}
-    {% for bf in reg.bitfields[::-1] %}
-        {% if tmp.reserved_msb > bf.msb %}
-            {% set tmp.reserved_lsb = bf.msb + 1 %}
-            {% set tmp.reserved_width = tmp.reserved_msb - tmp.reserved_lsb + 1 %}
-   * - --
-     - {{ range(tmp.reserved_msb, tmp.reserved_lsb) }}
-     - --
-     - {{ literal(0, tmp.reserved_width) }}
-     - Reserved
-        {% endif %}
-   * - {{ bf.name }}
-     - {{ range(bf.msb, bf.lsb) }}
-     - {{ mode(bf) }}
-     - {{ literal(bf.reset, bf.width) }}
-     - {{ rnl(bf.description) }}
-        {% set tmp.reserved_msb = bf.lsb - 1 %}
-    {% endfor %}
-
-    {% for bf in reg %}
-        {% if bf.enums %}
-{{ make_title('Enumerated значения для %s.%s' % (reg.name, bf.name), '.') }}
-
-.. list-table::
-   :header-rows: 1
-   :widths: auto
-
-   * - Enum
-     - Значение
-     - Описание
-            {% for enum in bf %}
-   * - {{ enum.name }}
-     - {{ literal(enum.value, bf.width) }}
-     - {{ rnl(enum.description) }}
-            {% endfor %}
-
-        {% endif %}
-    {% endfor %}
-Назад к `Регистры и команды <#Регистры-и-команды>`__.
+{# MACRO #}
+{#- generic range #}
+{% from "regmap_md.j2" import range with context %}
+{#- bit field mode #}
+{% from "regmap_md.j2" import mode with context %}
+{#- value in hex format #}
+{% from "regmap_md.j2" import literal with context %}
+{#- linkify title #}
+{% macro linkify(title) %}
+{{ title | lower | replace('_', '-') }}
+{%- endmacro %}
+{#- title with underline #}
+{% macro make_title(title, symbol) %}
+{{ title }}
+{{ symbol * title | length }}
+{%- endmacro %}
+{#- replace newlines #}
+{% macro rnl(string) %}
+{{ string | replace('\r', '') | replace('\n', ' |br| ') }}
+{%- endmacro %}
+
+{#- TEMPLATE NAMESPACE #}
+{% set tmp = namespace() %}
+
+{#- TEMPLATE #}
+.. |br| raw:: html
+
+   <br/>
+
+{{ make_title(title , '=') }}
+
+Автоматически сгенерировано с помощью программы regmapGen.
+
+{% if print_conventions %}
+{{ make_title("Сокращения", '-') }}
+
+.. list-table::
+   :header-rows: 1
+
+   * - Тип доступа
+     - Описание
+   * - rw
+     - Read and Write
+   * - rw1c
+     - Read and Write 1 to Clear
+   * - rw1s
+     - Read and Write 1 to Set
+   * - ro
+     - Read Only
+   * - roc
+     - Read Only to Clear
+   * - roll
+     - Read Only / Latch Low
+   * - rolh
+     - Read Only / Latch High
+   * - wo
+     - Write only
+   * - wosc
+     - Write Only / Self Clear
+{% endif %}
+
+{{ make_title("Регистры и команды", '-') }}
+
+Base address: {{ "0x%08x" % config['base_address'] }}
+
+.. list-table::
+   :header-rows: 1
+   :widths: auto
+
+   * - Регистр
+     - Адрес
+     - Описание
+{% for reg in rmap %}
+   * - `{{ reg.name }} <#{{ linkify(reg.name) }}>`__
+     - {{ literal(reg.address, config['address_width']) }}
+     - {{ rnl(reg.description) }}
+{% endfor %}
+{% for reg in rmap %}
+
+
+{{ make_title(reg.name, '-') }}
+
+Описание
+
+{{ reg.description }}
+
+Смещение адреса
+
+{{ literal(reg.address, config['address_width']) }}
+
+Значение при сбросе
+
+{{ literal(reg.reset, config['data_width']) }}
+
+{% if print_images %}
+.. image:: {{ image_dir }}/{{ reg.name.lower()}}.svg
+   :alt: {{ reg.name.lower()}}
+{% endif %}
+
+.. list-table::
+   :header-rows: 1
+   :widths: auto
+
+   * - Поле
+     - Биты
+     - Тип
+     - Значение
+     - Описание
+    {% set tmp.reserved_msb = config['data_width'] - 1 %}
+    {% for bf in reg.bitfields[::-1] %}
+        {% if tmp.reserved_msb > bf.msb %}
+            {% set tmp.reserved_lsb = bf.msb + 1 %}
+            {% set tmp.reserved_width = tmp.reserved_msb - tmp.reserved_lsb + 1 %}
+   * - --
+     - {{ range(tmp.reserved_msb, tmp.reserved_lsb) }}
+     - --
+     - {{ literal(0, tmp.reserved_width) }}
+     - Reserved
+        {% endif %}
+   * - {{ bf.name }}
+     - {{ range(bf.msb, bf.lsb) }}
+     - {{ mode(bf) }}
+     - {{ literal(bf.reset, bf.width) }}
+     - {{ rnl(bf.description) }}
+        {% set tmp.reserved_msb = bf.lsb - 1 %}
+    {% endfor %}
+
+    {% for bf in reg %}
+        {% if bf.enums %}
+{{ make_title('Enumerated значения для %s.%s' % (reg.name, bf.name), '.') }}
+
+.. list-table::
+   :header-rows: 1
+   :widths: auto
+
+   * - Enum
+     - Значение
+     - Описание
+            {% for enum in bf %}
+   * - {{ enum.name }}
+     - {{ literal(enum.value, bf.width) }}
+     - {{ rnl(enum.description) }}
+            {% endfor %}
+
+        {% endif %}
+    {% endfor %}
+Назад к `Регистры и команды <#Регистры-и-команды>`__.
 {% endfor %}
```

### Comparing `regmapGen-1.0.2/regmapGen/templates/regmap_sv.j2` & `regmapGen-1.0.3/regmapGen/templates/regmap_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/spi2lb_sv.j2` & `regmapGen-1.0.3/regmapGen/templates/spi2lb_sv.j2`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-// Created with regmapGen v{{ regmapGen_ver }}
-//
-// SPI to Local Bus bridge
-//
-// SPI parameters:
-//   - slave;
-//   - mode 0 only;
-//   - most significant bit transmitted first;
-//   - byte order from high to low;
-//   - SCK frequency must at least 8 lower than system frequency.
-
-module {{ module_name }} #(
-    parameter ADDR_W = {{ config['address_width'] }},
-    parameter DATA_W = {{ config['data_width'] }},
-    parameter STRB_W = DATA_W / 8
-)(
-    input                   clk,
-    input                   rst,
-    // Local Bus
-    input                   wready,
-    output reg [ADDR_W-1:0] waddr,
-    output reg [DATA_W-1:0] wdata,
-    output reg              wen,
-    output reg [STRB_W-1:0] wstrb,
-    input      [DATA_W-1:0] rdata,
-    input                   rvalid,
-    output     [ADDR_W-1:0] raddr,
-    output reg              ren,
-{% macro spi_core(regmap_embed=False) %}
-    // SPI
-    input                   spi_sck,
-    input                   spi_cs_n,
-    input                   spi_mosi,
-    output reg              spi_miso
-);
-{% if regmap_embed %}
-wire              wready;
-reg  [ADDR_W-1:0] waddr;
-reg  [DATA_W-1:0] wdata;
-reg               wen;
-reg  [STRB_W-1:0] wstrb;
-wire [DATA_W-1:0] rdata;
-wire              rvalid;
-wire [ADDR_W-1:0] raddr;
-reg               ren;
-{% endif %}
-
-//------------------------------------------------------------------------------
-// Inputs syncronization
-//------------------------------------------------------------------------------
-reg [1:0] cs_n_ff;
-wire      cs;
-reg [1:0] mosi_ff;
-wire      mo;
-reg [2:0] sck_ff;
-wire      sck_rise, sck_fall;
-
-// MOSI syncronization chain
-{% set rst_type = config['register_reset'] %}
-{%- if rst_type == 'async_pos' or rst_type == 'sync_pos' %}
-    {% set rst_active = 1%}
-{%- elif rst_type == 'async_neg' or rst_type == 'sync_neg' %}
-    {% set rst_active = 0%}
-{%- endif %}
-
-{% set rst_type = config['register_reset'] %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        mosi_ff <= 0;
-    end else begin
-        mosi_ff <= {mosi_ff[0], spi_mosi};
-    end
-end
-
-assign mo = mosi_ff[1];
-
-// CSn syncronization chain
-{% set rst_type = config['register_reset'] %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        cs_n_ff <= 0;
-    end else begin
-        cs_n_ff <= {cs_n_ff[0], spi_cs_n};
-    end
-end
-
-assign cs = ~cs_n_ff[1];
-
-// SCK syncronization and edge extraction
-{% set rst_type = config['register_reset'] %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        sck_ff <= 0;
-    end else begin
-        sck_ff <= {sck_ff[1:0], spi_sck};
-    end
-end
-
-assign sck_rise = (~sck_ff[2]) & ( sck_ff[1]);
-assign sck_fall = ( sck_ff[2]) & (~sck_ff[1]);
-
-//------------------------------------------------------------------------------
-// SPI slave FSM
-//------------------------------------------------------------------------------
-localparam BIT_CNT_W = ($clog2(DATA_W) > $clog2(ADDR_W)) ? $clog2(DATA_W) : $clog2(ADDR_W);
-localparam CTRL_W    = 8;
-
-// FSM states
-localparam IDLE_S        = 0;
-localparam RECV_MODE_S   = 1;
-localparam RECV_STRB_S   = 2;
-localparam RECV_ADDR_S   = 3;
-localparam WAIT_TA_S     = 4;
-localparam RECV_DATA_S   = 5;
-localparam TRAN_DATA_S   = 6;
-localparam WAIT_FINISH_S = 7;
-
-reg [2:0] fsm_state;
-reg [2:0] fsm_next;
-
-reg [ADDR_W-1:0] waddr_next;
-reg [DATA_W-1:0] wdata_next;
-reg [STRB_W-1:0] wstrb_next;
-reg              wen_next;
-reg              ren_next;
-
-reg spi_miso_next;
-
-reg [DATA_W-1:0]   dout_shifter, dout_shifter_next;
-reg                mode_wr, mode_wr_next;
-reg [BIT_CNT_W:0]  bit_cnt, bit_cnt_next;
-reg                force_tran, force_tran_next;
-
-{% set rst_type = config['register_reset'] %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        fsm_state <= IDLE_S;
-    end else begin
-        fsm_state <= fsm_next;
-    end
-end
-
-always @(*) begin
-    fsm_next          = fsm_state;
-    mode_wr_next      = mode_wr;
-    dout_shifter_next = dout_shifter;
-    bit_cnt_next      = bit_cnt;
-    force_tran_next   = force_tran;
-    spi_miso_next     = spi_miso;
-    waddr_next     = waddr;
-    wdata_next     = wdata;
-    wstrb_next     = wstrb;
-    wen_next       = wen;
-    ren_next       = ren;
-    case (fsm_state)
-        IDLE_S : begin
-            // wait cs_n assertion
-            spi_miso_next = 1'b0;
-            bit_cnt_next  = ADDR_W - 1;
-            if (cs)
-                fsm_next = RECV_ADDR_S;
-        end
-
-        RECV_ADDR_S : begin
-            // receive address
-            if (sck_rise) begin
-                waddr_next = {waddr[ADDR_W-2:0], mo};
-                if (bit_cnt == 0) begin
-                    bit_cnt_next = 0;
-                    fsm_next     = RECV_MODE_S;
-                end else begin
-                    bit_cnt_next = bit_cnt - 1;
-                end
-            end else if (!cs) // or finish packet
-                fsm_next = WAIT_FINISH_S;
-        end
-
-        RECV_MODE_S : begin
-            // receive transaction mode: write (1) or read (0)
-            if (sck_rise) begin
-                mode_wr_next = mo;
-                ren_next  = ~mo;
-                bit_cnt_next = CTRL_W - 2;
-                fsm_next     = RECV_STRB_S;
-            end else if (!cs) // or finish packet
-                fsm_next = WAIT_FINISH_S;
-        end
-
-        RECV_STRB_S : begin
-            // receive byte strobe bits for write
-            if (sck_rise) begin
-                wstrb_next = {wstrb[STRB_W-2:0], mo};
-                if (bit_cnt == 0) begin
-                    bit_cnt_next = DATA_W - 1;
-                    fsm_next     = mode_wr ? RECV_DATA_S : WAIT_TA_S;
-                end else begin
-                    bit_cnt_next = bit_cnt - 1;
-                end
-            end  else if (!cs) // or finish packet
-                fsm_next = WAIT_FINISH_S;
-
-            // and prepare data for reading at the same time
-            if (rvalid && ren) begin
-                dout_shifter_next = rdata;
-                ren_next       = 1'b0;
-            end
-        end
-
-        WAIT_TA_S : begin
-            // wait turnaround to start
-            if (sck_fall) begin
-                force_tran_next = 1'b1;
-                fsm_next        = TRAN_DATA_S;
-            end else if (!cs) // or finish packet
-                fsm_next = WAIT_FINISH_S;
-        end
-
-        RECV_DATA_S : begin
-            // receive data bit by bit at every sck posedge
-            if (sck_rise) begin
-                wdata_next = {wdata[DATA_W-2:0], mo};
-                if (bit_cnt == 0) begin
-                    wen_next  = 1'b1;
-                    fsm_next     = WAIT_FINISH_S;
-                end else begin
-                    bit_cnt_next = bit_cnt - 1;
-                end
-            end else if (!cs) // or finish packet
-                fsm_next = WAIT_FINISH_S;
-        end
-
-        TRAN_DATA_S : begin
-            force_tran_next   = 1'b0;
-            // transmit data bit by bit at every sck negedge
-            if (sck_fall || force_tran) begin
-                spi_miso_next     = dout_shifter[DATA_W-1];
-                dout_shifter_next = {dout_shifter[DATA_W-2:0], 1'b0};
-                if (bit_cnt == 0) begin
-                    fsm_next = WAIT_FINISH_S;
-                end else begin
-                    bit_cnt_next = bit_cnt - 1;
-                end
-            end else if (!cs) // or finish packet
-                fsm_next = WAIT_FINISH_S;
-        end
-
-        WAIT_FINISH_S : begin
-            // finish write transaction if any
-            if (wready && wen) begin
-                wen_next = 1'b0;
-            end
-            // finish read transaction if any
-            if (rvalid && ren) begin
-                ren_next = 1'b0;
-            end
-            // and then just wait when it will be safe to go to idle
-            if ((!wen) && (!ren) && (!cs)) begin
-                fsm_next = IDLE_S;
-            end
-        end
-    endcase
-end
-
-{% set rst_type = config['register_reset'] %}
-always @(posedge clk
-{%- if rst_type == 'async_pos' %} or posedge rst)
-{%- elif rst_type == 'async_neg' %} or negedge rst)
-{%- else -%} ) {%- endif %} begin
-    if (rst == 1'b{{ rst_active }}) begin
-        mode_wr      <= 1'b0;
-        dout_shifter <= 0;
-        bit_cnt      <= 0;
-        force_tran   <= 1'b0;
-        spi_miso     <= 1'b0;
-        waddr     <= 0;
-        wdata     <= 0;
-        wstrb     <= 0;
-        wen       <= 1'b0;
-        ren       <= 1'b0;
-    end else begin
-        mode_wr      <= mode_wr_next;
-        dout_shifter <= dout_shifter_next;
-        bit_cnt      <= bit_cnt_next;
-        force_tran   <= force_tran_next;
-        spi_miso     <= spi_miso_next;
-        waddr     <= waddr_next;
-        wdata     <= wdata_next;
-        wstrb     <= wstrb_next;
-        wen       <= wen_next;
-        ren       <= ren_next;
-    end
-end
-
-assign raddr = waddr;
-{% endmacro %}
-{{ spi_core() }}
+// Created with regmapGen v{{ regmapGen_ver }}
+//
+// SPI to Local Bus bridge
+//
+// SPI parameters:
+//   - slave;
+//   - mode 0 only;
+//   - most significant bit transmitted first;
+//   - byte order from high to low;
+//   - SCK frequency must at least 8 lower than system frequency.
+
+module {{ module_name }} #(
+    parameter ADDR_W = {{ config['address_width'] }},
+    parameter DATA_W = {{ config['data_width'] }},
+    parameter STRB_W = DATA_W / 8
+)(
+    input                   clk,
+    input                   rst,
+    // Local Bus
+    input                   wready,
+    output reg [ADDR_W-1:0] waddr,
+    output reg [DATA_W-1:0] wdata,
+    output reg              wen,
+    output reg [STRB_W-1:0] wstrb,
+    input      [DATA_W-1:0] rdata,
+    input                   rvalid,
+    output     [ADDR_W-1:0] raddr,
+    output reg              ren,
+{% macro spi_core(regmap_embed=False) %}
+    // SPI
+    input                   spi_sck,
+    input                   spi_cs_n,
+    input                   spi_mosi,
+    output reg              spi_miso
+);
+{% if regmap_embed %}
+wire              wready;
+reg  [ADDR_W-1:0] waddr;
+reg  [DATA_W-1:0] wdata;
+reg               wen;
+reg  [STRB_W-1:0] wstrb;
+wire [DATA_W-1:0] rdata;
+wire              rvalid;
+wire [ADDR_W-1:0] raddr;
+reg               ren;
+{% endif %}
+
+//------------------------------------------------------------------------------
+// Inputs syncronization
+//------------------------------------------------------------------------------
+reg [1:0] cs_n_ff;
+wire      cs;
+reg [1:0] mosi_ff;
+wire      mo;
+reg [2:0] sck_ff;
+wire      sck_rise, sck_fall;
+
+// MOSI syncronization chain
+{% set rst_type = config['register_reset'] %}
+{%- if rst_type == 'async_pos' or rst_type == 'sync_pos' %}
+    {% set rst_active = 1%}
+{%- elif rst_type == 'async_neg' or rst_type == 'sync_neg' %}
+    {% set rst_active = 0%}
+{%- endif %}
+
+{% set rst_type = config['register_reset'] %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        mosi_ff <= 0;
+    end else begin
+        mosi_ff <= {mosi_ff[0], spi_mosi};
+    end
+end
+
+assign mo = mosi_ff[1];
+
+// CSn syncronization chain
+{% set rst_type = config['register_reset'] %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        cs_n_ff <= 0;
+    end else begin
+        cs_n_ff <= {cs_n_ff[0], spi_cs_n};
+    end
+end
+
+assign cs = ~cs_n_ff[1];
+
+// SCK syncronization and edge extraction
+{% set rst_type = config['register_reset'] %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        sck_ff <= 0;
+    end else begin
+        sck_ff <= {sck_ff[1:0], spi_sck};
+    end
+end
+
+assign sck_rise = (~sck_ff[2]) & ( sck_ff[1]);
+assign sck_fall = ( sck_ff[2]) & (~sck_ff[1]);
+
+//------------------------------------------------------------------------------
+// SPI slave FSM
+//------------------------------------------------------------------------------
+localparam BIT_CNT_W = ($clog2(DATA_W) > $clog2(ADDR_W)) ? $clog2(DATA_W) : $clog2(ADDR_W);
+localparam CTRL_W    = 8;
+
+// FSM states
+localparam IDLE_S        = 0;
+localparam RECV_MODE_S   = 1;
+localparam RECV_STRB_S   = 2;
+localparam RECV_ADDR_S   = 3;
+localparam WAIT_TA_S     = 4;
+localparam RECV_DATA_S   = 5;
+localparam TRAN_DATA_S   = 6;
+localparam WAIT_FINISH_S = 7;
+
+reg [2:0] fsm_state;
+reg [2:0] fsm_next;
+
+reg [ADDR_W-1:0] waddr_next;
+reg [DATA_W-1:0] wdata_next;
+reg [STRB_W-1:0] wstrb_next;
+reg              wen_next;
+reg              ren_next;
+
+reg spi_miso_next;
+
+reg [DATA_W-1:0]   dout_shifter, dout_shifter_next;
+reg                mode_wr, mode_wr_next;
+reg [BIT_CNT_W:0]  bit_cnt, bit_cnt_next;
+reg                force_tran, force_tran_next;
+
+{% set rst_type = config['register_reset'] %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        fsm_state <= IDLE_S;
+    end else begin
+        fsm_state <= fsm_next;
+    end
+end
+
+always @(*) begin
+    fsm_next          = fsm_state;
+    mode_wr_next      = mode_wr;
+    dout_shifter_next = dout_shifter;
+    bit_cnt_next      = bit_cnt;
+    force_tran_next   = force_tran;
+    spi_miso_next     = spi_miso;
+    waddr_next     = waddr;
+    wdata_next     = wdata;
+    wstrb_next     = wstrb;
+    wen_next       = wen;
+    ren_next       = ren;
+    case (fsm_state)
+        IDLE_S : begin
+            // wait cs_n assertion
+            spi_miso_next = 1'b0;
+            bit_cnt_next  = ADDR_W - 1;
+            if (cs)
+                fsm_next = RECV_ADDR_S;
+        end
+
+        RECV_ADDR_S : begin
+            // receive address
+            if (sck_rise) begin
+                waddr_next = {waddr[ADDR_W-2:0], mo};
+                if (bit_cnt == 0) begin
+                    bit_cnt_next = 0;
+                    fsm_next     = RECV_MODE_S;
+                end else begin
+                    bit_cnt_next = bit_cnt - 1;
+                end
+            end else if (!cs) // or finish packet
+                fsm_next = WAIT_FINISH_S;
+        end
+
+        RECV_MODE_S : begin
+            // receive transaction mode: write (1) or read (0)
+            if (sck_rise) begin
+                mode_wr_next = mo;
+                ren_next  = ~mo;
+                bit_cnt_next = CTRL_W - 2;
+                fsm_next     = RECV_STRB_S;
+            end else if (!cs) // or finish packet
+                fsm_next = WAIT_FINISH_S;
+        end
+
+        RECV_STRB_S : begin
+            // receive byte strobe bits for write
+            if (sck_rise) begin
+                wstrb_next = {wstrb[STRB_W-2:0], mo};
+                if (bit_cnt == 0) begin
+                    bit_cnt_next = DATA_W - 1;
+                    fsm_next     = mode_wr ? RECV_DATA_S : WAIT_TA_S;
+                end else begin
+                    bit_cnt_next = bit_cnt - 1;
+                end
+            end  else if (!cs) // or finish packet
+                fsm_next = WAIT_FINISH_S;
+
+            // and prepare data for reading at the same time
+            if (rvalid && ren) begin
+                dout_shifter_next = rdata;
+                ren_next       = 1'b0;
+            end
+        end
+
+        WAIT_TA_S : begin
+            // wait turnaround to start
+            if (sck_fall) begin
+                force_tran_next = 1'b1;
+                fsm_next        = TRAN_DATA_S;
+            end else if (!cs) // or finish packet
+                fsm_next = WAIT_FINISH_S;
+        end
+
+        RECV_DATA_S : begin
+            // receive data bit by bit at every sck posedge
+            if (sck_rise) begin
+                wdata_next = {wdata[DATA_W-2:0], mo};
+                if (bit_cnt == 0) begin
+                    wen_next  = 1'b1;
+                    fsm_next     = WAIT_FINISH_S;
+                end else begin
+                    bit_cnt_next = bit_cnt - 1;
+                end
+            end else if (!cs) // or finish packet
+                fsm_next = WAIT_FINISH_S;
+        end
+
+        TRAN_DATA_S : begin
+            force_tran_next   = 1'b0;
+            // transmit data bit by bit at every sck negedge
+            if (sck_fall || force_tran) begin
+                spi_miso_next     = dout_shifter[DATA_W-1];
+                dout_shifter_next = {dout_shifter[DATA_W-2:0], 1'b0};
+                if (bit_cnt == 0) begin
+                    fsm_next = WAIT_FINISH_S;
+                end else begin
+                    bit_cnt_next = bit_cnt - 1;
+                end
+            end else if (!cs) // or finish packet
+                fsm_next = WAIT_FINISH_S;
+        end
+
+        WAIT_FINISH_S : begin
+            // finish write transaction if any
+            if (wready && wen) begin
+                wen_next = 1'b0;
+            end
+            // finish read transaction if any
+            if (rvalid && ren) begin
+                ren_next = 1'b0;
+            end
+            // and then just wait when it will be safe to go to idle
+            if ((!wen) && (!ren) && (!cs)) begin
+                fsm_next = IDLE_S;
+            end
+        end
+    endcase
+end
+
+{% set rst_type = config['register_reset'] %}
+always @(posedge clk
+{%- if rst_type == 'async_pos' %} or posedge rst)
+{%- elif rst_type == 'async_neg' %} or negedge rst)
+{%- else -%} ) {%- endif %} begin
+    if (rst == 1'b{{ rst_active }}) begin
+        mode_wr      <= 1'b0;
+        dout_shifter <= 0;
+        bit_cnt      <= 0;
+        force_tran   <= 1'b0;
+        spi_miso     <= 1'b0;
+        waddr     <= 0;
+        wdata     <= 0;
+        wstrb     <= 0;
+        wen       <= 1'b0;
+        ren       <= 1'b0;
+    end else begin
+        mode_wr      <= mode_wr_next;
+        dout_shifter <= dout_shifter_next;
+        bit_cnt      <= bit_cnt_next;
+        force_tran   <= force_tran_next;
+        spi_miso     <= spi_miso_next;
+        waddr     <= waddr_next;
+        wdata     <= wdata_next;
+        wstrb     <= wstrb_next;
+        wen       <= wen_next;
+        ren       <= ren_next;
+    end
+end
+
+assign raddr = waddr;
+{% endmacro %}
+{{ spi_core() }}
 endmodule
```

### Comparing `regmapGen-1.0.2/regmapGen/templates/sv_header.j2` & `regmapGen-1.0.3/regmapGen/templates/sv_header.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/templates/sv_package.j2` & `regmapGen-1.0.3/regmapGen/templates/sv_package.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen/utils.py` & `regmapGen-1.0.3/regmapGen/utils.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.2/regmapGen.egg-info/PKG-INFO` & `regmapGen-1.0.3/regmapGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regmapGen
-Version: 1.0.2
+Version: 1.0.3
 Summary: Генератор Регистровой Карты
 Home-page: https://github.com/paulmsv/regmapGen
 Author: paulmsv
 Author-email: bobkovpg@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://regmapGen.readthedocs.io
 Platform: UNKNOWN
```

### Comparing `regmapGen-1.0.2/regmapGen.egg-info/SOURCES.txt` & `regmapGen-1.0.3/regmapGen.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 regmapGen/templates/regmap_asciidoc.j2
 regmapGen/templates/regmap_md.j2
 regmapGen/templates/regmap_py.j2
 regmapGen/templates/regmap_rst.j2
 regmapGen/templates/regmap_sv.j2
 regmapGen/templates/spi2lb_sv.j2
 regmapGen/templates/sv_header.j2
-regmapGen/templates/sv_package.j2
+regmapGen/templates/sv_package.j2
+regmapGen/templates/sv_wrapper.j2
```

### Comparing `regmapGen-1.0.2/setup.py` & `regmapGen-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Install package
 setuptools.setup(
     name="regmapGen",
-    version='1.0.2',
+    version='1.0.3',
     author="paulmsv",
     author_email="bobkovpg@gmail.com",
     description="Генератор Регистровой Карты",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/paulmsv/regmapGen",
     project_urls={
```

