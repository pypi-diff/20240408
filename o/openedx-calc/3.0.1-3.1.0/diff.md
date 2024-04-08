# Comparing `tmp/openedx-calc-3.0.1.tar.gz` & `tmp/openedx-calc-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-calc-3.0.1.tar", last modified: Mon Feb  7 17:14:30 2022, max compression
+gzip compressed data, was "openedx-calc-3.1.0.tar", last modified: Mon Apr  8 18:57:14 2024, max compression
```

## Comparing `openedx-calc-3.0.1.tar` & `openedx-calc-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 17:14:30.726535 openedx-calc-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-07 17:14:30.730535 openedx-calc-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 17:14:30.726535 openedx-calc-3.0.1/calc/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16386 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/calc/calc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/calc/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12154 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/calc/preview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 17:14:30.726535 openedx-calc-3.0.1/openedx_calc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-07 17:14:30.000000 openedx-calc-3.0.1/openedx_calc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-02-07 17:14:30.000000 openedx-calc-3.0.1/openedx_calc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 17:14:30.000000 openedx-calc-3.0.1/openedx_calc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 17:14:30.000000 openedx-calc-3.0.1/openedx_calc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-02-07 17:14:30.000000 openedx-calc-3.0.1/openedx_calc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-07 17:14:30.000000 openedx-calc-3.0.1/openedx_calc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 17:14:30.726535 openedx-calc-3.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-07 17:14:30.730535 openedx-calc-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 17:14:30.726535 openedx-calc-3.0.1/symmath/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/symmath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22016 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/symmath/formula.py
--rw-r--r--   0 runner    (1001) docker     (121)    14179 2022-02-07 17:14:26.000000 openedx-calc-3.0.1/symmath/symmath_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:57:14.338118 openedx-calc-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 18:57:14.338118 openedx-calc-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:57:14.334118 openedx-calc-3.1.0/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16631 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/calc/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/calc/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/calc/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:57:14.334118 openedx-calc-3.1.0/openedx_calc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 18:57:14.000000 openedx-calc-3.1.0/openedx_calc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-08 18:57:14.000000 openedx-calc-3.1.0/openedx_calc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:57:14.000000 openedx-calc-3.1.0/openedx_calc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:57:14.000000 openedx-calc-3.1.0/openedx_calc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 18:57:14.000000 openedx-calc-3.1.0/openedx_calc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 18:57:14.000000 openedx-calc-3.1.0/openedx_calc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:57:14.334118 openedx-calc-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 18:57:14.338118 openedx-calc-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:57:14.334118 openedx-calc-3.1.0/symmath/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/symmath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/symmath/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/symmath/symmath_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:57:14.334118 openedx-calc-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/tests/test_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-08 18:57:10.000000 openedx-calc-3.1.0/tests/test_symmath_check.py
```

### Comparing `openedx-calc-3.0.1/LICENSE` & `openedx-calc-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openedx-calc-3.0.1/PKG-INFO` & `openedx-calc-3.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: openedx-calc
-Version: 3.0.1
+Version: 3.1.0
 Summary: A helper library for mathematical calculations and symbolic mathematics, used by Open edX.
-Home-page: https://github.com/edx/openedx-calc
+Home-page: https://github.com/openedx/openedx-calc
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: edx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: sympy
+Requires-Dist: numpy
+Requires-Dist: markupsafe
+Requires-Dist: scipy
+Requires-Dist: lxml
+Requires-Dist: pyparsing
 
 openedx-calc
 ============
 
 A helper library for mathematical calculations and symbolic mathematics, used by the `edx-platform`_.
 
 This code originally lived in the `edx-platform`_ repo, but now exists here independently.
@@ -28,11 +34,9 @@
 
 License
 -------
 
 The code in this repository is licensed under version 3 of the AGPL unless otherwise noted. Please see the `LICENSE`_ file for details.
 
 
-.. _edx-platform: https://github.com/edx/edx-platform
-.. _LICENSE: https://github.com/edx/openedx-calc/blob/master/LICENSE
-
-
+.. _edx-platform: https://github.com/openedx/edx-platform
+.. _LICENSE: https://github.com/openedx/openedx-calc/blob/master/LICENSE
```

### Comparing `openedx-calc-3.0.1/calc/calc.py` & `openedx-calc-3.1.0/calc/calc.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,19 @@
 def eval_number(parse_result):
     """
     Create a float out of its string parts.
 
     e.g. [ '7.13', 'e', '3' ] ->  7130
     Calls super_float above.
     """
-    return super_float("".join(parse_result))
+    for item in parse_result:
+        if "." in item or "e" in item or "E" in item:
+            return super_float("".join(parse_result))
+
+    return int("".join(parse_result))
 
 
 def eval_atom(parse_result):
     """
     Return the value wrapped by the atom.
 
     In the case of parenthesis, ignore them.
@@ -181,15 +185,15 @@
     """
     Add the inputs, keeping in mind their sign.
 
     [ 1, '+', 2, '-', 3 ] -> 0
 
     Allow a leading + or -.
     """
-    total = 0.0
+    total = 0
     current_op = operator.add
     for token in parse_result:
         if token == '+':
             current_op = operator.add
         elif token == '-':
             current_op = operator.sub
         else:
@@ -199,15 +203,15 @@
 
 def eval_product(parse_result):
     """
     Multiply the inputs.
 
     [ 1, '*', 2, '/', 3 ] -> 0.66
     """
-    prod = 1.0
+    prod = 1
     current_op = operator.mul
     for token in parse_result:
         if token == '*':
             current_op = operator.mul
         elif token == '/':
             current_op = operator.truediv
         else:
@@ -251,23 +255,30 @@
     # Get our variables together.
     all_variables, all_functions = add_defaults(variables, unary_functions, case_sensitive)
 
     # ...and check them
     math_interpreter.check_variables(all_variables, all_functions)
 
     # Create a recursion to evaluate the tree.
-    if case_sensitive:
-        casify = lambda x: x
-    else:
-        casify = lambda x: x.lower()  # Lowercase for case insens.
+    def casify(x):
+        if case_sensitive:
+            return x
+        else:
+            return x.lower()  # Lowercase for case insens.
+
+    def eval_variable(x):
+        return all_variables[casify(x[0])]
+
+    def eval_function(x):
+        return all_functions[casify(x[0])](x[1])
 
     evaluate_actions = {
         'number': eval_number,
-        'variable': lambda x: all_variables[casify(x[0])],
-        'function': lambda x: all_functions[casify(x[0])](x[1]),
+        'variable': eval_variable,
+        'function': eval_function,
         'atom': eval_atom,
         'power': eval_power,
         'parallel': eval_parallel,
         'product': eval_product,
         'sum': eval_sum
     }
 
@@ -448,18 +459,19 @@
 
     def check_variables(self, valid_variables, valid_functions):
         """
         Confirm that all the variables used in the tree are valid/defined.
 
         Otherwise, raise an UndefinedVariable containing all bad variables.
         """
-        if self.case_sensitive:
-            casify = lambda x: x
-        else:
-            casify = lambda x: x.lower()  # Lowercase for case insens.
+        def casify(x):
+            if self.case_sensitive:
+                return x
+            else:
+                return x.lower()  # Lowercase for case insens.
 
         bad_vars = {var for var in self.variables_used
                     if casify(var) not in valid_variables}
 
         if bad_vars:
             varnames = ", ".join(sorted(bad_vars))
             message = f"Invalid Input: {varnames} not permitted in answer as a variable"
```

### Comparing `openedx-calc-3.0.1/calc/functions.py` & `openedx-calc-3.1.0/calc/functions.py`

 * *Files identical despite different names*

### Comparing `openedx-calc-3.0.1/calc/preview.py` & `openedx-calc-3.1.0/calc/preview.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,15 +206,17 @@
     """
     if len(children) == 1:
         return children[0]
 
     children_latex = [k.latex for k in children if k.latex != "^"]
     children_latex[-1] = children[-1].sans_parens
 
-    raise_power = lambda x, y: f"{y}^{{{x}}}"
+    def raise_power(x, y):
+        return f"{y}^{{{x}}}"
+
     latex = reduce(raise_power, reversed(children_latex))
     return LatexRendered(latex, tall=True)
 
 
 def render_parallel(children):
     """
     Simply join the child nodes with a double vertical line.
@@ -368,33 +370,36 @@
     latex_interpreter = ParseAugmenter(math_expr, case_sensitive)
     latex_interpreter.parse_algebra()
 
     # Get our variables together.
     variables, functions = add_defaults(variables, functions, case_sensitive)
 
     # Create a recursion to evaluate the tree.
-    if case_sensitive:
-        casify = lambda x: x
-    else:
-        casify = lambda x: x.lower()  # Lowercase for case insens.
+    def casify(x):
+        if case_sensitive:
+            return x
+        else:
+            return x.lower()  # Lowercase for case insens.
 
     render_actions = {
         'number': render_number,
         'variable': variable_closure(variables, casify),
         'function': function_closure(functions, casify),
         'atom': render_atom,
         'power': render_power,
         'parallel': render_parallel,
         'product': render_product,
         'sum': render_sum
     }
 
     backslash = "\\"
-    wrap_escaped_strings = lambda s: LatexRendered(
-        s.replace(backslash, backslash * 2)
-    )
+
+    def wrap_escaped_strings(s):
+        return LatexRendered(
+            s.replace(backslash, backslash * 2)
+        )
 
     output = latex_interpreter.reduce_tree(
         render_actions,
         terminal_converter=wrap_escaped_strings
     )
     return output.latex
```

### Comparing `openedx-calc-3.0.1/openedx_calc.egg-info/PKG-INFO` & `openedx-calc-3.1.0/openedx_calc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: openedx-calc
-Version: 3.0.1
+Version: 3.1.0
 Summary: A helper library for mathematical calculations and symbolic mathematics, used by Open edX.
-Home-page: https://github.com/edx/openedx-calc
+Home-page: https://github.com/openedx/openedx-calc
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: edx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: sympy
+Requires-Dist: numpy
+Requires-Dist: markupsafe
+Requires-Dist: scipy
+Requires-Dist: lxml
+Requires-Dist: pyparsing
 
 openedx-calc
 ============
 
 A helper library for mathematical calculations and symbolic mathematics, used by the `edx-platform`_.
 
 This code originally lived in the `edx-platform`_ repo, but now exists here independently.
@@ -28,11 +34,9 @@
 
 License
 -------
 
 The code in this repository is licensed under version 3 of the AGPL unless otherwise noted. Please see the `LICENSE`_ file for details.
 
 
-.. _edx-platform: https://github.com/edx/edx-platform
-.. _LICENSE: https://github.com/edx/openedx-calc/blob/master/LICENSE
-
-
+.. _edx-platform: https://github.com/openedx/edx-platform
+.. _LICENSE: https://github.com/openedx/openedx-calc/blob/master/LICENSE
```

### Comparing `openedx-calc-3.0.1/setup.py` & `openedx-calc-3.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     version=VERSION,
     description=('A helper library for mathematical calculations and symbolic '
                  'mathematics, used by Open edX.'),
     long_description=README,
     long_description_content_type="text/x-rst",
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/openedx-calc',
+    url='https://github.com/openedx/openedx-calc',
     packages=[
         'calc',
         "symmath"
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     python_requires=">=3.8",
@@ -74,9 +74,10 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `openedx-calc-3.0.1/symmath/formula.py` & `openedx-calc-3.1.0/symmath/formula.py`

 * *Files identical despite different names*

### Comparing `openedx-calc-3.0.1/symmath/symmath_check.py` & `openedx-calc-3.1.0/symmath/symmath_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 def symmath_check_simple(expect, ans, adict={}, symtab=None, extra_options=None):  # lint-amnesty, pylint: disable=dangerous-default-value, unused-argument
     """
     Check a symbolic mathematical expression using sympy.
     The input is an ascii string (not MathML) converted to math using sympy.sympify.
     """
 
     options = {'__MATRIX__': False, '__ABC__': False, '__LOWER__': False}
+    options_copy = options
     if extra_options:
         options.update(extra_options)
-    for op in options:				# find options in expect string
+    for op in options_copy:				# find options in expect string
         if op in expect:
             expect = expect.replace(op, '')
             options[op] = True
     expect = expect.replace('__OR__', '__or__')	 # backwards compatibility
 
     if options['__LOWER__']:
         expect = expect.lower()
@@ -319,15 +320,15 @@
                 msg += Markup("<p/><pre>{format_exc}</pre>").format(format_exc=traceback.format_exc())
             return {'ok': False, 'msg': make_error_message(msg)}
 
     #diff = (fexpect-fsym).simplify()
     #fsym = fsym.simplify()
     #fexpect = fexpect.simplify()
     try:
-        diff = (fexpect - fsym)
+        diff = fexpect - fsym
     except Exception as err:  # lint-amnesty, pylint: disable=broad-except
         diff = None
 
     if DEBUG:
         msg += Markup('<hr><p><font color="blue">DEBUG messages:</p><p>Got: {fsym}</p><p>Expecting: {fexpect}</p>')\
             .format(fsym=repr(fsym), fexpect=repr(fexpect).replace('**', '^').replace('hat(I)', 'hat(i)'))
         # msg += "<p/>Got: %s" % str([type(x) for x in fsym.atoms()]).replace('<','&lt;')
```

