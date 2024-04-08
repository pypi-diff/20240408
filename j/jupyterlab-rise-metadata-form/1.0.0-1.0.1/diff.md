# Comparing `tmp/jupyterlab_rise_metadata_form-1.0.0.tar.gz` & `tmp/jupyterlab_rise_metadata_form-1.0.1.tar.gz`

## Comparing `jupyterlab_rise_metadata_form-1.0.0.tar` & `jupyterlab_rise_metadata_form-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/.yarnrc.yml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/install.json
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form.png
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/tsconfig.json
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/_version.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/package.json
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/package.json.orig
--rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/risemdf.json
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/568.523b878894628ce0ce6f.js
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/747.9b83aa6cc639b78d65e7.js
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/remoteEntry.46bdb8f3cf2cfa8594cb.js
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/schema/risemdf.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/style/index.js
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/LICENSE
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/README.md
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/install.json
+-rw-r--r--   0        0        0    24863 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form.png
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/_version.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/package.json
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/package.json.orig
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/risemdf.json
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/509.82c83d88a314838bd37c.js
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/728.8dcd6beb31a2181fb758.js
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/remoteEntry.952aa98dd7822da17116.js
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/schema/risemdf.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/style/index.js
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/LICENSE
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/README.md
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 jupyterlab_rise_metadata_form-1.0.1/PKG-INFO
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/package.json` & `jupyterlab_rise_metadata_form-1.0.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -189,9 +189,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/tsconfig.json` & `jupyterlab_rise_metadata_form-1.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/__init__.py` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/package.json` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.952aa98dd7822da17116.js'}}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -107,15 +107,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/jans-code/jupyterlab_rise_metadata_form",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.46bdb8f3cf2cfa8594cb.js",
+            "load": "static/remoteEntry.952aa98dd7822da17116.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_rise_metadata_form/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -194,9 +194,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/package.json.orig` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -189,9 +189,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/risemdf.json` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/schemas/@jans-code/jupyterlab_rise_metadata_form/risemdf.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999881628787879%*

 * *Differences: {"'jupyter.lab.metadataforms'": "{0: {'metadataSchema': {'properties': {'/rise/controls': "*

 * *                                "{'title': 'Controls'}}}}}"}*

```diff
@@ -133,15 +133,15 @@
                     "/rise/center": {
                         "default": true,
                         "title": "Reveal center",
                         "type": "boolean"
                     },
                     "/rise/controls": {
                         "default": true,
-                        "title": "Autolaunch",
+                        "title": "Controls",
                         "type": "boolean"
                     },
                     "/rise/enable_chalkboard": {
                         "title": "Chalkboard",
                         "type": "boolean"
                     },
                     "/rise/footer": {
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/747.9b83aa6cc639b78d65e7.js` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/728.8dcd6beb31a2181fb758.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_jans_code_jupyterlab_rise_metadata_form = self.webpackChunk_jans_code_jupyterlab_rise_metadata_form || []).push([
-    [747], {
-        150: (e, t, n) => {
+    [728], {
+        475: (e, t, n) => {
             n.d(t, {
-                Z: () => c
+                A: () => c
             });
-            var r = n(81),
+            var r = n(601),
                 a = n.n(r),
-                o = n(645),
+                o = n(314),
                 s = n.n(o)()(a());
             s.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
             const c = s
         },
-        645: e => {
+        314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = "",
                             r = void 0 !== t[5];
                         return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), r && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), r && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
@@ -34,20 +34,20 @@
                     for (var u = 0; u < e.length; u++) {
                         var l = [].concat(e[u]);
                         r && s[l[0]] || (void 0 !== o && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = o), n && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = n) : l[2] = n), a && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = a) : l[4] = "".concat(a)), t.push(l))
                     }
                 }, t
             }
         },
-        81: e => {
+        601: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
-        379: e => {
+        72: e => {
             var t = [];
 
             function n(e) {
                 for (var n = -1, r = 0; r < t.length; r++)
                     if (t[r].identifier === e) {
                         n = r;
                         break
@@ -105,15 +105,15 @@
                         var l = n(o[u]);
                         0 === t[l].references && (t[l].updater(), t.splice(l, 1))
                     }
                     o = i
                 }
             }
         },
-        569: e => {
+        659: e => {
             var t = {};
             e.exports = function(e, n) {
                 var r = function(e) {
                     if (void 0 === t[e]) {
                         var n = document.querySelector(e);
                         if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                             n = n.contentDocument.head
@@ -124,27 +124,27 @@
                     }
                     return t[e]
                 }(e);
                 if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                 r.appendChild(n)
             }
         },
-        216: e => {
+        540: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
         },
-        565: (e, t, n) => {
+        56: (e, t, n) => {
             e.exports = function(e) {
                 var t = n.nc;
                 t && e.setAttribute("nonce", t)
             }
         },
-        795: e => {
+        825: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
@@ -163,36 +163,36 @@
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
                     }
                 }
             }
         },
-        589: e => {
+        113: e => {
             e.exports = function(e, t) {
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        747: (e, t, n) => {
+        728: (e, t, n) => {
             n.r(t);
-            var r = n(379),
+            var r = n(72),
                 a = n.n(r),
-                o = n(795),
+                o = n(825),
                 s = n.n(o),
-                c = n(569),
+                c = n(659),
                 i = n.n(c),
-                u = n(565),
+                u = n(56),
                 l = n.n(u),
-                p = n(216),
+                p = n(540),
                 d = n.n(p),
-                f = n(589),
+                f = n(113),
                 v = n.n(f),
-                m = n(150),
+                m = n(475),
                 h = {};
-            h.styleTagTransform = v(), h.setAttributes = l(), h.insert = i().bind(null, "head"), h.domAPI = s(), h.insertStyleElement = d(), a()(m.Z, h), m.Z && m.Z.locals && m.Z.locals
+            h.styleTagTransform = v(), h.setAttributes = l(), h.insert = i().bind(null, "head"), h.domAPI = s(), h.insertStyleElement = d(), a()(m.A, h), m.A && m.A.locals && m.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/remoteEntry.46bdb8f3cf2cfa8594cb.js` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/remoteEntry.952aa98dd7822da17116.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t = {
-            974: (e, r, t) => {
+            487: (e, r, t) => {
                 var a = {
-                        "./index": () => t.e(568).then((() => () => t(568))),
-                        "./extension": () => t.e(568).then((() => () => t(568))),
-                        "./style": () => t.e(747).then((() => () => t(747)))
+                        "./index": () => t.e(509).then((() => () => t(509))),
+                        "./extension": () => t.e(509).then((() => () => t(509))),
+                        "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
                             var a = "default",
@@ -43,49 +43,49 @@
         }), r
     }, o.d = (e, r) => {
         for (var t in r) o.o(r, t) && !o.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, o.f = {}, o.e = e => Promise.all(Object.keys(o.f).reduce(((r, t) => (o.f[t](e, r), r)), [])), o.u = e => e + "." + {
-        568: "523b878894628ce0ce6f",
-        747: "9b83aa6cc639b78d65e7"
+        509: "82c83d88a314838bd37c",
+        728: "8dcd6beb31a2181fb758"
     } [e] + ".js?v=" + {
-        568: "523b878894628ce0ce6f",
-        747: "9b83aa6cc639b78d65e7"
+        509: "82c83d88a314838bd37c",
+        728: "8dcd6beb31a2181fb758"
     } [e], o.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), o.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jans-code/jupyterlab_rise_metadata_form:", o.l = (t, a, n, i) => {
         if (e[t]) e[t].push(a);
         else {
-            var d, l;
+            var d, s;
             if (void 0 !== n)
-                for (var s = document.getElementsByTagName("script"), u = 0; u < s.length; u++) {
-                    var f = s[u];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        d = f;
+                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
+                    var c = l[u];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + n) {
+                        d = c;
                         break
                     }
                 }
-            d || (l = !0, (d = document.createElement("script")).charset = "utf-8", d.timeout = 120, o.nc && d.setAttribute("nonce", o.nc), d.setAttribute("data-webpack", r + n), d.src = t), e[t] = [a];
-            var c = (r, a) => {
+            d || (s = !0, (d = document.createElement("script")).charset = "utf-8", d.timeout = 120, o.nc && d.setAttribute("nonce", o.nc), d.setAttribute("data-webpack", r + n), d.src = t), e[t] = [a];
+            var f = (r, a) => {
                     d.onerror = d.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], d.parentNode && d.parentNode.removeChild(d), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(c.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: d
                 }), 12e4);
-            d.onerror = c.bind(null, d.onerror), d.onload = c.bind(null, d.onload), l && document.head.appendChild(d)
+            d.onerror = f.bind(null, d.onerror), d.onload = f.bind(null, d.onload), s && document.head.appendChild(d)
         }
     }, o.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -97,40 +97,40 @@
             a || (a = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
                 if (a.push(n), e[t]) return e[t];
                 o.o(o.S, t) || (o.S[t] = {});
                 var i = o.S[t],
                     d = "@jans-code/jupyterlab_rise_metadata_form",
-                    l = [];
+                    s = [];
                 return "default" === t && ((e, r, t, a) => {
                     var n = i[e] = i[e] || {},
-                        l = n[r];
-                    (!l || !l.loaded && (1 != !l.eager ? a : d > l.from)) && (n[r] = {
-                        get: () => o.e(568).then((() => () => o(568))),
+                        s = n[r];
+                    (!s || !s.loaded && (1 != !s.eager ? a : d > s.from)) && (n[r] = {
+                        get: () => o.e(509).then((() => () => o(509))),
                         from: d,
                         eager: !1
                     })
-                })("@jans-code/jupyterlab_rise_metadata_form", "1.0.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@jans-code/jupyterlab_rise_metadata_form", "1.0.1"), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         o.g.importScripts && (e = o.g.location + "");
         var r = o.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
+                for (var a = t.length - 1; a > -1 && (!e || !/^http(s?):/.test(e));) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), o.p = e
     })(), (() => {
         var e = {
-            679: 0
+            487: 0
         };
         o.f.j = (r, t) => {
             var a = o.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
                 else {
                     var n = new Promise(((t, o) => a = e[r] = [t, o]));
@@ -143,21 +143,21 @@
                                 i = t && t.target && t.target.src;
                             d.message = "Loading chunk " + r + " failed.\n(" + n + ": " + i + ")", d.name = "ChunkLoadError", d.type = n, d.request = i, a[1](d)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var a, n, [i, d, l] = t,
-                    s = 0;
+                var a, n, [i, d, s] = t,
+                    l = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (a in d) o.o(d, a) && (o.m[a] = d[a]);
-                    l && l(o)
+                    s && s(o)
                 }
-                for (r && r(t); s < i.length; s++) n = i[s], o.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); l < i.length; l++) n = i[l], o.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_jans_code_jupyterlab_rise_metadata_form = self.webpackChunk_jans_code_jupyterlab_rise_metadata_form || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), o.nc = void 0;
-    var n = o(974);
+    var n = o(487);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jans-code/jupyterlab_rise_metadata_form"] = n
 })();
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/jupyterlab_rise_metadata_form/labextension/static/third-party-licenses.json` & `jupyterlab_rise_metadata_form-1.0.1/jupyterlab_rise_metadata_form/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.11.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "3.3.4"
         }
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/schema/risemdf.json` & `jupyterlab_rise_metadata_form-1.0.1/schema/risemdf.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999881628787879%*

 * *Differences: {"'jupyter.lab.metadataforms'": "{0: {'metadataSchema': {'properties': {'/rise/controls': "*

 * *                                "{'title': 'Controls'}}}}}"}*

```diff
@@ -133,15 +133,15 @@
                     "/rise/center": {
                         "default": true,
                         "title": "Reveal center",
                         "type": "boolean"
                     },
                     "/rise/controls": {
                         "default": true,
-                        "title": "Autolaunch",
+                        "title": "Controls",
                         "type": "boolean"
                     },
                     "/rise/enable_chalkboard": {
                         "title": "Chalkboard",
                         "type": "boolean"
                     },
                     "/rise/footer": {
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/.gitignore` & `jupyterlab_rise_metadata_form-1.0.1/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 node_modules/
 *.log
 .eslintcache
 .stylelintcache
 *.egg-info/
 .ipynb_checkpoints
 *.tsbuildinfo
-pretty_jupyter_metadata_form/labextension
+jupyterlab_rise_metadata_form/labextension
 # Version file is handled by hatchling
-pretty_jupyter_metadata_form/_version.py
+jupyterlab_rise_metadata_form/_version.py
 
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
@@ -120,7 +120,9 @@
 
 # OSX files
 .DS_Store
 
 # Yarn cache
 .yarn/
 yarn.lock
+
+cleanup
```

### Comparing `jupyterlab_rise_metadata_form-1.0.0/LICENSE` & `jupyterlab_rise_metadata_form-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_rise_metadata_form-1.0.0/pyproject.toml` & `jupyterlab_rise_metadata_form-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_rise_metadata_form-1.0.0/PKG-INFO` & `jupyterlab_rise_metadata_form-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_rise_metadata_form
-Version: 1.0.0
+Version: 1.0.1
+Dynamic: Keywords
 Summary: Jupyterlab rise metadata form extension.
 Project-URL: Homepage, https://github.com/jans-code/jupyterlab_rise_metadata_form
 Project-URL: Bug Tracker, https://github.com/jans-code/jupyterlab_rise_metadata_form/issues
 Project-URL: Repository, https://github.com/jans-code/jupyterlab_rise_metadata_form.git
 Author: Project Jupyter Contributors
 License: BSD-3-Clause License
 License-File: LICENSE
```

