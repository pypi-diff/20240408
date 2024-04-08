# Comparing `tmp/django_js_lib_editor_js-2.29.1.0.tar.gz` & `tmp/django_js_lib_editor_js-2.29.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_js_lib_editor_js-2.29.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_js_lib_editor_js-2.29.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_js_lib_editor_js-2.29.1.0.tar` & `django_js_lib_editor_js-2.29.1.1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0       13 2024-03-11 16:15:36.768484 django_js_lib_editor_js-2.29.1.0/.gitignore
--rw-r--r--   0        0        0    10761 2024-03-11 16:39:16.361938 django_js_lib_editor_js-2.29.1.0/LICENSE
--rw-r--r--   0        0        0      482 2024-03-11 16:42:22.133005 django_js_lib_editor_js-2.29.1.0/README.md
--rw-r--r--   0        0        0      678 2024-03-11 16:26:37.681486 django_js_lib_editor_js-2.29.1.0/fetch.py
--rw-r--r--   0        0        0       87 2024-03-11 16:37:44.861474 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/__init__.py
--rw-r--r--   0        0        0      159 2024-03-11 16:28:14.711959 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/apps.py
--rw-r--r--   0        0        0     7233 2024-03-11 16:27:37.385109 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/checklist.js
--rw-r--r--   0        0        0     3222 2024-03-11 16:27:37.825111 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/code.js
--rw-r--r--   0        0        0     1864 2024-03-11 16:27:38.508448 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/delimiter.js
--rw-r--r--   0        0        0   208234 2024-03-11 16:27:36.705106 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/editorjs.js
--rw-r--r--   0        0        0    11825 2024-03-11 16:27:38.348447 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/embed.js
--rw-r--r--   0        0        0     6993 2024-03-11 16:27:37.118441 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/header.js
--rw-r--r--   0        0        0    29531 2024-03-11 16:27:36.988441 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/image.js
--rw-r--r--   0        0        0     2440 2024-03-11 16:27:38.148446 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/inline-code.js
--rw-r--r--   0        0        0    30466 2024-03-11 16:27:39.051784 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/link.js
--rw-r--r--   0        0        0     6016 2024-03-11 16:27:37.251775 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/list.js
--rw-r--r--   0        0        0     2550 2024-03-11 16:27:39.215118 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/marker.js
--rw-r--r--   0        0        0     3423 2024-03-11 16:27:36.851773 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/paragraph.js
--rw-r--r--   0        0        0     5481 2024-03-11 16:27:37.515110 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/quote.js
--rw-r--r--   0        0        0     3198 2024-03-11 16:27:37.651777 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/raw.js
--rw-r--r--   0        0        0    23954 2024-03-11 16:27:39.371786 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/table.js
--rw-r--r--   0        0        0     3713 2024-03-11 16:27:38.685116 django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/warning.js
--rw-r--r--   0        0        0      346 2024-03-11 16:40:39.937638 django_js_lib_editor_js-2.29.1.0/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 django_js_lib_editor_js-2.29.1.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-03-11 16:15:36.768484 django_js_lib_editor_js-2.29.1.1/.gitignore
+-rw-r--r--   0        0        0    10761 2024-03-11 16:39:16.361938 django_js_lib_editor_js-2.29.1.1/LICENSE
+-rw-r--r--   0        0        0      482 2024-03-11 16:42:22.133005 django_js_lib_editor_js-2.29.1.1/README.md
+-rw-r--r--   0        0        0      678 2024-03-11 16:26:37.681486 django_js_lib_editor_js-2.29.1.1/fetch.py
+-rw-r--r--   0        0        0      609 2024-04-08 15:52:03.681858 django_js_lib_editor_js-2.29.1.1/fetch_3rdparty.py
+-rw-r--r--   0        0        0       87 2024-04-08 15:54:38.948978 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-11 16:28:14.711959 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/apps.py
+-rw-r--r--   0        0        0     7233 2024-04-08 15:53:06.600691 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/checklist.js
+-rw-r--r--   0        0        0     3222 2024-04-08 15:53:08.203995 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/code.js
+-rw-r--r--   0        0        0     1864 2024-04-08 15:53:10.190624 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/delimiter.js
+-rw-r--r--   0        0        0    10151 2024-04-08 15:52:31.038017 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/editorjs-drag-drop.js
+-rw-r--r--   0        0        0     9463 2024-04-08 15:52:39.741189 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/editorjs-text-alignment-blocktune.js
+-rw-r--r--   0        0        0    21451 2024-04-08 15:52:33.584637 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/editorjs-undo.js
+-rw-r--r--   0        0        0   208234 2024-04-08 15:53:03.734078 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/editorjs.js
+-rw-r--r--   0        0        0    11825 2024-04-08 15:53:09.537303 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/embed.js
+-rw-r--r--   0        0        0     6993 2024-04-08 15:53:05.660708 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/header.js
+-rw-r--r--   0        0        0    29531 2024-04-08 15:53:05.234050 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/image.js
+-rw-r--r--   0        0        0     2440 2024-04-08 15:53:08.787317 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/inline-code.js
+-rw-r--r--   0        0        0    30466 2024-04-08 15:53:11.197272 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/link.js
+-rw-r--r--   0        0        0     6016 2024-04-08 15:53:06.157366 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/list.js
+-rw-r--r--   0        0        0     2550 2024-04-08 15:53:11.847260 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/marker.js
+-rw-r--r--   0        0        0     3445 2024-04-08 15:53:04.110737 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/paragraph.js
+-rw-r--r--   0        0        0     5481 2024-04-08 15:53:07.074015 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/quote.js
+-rw-r--r--   0        0        0     3198 2024-04-08 15:53:07.337344 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/raw.js
+-rw-r--r--   0        0        0    23954 2024-04-08 15:53:12.200587 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/table.js
+-rw-r--r--   0        0        0     3713 2024-04-08 15:53:10.563951 django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/warning.js
+-rw-r--r--   0        0        0      346 2024-03-11 16:40:39.937638 django_js_lib_editor_js-2.29.1.1/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 django_js_lib_editor_js-2.29.1.1/PKG-INFO
```

### Comparing `django_js_lib_editor_js-2.29.1.0/LICENSE` & `django_js_lib_editor_js-2.29.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/fetch.py` & `django_js_lib_editor_js-2.29.1.1/fetch.py`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/checklist.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/checklist.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/code.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/code.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/delimiter.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/delimiter.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/editorjs.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/editorjs.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/embed.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/embed.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/header.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/header.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/image.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/image.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/inline-code.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/inline-code.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/link.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/link.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/list.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/list.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/marker.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/marker.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/paragraph.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/paragraph.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,86 +1,94 @@
 /**
  * Skipped minification because the original files appears to be already minified.
- * Original file: /npm/@editorjs/paragraph@2.11.3/dist/paragraph.umd.js
+ * Original file: /npm/@editorjs/paragraph@2.11.4/dist/paragraph.umd.js
  *
  * Do NOT use SRI with dynamically generated files! More information: https://www.jsdelivr.com/using-sri-with-dynamic-files
  */
 (function() {
     "use strict";
     try {
         if (typeof document < "u") {
             var e = document.createElement("style");
             e.appendChild(document.createTextNode(".ce-paragraph{line-height:1.6em;outline:none}.ce-paragraph[data-placeholder]:empty:before{content:attr(data-placeholder);color:#707684;font-weight:400;opacity:0}.codex-editor--empty .ce-block:first-child .ce-paragraph[data-placeholder]:empty:before{opacity:1}.codex-editor--toolbox-opened .ce-block:first-child .ce-paragraph[data-placeholder]:empty:before,.codex-editor--empty .ce-block:first-child .ce-paragraph[data-placeholder]:empty:focus:before{opacity:0}.ce-paragraph p:first-of-type{margin-top:0}.ce-paragraph p:last-of-type{margin-bottom:0}")), document.head.appendChild(e)
         }
     } catch (t) {
         console.error("vite-plugin-css-injected-by-js", t)
     }
 })();
-(function(n, i) {
-    typeof exports == "object" && typeof module < "u" ? module.exports = i() : typeof define == "function" && define.amd ? define(i) : (n = typeof globalThis < "u" ? globalThis : n || self, n.Paragraph = i())
+(function(i, n) {
+    typeof exports == "object" && typeof module < "u" ? module.exports = n() : typeof define == "function" && define.amd ? define(n) : (i = typeof globalThis < "u" ? globalThis : i || self, i.Paragraph = n())
 })(this, function() {
     "use strict";
-    const n = "",
-        i = '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path stroke="currentColor" stroke-linecap="round" stroke-width="2" d="M8 9V7.2C8 7.08954 8.08954 7 8.2 7L12 7M16 9V7.2C16 7.08954 15.9105 7 15.8 7L12 7M12 7L12 17M12 17H10M12 17H14"/></svg>';
+    const i = "",
+        n = '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path stroke="currentColor" stroke-linecap="round" stroke-width="2" d="M8 9V7.2C8 7.08954 8.08954 7 8.2 7L12 7M16 9V7.2C16 7.08954 15.9105 7 15.8 7L12 7M12 7L12 17M12 17H10M12 17H14"/></svg>';
+
+    function s(a) {
+        const e = document.createElement("div");
+        e.innerHTML = a.trim();
+        const t = document.createDocumentFragment();
+        return t.append(...Array.from(e.childNodes)), t
+    }
     /**
      * Base Paragraph Block for the Editor.js.
      * Represents a regular text block
      *
      * @author CodeX (team@codex.so)
      * @copyright CodeX 2018
      * @license The MIT License (MIT)
      */
-    class s {
+    class r {
         static get DEFAULT_PLACEHOLDER() {
             return ""
         }
         constructor({
-            data: t,
-            config: e,
-            api: a,
-            readOnly: r
+            data: e,
+            config: t,
+            api: o,
+            readOnly: d
         }) {
-            this.api = a, this.readOnly = r, this._CSS = {
+            this.api = o, this.readOnly = d, this._CSS = {
                 block: this.api.styles.block,
                 wrapper: "ce-paragraph"
-            }, this.readOnly || (this.onKeyUp = this.onKeyUp.bind(this)), this._placeholder = e.placeholder ? e.placeholder : s.DEFAULT_PLACEHOLDER, this._data = {}, this._element = null, this._preserveBlank = e.preserveBlank !== void 0 ? e.preserveBlank : !1, this.data = t
+            }, this.readOnly || (this.onKeyUp = this.onKeyUp.bind(this)), this._placeholder = t.placeholder ? t.placeholder : r.DEFAULT_PLACEHOLDER, this._data = e ?? {}, this._element = null, this._preserveBlank = t.preserveBlank !== void 0 ? t.preserveBlank : !1
         }
-        onKeyUp(t) {
-            if (t.code !== "Backspace" && t.code !== "Delete") return;
+        onKeyUp(e) {
+            if (e.code !== "Backspace" && e.code !== "Delete") return;
             const {
-                textContent: e
+                textContent: t
             } = this._element;
-            e === "" && (this._element.innerHTML = "")
+            t === "" && (this._element.innerHTML = "")
         }
         drawView() {
-            const t = document.createElement("DIV");
-            return t.classList.add(this._CSS.wrapper, this._CSS.block), t.contentEditable = !1, t.dataset.placeholder = this.api.i18n.t(this._placeholder), this._data.text && (t.innerHTML = this._data.text), this.readOnly || (t.contentEditable = !0, t.addEventListener("keyup", this.onKeyUp)), t
+            const e = document.createElement("DIV");
+            return e.classList.add(this._CSS.wrapper, this._CSS.block), e.contentEditable = !1, e.dataset.placeholder = this.api.i18n.t(this._placeholder), this._data.text && (e.innerHTML = this._data.text), this.readOnly || (e.contentEditable = !0, e.addEventListener("keyup", this.onKeyUp)), e
         }
         render() {
             return this._element = this.drawView(), this._element
         }
-        merge(t) {
-            const e = {
-                text: this.data.text + t.text
-            };
-            this.data = e
+        merge(e) {
+            this._data.text += e.text;
+            const t = s(e.text);
+            this._element.appendChild(t), this._element.normalize()
         }
-        validate(t) {
-            return !(t.text.trim() === "" && !this._preserveBlank)
+        validate(e) {
+            return !(e.text.trim() === "" && !this._preserveBlank)
         }
-        save(t) {
+        save(e) {
             return {
-                text: t.innerHTML
+                text: e.innerHTML
             }
         }
-        onPaste(t) {
-            const e = {
-                text: t.detail.data.innerHTML
+        onPaste(e) {
+            const t = {
+                text: e.detail.data.innerHTML
             };
-            this.data = e
+            this._data = t, window.requestAnimationFrame(() => {
+                this._element.innerHTML = this._data.text || ""
+            })
         }
         static get conversionConfig() {
             return {
                 export: "text",
                 import: "text"
             }
         }
@@ -90,36 +98,21 @@
                     br: !0
                 }
             }
         }
         static get isReadOnlySupported() {
             return !0
         }
-        get data() {
-            if (this._element !== null) {
-                const t = this._element.innerHTML;
-                this._data.text = t
-            }
-            return this._data
-        }
-        set data(t) {
-            this._data = t || {}, this._element !== null && this.hydrate()
-        }
-        hydrate() {
-            window.requestAnimationFrame(() => {
-                this._element.innerHTML = this._data.text || ""
-            })
-        }
         static get pasteConfig() {
             return {
                 tags: ["P"]
             }
         }
         static get toolbox() {
             return {
-                icon: i,
+                icon: n,
                 title: "Text"
             }
         }
     }
-    return s
+    return r
 });
```

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/quote.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/quote.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/raw.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/raw.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/table.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/table.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/js_lib_editor_js/static/editorjs/warning.js` & `django_js_lib_editor_js-2.29.1.1/js_lib_editor_js/static/editorjs/warning.js`

 * *Files identical despite different names*

### Comparing `django_js_lib_editor_js-2.29.1.0/PKG-INFO` & `django_js_lib_editor_js-2.29.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-js-lib-editor-js
-Version: 2.29.1.0
+Version: 2.29.1.1
 Summary: Editor JS Repackaged for Django
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 
 # Editor.JS Repackaged for Django
 
 [Editor.JS](https://editorjs.io/) packaged in a Django reusable app.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-js-lib-editor-js Version: 2.29.1.0 Summary:
+Metadata-Version: 2.1 Name: django-js-lib-editor-js Version: 2.29.1.1 Summary:
 Editor JS Repackaged for Django Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License # Editor.JS
 Repackaged for Django [Editor.JS](https://editorjs.io/) packaged in a Django
 reusable app. ## Installation pip install django-js-lib-editor-js ## Usage 1.
 Add `"js_lib_editor_js"` to your `INSTALLED_APPS` setting like this::
 INSTALLED_APPS = [ ... "js_lib_editor_js", ... ] 2. In your template use: {%
 load static %} ...
```

