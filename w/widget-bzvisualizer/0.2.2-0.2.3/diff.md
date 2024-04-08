# Comparing `tmp/widget_bzvisualizer-0.2.2.tar.gz` & `tmp/widget_bzvisualizer-0.2.3.tar.gz`

## Comparing `widget_bzvisualizer-0.2.2.tar` & `widget_bzvisualizer-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/src/widget_bzvisualizer/__init__.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/src/widget_bzvisualizer/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/src/widget_bzvisualizer/static/widget.css
--rw-r--r--   0        0        0   484228 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/src/widget_bzvisualizer/static/widget.js
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/.gitignore
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/README.md
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/__init__.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/static/widget.css
+-rw-r--r--   0        0        0   484471 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/static/widget.js
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/README.md
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/PKG-INFO
```

### Comparing `widget_bzvisualizer-0.2.2/src/widget_bzvisualizer/utils.py` & `widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/utils.py`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.2/src/widget_bzvisualizer/static/widget.js` & `widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/static/widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
 var ka = "162",
-    Ui = {
+    Di = {
         LEFT: 0,
         MIDDLE: 1,
         RIGHT: 2,
         ROTATE: 0,
         DOLLY: 1,
         PAN: 2
     },
-    Di = {
+    Ui = {
         ROTATE: 0,
         PAN: 1,
         DOLLY_PAN: 2,
         DOLLY_ROTATE: 3
     },
     il = 0,
     Qa = 1,
     rl = 2,
     Lo = 1,
     nl = 2,
     Yt = 3,
     pi = 0,
-    Et = 1,
+    yt = 1,
     qt = 2,
     ci = 0,
     er = 1,
     es = 2,
     ts = 3,
     is = 4,
     al = 5,
-    bi = 100,
+    Ti = 100,
     sl = 101,
     ol = 102,
     rs = 103,
     ns = 104,
     ll = 200,
     cl = 201,
     hl = 202,
@@ -44,95 +44,95 @@
     fl = 208,
     ml = 209,
     gl = 210,
     _l = 211,
     vl = 212,
     xl = 213,
     Ml = 214,
-    El = 0,
-    Sl = 1,
-    yl = 2,
+    yl = 0,
+    El = 1,
+    Sl = 2,
     en = 3,
-    bl = 4,
-    Tl = 5,
+    Tl = 4,
+    bl = 5,
     wl = 6,
     Al = 7,
     Po = 0,
     Rl = 1,
     Cl = 2,
     hi = 0,
     Ll = 1,
     Pl = 2,
-    Ul = 3,
-    Dl = 4,
-    Nl = 5,
-    Il = 6,
+    Dl = 3,
+    Ul = 4,
+    Il = 5,
+    Nl = 6,
     Ol = 7,
-    Uo = 300,
+    Do = 300,
     nr = 301,
     ar = 302,
     fa = 303,
     ma = 304,
-    bn = 306,
+    Tn = 306,
     ga = 1e3,
-    It = 1001,
+    Nt = 1001,
     _a = 1002,
     _t = 1003,
     as = 1004,
     pr = 1005,
     xt = 1006,
-    Un = 1007,
+    Dn = 1007,
     wi = 1008,
     ui = 1009,
     Fl = 1010,
-    Bl = 1011,
+    zl = 1011,
     Va = 1012,
-    Do = 1013,
+    Uo = 1013,
     li = 1014,
     Zt = 1015,
     Mr = 1016,
-    No = 1017,
-    Io = 1018,
+    Io = 1017,
+    No = 1018,
     Ri = 1020,
-    zl = 1021,
+    Bl = 1021,
     Ot = 1023,
-    Gl = 1024,
-    Hl = 1025,
+    Hl = 1024,
+    Gl = 1025,
     Ci = 1026,
     sr = 1027,
     kl = 1028,
     Oo = 1029,
     Vl = 1030,
     Fo = 1031,
-    Bo = 1033,
-    Dn = 33776,
-    Nn = 33777,
-    In = 33778,
+    zo = 1033,
+    Un = 33776,
+    In = 33777,
+    Nn = 33778,
     On = 33779,
     ss = 35840,
     os = 35841,
     ls = 35842,
     cs = 35843,
-    zo = 36196,
+    Bo = 36196,
     hs = 37492,
     us = 37496,
     ds = 37808,
     ps = 37809,
     fs = 37810,
     ms = 37811,
     gs = 37812,
     _s = 37813,
     vs = 37814,
     xs = 37815,
     Ms = 37816,
-    Es = 37817,
-    Ss = 37818,
-    ys = 37819,
-    bs = 37820,
-    Ts = 37821,
+    ys = 37817,
+    Es = 37818,
+    Ss = 37819,
+    Ts = 37820,
+    bs = 37821,
     Fn = 36492,
     ws = 36494,
     As = 36495,
     Wl = 36283,
     Rs = 36284,
     Cs = 36285,
     Ls = 36286,
@@ -140,31 +140,31 @@
     jl = 3201,
     Yl = 0,
     ql = 1,
     oi = "",
     Ft = "srgb",
     fi = "srgb-linear",
     Wa = "display-p3",
-    Tn = "display-p3-linear",
+    bn = "display-p3-linear",
     tn = "linear",
     Ze = "srgb",
     rn = "rec709",
     nn = "p3",
-    Ni = 7680,
+    Ii = 7680,
     Ps = 519,
     Zl = 512,
     Kl = 513,
     Jl = 514,
-    Go = 515,
+    Ho = 515,
     $l = 516,
     Ql = 517,
     ec = 518,
     tc = 519,
-    Us = 35044,
-    Ds = "300 es",
+    Ds = 35044,
+    Us = "300 es",
     va = 1035,
     Kt = 2e3,
     an = 2001,
     Jt = class {
         addEventListener(e, t) {
             this._listeners === void 0 && (this._listeners = {});
             let i = this._listeners;
@@ -191,17 +191,17 @@
                 let i = t.slice(0);
                 for (let n = 0, a = i.length; n < a; n++) i[n].call(this, e);
                 e.target = null
             }
         }
     },
     dt = ["00", "01", "02", "03", "04", "05", "06", "07", "08", "09", "0a", "0b", "0c", "0d", "0e", "0f", "10", "11", "12", "13", "14", "15", "16", "17", "18", "19", "1a", "1b", "1c", "1d", "1e", "1f", "20", "21", "22", "23", "24", "25", "26", "27", "28", "29", "2a", "2b", "2c", "2d", "2e", "2f", "30", "31", "32", "33", "34", "35", "36", "37", "38", "39", "3a", "3b", "3c", "3d", "3e", "3f", "40", "41", "42", "43", "44", "45", "46", "47", "48", "49", "4a", "4b", "4c", "4d", "4e", "4f", "50", "51", "52", "53", "54", "55", "56", "57", "58", "59", "5a", "5b", "5c", "5d", "5e", "5f", "60", "61", "62", "63", "64", "65", "66", "67", "68", "69", "6a", "6b", "6c", "6d", "6e", "6f", "70", "71", "72", "73", "74", "75", "76", "77", "78", "79", "7a", "7b", "7c", "7d", "7e", "7f", "80", "81", "82", "83", "84", "85", "86", "87", "88", "89", "8a", "8b", "8c", "8d", "8e", "8f", "90", "91", "92", "93", "94", "95", "96", "97", "98", "99", "9a", "9b", "9c", "9d", "9e", "9f", "a0", "a1", "a2", "a3", "a4", "a5", "a6", "a7", "a8", "a9", "aa", "ab", "ac", "ad", "ae", "af", "b0", "b1", "b2", "b3", "b4", "b5", "b6", "b7", "b8", "b9", "ba", "bb", "bc", "bd", "be", "bf", "c0", "c1", "c2", "c3", "c4", "c5", "c6", "c7", "c8", "c9", "ca", "cb", "cc", "cd", "ce", "cf", "d0", "d1", "d2", "d3", "d4", "d5", "d6", "d7", "d8", "d9", "da", "db", "dc", "dd", "de", "df", "e0", "e1", "e2", "e3", "e4", "e5", "e6", "e7", "e8", "e9", "ea", "eb", "ec", "ed", "ee", "ef", "f0", "f1", "f2", "f3", "f4", "f5", "f6", "f7", "f8", "f9", "fa", "fb", "fc", "fd", "fe", "ff"],
-    Ns = 1234567,
+    Is = 1234567,
     tr = Math.PI / 180,
-    Er = 180 / Math.PI;
+    yr = 180 / Math.PI;
 
 function hr() {
     let r = Math.random() * 4294967295 | 0,
         e = Math.random() * 4294967295 | 0,
         t = Math.random() * 4294967295 | 0,
         i = Math.random() * 4294967295 | 0;
     return (dt[r & 255] + dt[r >> 8 & 255] + dt[r >> 16 & 255] + dt[r >> 24 & 255] + "-" + dt[e & 255] + dt[e >> 8 & 255] + "-" + dt[e >> 16 & 15 | 64] + dt[e >> 24 & 255] + "-" + dt[t & 63 | 128] + dt[t >> 8 & 255] + "-" + dt[t >> 16 & 255] + dt[t >> 24 & 255] + dt[i & 255] + dt[i >> 8 & 255] + dt[i >> 16 & 255] + dt[i >> 24 & 255]).toLowerCase()
@@ -252,25 +252,25 @@
 }
 
 function hc(r) {
     return r * (.5 - Math.random())
 }
 
 function uc(r) {
-    r !== void 0 && (Ns = r);
-    let e = Ns += 1831565813;
+    r !== void 0 && (Is = r);
+    let e = Is += 1831565813;
     return e = Math.imul(e ^ e >>> 15, e | 1), e ^= e + Math.imul(e ^ e >>> 7, e | 61), ((e ^ e >>> 14) >>> 0) / 4294967296
 }
 
 function dc(r) {
     return r * tr
 }
 
 function pc(r) {
-    return r * Er
+    return r * yr
 }
 
 function xa(r) {
     return (r & r - 1) === 0 && r !== 0
 }
 
 function fc(r) {
@@ -283,37 +283,37 @@
 
 function mc(r, e, t, i, n) {
     let a = Math.cos,
         o = Math.sin,
         s = a(t / 2),
         l = o(t / 2),
         c = a((e + i) / 2),
-        u = o((e + i) / 2),
+        h = o((e + i) / 2),
         p = a((e - i) / 2),
         f = o((e - i) / 2),
         m = a((i - e) / 2),
         _ = o((i - e) / 2);
     switch (n) {
         case "XYX":
-            r.set(s * u, l * p, l * f, s * c);
+            r.set(s * h, l * p, l * f, s * c);
             break;
         case "YZY":
-            r.set(l * f, s * u, l * p, s * c);
+            r.set(l * f, s * h, l * p, s * c);
             break;
         case "ZXZ":
-            r.set(l * p, l * f, s * u, s * c);
+            r.set(l * p, l * f, s * h, s * c);
             break;
         case "XZX":
-            r.set(s * u, l * _, l * m, s * c);
+            r.set(s * h, l * _, l * m, s * c);
             break;
         case "YXY":
-            r.set(l * m, s * u, l * _, s * c);
+            r.set(l * m, s * h, l * _, s * c);
             break;
         case "ZYZ":
-            r.set(l * _, l * m, s * u, s * c);
+            r.set(l * _, l * m, s * h, s * c);
             break;
         default:
             console.warn("THREE.MathUtils: .setQuaternionFromProperEuler() encountered an unknown order: " + n)
     }
 }
 
 function Ki(r, e) {
@@ -355,15 +355,15 @@
             return Math.round(r * 127);
         default:
             throw new Error("Invalid component type.")
     }
 }
 var gc = {
         DEG2RAD: tr,
-        RAD2DEG: Er,
+        RAD2DEG: yr,
         generateUUID: hr,
         clamp: ft,
         euclideanModulo: Xa,
         mapLinear: ic,
         inverseLerp: rc,
         lerp: vr,
         damp: nc,
@@ -379,15 +379,15 @@
         isPowerOfTwo: xa,
         ceilPowerOfTwo: fc,
         floorPowerOfTwo: sn,
         setQuaternionFromProperEuler: mc,
         normalize: mt,
         denormalize: Ki
     },
-    De = class r {
+    Ue = class r {
         constructor(e = 0, t = 0) {
             r.prototype.isVector2 = !0, this.x = e, this.y = t
         }
         get width() {
             return this.x
         }
         set width(e) {
@@ -578,21 +578,21 @@
         }
         random() {
             return this.x = Math.random(), this.y = Math.random(), this
         }*[Symbol.iterator]() {
             yield this.x, yield this.y
         }
     },
-    Be = class r {
+    ze = class r {
         constructor(e, t, i, n, a, o, s, l, c) {
             r.prototype.isMatrix3 = !0, this.elements = [1, 0, 0, 0, 1, 0, 0, 0, 1], e !== void 0 && this.set(e, t, i, n, a, o, s, l, c)
         }
         set(e, t, i, n, a, o, s, l, c) {
-            let u = this.elements;
-            return u[0] = e, u[1] = n, u[2] = s, u[3] = t, u[4] = a, u[5] = l, u[6] = i, u[7] = o, u[8] = c, this
+            let h = this.elements;
+            return h[0] = e, h[1] = n, h[2] = s, h[3] = t, h[4] = a, h[5] = l, h[6] = i, h[7] = o, h[8] = c, this
         }
         identity() {
             return this.set(1, 0, 0, 0, 1, 0, 0, 0, 1), this
         }
         copy(e) {
             let t = this.elements,
                 i = e.elements;
@@ -615,29 +615,29 @@
             let i = e.elements,
                 n = t.elements,
                 a = this.elements,
                 o = i[0],
                 s = i[3],
                 l = i[6],
                 c = i[1],
-                u = i[4],
+                h = i[4],
                 p = i[7],
                 f = i[2],
                 m = i[5],
                 _ = i[8],
                 M = n[0],
                 d = n[3],
-                h = n[6],
-                w = n[1],
+                u = n[6],
+                T = n[1],
                 x = n[4],
-                R = n[7],
-                U = n[2],
-                A = n[5],
-                y = n[8];
-            return a[0] = o * M + s * w + l * U, a[3] = o * d + s * x + l * A, a[6] = o * h + s * R + l * y, a[1] = c * M + u * w + p * U, a[4] = c * d + u * x + p * A, a[7] = c * h + u * R + p * y, a[2] = f * M + m * w + _ * U, a[5] = f * d + m * x + _ * A, a[8] = f * h + m * R + _ * y, this
+                A = n[7],
+                D = n[2],
+                R = n[5],
+                b = n[8];
+            return a[0] = o * M + s * T + l * D, a[3] = o * d + s * x + l * R, a[6] = o * u + s * A + l * b, a[1] = c * M + h * T + p * D, a[4] = c * d + h * x + p * R, a[7] = c * u + h * A + p * b, a[2] = f * M + m * T + _ * D, a[5] = f * d + m * x + _ * R, a[8] = f * u + m * A + _ * b, this
         }
         multiplyScalar(e) {
             let t = this.elements;
             return t[0] *= e, t[3] *= e, t[6] *= e, t[1] *= e, t[4] *= e, t[7] *= e, t[2] *= e, t[5] *= e, t[8] *= e, this
         }
         determinant() {
             let e = this.elements,
@@ -645,35 +645,35 @@
                 i = e[1],
                 n = e[2],
                 a = e[3],
                 o = e[4],
                 s = e[5],
                 l = e[6],
                 c = e[7],
-                u = e[8];
-            return t * o * u - t * s * c - i * a * u + i * s * l + n * a * c - n * o * l
+                h = e[8];
+            return t * o * h - t * s * c - i * a * h + i * s * l + n * a * c - n * o * l
         }
         invert() {
             let e = this.elements,
                 t = e[0],
                 i = e[1],
                 n = e[2],
                 a = e[3],
                 o = e[4],
                 s = e[5],
                 l = e[6],
                 c = e[7],
-                u = e[8],
-                p = u * o - s * c,
-                f = s * l - u * a,
+                h = e[8],
+                p = h * o - s * c,
+                f = s * l - h * a,
                 m = c * a - o * l,
                 _ = t * p + i * f + n * m;
             if (_ === 0) return this.set(0, 0, 0, 0, 0, 0, 0, 0, 0);
             let M = 1 / _;
-            return e[0] = p * M, e[1] = (n * c - u * i) * M, e[2] = (s * i - n * o) * M, e[3] = f * M, e[4] = (u * t - n * l) * M, e[5] = (n * a - s * t) * M, e[6] = m * M, e[7] = (i * l - c * t) * M, e[8] = (o * t - i * a) * M, this
+            return e[0] = p * M, e[1] = (n * c - h * i) * M, e[2] = (s * i - n * o) * M, e[3] = f * M, e[4] = (h * t - n * l) * M, e[5] = (n * a - s * t) * M, e[6] = m * M, e[7] = (i * l - c * t) * M, e[8] = (o * t - i * a) * M, this
         }
         transpose() {
             let e, t = this.elements;
             return e = t[1], t[1] = t[3], t[3] = e, e = t[2], t[2] = t[6], t[6] = e, e = t[5], t[5] = t[7], t[7] = e, this
         }
         getNormalMatrix(e) {
             return this.setFromMatrix4(e).invert().transpose()
@@ -684,21 +684,21 @@
         }
         setUvTransform(e, t, i, n, a, o, s) {
             let l = Math.cos(a),
                 c = Math.sin(a);
             return this.set(i * l, i * c, -i * (l * o + c * s) + o + e, -n * c, n * l, -n * (-c * o + l * s) + s + t, 0, 0, 1), this
         }
         scale(e, t) {
-            return this.premultiply(Bn.makeScale(e, t)), this
+            return this.premultiply(zn.makeScale(e, t)), this
         }
         rotate(e) {
-            return this.premultiply(Bn.makeRotation(-e)), this
+            return this.premultiply(zn.makeRotation(-e)), this
         }
         translate(e, t) {
-            return this.premultiply(Bn.makeTranslation(e, t)), this
+            return this.premultiply(zn.makeTranslation(e, t)), this
         }
         makeTranslation(e, t) {
             return e.isVector2 ? this.set(1, 0, e.x, 0, 1, e.y, 0, 0, 1) : this.set(1, 0, e, 0, 1, t, 0, 0, 1), this
         }
         makeRotation(e) {
             let t = Math.cos(e),
                 i = Math.sin(e);
@@ -722,64 +722,64 @@
             let i = this.elements;
             return e[t] = i[0], e[t + 1] = i[1], e[t + 2] = i[2], e[t + 3] = i[3], e[t + 4] = i[4], e[t + 5] = i[5], e[t + 6] = i[6], e[t + 7] = i[7], e[t + 8] = i[8], e
         }
         clone() {
             return new this.constructor().fromArray(this.elements)
         }
     },
-    Bn = new Be;
+    zn = new ze;
 
-function Ho(r) {
+function Go(r) {
     for (let e = r.length - 1; e >= 0; --e)
         if (r[e] >= 65535) return !0;
     return !1
 }
 
 function on(r) {
     return document.createElementNS("http://www.w3.org/1999/xhtml", r)
 }
 
 function _c() {
     let r = on("canvas");
     return r.style.display = "block", r
 }
-var Is = {};
+var Ns = {};
 
 function vc(r) {
-    r in Is || (Is[r] = !0, console.warn(r))
+    r in Ns || (Ns[r] = !0, console.warn(r))
 }
-var Os = new Be().set(.8224621, .177538, 0, .0331941, .9668058, 0, .0170827, .0723974, .9105199),
-    Fs = new Be().set(1.2249401, -.2249404, 0, -.0420569, 1.0420571, 0, -.0196376, -.0786361, 1.0982735),
+var Os = new ze().set(.8224621, .177538, 0, .0331941, .9668058, 0, .0170827, .0723974, .9105199),
+    Fs = new ze().set(1.2249401, -.2249404, 0, -.0420569, 1.0420571, 0, -.0196376, -.0786361, 1.0982735),
     Ar = {
         [fi]: {
             transfer: tn,
             primaries: rn,
             toReference: r => r,
             fromReference: r => r
         },
         [Ft]: {
             transfer: Ze,
             primaries: rn,
             toReference: r => r.convertSRGBToLinear(),
             fromReference: r => r.convertLinearToSRGB()
         },
-        [Tn]: {
+        [bn]: {
             transfer: tn,
             primaries: nn,
             toReference: r => r.applyMatrix3(Fs),
             fromReference: r => r.applyMatrix3(Os)
         },
         [Wa]: {
             transfer: Ze,
             primaries: nn,
             toReference: r => r.convertSRGBToLinear().applyMatrix3(Fs),
             fromReference: r => r.applyMatrix3(Os).convertLinearToSRGB()
         }
     },
-    xc = new Set([fi, Tn]),
+    xc = new Set([fi, bn]),
     qe = {
         enabled: !0,
         _workingColorSpace: fi,
         get workingColorSpace() {
             return this._workingColorSpace
         },
         set workingColorSpace(r) {
@@ -806,26 +806,26 @@
         }
     };
 
 function ir(r) {
     return r < .04045 ? r * .0773993808 : Math.pow(r * .9478672986 + .0521327014, 2.4)
 }
 
-function zn(r) {
+function Bn(r) {
     return r < .0031308 ? r * 12.92 : 1.055 * Math.pow(r, .41666) - .055
 }
-var Ii, ln = class {
+var Ni, ln = class {
         static getDataURL(e) {
             if (/^data:/i.test(e.src) || typeof HTMLCanvasElement > "u") return e.src;
             let t;
             if (e instanceof HTMLCanvasElement) t = e;
             else {
-                Ii === void 0 && (Ii = on("canvas")), Ii.width = e.width, Ii.height = e.height;
-                let i = Ii.getContext("2d");
-                e instanceof ImageData ? i.putImageData(e, 0, 0) : i.drawImage(e, 0, 0, e.width, e.height), t = Ii
+                Ni === void 0 && (Ni = on("canvas")), Ni.width = e.width, Ni.height = e.height;
+                let i = Ni.getContext("2d");
+                e instanceof ImageData ? i.putImageData(e, 0, 0) : i.drawImage(e, 0, 0, e.width, e.height), t = Ni
             }
             return t.width > 2048 || t.height > 2048 ? (console.warn("THREE.ImageUtils.getDataURL: Image converted to jpg for performance reasons", e), t.toDataURL("image/jpeg", .6)) : t.toDataURL("image/png")
         }
         static sRGBToLinear(e) {
             if (typeof HTMLImageElement < "u" && e instanceof HTMLImageElement || typeof HTMLCanvasElement < "u" && e instanceof HTMLCanvasElement || typeof ImageBitmap < "u" && e instanceof ImageBitmap) {
                 let t = on("canvas");
                 t.width = e.width, t.height = e.height;
@@ -864,36 +864,36 @@
                     url: ""
                 },
                 n = this.data;
             if (n !== null) {
                 let a;
                 if (Array.isArray(n)) {
                     a = [];
-                    for (let o = 0, s = n.length; o < s; o++) n[o].isDataTexture ? a.push(Gn(n[o].image)) : a.push(Gn(n[o]))
-                } else a = Gn(n);
+                    for (let o = 0, s = n.length; o < s; o++) n[o].isDataTexture ? a.push(Hn(n[o].image)) : a.push(Hn(n[o]))
+                } else a = Hn(n);
                 i.url = a
             }
             return t || (e.images[this.uuid] = i), i
         }
     };
 
-function Gn(r) {
+function Hn(r) {
     return typeof HTMLImageElement < "u" && r instanceof HTMLImageElement || typeof HTMLCanvasElement < "u" && r instanceof HTMLCanvasElement || typeof ImageBitmap < "u" && r instanceof ImageBitmap ? ln.getDataURL(r) : r.data ? {
         data: Array.from(r.data),
         width: r.width,
         height: r.height,
         type: r.data.constructor.name
     } : (console.warn("THREE.Texture: Unable to serialize Texture."), {})
 }
-var Ec = 0,
+var yc = 0,
     Pt = class r extends Jt {
-        constructor(e = r.DEFAULT_IMAGE, t = r.DEFAULT_MAPPING, i = It, n = It, a = xt, o = wi, s = Ot, l = ui, c = r.DEFAULT_ANISOTROPY, u = oi) {
+        constructor(e = r.DEFAULT_IMAGE, t = r.DEFAULT_MAPPING, i = Nt, n = Nt, a = xt, o = wi, s = Ot, l = ui, c = r.DEFAULT_ANISOTROPY, h = oi) {
             super(), this.isTexture = !0, Object.defineProperty(this, "id", {
-                value: Ec++
-            }), this.uuid = hr(), this.name = "", this.source = new cn(e), this.mipmaps = [], this.mapping = t, this.channel = 0, this.wrapS = i, this.wrapT = n, this.magFilter = a, this.minFilter = o, this.anisotropy = c, this.format = s, this.internalFormat = null, this.type = l, this.offset = new De(0, 0), this.repeat = new De(1, 1), this.center = new De(0, 0), this.rotation = 0, this.matrixAutoUpdate = !0, this.matrix = new Be, this.generateMipmaps = !0, this.premultiplyAlpha = !1, this.flipY = !0, this.unpackAlignment = 4, this.colorSpace = u, this.userData = {}, this.version = 0, this.onUpdate = null, this.isRenderTargetTexture = !1, this.needsPMREMUpdate = !1
+                value: yc++
+            }), this.uuid = hr(), this.name = "", this.source = new cn(e), this.mipmaps = [], this.mapping = t, this.channel = 0, this.wrapS = i, this.wrapT = n, this.magFilter = a, this.minFilter = o, this.anisotropy = c, this.format = s, this.internalFormat = null, this.type = l, this.offset = new Ue(0, 0), this.repeat = new Ue(1, 1), this.center = new Ue(0, 0), this.rotation = 0, this.matrixAutoUpdate = !0, this.matrix = new ze, this.generateMipmaps = !0, this.premultiplyAlpha = !1, this.flipY = !0, this.unpackAlignment = 4, this.colorSpace = h, this.userData = {}, this.version = 0, this.onUpdate = null, this.isRenderTargetTexture = !1, this.needsPMREMUpdate = !1
         }
         get image() {
             return this.source.data
         }
         set image(e = null) {
             this.source.data = e
         }
@@ -941,45 +941,45 @@
         }
         dispose() {
             this.dispatchEvent({
                 type: "dispose"
             })
         }
         transformUv(e) {
-            if (this.mapping !== Uo) return e;
+            if (this.mapping !== Do) return e;
             if (e.applyMatrix3(this.matrix), e.x < 0 || e.x > 1) switch (this.wrapS) {
                 case ga:
                     e.x = e.x - Math.floor(e.x);
                     break;
-                case It:
+                case Nt:
                     e.x = e.x < 0 ? 0 : 1;
                     break;
                 case _a:
                     Math.abs(Math.floor(e.x) % 2) === 1 ? e.x = Math.ceil(e.x) - e.x : e.x = e.x - Math.floor(e.x);
                     break
             }
             if (e.y < 0 || e.y > 1) switch (this.wrapT) {
                 case ga:
                     e.y = e.y - Math.floor(e.y);
                     break;
-                case It:
+                case Nt:
                     e.y = e.y < 0 ? 0 : 1;
                     break;
                 case _a:
                     Math.abs(Math.floor(e.y) % 2) === 1 ? e.y = Math.ceil(e.y) - e.y : e.y = e.y - Math.floor(e.y);
                     break
             }
             return this.flipY && (e.y = 1 - e.y), e
         }
         set needsUpdate(e) {
             e === !0 && (this.version++, this.source.needsUpdate = !0)
         }
     };
 Pt.DEFAULT_IMAGE = null;
-Pt.DEFAULT_MAPPING = Uo;
+Pt.DEFAULT_MAPPING = Do;
 Pt.DEFAULT_ANISOTROPY = 1;
 var ct = class r {
         constructor(e = 0, t = 0, i = 0, n = 1) {
             r.prototype.isVector4 = !0, this.x = e, this.y = t, this.z = i, this.w = n
         }
         get width() {
             return this.z
@@ -1094,33 +1094,33 @@
             return t < 1e-4 ? (this.x = 1, this.y = 0, this.z = 0) : (this.x = e.x / t, this.y = e.y / t, this.z = e.z / t), this
         }
         setAxisAngleFromRotationMatrix(e) {
             let t, i, n, a, o = e.elements,
                 s = o[0],
                 l = o[4],
                 c = o[8],
-                u = o[1],
+                h = o[1],
                 p = o[5],
                 f = o[9],
                 m = o[2],
                 _ = o[6],
                 M = o[10];
-            if (Math.abs(l - u) < .01 && Math.abs(c - m) < .01 && Math.abs(f - _) < .01) {
-                if (Math.abs(l + u) < .1 && Math.abs(c + m) < .1 && Math.abs(f + _) < .1 && Math.abs(s + p + M - 3) < .1) return this.set(1, 0, 0, 0), this;
+            if (Math.abs(l - h) < .01 && Math.abs(c - m) < .01 && Math.abs(f - _) < .01) {
+                if (Math.abs(l + h) < .1 && Math.abs(c + m) < .1 && Math.abs(f + _) < .1 && Math.abs(s + p + M - 3) < .1) return this.set(1, 0, 0, 0), this;
                 t = Math.PI;
-                let h = (s + 1) / 2,
-                    w = (p + 1) / 2,
+                let u = (s + 1) / 2,
+                    T = (p + 1) / 2,
                     x = (M + 1) / 2,
-                    R = (l + u) / 4,
-                    U = (c + m) / 4,
-                    A = (f + _) / 4;
-                return h > w && h > x ? h < .01 ? (i = 0, n = .707106781, a = .707106781) : (i = Math.sqrt(h), n = R / i, a = U / i) : w > x ? w < .01 ? (i = .707106781, n = 0, a = .707106781) : (n = Math.sqrt(w), i = R / n, a = A / n) : x < .01 ? (i = .707106781, n = .707106781, a = 0) : (a = Math.sqrt(x), i = U / a, n = A / a), this.set(i, n, a, t), this
+                    A = (l + h) / 4,
+                    D = (c + m) / 4,
+                    R = (f + _) / 4;
+                return u > T && u > x ? u < .01 ? (i = 0, n = .707106781, a = .707106781) : (i = Math.sqrt(u), n = A / i, a = D / i) : T > x ? T < .01 ? (i = .707106781, n = 0, a = .707106781) : (n = Math.sqrt(T), i = A / n, a = R / n) : x < .01 ? (i = .707106781, n = .707106781, a = 0) : (a = Math.sqrt(x), i = D / a, n = R / a), this.set(i, n, a, t), this
             }
-            let d = Math.sqrt((_ - f) * (_ - f) + (c - m) * (c - m) + (u - l) * (u - l));
-            return Math.abs(d) < .001 && (d = 1), this.x = (_ - f) / d, this.y = (c - m) / d, this.z = (u - l) / d, this.w = Math.acos((s + p + M - 1) / 2), this
+            let d = Math.sqrt((_ - f) * (_ - f) + (c - m) * (c - m) + (h - l) * (h - l));
+            return Math.abs(d) < .001 && (d = 1), this.x = (_ - f) / d, this.y = (c - m) / d, this.z = (h - l) / d, this.w = Math.acos((s + p + M - 1) / 2), this
         }
         min(e) {
             return this.x = Math.min(this.x, e.x), this.y = Math.min(this.y, e.y), this.z = Math.min(this.z, e.z), this.w = Math.min(this.w, e.w), this
         }
         max(e) {
             return this.x = Math.max(this.x, e.x), this.y = Math.max(this.y, e.y), this.z = Math.max(this.z, e.z), this.w = Math.max(this.w, e.w), this
         }
@@ -1252,76 +1252,76 @@
     hn = class extends Pt {
         constructor(e = null, t = 1, i = 1, n = 1) {
             super(null), this.isDataArrayTexture = !0, this.image = {
                 data: e,
                 width: t,
                 height: i,
                 depth: n
-            }, this.magFilter = _t, this.minFilter = _t, this.wrapR = It, this.generateMipmaps = !1, this.flipY = !1, this.unpackAlignment = 1
+            }, this.magFilter = _t, this.minFilter = _t, this.wrapR = Nt, this.generateMipmaps = !1, this.flipY = !1, this.unpackAlignment = 1
         }
     },
-    Ea = class extends Pt {
+    ya = class extends Pt {
         constructor(e = null, t = 1, i = 1, n = 1) {
             super(null), this.isData3DTexture = !0, this.image = {
                 data: e,
                 width: t,
                 height: i,
                 depth: n
-            }, this.magFilter = _t, this.minFilter = _t, this.wrapR = It, this.generateMipmaps = !1, this.flipY = !1, this.unpackAlignment = 1
+            }, this.magFilter = _t, this.minFilter = _t, this.wrapR = Nt, this.generateMipmaps = !1, this.flipY = !1, this.unpackAlignment = 1
         }
     },
     Qt = class {
         constructor(e = 0, t = 0, i = 0, n = 1) {
             this.isQuaternion = !0, this._x = e, this._y = t, this._z = i, this._w = n
         }
         static slerpFlat(e, t, i, n, a, o, s) {
             let l = i[n + 0],
                 c = i[n + 1],
-                u = i[n + 2],
+                h = i[n + 2],
                 p = i[n + 3],
                 f = a[o + 0],
                 m = a[o + 1],
                 _ = a[o + 2],
                 M = a[o + 3];
             if (s === 0) {
-                e[t + 0] = l, e[t + 1] = c, e[t + 2] = u, e[t + 3] = p;
+                e[t + 0] = l, e[t + 1] = c, e[t + 2] = h, e[t + 3] = p;
                 return
             }
             if (s === 1) {
                 e[t + 0] = f, e[t + 1] = m, e[t + 2] = _, e[t + 3] = M;
                 return
             }
-            if (p !== M || l !== f || c !== m || u !== _) {
+            if (p !== M || l !== f || c !== m || h !== _) {
                 let d = 1 - s,
-                    h = l * f + c * m + u * _ + p * M,
-                    w = h >= 0 ? 1 : -1,
-                    x = 1 - h * h;
+                    u = l * f + c * m + h * _ + p * M,
+                    T = u >= 0 ? 1 : -1,
+                    x = 1 - u * u;
                 if (x > Number.EPSILON) {
-                    let U = Math.sqrt(x),
-                        A = Math.atan2(U, h * w);
-                    d = Math.sin(d * A) / U, s = Math.sin(s * A) / U
+                    let D = Math.sqrt(x),
+                        R = Math.atan2(D, u * T);
+                    d = Math.sin(d * R) / D, s = Math.sin(s * R) / D
                 }
-                let R = s * w;
-                if (l = l * d + f * R, c = c * d + m * R, u = u * d + _ * R, p = p * d + M * R, d === 1 - s) {
-                    let U = 1 / Math.sqrt(l * l + c * c + u * u + p * p);
-                    l *= U, c *= U, u *= U, p *= U
+                let A = s * T;
+                if (l = l * d + f * A, c = c * d + m * A, h = h * d + _ * A, p = p * d + M * A, d === 1 - s) {
+                    let D = 1 / Math.sqrt(l * l + c * c + h * h + p * p);
+                    l *= D, c *= D, h *= D, p *= D
                 }
             }
-            e[t] = l, e[t + 1] = c, e[t + 2] = u, e[t + 3] = p
+            e[t] = l, e[t + 1] = c, e[t + 2] = h, e[t + 3] = p
         }
         static multiplyQuaternionsFlat(e, t, i, n, a, o) {
             let s = i[n],
                 l = i[n + 1],
                 c = i[n + 2],
-                u = i[n + 3],
+                h = i[n + 3],
                 p = a[o],
                 f = a[o + 1],
                 m = a[o + 2],
                 _ = a[o + 3];
-            return e[t] = s * _ + u * p + l * m - c * f, e[t + 1] = l * _ + u * f + c * p - s * m, e[t + 2] = c * _ + u * m + s * f - l * p, e[t + 3] = u * _ - s * p - l * f - c * m, e
+            return e[t] = s * _ + h * p + l * m - c * f, e[t + 1] = l * _ + h * f + c * p - s * m, e[t + 2] = c * _ + h * m + s * f - l * p, e[t + 3] = h * _ - s * p - l * f - c * m, e
         }
         get x() {
             return this._x
         }
         set x(e) {
             this._x = e, this._onChangeCallback()
         }
@@ -1356,37 +1356,37 @@
             let i = e._x,
                 n = e._y,
                 a = e._z,
                 o = e._order,
                 s = Math.cos,
                 l = Math.sin,
                 c = s(i / 2),
-                u = s(n / 2),
+                h = s(n / 2),
                 p = s(a / 2),
                 f = l(i / 2),
                 m = l(n / 2),
                 _ = l(a / 2);
             switch (o) {
                 case "XYZ":
-                    this._x = f * u * p + c * m * _, this._y = c * m * p - f * u * _, this._z = c * u * _ + f * m * p, this._w = c * u * p - f * m * _;
+                    this._x = f * h * p + c * m * _, this._y = c * m * p - f * h * _, this._z = c * h * _ + f * m * p, this._w = c * h * p - f * m * _;
                     break;
                 case "YXZ":
-                    this._x = f * u * p + c * m * _, this._y = c * m * p - f * u * _, this._z = c * u * _ - f * m * p, this._w = c * u * p + f * m * _;
+                    this._x = f * h * p + c * m * _, this._y = c * m * p - f * h * _, this._z = c * h * _ - f * m * p, this._w = c * h * p + f * m * _;
                     break;
                 case "ZXY":
-                    this._x = f * u * p - c * m * _, this._y = c * m * p + f * u * _, this._z = c * u * _ + f * m * p, this._w = c * u * p - f * m * _;
+                    this._x = f * h * p - c * m * _, this._y = c * m * p + f * h * _, this._z = c * h * _ + f * m * p, this._w = c * h * p - f * m * _;
                     break;
                 case "ZYX":
-                    this._x = f * u * p - c * m * _, this._y = c * m * p + f * u * _, this._z = c * u * _ - f * m * p, this._w = c * u * p + f * m * _;
+                    this._x = f * h * p - c * m * _, this._y = c * m * p + f * h * _, this._z = c * h * _ - f * m * p, this._w = c * h * p + f * m * _;
                     break;
                 case "YZX":
-                    this._x = f * u * p + c * m * _, this._y = c * m * p + f * u * _, this._z = c * u * _ - f * m * p, this._w = c * u * p - f * m * _;
+                    this._x = f * h * p + c * m * _, this._y = c * m * p + f * h * _, this._z = c * h * _ - f * m * p, this._w = c * h * p - f * m * _;
                     break;
                 case "XZY":
-                    this._x = f * u * p - c * m * _, this._y = c * m * p - f * u * _, this._z = c * u * _ + f * m * p, this._w = c * u * p + f * m * _;
+                    this._x = f * h * p - c * m * _, this._y = c * m * p - f * h * _, this._z = c * h * _ + f * m * p, this._w = c * h * p + f * m * _;
                     break;
                 default:
                     console.warn("THREE.Quaternion: .setFromEuler() encountered an unknown order: " + o)
             }
             return t === !0 && this._onChangeCallback(), this
         }
         setFromAxisAngle(e, t) {
@@ -1399,29 +1399,29 @@
                 i = t[0],
                 n = t[4],
                 a = t[8],
                 o = t[1],
                 s = t[5],
                 l = t[9],
                 c = t[2],
-                u = t[6],
+                h = t[6],
                 p = t[10],
                 f = i + s + p;
             if (f > 0) {
                 let m = .5 / Math.sqrt(f + 1);
-                this._w = .25 / m, this._x = (u - l) * m, this._y = (a - c) * m, this._z = (o - n) * m
+                this._w = .25 / m, this._x = (h - l) * m, this._y = (a - c) * m, this._z = (o - n) * m
             } else if (i > s && i > p) {
                 let m = 2 * Math.sqrt(1 + i - s - p);
-                this._w = (u - l) / m, this._x = .25 * m, this._y = (n + o) / m, this._z = (a + c) / m
+                this._w = (h - l) / m, this._x = .25 * m, this._y = (n + o) / m, this._z = (a + c) / m
             } else if (s > p) {
                 let m = 2 * Math.sqrt(1 + s - i - p);
-                this._w = (a - c) / m, this._x = (n + o) / m, this._y = .25 * m, this._z = (l + u) / m
+                this._w = (a - c) / m, this._x = (n + o) / m, this._y = .25 * m, this._z = (l + h) / m
             } else {
                 let m = 2 * Math.sqrt(1 + p - i - s);
-                this._w = (o - n) / m, this._x = (a + c) / m, this._y = (l + u) / m, this._z = .25 * m
+                this._w = (o - n) / m, this._x = (a + c) / m, this._y = (l + h) / m, this._z = .25 * m
             }
             return this._onChangeCallback(), this
         }
         setFromUnitVectors(e, t) {
             let i = e.dot(t) + 1;
             return i < Number.EPSILON ? (i = 0, Math.abs(e.x) > Math.abs(e.z) ? (this._x = -e.y, this._y = e.x, this._z = 0, this._w = i) : (this._x = 0, this._y = -e.z, this._z = e.y, this._w = i)) : (this._x = e.y * t.z - e.z * t.y, this._y = e.z * t.x - e.x * t.z, this._z = e.x * t.y - e.y * t.x, this._w = i), this.normalize()
         }
@@ -1466,16 +1466,16 @@
             let i = e._x,
                 n = e._y,
                 a = e._z,
                 o = e._w,
                 s = t._x,
                 l = t._y,
                 c = t._z,
-                u = t._w;
-            return this._x = i * u + o * s + n * c - a * l, this._y = n * u + o * l + a * s - i * c, this._z = a * u + o * c + i * l - n * s, this._w = o * u - i * s - n * l - a * c, this._onChangeCallback(), this
+                h = t._w;
+            return this._x = i * h + o * s + n * c - a * l, this._y = n * h + o * l + a * s - i * c, this._z = a * h + o * c + i * l - n * s, this._w = o * h - i * s - n * l - a * c, this._onChangeCallback(), this
         }
         slerp(e, t) {
             if (t === 0) return this;
             if (t === 1) return this.copy(e);
             let i = this._x,
                 n = this._y,
                 a = this._z,
@@ -1484,17 +1484,17 @@
             if (s < 0 ? (this._w = -e._w, this._x = -e._x, this._y = -e._y, this._z = -e._z, s = -s) : this.copy(e), s >= 1) return this._w = o, this._x = i, this._y = n, this._z = a, this;
             let l = 1 - s * s;
             if (l <= Number.EPSILON) {
                 let m = 1 - t;
                 return this._w = m * o + t * this._w, this._x = m * i + t * this._x, this._y = m * n + t * this._y, this._z = m * a + t * this._z, this.normalize(), this
             }
             let c = Math.sqrt(l),
-                u = Math.atan2(c, s),
-                p = Math.sin((1 - t) * u) / c,
-                f = Math.sin(t * u) / c;
+                h = Math.atan2(c, s),
+                p = Math.sin((1 - t) * h) / c,
+                f = Math.sin(t * h) / c;
             return this._w = o * p + this._w * f, this._x = i * p + this._x * f, this._y = n * p + this._y * f, this._z = a * p + this._z * f, this._onChangeCallback(), this
         }
         slerpQuaternions(e, t, i) {
             return this.copy(e).slerp(t, i)
         }
         random() {
             let e = 2 * Math.PI * Math.random(),
@@ -1522,15 +1522,15 @@
         _onChange(e) {
             return this._onChangeCallback = e, this
         }
         _onChangeCallback() {}*[Symbol.iterator]() {
             yield this._x, yield this._y, yield this._z, yield this._w
         }
     },
-    D = class r {
+    U = class r {
         constructor(e = 0, t = 0, i = 0) {
             r.prototype.isVector3 = !0, this.x = e, this.y = t, this.z = i
         }
         set(e, t, i) {
             return i === void 0 && (i = this.z), this.x = e, this.y = t, this.z = i, this
         }
         setScalar(e) {
@@ -1606,18 +1606,18 @@
         multiplyScalar(e) {
             return this.x *= e, this.y *= e, this.z *= e, this
         }
         multiplyVectors(e, t) {
             return this.x = e.x * t.x, this.y = e.y * t.y, this.z = e.z * t.z, this
         }
         applyEuler(e) {
-            return this.applyQuaternion(Bs.setFromEuler(e))
+            return this.applyQuaternion(zs.setFromEuler(e))
         }
         applyAxisAngle(e, t) {
-            return this.applyQuaternion(Bs.setFromAxisAngle(e, t))
+            return this.applyQuaternion(zs.setFromAxisAngle(e, t))
         }
         applyMatrix3(e) {
             let t = this.x,
                 i = this.y,
                 n = this.z,
                 a = e.elements;
             return this.x = a[0] * t + a[3] * i + a[6] * n, this.y = a[1] * t + a[4] * i + a[7] * n, this.z = a[2] * t + a[5] * i + a[8] * n, this
@@ -1638,17 +1638,17 @@
                 i = this.y,
                 n = this.z,
                 a = e.x,
                 o = e.y,
                 s = e.z,
                 l = e.w,
                 c = 2 * (o * n - s * i),
-                u = 2 * (s * t - a * n),
+                h = 2 * (s * t - a * n),
                 p = 2 * (a * i - o * t);
-            return this.x = t + l * c + o * p - s * u, this.y = i + l * u + s * c - a * p, this.z = n + l * p + a * u - o * c, this
+            return this.x = t + l * c + o * p - s * h, this.y = i + l * h + s * c - a * p, this.z = n + l * p + a * h - o * c, this
         }
         project(e) {
             return this.applyMatrix4(e.matrixWorldInverse).applyMatrix4(e.projectionMatrix)
         }
         unproject(e) {
             return this.applyMatrix4(e.projectionMatrixInverse).applyMatrix4(e.matrixWorld)
         }
@@ -1735,18 +1735,18 @@
         projectOnVector(e) {
             let t = e.lengthSq();
             if (t === 0) return this.set(0, 0, 0);
             let i = e.dot(this) / t;
             return this.copy(e).multiplyScalar(i)
         }
         projectOnPlane(e) {
-            return Hn.copy(this).projectOnVector(e), this.sub(Hn)
+            return Gn.copy(this).projectOnVector(e), this.sub(Gn)
         }
         reflect(e) {
-            return this.sub(Hn.copy(e).multiplyScalar(2 * this.dot(e)))
+            return this.sub(Gn.copy(e).multiplyScalar(2 * this.dot(e)))
         }
         angleTo(e) {
             let t = Math.sqrt(this.lengthSq() * e.lengthSq());
             if (t === 0) return Math.PI / 2;
             let i = this.dot(e) / t;
             return Math.acos(ft(i, -1, 1))
         }
@@ -1817,40 +1817,40 @@
                 t = Math.random() * 2 - 1,
                 i = Math.sqrt(1 - t * t);
             return this.x = i * Math.cos(e), this.y = t, this.z = i * Math.sin(e), this
         }*[Symbol.iterator]() {
             yield this.x, yield this.y, yield this.z
         }
     },
-    Hn = new D,
-    Bs = new Qt,
+    Gn = new U,
+    zs = new Qt,
     Li = class {
-        constructor(e = new D(1 / 0, 1 / 0, 1 / 0), t = new D(-1 / 0, -1 / 0, -1 / 0)) {
+        constructor(e = new U(1 / 0, 1 / 0, 1 / 0), t = new U(-1 / 0, -1 / 0, -1 / 0)) {
             this.isBox3 = !0, this.min = e, this.max = t
         }
         set(e, t) {
             return this.min.copy(e), this.max.copy(t), this
         }
         setFromArray(e) {
             this.makeEmpty();
-            for (let t = 0, i = e.length; t < i; t += 3) this.expandByPoint(Ut.fromArray(e, t));
+            for (let t = 0, i = e.length; t < i; t += 3) this.expandByPoint(Dt.fromArray(e, t));
             return this
         }
         setFromBufferAttribute(e) {
             this.makeEmpty();
-            for (let t = 0, i = e.count; t < i; t++) this.expandByPoint(Ut.fromBufferAttribute(e, t));
+            for (let t = 0, i = e.count; t < i; t++) this.expandByPoint(Dt.fromBufferAttribute(e, t));
             return this
         }
         setFromPoints(e) {
             this.makeEmpty();
             for (let t = 0, i = e.length; t < i; t++) this.expandByPoint(e[t]);
             return this
         }
         setFromCenterAndSize(e, t) {
-            let i = Ut.copy(t).multiplyScalar(.5);
+            let i = Dt.copy(t).multiplyScalar(.5);
             return this.min.copy(e).sub(i), this.max.copy(e).add(i), this
         }
         setFromObject(e, t = !1) {
             return this.makeEmpty(), this.expandByObject(e, t)
         }
         clone() {
             return new this.constructor().copy(this)
@@ -1881,15 +1881,15 @@
         }
         expandByObject(e, t = !1) {
             e.updateWorldMatrix(!1, !1);
             let i = e.geometry;
             if (i !== void 0) {
                 let a = i.getAttribute("position");
                 if (t === !0 && a !== void 0 && e.isInstancedMesh !== !0)
-                    for (let o = 0, s = a.count; o < s; o++) e.isMesh === !0 ? e.getVertexPosition(o, Ut) : Ut.fromBufferAttribute(a, o), Ut.applyMatrix4(e.matrixWorld), this.expandByPoint(Ut);
+                    for (let o = 0, s = a.count; o < s; o++) e.isMesh === !0 ? e.getVertexPosition(o, Dt) : Dt.fromBufferAttribute(a, o), Dt.applyMatrix4(e.matrixWorld), this.expandByPoint(Dt);
                 else e.boundingBox !== void 0 ? (e.boundingBox === null && e.computeBoundingBox(), Rr.copy(e.boundingBox)) : (i.boundingBox === null && i.computeBoundingBox(), Rr.copy(i.boundingBox)), Rr.applyMatrix4(e.matrixWorld), this.union(Rr)
             }
             let n = e.children;
             for (let a = 0, o = n.length; a < o; a++) this.expandByObject(n[a], t);
             return this
         }
         containsPoint(e) {
@@ -1901,34 +1901,34 @@
         getParameter(e, t) {
             return t.set((e.x - this.min.x) / (this.max.x - this.min.x), (e.y - this.min.y) / (this.max.y - this.min.y), (e.z - this.min.z) / (this.max.z - this.min.z))
         }
         intersectsBox(e) {
             return !(e.max.x < this.min.x || e.min.x > this.max.x || e.max.y < this.min.y || e.min.y > this.max.y || e.max.z < this.min.z || e.min.z > this.max.z)
         }
         intersectsSphere(e) {
-            return this.clampPoint(e.center, Ut), Ut.distanceToSquared(e.center) <= e.radius * e.radius
+            return this.clampPoint(e.center, Dt), Dt.distanceToSquared(e.center) <= e.radius * e.radius
         }
         intersectsPlane(e) {
             let t, i;
             return e.normal.x > 0 ? (t = e.normal.x * this.min.x, i = e.normal.x * this.max.x) : (t = e.normal.x * this.max.x, i = e.normal.x * this.min.x), e.normal.y > 0 ? (t += e.normal.y * this.min.y, i += e.normal.y * this.max.y) : (t += e.normal.y * this.max.y, i += e.normal.y * this.min.y), e.normal.z > 0 ? (t += e.normal.z * this.min.z, i += e.normal.z * this.max.z) : (t += e.normal.z * this.max.z, i += e.normal.z * this.min.z), t <= -e.constant && i >= -e.constant
         }
         intersectsTriangle(e) {
             if (this.isEmpty()) return !1;
-            this.getCenter(fr), Cr.subVectors(this.max, fr), Oi.subVectors(e.a, fr), Fi.subVectors(e.b, fr), Bi.subVectors(e.c, fr), ti.subVectors(Fi, Oi), ii.subVectors(Bi, Fi), _i.subVectors(Oi, Bi);
+            this.getCenter(fr), Cr.subVectors(this.max, fr), Oi.subVectors(e.a, fr), Fi.subVectors(e.b, fr), zi.subVectors(e.c, fr), ti.subVectors(Fi, Oi), ii.subVectors(zi, Fi), _i.subVectors(Oi, zi);
             let t = [0, -ti.z, ti.y, 0, -ii.z, ii.y, 0, -_i.z, _i.y, ti.z, 0, -ti.x, ii.z, 0, -ii.x, _i.z, 0, -_i.x, -ti.y, ti.x, 0, -ii.y, ii.x, 0, -_i.y, _i.x, 0];
-            return !kn(t, Oi, Fi, Bi, Cr) || (t = [1, 0, 0, 0, 1, 0, 0, 0, 1], !kn(t, Oi, Fi, Bi, Cr)) ? !1 : (Lr.crossVectors(ti, ii), t = [Lr.x, Lr.y, Lr.z], kn(t, Oi, Fi, Bi, Cr))
+            return !kn(t, Oi, Fi, zi, Cr) || (t = [1, 0, 0, 0, 1, 0, 0, 0, 1], !kn(t, Oi, Fi, zi, Cr)) ? !1 : (Lr.crossVectors(ti, ii), t = [Lr.x, Lr.y, Lr.z], kn(t, Oi, Fi, zi, Cr))
         }
         clampPoint(e, t) {
             return t.copy(e).clamp(this.min, this.max)
         }
         distanceToPoint(e) {
-            return this.clampPoint(e, Ut).distanceTo(e)
+            return this.clampPoint(e, Dt).distanceTo(e)
         }
         getBoundingSphere(e) {
-            return this.isEmpty() ? e.makeEmpty() : (this.getCenter(e.center), e.radius = this.getSize(Ut).length() * .5), e
+            return this.isEmpty() ? e.makeEmpty() : (this.getCenter(e.center), e.radius = this.getSize(Dt).length() * .5), e
         }
         intersect(e) {
             return this.min.max(e.min), this.max.min(e.max), this.isEmpty() && this.makeEmpty(), this
         }
         union(e) {
             return this.min.min(e.min), this.max.max(e.max), this
         }
@@ -1938,52 +1938,52 @@
         translate(e) {
             return this.min.add(e), this.max.add(e), this
         }
         equals(e) {
             return e.min.equals(this.min) && e.max.equals(this.max)
         }
     },
-    kt = [new D, new D, new D, new D, new D, new D, new D, new D],
-    Ut = new D,
+    kt = [new U, new U, new U, new U, new U, new U, new U, new U],
+    Dt = new U,
     Rr = new Li,
-    Oi = new D,
-    Fi = new D,
-    Bi = new D,
-    ti = new D,
-    ii = new D,
-    _i = new D,
-    fr = new D,
-    Cr = new D,
-    Lr = new D,
-    vi = new D;
+    Oi = new U,
+    Fi = new U,
+    zi = new U,
+    ti = new U,
+    ii = new U,
+    _i = new U,
+    fr = new U,
+    Cr = new U,
+    Lr = new U,
+    vi = new U;
 
 function kn(r, e, t, i, n) {
     for (let a = 0, o = r.length - 3; a <= o; a += 3) {
         vi.fromArray(r, a);
         let s = n.x * Math.abs(vi.x) + n.y * Math.abs(vi.y) + n.z * Math.abs(vi.z),
             l = e.dot(vi),
             c = t.dot(vi),
-            u = i.dot(vi);
-        if (Math.max(-Math.max(l, c, u), Math.min(l, c, u)) > s) return !1
+            h = i.dot(vi);
+        if (Math.max(-Math.max(l, c, h), Math.min(l, c, h)) > s) return !1
     }
     return !0
 }
-var Sc = new Li,
-    mr = new D,
-    Vn = new D,
+var Ec = new Li,
+    mr = new U,
+    Vn = new U,
     or = class {
-        constructor(e = new D, t = -1) {
+        constructor(e = new U, t = -1) {
             this.isSphere = !0, this.center = e, this.radius = t
         }
         set(e, t) {
             return this.center.copy(e), this.radius = t, this
         }
         setFromPoints(e, t) {
             let i = this.center;
-            t !== void 0 ? i.copy(t) : Sc.setFromPoints(e).getCenter(i);
+            t !== void 0 ? i.copy(t) : Ec.setFromPoints(e).getCenter(i);
             let n = 0;
             for (let a = 0, o = e.length; a < o; a++) n = Math.max(n, i.distanceToSquared(e[a]));
             return this.radius = Math.sqrt(n), this
         }
         copy(e) {
             return this.center.copy(e.center), this.radius = e.radius, this
         }
@@ -2039,23 +2039,23 @@
         equals(e) {
             return e.center.equals(this.center) && e.radius === this.radius
         }
         clone() {
             return new this.constructor().copy(this)
         }
     },
-    Vt = new D,
-    Wn = new D,
-    Pr = new D,
-    ri = new D,
-    Xn = new D,
-    Ur = new D,
-    jn = new D,
-    Sr = class {
-        constructor(e = new D, t = new D(0, 0, -1)) {
+    Vt = new U,
+    Wn = new U,
+    Pr = new U,
+    ri = new U,
+    Xn = new U,
+    Dr = new U,
+    jn = new U,
+    Er = class {
+        constructor(e = new U, t = new U(0, 0, -1)) {
             this.origin = e, this.direction = t
         }
         set(e, t) {
             return this.origin.copy(e), this.direction.copy(t), this
         }
         copy(e) {
             return this.origin.copy(e.origin), this.direction.copy(e.direction), this
@@ -2084,21 +2084,21 @@
         distanceSqToSegment(e, t, i, n) {
             Wn.copy(e).add(t).multiplyScalar(.5), Pr.copy(t).sub(e).normalize(), ri.copy(this.origin).sub(Wn);
             let a = e.distanceTo(t) * .5,
                 o = -this.direction.dot(Pr),
                 s = ri.dot(this.direction),
                 l = -ri.dot(Pr),
                 c = ri.lengthSq(),
-                u = Math.abs(1 - o * o),
+                h = Math.abs(1 - o * o),
                 p, f, m, _;
-            if (u > 0)
-                if (p = o * l - s, f = o * s - l, _ = a * u, p >= 0)
+            if (h > 0)
+                if (p = o * l - s, f = o * s - l, _ = a * h, p >= 0)
                     if (f >= -_)
                         if (f <= _) {
-                            let M = 1 / u;
+                            let M = 1 / h;
                             p *= M, f *= M, m = p * (p + o * f + 2 * s) + f * (o * p + f + 2 * l) + c
                         } else f = a, p = Math.max(0, -(o * f + s)), m = -p * p + f * (f + 2 * l) + c;
             else f = -a, p = Math.max(0, -(o * f + s)), m = -p * p + f * (f + 2 * l) + c;
             else f <= -_ ? (p = Math.max(0, -(-o * a + s)), f = p > 0 ? -a : Math.min(Math.max(-a, -l), a), m = -p * p + f * (f + 2 * l) + c) : f <= _ ? (p = 0, f = Math.min(Math.max(-a, -l), a), m = f * (f + 2 * l) + c) : (p = Math.max(0, -(o * a + s)), f = p > 0 ? a : Math.min(Math.max(-a, -l), a), m = -p * p + f * (f + 2 * l) + c);
             else f = o > 0 ? -a : a, p = Math.max(0, -(o * f + s)), m = -p * p + f * (f + 2 * l) + c;
             return i && i.copy(this.origin).addScaledVector(this.direction, p), n && n.copy(Wn).addScaledVector(Pr, f), m
         }
@@ -2128,56 +2128,56 @@
         }
         intersectsPlane(e) {
             let t = e.distanceToPoint(this.origin);
             return t === 0 || e.normal.dot(this.direction) * t < 0
         }
         intersectBox(e, t) {
             let i, n, a, o, s, l, c = 1 / this.direction.x,
-                u = 1 / this.direction.y,
+                h = 1 / this.direction.y,
                 p = 1 / this.direction.z,
                 f = this.origin;
-            return c >= 0 ? (i = (e.min.x - f.x) * c, n = (e.max.x - f.x) * c) : (i = (e.max.x - f.x) * c, n = (e.min.x - f.x) * c), u >= 0 ? (a = (e.min.y - f.y) * u, o = (e.max.y - f.y) * u) : (a = (e.max.y - f.y) * u, o = (e.min.y - f.y) * u), i > o || a > n || ((a > i || isNaN(i)) && (i = a), (o < n || isNaN(n)) && (n = o), p >= 0 ? (s = (e.min.z - f.z) * p, l = (e.max.z - f.z) * p) : (s = (e.max.z - f.z) * p, l = (e.min.z - f.z) * p), i > l || s > n) || ((s > i || i !== i) && (i = s), (l < n || n !== n) && (n = l), n < 0) ? null : this.at(i >= 0 ? i : n, t)
+            return c >= 0 ? (i = (e.min.x - f.x) * c, n = (e.max.x - f.x) * c) : (i = (e.max.x - f.x) * c, n = (e.min.x - f.x) * c), h >= 0 ? (a = (e.min.y - f.y) * h, o = (e.max.y - f.y) * h) : (a = (e.max.y - f.y) * h, o = (e.min.y - f.y) * h), i > o || a > n || ((a > i || isNaN(i)) && (i = a), (o < n || isNaN(n)) && (n = o), p >= 0 ? (s = (e.min.z - f.z) * p, l = (e.max.z - f.z) * p) : (s = (e.max.z - f.z) * p, l = (e.min.z - f.z) * p), i > l || s > n) || ((s > i || i !== i) && (i = s), (l < n || n !== n) && (n = l), n < 0) ? null : this.at(i >= 0 ? i : n, t)
         }
         intersectsBox(e) {
             return this.intersectBox(e, Vt) !== null
         }
         intersectTriangle(e, t, i, n, a) {
-            Xn.subVectors(t, e), Ur.subVectors(i, e), jn.crossVectors(Xn, Ur);
+            Xn.subVectors(t, e), Dr.subVectors(i, e), jn.crossVectors(Xn, Dr);
             let o = this.direction.dot(jn),
                 s;
             if (o > 0) {
                 if (n) return null;
                 s = 1
             } else if (o < 0) s = -1, o = -o;
             else return null;
             ri.subVectors(this.origin, e);
-            let l = s * this.direction.dot(Ur.crossVectors(ri, Ur));
+            let l = s * this.direction.dot(Dr.crossVectors(ri, Dr));
             if (l < 0) return null;
             let c = s * this.direction.dot(Xn.cross(ri));
             if (c < 0 || l + c > o) return null;
-            let u = -s * ri.dot(jn);
-            return u < 0 ? null : this.at(u / o, a)
+            let h = -s * ri.dot(jn);
+            return h < 0 ? null : this.at(h / o, a)
         }
         applyMatrix4(e) {
             return this.origin.applyMatrix4(e), this.direction.transformDirection(e), this
         }
         equals(e) {
             return e.origin.equals(this.origin) && e.direction.equals(this.direction)
         }
         clone() {
             return new this.constructor().copy(this)
         }
     },
     at = class r {
-        constructor(e, t, i, n, a, o, s, l, c, u, p, f, m, _, M, d) {
-            r.prototype.isMatrix4 = !0, this.elements = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1], e !== void 0 && this.set(e, t, i, n, a, o, s, l, c, u, p, f, m, _, M, d)
+        constructor(e, t, i, n, a, o, s, l, c, h, p, f, m, _, M, d) {
+            r.prototype.isMatrix4 = !0, this.elements = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1], e !== void 0 && this.set(e, t, i, n, a, o, s, l, c, h, p, f, m, _, M, d)
         }
-        set(e, t, i, n, a, o, s, l, c, u, p, f, m, _, M, d) {
-            let h = this.elements;
-            return h[0] = e, h[4] = t, h[8] = i, h[12] = n, h[1] = a, h[5] = o, h[9] = s, h[13] = l, h[2] = c, h[6] = u, h[10] = p, h[14] = f, h[3] = m, h[7] = _, h[11] = M, h[15] = d, this
+        set(e, t, i, n, a, o, s, l, c, h, p, f, m, _, M, d) {
+            let u = this.elements;
+            return u[0] = e, u[4] = t, u[8] = i, u[12] = n, u[1] = a, u[5] = o, u[9] = s, u[13] = l, u[2] = c, u[6] = h, u[10] = p, u[14] = f, u[3] = m, u[7] = _, u[11] = M, u[15] = d, this
         }
         identity() {
             return this.set(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1), this
         }
         clone() {
             return new r().fromArray(this.elements)
         }
@@ -2200,75 +2200,75 @@
         }
         makeBasis(e, t, i) {
             return this.set(e.x, t.x, i.x, 0, e.y, t.y, i.y, 0, e.z, t.z, i.z, 0, 0, 0, 0, 1), this
         }
         extractRotation(e) {
             let t = this.elements,
                 i = e.elements,
-                n = 1 / zi.setFromMatrixColumn(e, 0).length(),
-                a = 1 / zi.setFromMatrixColumn(e, 1).length(),
-                o = 1 / zi.setFromMatrixColumn(e, 2).length();
+                n = 1 / Bi.setFromMatrixColumn(e, 0).length(),
+                a = 1 / Bi.setFromMatrixColumn(e, 1).length(),
+                o = 1 / Bi.setFromMatrixColumn(e, 2).length();
             return t[0] = i[0] * n, t[1] = i[1] * n, t[2] = i[2] * n, t[3] = 0, t[4] = i[4] * a, t[5] = i[5] * a, t[6] = i[6] * a, t[7] = 0, t[8] = i[8] * o, t[9] = i[9] * o, t[10] = i[10] * o, t[11] = 0, t[12] = 0, t[13] = 0, t[14] = 0, t[15] = 1, this
         }
         makeRotationFromEuler(e) {
             let t = this.elements,
                 i = e.x,
                 n = e.y,
                 a = e.z,
                 o = Math.cos(i),
                 s = Math.sin(i),
                 l = Math.cos(n),
                 c = Math.sin(n),
-                u = Math.cos(a),
+                h = Math.cos(a),
                 p = Math.sin(a);
             if (e.order === "XYZ") {
-                let f = o * u,
+                let f = o * h,
                     m = o * p,
-                    _ = s * u,
+                    _ = s * h,
                     M = s * p;
-                t[0] = l * u, t[4] = -l * p, t[8] = c, t[1] = m + _ * c, t[5] = f - M * c, t[9] = -s * l, t[2] = M - f * c, t[6] = _ + m * c, t[10] = o * l
+                t[0] = l * h, t[4] = -l * p, t[8] = c, t[1] = m + _ * c, t[5] = f - M * c, t[9] = -s * l, t[2] = M - f * c, t[6] = _ + m * c, t[10] = o * l
             } else if (e.order === "YXZ") {
-                let f = l * u,
+                let f = l * h,
                     m = l * p,
-                    _ = c * u,
+                    _ = c * h,
                     M = c * p;
-                t[0] = f + M * s, t[4] = _ * s - m, t[8] = o * c, t[1] = o * p, t[5] = o * u, t[9] = -s, t[2] = m * s - _, t[6] = M + f * s, t[10] = o * l
+                t[0] = f + M * s, t[4] = _ * s - m, t[8] = o * c, t[1] = o * p, t[5] = o * h, t[9] = -s, t[2] = m * s - _, t[6] = M + f * s, t[10] = o * l
             } else if (e.order === "ZXY") {
-                let f = l * u,
+                let f = l * h,
                     m = l * p,
-                    _ = c * u,
+                    _ = c * h,
                     M = c * p;
-                t[0] = f - M * s, t[4] = -o * p, t[8] = _ + m * s, t[1] = m + _ * s, t[5] = o * u, t[9] = M - f * s, t[2] = -o * c, t[6] = s, t[10] = o * l
+                t[0] = f - M * s, t[4] = -o * p, t[8] = _ + m * s, t[1] = m + _ * s, t[5] = o * h, t[9] = M - f * s, t[2] = -o * c, t[6] = s, t[10] = o * l
             } else if (e.order === "ZYX") {
-                let f = o * u,
+                let f = o * h,
                     m = o * p,
-                    _ = s * u,
+                    _ = s * h,
                     M = s * p;
-                t[0] = l * u, t[4] = _ * c - m, t[8] = f * c + M, t[1] = l * p, t[5] = M * c + f, t[9] = m * c - _, t[2] = -c, t[6] = s * l, t[10] = o * l
+                t[0] = l * h, t[4] = _ * c - m, t[8] = f * c + M, t[1] = l * p, t[5] = M * c + f, t[9] = m * c - _, t[2] = -c, t[6] = s * l, t[10] = o * l
             } else if (e.order === "YZX") {
                 let f = o * l,
                     m = o * c,
                     _ = s * l,
                     M = s * c;
-                t[0] = l * u, t[4] = M - f * p, t[8] = _ * p + m, t[1] = p, t[5] = o * u, t[9] = -s * u, t[2] = -c * u, t[6] = m * p + _, t[10] = f - M * p
+                t[0] = l * h, t[4] = M - f * p, t[8] = _ * p + m, t[1] = p, t[5] = o * h, t[9] = -s * h, t[2] = -c * h, t[6] = m * p + _, t[10] = f - M * p
             } else if (e.order === "XZY") {
                 let f = o * l,
                     m = o * c,
                     _ = s * l,
                     M = s * c;
-                t[0] = l * u, t[4] = -p, t[8] = c * u, t[1] = f * p + M, t[5] = o * u, t[9] = m * p - _, t[2] = _ * p - m, t[6] = s * u, t[10] = M * p + f
+                t[0] = l * h, t[4] = -p, t[8] = c * h, t[1] = f * p + M, t[5] = o * h, t[9] = m * p - _, t[2] = _ * p - m, t[6] = s * h, t[10] = M * p + f
             }
             return t[3] = 0, t[7] = 0, t[11] = 0, t[12] = 0, t[13] = 0, t[14] = 0, t[15] = 1, this
         }
         makeRotationFromQuaternion(e) {
-            return this.compose(yc, e, bc)
+            return this.compose(Sc, e, Tc)
         }
         lookAt(e, t, i) {
             let n = this.elements;
-            return bt.subVectors(e, t), bt.lengthSq() === 0 && (bt.z = 1), bt.normalize(), ni.crossVectors(i, bt), ni.lengthSq() === 0 && (Math.abs(i.z) === 1 ? bt.x += 1e-4 : bt.z += 1e-4, bt.normalize(), ni.crossVectors(i, bt)), ni.normalize(), Dr.crossVectors(bt, ni), n[0] = ni.x, n[4] = Dr.x, n[8] = bt.x, n[1] = ni.y, n[5] = Dr.y, n[9] = bt.y, n[2] = ni.z, n[6] = Dr.z, n[10] = bt.z, this
+            return Tt.subVectors(e, t), Tt.lengthSq() === 0 && (Tt.z = 1), Tt.normalize(), ni.crossVectors(i, Tt), ni.lengthSq() === 0 && (Math.abs(i.z) === 1 ? Tt.x += 1e-4 : Tt.z += 1e-4, Tt.normalize(), ni.crossVectors(i, Tt)), ni.normalize(), Ur.crossVectors(Tt, ni), n[0] = ni.x, n[4] = Ur.x, n[8] = Tt.x, n[1] = ni.y, n[5] = Ur.y, n[9] = Tt.y, n[2] = ni.z, n[6] = Ur.z, n[10] = Tt.z, this
         }
         multiply(e) {
             return this.multiplyMatrices(this, e)
         }
         premultiply(e) {
             return this.multiplyMatrices(e, this)
         }
@@ -2276,43 +2276,43 @@
             let i = e.elements,
                 n = t.elements,
                 a = this.elements,
                 o = i[0],
                 s = i[4],
                 l = i[8],
                 c = i[12],
-                u = i[1],
+                h = i[1],
                 p = i[5],
                 f = i[9],
                 m = i[13],
                 _ = i[2],
                 M = i[6],
                 d = i[10],
-                h = i[14],
-                w = i[3],
+                u = i[14],
+                T = i[3],
                 x = i[7],
-                R = i[11],
-                U = i[15],
-                A = n[0],
-                y = n[4],
-                C = n[8],
-                Z = n[12],
+                A = i[11],
+                D = i[15],
+                R = n[0],
+                b = n[4],
+                P = n[8],
+                I = n[12],
                 v = n[1],
-                T = n[5],
-                V = n[9],
+                w = n[5],
+                W = n[9],
                 K = n[13],
-                P = n[2],
-                X = n[6],
+                L = n[2],
+                j = n[6],
                 k = n[10],
-                j = n[14],
+                Y = n[14],
                 q = n[3],
-                W = n[7],
-                te = n[11],
-                ee = n[15];
-            return a[0] = o * A + s * v + l * P + c * q, a[4] = o * y + s * T + l * X + c * W, a[8] = o * C + s * V + l * k + c * te, a[12] = o * Z + s * K + l * j + c * ee, a[1] = u * A + p * v + f * P + m * q, a[5] = u * y + p * T + f * X + m * W, a[9] = u * C + p * V + f * k + m * te, a[13] = u * Z + p * K + f * j + m * ee, a[2] = _ * A + M * v + d * P + h * q, a[6] = _ * y + M * T + d * X + h * W, a[10] = _ * C + M * V + d * k + h * te, a[14] = _ * Z + M * K + d * j + h * ee, a[3] = w * A + x * v + R * P + U * q, a[7] = w * y + x * T + R * X + U * W, a[11] = w * C + x * V + R * k + U * te, a[15] = w * Z + x * K + R * j + U * ee, this
+                Z = n[7],
+                ee = n[11],
+                ie = n[15];
+            return a[0] = o * R + s * v + l * L + c * q, a[4] = o * b + s * w + l * j + c * Z, a[8] = o * P + s * W + l * k + c * ee, a[12] = o * I + s * K + l * Y + c * ie, a[1] = h * R + p * v + f * L + m * q, a[5] = h * b + p * w + f * j + m * Z, a[9] = h * P + p * W + f * k + m * ee, a[13] = h * I + p * K + f * Y + m * ie, a[2] = _ * R + M * v + d * L + u * q, a[6] = _ * b + M * w + d * j + u * Z, a[10] = _ * P + M * W + d * k + u * ee, a[14] = _ * I + M * K + d * Y + u * ie, a[3] = T * R + x * v + A * L + D * q, a[7] = T * b + x * w + A * j + D * Z, a[11] = T * P + x * W + A * k + D * ee, a[15] = T * I + x * K + A * Y + D * ie, this
         }
         multiplyScalar(e) {
             let t = this.elements;
             return t[0] *= e, t[4] *= e, t[8] *= e, t[12] *= e, t[1] *= e, t[5] *= e, t[9] *= e, t[13] *= e, t[2] *= e, t[6] *= e, t[10] *= e, t[14] *= e, t[3] *= e, t[7] *= e, t[11] *= e, t[15] *= e, this
         }
         determinant() {
             let e = this.elements,
@@ -2320,23 +2320,23 @@
                 i = e[4],
                 n = e[8],
                 a = e[12],
                 o = e[1],
                 s = e[5],
                 l = e[9],
                 c = e[13],
-                u = e[2],
+                h = e[2],
                 p = e[6],
                 f = e[10],
                 m = e[14],
                 _ = e[3],
                 M = e[7],
                 d = e[11],
-                h = e[15];
-            return _ * (+a * l * p - n * c * p - a * s * f + i * c * f + n * s * m - i * l * m) + M * (+t * l * m - t * c * f + a * o * f - n * o * m + n * c * u - a * l * u) + d * (+t * c * p - t * s * m - a * o * p + i * o * m + a * s * u - i * c * u) + h * (-n * s * u - t * l * p + t * s * f + n * o * p - i * o * f + i * l * u)
+                u = e[15];
+            return _ * (+a * l * p - n * c * p - a * s * f + i * c * f + n * s * m - i * l * m) + M * (+t * l * m - t * c * f + a * o * f - n * o * m + n * c * h - a * l * h) + d * (+t * c * p - t * s * m - a * o * p + i * o * m + a * s * h - i * c * h) + u * (-n * s * h - t * l * p + t * s * f + n * o * p - i * o * f + i * l * h)
         }
         transpose() {
             let e = this.elements,
                 t;
             return t = e[1], e[1] = e[4], e[4] = t, t = e[2], e[2] = e[8], e[8] = t, t = e[6], e[6] = e[9], e[9] = t, t = e[3], e[3] = e[12], e[12] = t, t = e[7], e[7] = e[13], e[13] = t, t = e[11], e[11] = e[14], e[14] = t, this
         }
         setPosition(e, t, i) {
@@ -2349,30 +2349,30 @@
                 i = e[1],
                 n = e[2],
                 a = e[3],
                 o = e[4],
                 s = e[5],
                 l = e[6],
                 c = e[7],
-                u = e[8],
+                h = e[8],
                 p = e[9],
                 f = e[10],
                 m = e[11],
                 _ = e[12],
                 M = e[13],
                 d = e[14],
-                h = e[15],
-                w = p * d * c - M * f * c + M * l * m - s * d * m - p * l * h + s * f * h,
-                x = _ * f * c - u * d * c - _ * l * m + o * d * m + u * l * h - o * f * h,
-                R = u * M * c - _ * p * c + _ * s * m - o * M * m - u * s * h + o * p * h,
-                U = _ * p * l - u * M * l - _ * s * f + o * M * f + u * s * d - o * p * d,
-                A = t * w + i * x + n * R + a * U;
-            if (A === 0) return this.set(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0);
-            let y = 1 / A;
-            return e[0] = w * y, e[1] = (M * f * a - p * d * a - M * n * m + i * d * m + p * n * h - i * f * h) * y, e[2] = (s * d * a - M * l * a + M * n * c - i * d * c - s * n * h + i * l * h) * y, e[3] = (p * l * a - s * f * a - p * n * c + i * f * c + s * n * m - i * l * m) * y, e[4] = x * y, e[5] = (u * d * a - _ * f * a + _ * n * m - t * d * m - u * n * h + t * f * h) * y, e[6] = (_ * l * a - o * d * a - _ * n * c + t * d * c + o * n * h - t * l * h) * y, e[7] = (o * f * a - u * l * a + u * n * c - t * f * c - o * n * m + t * l * m) * y, e[8] = R * y, e[9] = (_ * p * a - u * M * a - _ * i * m + t * M * m + u * i * h - t * p * h) * y, e[10] = (o * M * a - _ * s * a + _ * i * c - t * M * c - o * i * h + t * s * h) * y, e[11] = (u * s * a - o * p * a - u * i * c + t * p * c + o * i * m - t * s * m) * y, e[12] = U * y, e[13] = (u * M * n - _ * p * n + _ * i * f - t * M * f - u * i * d + t * p * d) * y, e[14] = (_ * s * n - o * M * n - _ * i * l + t * M * l + o * i * d - t * s * d) * y, e[15] = (o * p * n - u * s * n + u * i * l - t * p * l - o * i * f + t * s * f) * y, this
+                u = e[15],
+                T = p * d * c - M * f * c + M * l * m - s * d * m - p * l * u + s * f * u,
+                x = _ * f * c - h * d * c - _ * l * m + o * d * m + h * l * u - o * f * u,
+                A = h * M * c - _ * p * c + _ * s * m - o * M * m - h * s * u + o * p * u,
+                D = _ * p * l - h * M * l - _ * s * f + o * M * f + h * s * d - o * p * d,
+                R = t * T + i * x + n * A + a * D;
+            if (R === 0) return this.set(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0);
+            let b = 1 / R;
+            return e[0] = T * b, e[1] = (M * f * a - p * d * a - M * n * m + i * d * m + p * n * u - i * f * u) * b, e[2] = (s * d * a - M * l * a + M * n * c - i * d * c - s * n * u + i * l * u) * b, e[3] = (p * l * a - s * f * a - p * n * c + i * f * c + s * n * m - i * l * m) * b, e[4] = x * b, e[5] = (h * d * a - _ * f * a + _ * n * m - t * d * m - h * n * u + t * f * u) * b, e[6] = (_ * l * a - o * d * a - _ * n * c + t * d * c + o * n * u - t * l * u) * b, e[7] = (o * f * a - h * l * a + h * n * c - t * f * c - o * n * m + t * l * m) * b, e[8] = A * b, e[9] = (_ * p * a - h * M * a - _ * i * m + t * M * m + h * i * u - t * p * u) * b, e[10] = (o * M * a - _ * s * a + _ * i * c - t * M * c - o * i * u + t * s * u) * b, e[11] = (h * s * a - o * p * a - h * i * c + t * p * c + o * i * m - t * s * m) * b, e[12] = D * b, e[13] = (h * M * n - _ * p * n + _ * i * f - t * M * f - h * i * d + t * p * d) * b, e[14] = (_ * s * n - o * M * n - _ * i * l + t * M * l + o * i * d - t * s * d) * b, e[15] = (o * p * n - h * s * n + h * i * l - t * p * l - o * i * f + t * s * f) * b, this
         }
         scale(e) {
             let t = this.elements,
                 i = e.x,
                 n = e.y,
                 a = e.z;
             return t[0] *= i, t[4] *= n, t[8] *= a, t[1] *= i, t[5] *= n, t[9] *= a, t[2] *= i, t[6] *= n, t[10] *= a, t[3] *= i, t[7] *= n, t[11] *= a, this
@@ -2406,81 +2406,81 @@
             let i = Math.cos(t),
                 n = Math.sin(t),
                 a = 1 - i,
                 o = e.x,
                 s = e.y,
                 l = e.z,
                 c = a * o,
-                u = a * s;
-            return this.set(c * o + i, c * s - n * l, c * l + n * s, 0, c * s + n * l, u * s + i, u * l - n * o, 0, c * l - n * s, u * l + n * o, a * l * l + i, 0, 0, 0, 0, 1), this
+                h = a * s;
+            return this.set(c * o + i, c * s - n * l, c * l + n * s, 0, c * s + n * l, h * s + i, h * l - n * o, 0, c * l - n * s, h * l + n * o, a * l * l + i, 0, 0, 0, 0, 1), this
         }
         makeScale(e, t, i) {
             return this.set(e, 0, 0, 0, 0, t, 0, 0, 0, 0, i, 0, 0, 0, 0, 1), this
         }
         makeShear(e, t, i, n, a, o) {
             return this.set(1, i, a, 0, e, 1, o, 0, t, n, 1, 0, 0, 0, 0, 1), this
         }
         compose(e, t, i) {
             let n = this.elements,
                 a = t._x,
                 o = t._y,
                 s = t._z,
                 l = t._w,
                 c = a + a,
-                u = o + o,
+                h = o + o,
                 p = s + s,
                 f = a * c,
-                m = a * u,
+                m = a * h,
                 _ = a * p,
-                M = o * u,
+                M = o * h,
                 d = o * p,
-                h = s * p,
-                w = l * c,
-                x = l * u,
-                R = l * p,
-                U = i.x,
-                A = i.y,
-                y = i.z;
-            return n[0] = (1 - (M + h)) * U, n[1] = (m + R) * U, n[2] = (_ - x) * U, n[3] = 0, n[4] = (m - R) * A, n[5] = (1 - (f + h)) * A, n[6] = (d + w) * A, n[7] = 0, n[8] = (_ + x) * y, n[9] = (d - w) * y, n[10] = (1 - (f + M)) * y, n[11] = 0, n[12] = e.x, n[13] = e.y, n[14] = e.z, n[15] = 1, this
+                u = s * p,
+                T = l * c,
+                x = l * h,
+                A = l * p,
+                D = i.x,
+                R = i.y,
+                b = i.z;
+            return n[0] = (1 - (M + u)) * D, n[1] = (m + A) * D, n[2] = (_ - x) * D, n[3] = 0, n[4] = (m - A) * R, n[5] = (1 - (f + u)) * R, n[6] = (d + T) * R, n[7] = 0, n[8] = (_ + x) * b, n[9] = (d - T) * b, n[10] = (1 - (f + M)) * b, n[11] = 0, n[12] = e.x, n[13] = e.y, n[14] = e.z, n[15] = 1, this
         }
         decompose(e, t, i) {
             let n = this.elements,
-                a = zi.set(n[0], n[1], n[2]).length(),
-                o = zi.set(n[4], n[5], n[6]).length(),
-                s = zi.set(n[8], n[9], n[10]).length();
-            this.determinant() < 0 && (a = -a), e.x = n[12], e.y = n[13], e.z = n[14], Dt.copy(this);
+                a = Bi.set(n[0], n[1], n[2]).length(),
+                o = Bi.set(n[4], n[5], n[6]).length(),
+                s = Bi.set(n[8], n[9], n[10]).length();
+            this.determinant() < 0 && (a = -a), e.x = n[12], e.y = n[13], e.z = n[14], Ut.copy(this);
             let l = 1 / a,
                 c = 1 / o,
-                u = 1 / s;
-            return Dt.elements[0] *= l, Dt.elements[1] *= l, Dt.elements[2] *= l, Dt.elements[4] *= c, Dt.elements[5] *= c, Dt.elements[6] *= c, Dt.elements[8] *= u, Dt.elements[9] *= u, Dt.elements[10] *= u, t.setFromRotationMatrix(Dt), i.x = a, i.y = o, i.z = s, this
+                h = 1 / s;
+            return Ut.elements[0] *= l, Ut.elements[1] *= l, Ut.elements[2] *= l, Ut.elements[4] *= c, Ut.elements[5] *= c, Ut.elements[6] *= c, Ut.elements[8] *= h, Ut.elements[9] *= h, Ut.elements[10] *= h, t.setFromRotationMatrix(Ut), i.x = a, i.y = o, i.z = s, this
         }
         makePerspective(e, t, i, n, a, o, s = Kt) {
             let l = this.elements,
                 c = 2 * a / (t - e),
-                u = 2 * a / (i - n),
+                h = 2 * a / (i - n),
                 p = (t + e) / (t - e),
                 f = (i + n) / (i - n),
                 m, _;
             if (s === Kt) m = -(o + a) / (o - a), _ = -2 * o * a / (o - a);
             else if (s === an) m = -o / (o - a), _ = -o * a / (o - a);
             else throw new Error("THREE.Matrix4.makePerspective(): Invalid coordinate system: " + s);
-            return l[0] = c, l[4] = 0, l[8] = p, l[12] = 0, l[1] = 0, l[5] = u, l[9] = f, l[13] = 0, l[2] = 0, l[6] = 0, l[10] = m, l[14] = _, l[3] = 0, l[7] = 0, l[11] = -1, l[15] = 0, this
+            return l[0] = c, l[4] = 0, l[8] = p, l[12] = 0, l[1] = 0, l[5] = h, l[9] = f, l[13] = 0, l[2] = 0, l[6] = 0, l[10] = m, l[14] = _, l[3] = 0, l[7] = 0, l[11] = -1, l[15] = 0, this
         }
         makeOrthographic(e, t, i, n, a, o, s = Kt) {
             let l = this.elements,
                 c = 1 / (t - e),
-                u = 1 / (i - n),
+                h = 1 / (i - n),
                 p = 1 / (o - a),
                 f = (t + e) * c,
-                m = (i + n) * u,
+                m = (i + n) * h,
                 _, M;
             if (s === Kt) _ = (o + a) * p, M = -2 * p;
             else if (s === an) _ = a * p, M = -1 * p;
             else throw new Error("THREE.Matrix4.makeOrthographic(): Invalid coordinate system: " + s);
-            return l[0] = 2 * c, l[4] = 0, l[8] = 0, l[12] = -f, l[1] = 0, l[5] = 2 * u, l[9] = 0, l[13] = -m, l[2] = 0, l[6] = 0, l[10] = M, l[14] = -_, l[3] = 0, l[7] = 0, l[11] = 0, l[15] = 1, this
+            return l[0] = 2 * c, l[4] = 0, l[8] = 0, l[12] = -f, l[1] = 0, l[5] = 2 * h, l[9] = 0, l[13] = -m, l[2] = 0, l[6] = 0, l[10] = M, l[14] = -_, l[3] = 0, l[7] = 0, l[11] = 0, l[15] = 1, this
         }
         equals(e) {
             let t = this.elements,
                 i = e.elements;
             for (let n = 0; n < 16; n++)
                 if (t[n] !== i[n]) return !1;
             return !0
@@ -2490,23 +2490,23 @@
             return this
         }
         toArray(e = [], t = 0) {
             let i = this.elements;
             return e[t] = i[0], e[t + 1] = i[1], e[t + 2] = i[2], e[t + 3] = i[3], e[t + 4] = i[4], e[t + 5] = i[5], e[t + 6] = i[6], e[t + 7] = i[7], e[t + 8] = i[8], e[t + 9] = i[9], e[t + 10] = i[10], e[t + 11] = i[11], e[t + 12] = i[12], e[t + 13] = i[13], e[t + 14] = i[14], e[t + 15] = i[15], e
         }
     },
-    zi = new D,
-    Dt = new at,
-    yc = new D(0, 0, 0),
-    bc = new D(1, 1, 1),
-    ni = new D,
-    Dr = new D,
-    bt = new D,
-    zs = new at,
-    Gs = new Qt,
+    Bi = new U,
+    Ut = new at,
+    Sc = new U(0, 0, 0),
+    Tc = new U(1, 1, 1),
+    ni = new U,
+    Ur = new U,
+    Tt = new U,
+    Bs = new at,
+    Hs = new Qt,
     ei = class r {
         constructor(e = 0, t = 0, i = 0, n = r.DEFAULT_ORDER) {
             this.isEuler = !0, this._x = e, this._y = t, this._z = i, this._order = n
         }
         get x() {
             return this._x
         }
@@ -2543,50 +2543,50 @@
         setFromRotationMatrix(e, t = this._order, i = !0) {
             let n = e.elements,
                 a = n[0],
                 o = n[4],
                 s = n[8],
                 l = n[1],
                 c = n[5],
-                u = n[9],
+                h = n[9],
                 p = n[2],
                 f = n[6],
                 m = n[10];
             switch (t) {
                 case "XYZ":
-                    this._y = Math.asin(ft(s, -1, 1)), Math.abs(s) < .9999999 ? (this._x = Math.atan2(-u, m), this._z = Math.atan2(-o, a)) : (this._x = Math.atan2(f, c), this._z = 0);
+                    this._y = Math.asin(ft(s, -1, 1)), Math.abs(s) < .9999999 ? (this._x = Math.atan2(-h, m), this._z = Math.atan2(-o, a)) : (this._x = Math.atan2(f, c), this._z = 0);
                     break;
                 case "YXZ":
-                    this._x = Math.asin(-ft(u, -1, 1)), Math.abs(u) < .9999999 ? (this._y = Math.atan2(s, m), this._z = Math.atan2(l, c)) : (this._y = Math.atan2(-p, a), this._z = 0);
+                    this._x = Math.asin(-ft(h, -1, 1)), Math.abs(h) < .9999999 ? (this._y = Math.atan2(s, m), this._z = Math.atan2(l, c)) : (this._y = Math.atan2(-p, a), this._z = 0);
                     break;
                 case "ZXY":
                     this._x = Math.asin(ft(f, -1, 1)), Math.abs(f) < .9999999 ? (this._y = Math.atan2(-p, m), this._z = Math.atan2(-o, c)) : (this._y = 0, this._z = Math.atan2(l, a));
                     break;
                 case "ZYX":
                     this._y = Math.asin(-ft(p, -1, 1)), Math.abs(p) < .9999999 ? (this._x = Math.atan2(f, m), this._z = Math.atan2(l, a)) : (this._x = 0, this._z = Math.atan2(-o, c));
                     break;
                 case "YZX":
-                    this._z = Math.asin(ft(l, -1, 1)), Math.abs(l) < .9999999 ? (this._x = Math.atan2(-u, c), this._y = Math.atan2(-p, a)) : (this._x = 0, this._y = Math.atan2(s, m));
+                    this._z = Math.asin(ft(l, -1, 1)), Math.abs(l) < .9999999 ? (this._x = Math.atan2(-h, c), this._y = Math.atan2(-p, a)) : (this._x = 0, this._y = Math.atan2(s, m));
                     break;
                 case "XZY":
-                    this._z = Math.asin(-ft(o, -1, 1)), Math.abs(o) < .9999999 ? (this._x = Math.atan2(f, c), this._y = Math.atan2(s, a)) : (this._x = Math.atan2(-u, m), this._y = 0);
+                    this._z = Math.asin(-ft(o, -1, 1)), Math.abs(o) < .9999999 ? (this._x = Math.atan2(f, c), this._y = Math.atan2(s, a)) : (this._x = Math.atan2(-h, m), this._y = 0);
                     break;
                 default:
                     console.warn("THREE.Euler: .setFromRotationMatrix() encountered an unknown order: " + t)
             }
             return this._order = t, i === !0 && this._onChangeCallback(), this
         }
         setFromQuaternion(e, t, i) {
-            return zs.makeRotationFromQuaternion(e), this.setFromRotationMatrix(zs, t, i)
+            return Bs.makeRotationFromQuaternion(e), this.setFromRotationMatrix(Bs, t, i)
         }
         setFromVector3(e, t = this._order) {
             return this.set(e.x, e.y, e.z, t)
         }
         reorder(e) {
-            return Gs.setFromEuler(this), this.setFromQuaternion(Gs, e)
+            return Hs.setFromEuler(this), this.setFromQuaternion(Hs, e)
         }
         equals(e) {
             return e._x === this._x && e._y === this._y && e._z === this._z && e._order === this._order
         }
         fromArray(e) {
             return this._x = e[0], this._y = e[1], this._z = e[2], e[3] !== void 0 && (this._order = e[3]), this._onChangeCallback(), this
         }
@@ -2626,25 +2626,25 @@
         test(e) {
             return (this.mask & e.mask) !== 0
         }
         isEnabled(e) {
             return (this.mask & (1 << e | 0)) !== 0
         }
     },
-    Tc = 0,
-    Hs = new D,
-    Gi = new Qt,
+    bc = 0,
+    Gs = new U,
+    Hi = new Qt,
     Wt = new at,
-    Nr = new D,
-    gr = new D,
-    wc = new D,
+    Ir = new U,
+    gr = new U,
+    wc = new U,
     Ac = new Qt,
-    ks = new D(1, 0, 0),
-    Vs = new D(0, 1, 0),
-    Ws = new D(0, 0, 1),
+    ks = new U(1, 0, 0),
+    Vs = new U(0, 1, 0),
+    Ws = new U(0, 0, 1),
     Rc = {
         type: "added"
     },
     Cc = {
         type: "removed"
     },
     Yn = {
@@ -2654,20 +2654,20 @@
     qn = {
         type: "childremoved",
         child: null
     },
     wt = class r extends Jt {
         constructor() {
             super(), this.isObject3D = !0, Object.defineProperty(this, "id", {
-                value: Tc++
+                value: bc++
             }), this.uuid = hr(), this.name = "", this.type = "Object3D", this.parent = null, this.children = [], this.up = r.DEFAULT_UP.clone();
-            let e = new D,
+            let e = new U,
                 t = new ei,
                 i = new Qt,
-                n = new D(1, 1, 1);
+                n = new U(1, 1, 1);
 
             function a() {
                 i.setFromEuler(t, !1)
             }
 
             function o() {
                 t.setFromQuaternion(i, void 0, !1)
@@ -2693,15 +2693,15 @@
                     enumerable: !0,
                     value: n
                 },
                 modelViewMatrix: {
                     value: new at
                 },
                 normalMatrix: {
-                    value: new Be
+                    value: new ze
                 }
             }), this.matrix = new at, this.matrixWorld = new at, this.matrixAutoUpdate = r.DEFAULT_MATRIX_AUTO_UPDATE, this.matrixWorldAutoUpdate = r.DEFAULT_MATRIX_WORLD_AUTO_UPDATE, this.matrixWorldNeedsUpdate = !1, this.layers = new un, this.visible = !0, this.castShadow = !1, this.receiveShadow = !1, this.frustumCulled = !0, this.renderOrder = 0, this.animations = [], this.userData = {}
         }
         onBeforeShadow() {}
         onAfterShadow() {}
         onBeforeRender() {}
         onAfterRender() {}
@@ -2720,30 +2720,30 @@
         setRotationFromMatrix(e) {
             this.quaternion.setFromRotationMatrix(e)
         }
         setRotationFromQuaternion(e) {
             this.quaternion.copy(e)
         }
         rotateOnAxis(e, t) {
-            return Gi.setFromAxisAngle(e, t), this.quaternion.multiply(Gi), this
+            return Hi.setFromAxisAngle(e, t), this.quaternion.multiply(Hi), this
         }
         rotateOnWorldAxis(e, t) {
-            return Gi.setFromAxisAngle(e, t), this.quaternion.premultiply(Gi), this
+            return Hi.setFromAxisAngle(e, t), this.quaternion.premultiply(Hi), this
         }
         rotateX(e) {
             return this.rotateOnAxis(ks, e)
         }
         rotateY(e) {
             return this.rotateOnAxis(Vs, e)
         }
         rotateZ(e) {
             return this.rotateOnAxis(Ws, e)
         }
         translateOnAxis(e, t) {
-            return Hs.copy(e).applyQuaternion(this.quaternion), this.position.add(Hs.multiplyScalar(t)), this
+            return Gs.copy(e).applyQuaternion(this.quaternion), this.position.add(Gs.multiplyScalar(t)), this
         }
         translateX(e) {
             return this.translateOnAxis(ks, e)
         }
         translateY(e) {
             return this.translateOnAxis(Vs, e)
         }
@@ -2753,17 +2753,17 @@
         localToWorld(e) {
             return this.updateWorldMatrix(!0, !1), e.applyMatrix4(this.matrixWorld)
         }
         worldToLocal(e) {
             return this.updateWorldMatrix(!0, !1), e.applyMatrix4(Wt.copy(this.matrixWorld).invert())
         }
         lookAt(e, t, i) {
-            e.isVector3 ? Nr.copy(e) : Nr.set(e, t, i);
+            e.isVector3 ? Ir.copy(e) : Ir.set(e, t, i);
             let n = this.parent;
-            this.updateWorldMatrix(!0, !1), gr.setFromMatrixPosition(this.matrixWorld), this.isCamera || this.isLight ? Wt.lookAt(gr, Nr, this.up) : Wt.lookAt(Nr, gr, this.up), this.quaternion.setFromRotationMatrix(Wt), n && (Wt.extractRotation(n.matrixWorld), Gi.setFromRotationMatrix(Wt), this.quaternion.premultiply(Gi.invert()))
+            this.updateWorldMatrix(!0, !1), gr.setFromMatrixPosition(this.matrixWorld), this.isCamera || this.isLight ? Wt.lookAt(gr, Ir, this.up) : Wt.lookAt(Ir, gr, this.up), this.quaternion.setFromRotationMatrix(Wt), n && (Wt.extractRotation(n.matrixWorld), Hi.setFromRotationMatrix(Wt), this.quaternion.premultiply(Hi.invert()))
         }
         add(e) {
             if (arguments.length > 1) {
                 for (let t = 0; t < arguments.length; t++) this.add(arguments[t]);
                 return this
             }
             return e === this ? (console.error("THREE.Object3D.add: object can't be added as a child of itself.", e), this) : (e && e.isObject3D ? (e.parent !== null && e.parent.remove(e), e.parent = this, this.children.push(e), e.dispatchEvent(Rc), Yn.child = e, this.dispatchEvent(Yn), Yn.child = null) : console.error("THREE.Object3D.add: object not an instance of THREE.Object3D.", e), this)
@@ -2895,15 +2895,15 @@
             if (this.isScene) this.background && (this.background.isColor ? n.background = this.background.toJSON() : this.background.isTexture && (n.background = this.background.toJSON(e).uuid)), this.environment && this.environment.isTexture && this.environment.isRenderTargetTexture !== !0 && (n.environment = this.environment.toJSON(e).uuid);
             else if (this.isMesh || this.isLine || this.isPoints) {
                 n.geometry = a(e.geometries, this.geometry);
                 let s = this.geometry.parameters;
                 if (s !== void 0 && s.shapes !== void 0) {
                     let l = s.shapes;
                     if (Array.isArray(l))
-                        for (let c = 0, u = l.length; c < u; c++) {
+                        for (let c = 0, h = l.length; c < h; c++) {
                             let p = l[c];
                             a(e.shapes, p)
                         } else a(e.shapes, l)
                 }
             }
             if (this.isSkinnedMesh && (n.bindMode = this.bindMode, n.bindMatrix = this.bindMatrix.toArray(), this.skeleton !== void 0 && (a(e.skeletons, this.skeleton), n.skeleton = this.skeleton.uuid)), this.material !== void 0)
                 if (Array.isArray(this.material)) {
@@ -2922,28 +2922,28 @@
                     n.animations.push(a(e.animations, l))
                 }
             }
             if (t) {
                 let s = o(e.geometries),
                     l = o(e.materials),
                     c = o(e.textures),
-                    u = o(e.images),
+                    h = o(e.images),
                     p = o(e.shapes),
                     f = o(e.skeletons),
                     m = o(e.animations),
                     _ = o(e.nodes);
-                s.length > 0 && (i.geometries = s), l.length > 0 && (i.materials = l), c.length > 0 && (i.textures = c), u.length > 0 && (i.images = u), p.length > 0 && (i.shapes = p), f.length > 0 && (i.skeletons = f), m.length > 0 && (i.animations = m), _.length > 0 && (i.nodes = _)
+                s.length > 0 && (i.geometries = s), l.length > 0 && (i.materials = l), c.length > 0 && (i.textures = c), h.length > 0 && (i.images = h), p.length > 0 && (i.shapes = p), f.length > 0 && (i.skeletons = f), m.length > 0 && (i.animations = m), _.length > 0 && (i.nodes = _)
             }
             return i.object = n, i;
 
             function o(s) {
                 let l = [];
                 for (let c in s) {
-                    let u = s[c];
-                    delete u.metadata, l.push(u)
+                    let h = s[c];
+                    delete h.metadata, l.push(h)
                 }
                 return l
             }
         }
         clone(e) {
             return new this.constructor().copy(this, e)
         }
@@ -2952,58 +2952,58 @@
                 for (let i = 0; i < e.children.length; i++) {
                     let n = e.children[i];
                     this.add(n.clone())
                 }
             return this
         }
     };
-wt.DEFAULT_UP = new D(0, 1, 0);
+wt.DEFAULT_UP = new U(0, 1, 0);
 wt.DEFAULT_MATRIX_AUTO_UPDATE = !0;
 wt.DEFAULT_MATRIX_WORLD_AUTO_UPDATE = !0;
-var Nt = new D,
-    Xt = new D,
-    Zn = new D,
-    jt = new D,
-    Hi = new D,
-    ki = new D,
-    Xs = new D,
-    Kn = new D,
-    Jn = new D,
-    $n = new D,
+var It = new U,
+    Xt = new U,
+    Zn = new U,
+    jt = new U,
+    Gi = new U,
+    ki = new U,
+    Xs = new U,
+    Kn = new U,
+    Jn = new U,
+    $n = new U,
     Ai = class r {
-        constructor(e = new D, t = new D, i = new D) {
+        constructor(e = new U, t = new U, i = new U) {
             this.a = e, this.b = t, this.c = i
         }
         static getNormal(e, t, i, n) {
-            n.subVectors(i, t), Nt.subVectors(e, t), n.cross(Nt);
+            n.subVectors(i, t), It.subVectors(e, t), n.cross(It);
             let a = n.lengthSq();
             return a > 0 ? n.multiplyScalar(1 / Math.sqrt(a)) : n.set(0, 0, 0)
         }
         static getBarycoord(e, t, i, n, a) {
-            Nt.subVectors(n, t), Xt.subVectors(i, t), Zn.subVectors(e, t);
-            let o = Nt.dot(Nt),
-                s = Nt.dot(Xt),
-                l = Nt.dot(Zn),
+            It.subVectors(n, t), Xt.subVectors(i, t), Zn.subVectors(e, t);
+            let o = It.dot(It),
+                s = It.dot(Xt),
+                l = It.dot(Zn),
                 c = Xt.dot(Xt),
-                u = Xt.dot(Zn),
+                h = Xt.dot(Zn),
                 p = o * c - s * s;
             if (p === 0) return a.set(0, 0, 0), null;
             let f = 1 / p,
-                m = (c * l - s * u) * f,
-                _ = (o * u - s * l) * f;
+                m = (c * l - s * h) * f,
+                _ = (o * h - s * l) * f;
             return a.set(1 - m - _, _, m)
         }
         static containsPoint(e, t, i, n) {
             return this.getBarycoord(e, t, i, n, jt) === null ? !1 : jt.x >= 0 && jt.y >= 0 && jt.x + jt.y <= 1
         }
         static getInterpolation(e, t, i, n, a, o, s, l) {
             return this.getBarycoord(e, t, i, n, jt) === null ? (l.x = 0, l.y = 0, "z" in l && (l.z = 0), "w" in l && (l.w = 0), null) : (l.setScalar(0), l.addScaledVector(a, jt.x), l.addScaledVector(o, jt.y), l.addScaledVector(s, jt.z), l)
         }
         static isFrontFacing(e, t, i, n) {
-            return Nt.subVectors(i, t), Xt.subVectors(e, t), Nt.cross(Xt).dot(n) < 0
+            return It.subVectors(i, t), Xt.subVectors(e, t), It.cross(Xt).dot(n) < 0
         }
         set(e, t, i) {
             return this.a.copy(e), this.b.copy(t), this.c.copy(i), this
         }
         setFromPointsAndIndices(e, t, i, n) {
             return this.a.copy(e[t]), this.b.copy(e[i]), this.c.copy(e[n]), this
         }
@@ -3013,15 +3013,15 @@
         clone() {
             return new this.constructor().copy(this)
         }
         copy(e) {
             return this.a.copy(e.a), this.b.copy(e.b), this.c.copy(e.c), this
         }
         getArea() {
-            return Nt.subVectors(this.c, this.b), Xt.subVectors(this.a, this.b), Nt.cross(Xt).length() * .5
+            return It.subVectors(this.c, this.b), Xt.subVectors(this.a, this.b), It.cross(Xt).length() * .5
         }
         getMidpoint(e) {
             return e.addVectors(this.a, this.b).add(this.c).multiplyScalar(1 / 3)
         }
         getNormal(e) {
             return r.getNormal(this.a, this.b, this.c, e)
         }
@@ -3044,34 +3044,34 @@
             return e.intersectsTriangle(this)
         }
         closestPointToPoint(e, t) {
             let i = this.a,
                 n = this.b,
                 a = this.c,
                 o, s;
-            Hi.subVectors(n, i), ki.subVectors(a, i), Kn.subVectors(e, i);
-            let l = Hi.dot(Kn),
+            Gi.subVectors(n, i), ki.subVectors(a, i), Kn.subVectors(e, i);
+            let l = Gi.dot(Kn),
                 c = ki.dot(Kn);
             if (l <= 0 && c <= 0) return t.copy(i);
             Jn.subVectors(e, n);
-            let u = Hi.dot(Jn),
+            let h = Gi.dot(Jn),
                 p = ki.dot(Jn);
-            if (u >= 0 && p <= u) return t.copy(n);
-            let f = l * p - u * c;
-            if (f <= 0 && l >= 0 && u <= 0) return o = l / (l - u), t.copy(i).addScaledVector(Hi, o);
+            if (h >= 0 && p <= h) return t.copy(n);
+            let f = l * p - h * c;
+            if (f <= 0 && l >= 0 && h <= 0) return o = l / (l - h), t.copy(i).addScaledVector(Gi, o);
             $n.subVectors(e, a);
-            let m = Hi.dot($n),
+            let m = Gi.dot($n),
                 _ = ki.dot($n);
             if (_ >= 0 && m <= _) return t.copy(a);
             let M = m * c - l * _;
             if (M <= 0 && c >= 0 && _ <= 0) return s = c / (c - _), t.copy(i).addScaledVector(ki, s);
-            let d = u * _ - m * p;
-            if (d <= 0 && p - u >= 0 && m - _ >= 0) return Xs.subVectors(a, n), s = (p - u) / (p - u + (m - _)), t.copy(n).addScaledVector(Xs, s);
-            let h = 1 / (d + M + f);
-            return o = M * h, s = f * h, t.copy(i).addScaledVector(Hi, o).addScaledVector(ki, s)
+            let d = h * _ - m * p;
+            if (d <= 0 && p - h >= 0 && m - _ >= 0) return Xs.subVectors(a, n), s = (p - h) / (p - h + (m - _)), t.copy(n).addScaledVector(Xs, s);
+            let u = 1 / (d + M + f);
+            return o = M * u, s = f * u, t.copy(i).addScaledVector(Gi, o).addScaledVector(ki, s)
         }
         equals(e) {
             return e.a.equals(this.a) && e.b.equals(this.b) && e.c.equals(this.c)
         }
     },
     ko = {
         aliceblue: 15792383,
@@ -3224,15 +3224,15 @@
         yellowgreen: 10145074
     },
     ai = {
         h: 0,
         s: 0,
         l: 0
     },
-    Ir = {
+    Nr = {
         h: 0,
         s: 0,
         l: 0
     };
 
 function Qn(r, e, t) {
     return t < 0 && (t += 1), t > 1 && (t -= 1), t < 1 / 6 ? r + (e - r) * 6 * t : t < 1 / 2 ? e : t < 2 / 3 ? r + (e - r) * 6 * (2 / 3 - t) : r
@@ -3306,15 +3306,15 @@
         copy(e) {
             return this.r = e.r, this.g = e.g, this.b = e.b, this
         }
         copySRGBToLinear(e) {
             return this.r = ir(e.r), this.g = ir(e.g), this.b = ir(e.b), this
         }
         copyLinearToSRGB(e) {
-            return this.r = zn(e.r), this.g = zn(e.g), this.b = zn(e.b), this
+            return this.r = Bn(e.r), this.g = Bn(e.g), this.b = Bn(e.b), this
         }
         convertSRGBToLinear() {
             return this.copySRGBToLinear(this), this
         }
         convertLinearToSRGB() {
             return this.copyLinearToSRGB(this), this
         }
@@ -3327,32 +3327,32 @@
         getHSL(e, t = qe.workingColorSpace) {
             qe.fromWorkingColorSpace(pt.copy(this), t);
             let i = pt.r,
                 n = pt.g,
                 a = pt.b,
                 o = Math.max(i, n, a),
                 s = Math.min(i, n, a),
-                l, c, u = (s + o) / 2;
+                l, c, h = (s + o) / 2;
             if (s === o) l = 0, c = 0;
             else {
                 let p = o - s;
-                switch (c = u <= .5 ? p / (o + s) : p / (2 - o - s), o) {
+                switch (c = h <= .5 ? p / (o + s) : p / (2 - o - s), o) {
                     case i:
                         l = (n - a) / p + (n < a ? 6 : 0);
                         break;
                     case n:
                         l = (a - i) / p + 2;
                         break;
                     case a:
                         l = (i - n) / p + 4;
                         break
                 }
                 l /= 6
             }
-            return e.h = l, e.s = c, e.l = u, e
+            return e.h = l, e.s = c, e.l = h, e
         }
         getRGB(e, t = qe.workingColorSpace) {
             return qe.fromWorkingColorSpace(pt.copy(this), t), e.r = pt.r, e.g = pt.g, e.b = pt.b, e
         }
         getStyle(e = Ft) {
             qe.fromWorkingColorSpace(pt.copy(this), e);
             let t = pt.r,
@@ -3384,18 +3384,18 @@
         lerp(e, t) {
             return this.r += (e.r - this.r) * t, this.g += (e.g - this.g) * t, this.b += (e.b - this.b) * t, this
         }
         lerpColors(e, t, i) {
             return this.r = e.r + (t.r - e.r) * i, this.g = e.g + (t.g - e.g) * i, this.b = e.b + (t.b - e.b) * i, this
         }
         lerpHSL(e, t) {
-            this.getHSL(ai), e.getHSL(Ir);
-            let i = vr(ai.h, Ir.h, t),
-                n = vr(ai.s, Ir.s, t),
-                a = vr(ai.l, Ir.l, t);
+            this.getHSL(ai), e.getHSL(Nr);
+            let i = vr(ai.h, Nr.h, t),
+                n = vr(ai.s, Nr.s, t),
+                a = vr(ai.l, Nr.l, t);
             return this.setHSL(i, n, a), this
         }
         setFromVector3(e) {
             return this.r = e.x, this.g = e.y, this.b = e.z, this
         }
         applyMatrix3(e) {
             let t = this.r,
@@ -3425,15 +3425,15 @@
     pt = new Ye;
 Ye.NAMES = ko;
 var Lc = 0,
     Pi = class extends Jt {
         constructor() {
             super(), this.isMaterial = !0, Object.defineProperty(this, "id", {
                 value: Lc++
-            }), this.uuid = hr(), this.name = "", this.type = "Material", this.blending = er, this.side = pi, this.vertexColors = !1, this.opacity = 1, this.transparent = !1, this.alphaHash = !1, this.blendSrc = da, this.blendDst = pa, this.blendEquation = bi, this.blendSrcAlpha = null, this.blendDstAlpha = null, this.blendEquationAlpha = null, this.blendColor = new Ye(0, 0, 0), this.blendAlpha = 0, this.depthFunc = en, this.depthTest = !0, this.depthWrite = !0, this.stencilWriteMask = 255, this.stencilFunc = Ps, this.stencilRef = 0, this.stencilFuncMask = 255, this.stencilFail = Ni, this.stencilZFail = Ni, this.stencilZPass = Ni, this.stencilWrite = !1, this.clippingPlanes = null, this.clipIntersection = !1, this.clipShadows = !1, this.shadowSide = null, this.colorWrite = !0, this.precision = null, this.polygonOffset = !1, this.polygonOffsetFactor = 0, this.polygonOffsetUnits = 0, this.dithering = !1, this.alphaToCoverage = !1, this.premultipliedAlpha = !1, this.forceSinglePass = !1, this.visible = !0, this.toneMapped = !0, this.userData = {}, this.version = 0, this._alphaTest = 0
+            }), this.uuid = hr(), this.name = "", this.type = "Material", this.blending = er, this.side = pi, this.vertexColors = !1, this.opacity = 1, this.transparent = !1, this.alphaHash = !1, this.blendSrc = da, this.blendDst = pa, this.blendEquation = Ti, this.blendSrcAlpha = null, this.blendDstAlpha = null, this.blendEquationAlpha = null, this.blendColor = new Ye(0, 0, 0), this.blendAlpha = 0, this.depthFunc = en, this.depthTest = !0, this.depthWrite = !0, this.stencilWriteMask = 255, this.stencilFunc = Ps, this.stencilRef = 0, this.stencilFuncMask = 255, this.stencilFail = Ii, this.stencilZFail = Ii, this.stencilZPass = Ii, this.stencilWrite = !1, this.clippingPlanes = null, this.clipIntersection = !1, this.clipShadows = !1, this.shadowSide = null, this.colorWrite = !0, this.precision = null, this.polygonOffset = !1, this.polygonOffsetFactor = 0, this.polygonOffsetUnits = 0, this.dithering = !1, this.alphaToCoverage = !1, this.premultipliedAlpha = !1, this.forceSinglePass = !1, this.visible = !0, this.toneMapped = !0, this.userData = {}, this.version = 0, this._alphaTest = 0
         }
         get alphaTest() {
             return this._alphaTest
         }
         set alphaTest(e) {
             this._alphaTest > 0 != e > 0 && this.version++, this._alphaTest = e
         }
@@ -3468,15 +3468,15 @@
             let i = {
                 metadata: {
                     version: 4.6,
                     type: "Material",
                     generator: "Material.toJSON"
                 }
             };
-            i.uuid = this.uuid, i.type = this.type, this.name !== "" && (i.name = this.name), this.color && this.color.isColor && (i.color = this.color.getHex()), this.roughness !== void 0 && (i.roughness = this.roughness), this.metalness !== void 0 && (i.metalness = this.metalness), this.sheen !== void 0 && (i.sheen = this.sheen), this.sheenColor && this.sheenColor.isColor && (i.sheenColor = this.sheenColor.getHex()), this.sheenRoughness !== void 0 && (i.sheenRoughness = this.sheenRoughness), this.emissive && this.emissive.isColor && (i.emissive = this.emissive.getHex()), this.emissiveIntensity !== void 0 && this.emissiveIntensity !== 1 && (i.emissiveIntensity = this.emissiveIntensity), this.specular && this.specular.isColor && (i.specular = this.specular.getHex()), this.specularIntensity !== void 0 && (i.specularIntensity = this.specularIntensity), this.specularColor && this.specularColor.isColor && (i.specularColor = this.specularColor.getHex()), this.shininess !== void 0 && (i.shininess = this.shininess), this.clearcoat !== void 0 && (i.clearcoat = this.clearcoat), this.clearcoatRoughness !== void 0 && (i.clearcoatRoughness = this.clearcoatRoughness), this.clearcoatMap && this.clearcoatMap.isTexture && (i.clearcoatMap = this.clearcoatMap.toJSON(e).uuid), this.clearcoatRoughnessMap && this.clearcoatRoughnessMap.isTexture && (i.clearcoatRoughnessMap = this.clearcoatRoughnessMap.toJSON(e).uuid), this.clearcoatNormalMap && this.clearcoatNormalMap.isTexture && (i.clearcoatNormalMap = this.clearcoatNormalMap.toJSON(e).uuid, i.clearcoatNormalScale = this.clearcoatNormalScale.toArray()), this.iridescence !== void 0 && (i.iridescence = this.iridescence), this.iridescenceIOR !== void 0 && (i.iridescenceIOR = this.iridescenceIOR), this.iridescenceThicknessRange !== void 0 && (i.iridescenceThicknessRange = this.iridescenceThicknessRange), this.iridescenceMap && this.iridescenceMap.isTexture && (i.iridescenceMap = this.iridescenceMap.toJSON(e).uuid), this.iridescenceThicknessMap && this.iridescenceThicknessMap.isTexture && (i.iridescenceThicknessMap = this.iridescenceThicknessMap.toJSON(e).uuid), this.anisotropy !== void 0 && (i.anisotropy = this.anisotropy), this.anisotropyRotation !== void 0 && (i.anisotropyRotation = this.anisotropyRotation), this.anisotropyMap && this.anisotropyMap.isTexture && (i.anisotropyMap = this.anisotropyMap.toJSON(e).uuid), this.map && this.map.isTexture && (i.map = this.map.toJSON(e).uuid), this.matcap && this.matcap.isTexture && (i.matcap = this.matcap.toJSON(e).uuid), this.alphaMap && this.alphaMap.isTexture && (i.alphaMap = this.alphaMap.toJSON(e).uuid), this.lightMap && this.lightMap.isTexture && (i.lightMap = this.lightMap.toJSON(e).uuid, i.lightMapIntensity = this.lightMapIntensity), this.aoMap && this.aoMap.isTexture && (i.aoMap = this.aoMap.toJSON(e).uuid, i.aoMapIntensity = this.aoMapIntensity), this.bumpMap && this.bumpMap.isTexture && (i.bumpMap = this.bumpMap.toJSON(e).uuid, i.bumpScale = this.bumpScale), this.normalMap && this.normalMap.isTexture && (i.normalMap = this.normalMap.toJSON(e).uuid, i.normalMapType = this.normalMapType, i.normalScale = this.normalScale.toArray()), this.displacementMap && this.displacementMap.isTexture && (i.displacementMap = this.displacementMap.toJSON(e).uuid, i.displacementScale = this.displacementScale, i.displacementBias = this.displacementBias), this.roughnessMap && this.roughnessMap.isTexture && (i.roughnessMap = this.roughnessMap.toJSON(e).uuid), this.metalnessMap && this.metalnessMap.isTexture && (i.metalnessMap = this.metalnessMap.toJSON(e).uuid), this.emissiveMap && this.emissiveMap.isTexture && (i.emissiveMap = this.emissiveMap.toJSON(e).uuid), this.specularMap && this.specularMap.isTexture && (i.specularMap = this.specularMap.toJSON(e).uuid), this.specularIntensityMap && this.specularIntensityMap.isTexture && (i.specularIntensityMap = this.specularIntensityMap.toJSON(e).uuid), this.specularColorMap && this.specularColorMap.isTexture && (i.specularColorMap = this.specularColorMap.toJSON(e).uuid), this.envMap && this.envMap.isTexture && (i.envMap = this.envMap.toJSON(e).uuid, this.combine !== void 0 && (i.combine = this.combine)), this.envMapRotation !== void 0 && (i.envMapRotation = this.envMapRotation.toArray()), this.envMapIntensity !== void 0 && (i.envMapIntensity = this.envMapIntensity), this.reflectivity !== void 0 && (i.reflectivity = this.reflectivity), this.refractionRatio !== void 0 && (i.refractionRatio = this.refractionRatio), this.gradientMap && this.gradientMap.isTexture && (i.gradientMap = this.gradientMap.toJSON(e).uuid), this.transmission !== void 0 && (i.transmission = this.transmission), this.transmissionMap && this.transmissionMap.isTexture && (i.transmissionMap = this.transmissionMap.toJSON(e).uuid), this.thickness !== void 0 && (i.thickness = this.thickness), this.thicknessMap && this.thicknessMap.isTexture && (i.thicknessMap = this.thicknessMap.toJSON(e).uuid), this.attenuationDistance !== void 0 && this.attenuationDistance !== 1 / 0 && (i.attenuationDistance = this.attenuationDistance), this.attenuationColor !== void 0 && (i.attenuationColor = this.attenuationColor.getHex()), this.size !== void 0 && (i.size = this.size), this.shadowSide !== null && (i.shadowSide = this.shadowSide), this.sizeAttenuation !== void 0 && (i.sizeAttenuation = this.sizeAttenuation), this.blending !== er && (i.blending = this.blending), this.side !== pi && (i.side = this.side), this.vertexColors === !0 && (i.vertexColors = !0), this.opacity < 1 && (i.opacity = this.opacity), this.transparent === !0 && (i.transparent = !0), this.blendSrc !== da && (i.blendSrc = this.blendSrc), this.blendDst !== pa && (i.blendDst = this.blendDst), this.blendEquation !== bi && (i.blendEquation = this.blendEquation), this.blendSrcAlpha !== null && (i.blendSrcAlpha = this.blendSrcAlpha), this.blendDstAlpha !== null && (i.blendDstAlpha = this.blendDstAlpha), this.blendEquationAlpha !== null && (i.blendEquationAlpha = this.blendEquationAlpha), this.blendColor && this.blendColor.isColor && (i.blendColor = this.blendColor.getHex()), this.blendAlpha !== 0 && (i.blendAlpha = this.blendAlpha), this.depthFunc !== en && (i.depthFunc = this.depthFunc), this.depthTest === !1 && (i.depthTest = this.depthTest), this.depthWrite === !1 && (i.depthWrite = this.depthWrite), this.colorWrite === !1 && (i.colorWrite = this.colorWrite), this.stencilWriteMask !== 255 && (i.stencilWriteMask = this.stencilWriteMask), this.stencilFunc !== Ps && (i.stencilFunc = this.stencilFunc), this.stencilRef !== 0 && (i.stencilRef = this.stencilRef), this.stencilFuncMask !== 255 && (i.stencilFuncMask = this.stencilFuncMask), this.stencilFail !== Ni && (i.stencilFail = this.stencilFail), this.stencilZFail !== Ni && (i.stencilZFail = this.stencilZFail), this.stencilZPass !== Ni && (i.stencilZPass = this.stencilZPass), this.stencilWrite === !0 && (i.stencilWrite = this.stencilWrite), this.rotation !== void 0 && this.rotation !== 0 && (i.rotation = this.rotation), this.polygonOffset === !0 && (i.polygonOffset = !0), this.polygonOffsetFactor !== 0 && (i.polygonOffsetFactor = this.polygonOffsetFactor), this.polygonOffsetUnits !== 0 && (i.polygonOffsetUnits = this.polygonOffsetUnits), this.linewidth !== void 0 && this.linewidth !== 1 && (i.linewidth = this.linewidth), this.dashSize !== void 0 && (i.dashSize = this.dashSize), this.gapSize !== void 0 && (i.gapSize = this.gapSize), this.scale !== void 0 && (i.scale = this.scale), this.dithering === !0 && (i.dithering = !0), this.alphaTest > 0 && (i.alphaTest = this.alphaTest), this.alphaHash === !0 && (i.alphaHash = !0), this.alphaToCoverage === !0 && (i.alphaToCoverage = !0), this.premultipliedAlpha === !0 && (i.premultipliedAlpha = !0), this.forceSinglePass === !0 && (i.forceSinglePass = !0), this.wireframe === !0 && (i.wireframe = !0), this.wireframeLinewidth > 1 && (i.wireframeLinewidth = this.wireframeLinewidth), this.wireframeLinecap !== "round" && (i.wireframeLinecap = this.wireframeLinecap), this.wireframeLinejoin !== "round" && (i.wireframeLinejoin = this.wireframeLinejoin), this.flatShading === !0 && (i.flatShading = !0), this.visible === !1 && (i.visible = !1), this.toneMapped === !1 && (i.toneMapped = !1), this.fog === !1 && (i.fog = !1), Object.keys(this.userData).length > 0 && (i.userData = this.userData);
+            i.uuid = this.uuid, i.type = this.type, this.name !== "" && (i.name = this.name), this.color && this.color.isColor && (i.color = this.color.getHex()), this.roughness !== void 0 && (i.roughness = this.roughness), this.metalness !== void 0 && (i.metalness = this.metalness), this.sheen !== void 0 && (i.sheen = this.sheen), this.sheenColor && this.sheenColor.isColor && (i.sheenColor = this.sheenColor.getHex()), this.sheenRoughness !== void 0 && (i.sheenRoughness = this.sheenRoughness), this.emissive && this.emissive.isColor && (i.emissive = this.emissive.getHex()), this.emissiveIntensity !== void 0 && this.emissiveIntensity !== 1 && (i.emissiveIntensity = this.emissiveIntensity), this.specular && this.specular.isColor && (i.specular = this.specular.getHex()), this.specularIntensity !== void 0 && (i.specularIntensity = this.specularIntensity), this.specularColor && this.specularColor.isColor && (i.specularColor = this.specularColor.getHex()), this.shininess !== void 0 && (i.shininess = this.shininess), this.clearcoat !== void 0 && (i.clearcoat = this.clearcoat), this.clearcoatRoughness !== void 0 && (i.clearcoatRoughness = this.clearcoatRoughness), this.clearcoatMap && this.clearcoatMap.isTexture && (i.clearcoatMap = this.clearcoatMap.toJSON(e).uuid), this.clearcoatRoughnessMap && this.clearcoatRoughnessMap.isTexture && (i.clearcoatRoughnessMap = this.clearcoatRoughnessMap.toJSON(e).uuid), this.clearcoatNormalMap && this.clearcoatNormalMap.isTexture && (i.clearcoatNormalMap = this.clearcoatNormalMap.toJSON(e).uuid, i.clearcoatNormalScale = this.clearcoatNormalScale.toArray()), this.iridescence !== void 0 && (i.iridescence = this.iridescence), this.iridescenceIOR !== void 0 && (i.iridescenceIOR = this.iridescenceIOR), this.iridescenceThicknessRange !== void 0 && (i.iridescenceThicknessRange = this.iridescenceThicknessRange), this.iridescenceMap && this.iridescenceMap.isTexture && (i.iridescenceMap = this.iridescenceMap.toJSON(e).uuid), this.iridescenceThicknessMap && this.iridescenceThicknessMap.isTexture && (i.iridescenceThicknessMap = this.iridescenceThicknessMap.toJSON(e).uuid), this.anisotropy !== void 0 && (i.anisotropy = this.anisotropy), this.anisotropyRotation !== void 0 && (i.anisotropyRotation = this.anisotropyRotation), this.anisotropyMap && this.anisotropyMap.isTexture && (i.anisotropyMap = this.anisotropyMap.toJSON(e).uuid), this.map && this.map.isTexture && (i.map = this.map.toJSON(e).uuid), this.matcap && this.matcap.isTexture && (i.matcap = this.matcap.toJSON(e).uuid), this.alphaMap && this.alphaMap.isTexture && (i.alphaMap = this.alphaMap.toJSON(e).uuid), this.lightMap && this.lightMap.isTexture && (i.lightMap = this.lightMap.toJSON(e).uuid, i.lightMapIntensity = this.lightMapIntensity), this.aoMap && this.aoMap.isTexture && (i.aoMap = this.aoMap.toJSON(e).uuid, i.aoMapIntensity = this.aoMapIntensity), this.bumpMap && this.bumpMap.isTexture && (i.bumpMap = this.bumpMap.toJSON(e).uuid, i.bumpScale = this.bumpScale), this.normalMap && this.normalMap.isTexture && (i.normalMap = this.normalMap.toJSON(e).uuid, i.normalMapType = this.normalMapType, i.normalScale = this.normalScale.toArray()), this.displacementMap && this.displacementMap.isTexture && (i.displacementMap = this.displacementMap.toJSON(e).uuid, i.displacementScale = this.displacementScale, i.displacementBias = this.displacementBias), this.roughnessMap && this.roughnessMap.isTexture && (i.roughnessMap = this.roughnessMap.toJSON(e).uuid), this.metalnessMap && this.metalnessMap.isTexture && (i.metalnessMap = this.metalnessMap.toJSON(e).uuid), this.emissiveMap && this.emissiveMap.isTexture && (i.emissiveMap = this.emissiveMap.toJSON(e).uuid), this.specularMap && this.specularMap.isTexture && (i.specularMap = this.specularMap.toJSON(e).uuid), this.specularIntensityMap && this.specularIntensityMap.isTexture && (i.specularIntensityMap = this.specularIntensityMap.toJSON(e).uuid), this.specularColorMap && this.specularColorMap.isTexture && (i.specularColorMap = this.specularColorMap.toJSON(e).uuid), this.envMap && this.envMap.isTexture && (i.envMap = this.envMap.toJSON(e).uuid, this.combine !== void 0 && (i.combine = this.combine)), this.envMapRotation !== void 0 && (i.envMapRotation = this.envMapRotation.toArray()), this.envMapIntensity !== void 0 && (i.envMapIntensity = this.envMapIntensity), this.reflectivity !== void 0 && (i.reflectivity = this.reflectivity), this.refractionRatio !== void 0 && (i.refractionRatio = this.refractionRatio), this.gradientMap && this.gradientMap.isTexture && (i.gradientMap = this.gradientMap.toJSON(e).uuid), this.transmission !== void 0 && (i.transmission = this.transmission), this.transmissionMap && this.transmissionMap.isTexture && (i.transmissionMap = this.transmissionMap.toJSON(e).uuid), this.thickness !== void 0 && (i.thickness = this.thickness), this.thicknessMap && this.thicknessMap.isTexture && (i.thicknessMap = this.thicknessMap.toJSON(e).uuid), this.attenuationDistance !== void 0 && this.attenuationDistance !== 1 / 0 && (i.attenuationDistance = this.attenuationDistance), this.attenuationColor !== void 0 && (i.attenuationColor = this.attenuationColor.getHex()), this.size !== void 0 && (i.size = this.size), this.shadowSide !== null && (i.shadowSide = this.shadowSide), this.sizeAttenuation !== void 0 && (i.sizeAttenuation = this.sizeAttenuation), this.blending !== er && (i.blending = this.blending), this.side !== pi && (i.side = this.side), this.vertexColors === !0 && (i.vertexColors = !0), this.opacity < 1 && (i.opacity = this.opacity), this.transparent === !0 && (i.transparent = !0), this.blendSrc !== da && (i.blendSrc = this.blendSrc), this.blendDst !== pa && (i.blendDst = this.blendDst), this.blendEquation !== Ti && (i.blendEquation = this.blendEquation), this.blendSrcAlpha !== null && (i.blendSrcAlpha = this.blendSrcAlpha), this.blendDstAlpha !== null && (i.blendDstAlpha = this.blendDstAlpha), this.blendEquationAlpha !== null && (i.blendEquationAlpha = this.blendEquationAlpha), this.blendColor && this.blendColor.isColor && (i.blendColor = this.blendColor.getHex()), this.blendAlpha !== 0 && (i.blendAlpha = this.blendAlpha), this.depthFunc !== en && (i.depthFunc = this.depthFunc), this.depthTest === !1 && (i.depthTest = this.depthTest), this.depthWrite === !1 && (i.depthWrite = this.depthWrite), this.colorWrite === !1 && (i.colorWrite = this.colorWrite), this.stencilWriteMask !== 255 && (i.stencilWriteMask = this.stencilWriteMask), this.stencilFunc !== Ps && (i.stencilFunc = this.stencilFunc), this.stencilRef !== 0 && (i.stencilRef = this.stencilRef), this.stencilFuncMask !== 255 && (i.stencilFuncMask = this.stencilFuncMask), this.stencilFail !== Ii && (i.stencilFail = this.stencilFail), this.stencilZFail !== Ii && (i.stencilZFail = this.stencilZFail), this.stencilZPass !== Ii && (i.stencilZPass = this.stencilZPass), this.stencilWrite === !0 && (i.stencilWrite = this.stencilWrite), this.rotation !== void 0 && this.rotation !== 0 && (i.rotation = this.rotation), this.polygonOffset === !0 && (i.polygonOffset = !0), this.polygonOffsetFactor !== 0 && (i.polygonOffsetFactor = this.polygonOffsetFactor), this.polygonOffsetUnits !== 0 && (i.polygonOffsetUnits = this.polygonOffsetUnits), this.linewidth !== void 0 && this.linewidth !== 1 && (i.linewidth = this.linewidth), this.dashSize !== void 0 && (i.dashSize = this.dashSize), this.gapSize !== void 0 && (i.gapSize = this.gapSize), this.scale !== void 0 && (i.scale = this.scale), this.dithering === !0 && (i.dithering = !0), this.alphaTest > 0 && (i.alphaTest = this.alphaTest), this.alphaHash === !0 && (i.alphaHash = !0), this.alphaToCoverage === !0 && (i.alphaToCoverage = !0), this.premultipliedAlpha === !0 && (i.premultipliedAlpha = !0), this.forceSinglePass === !0 && (i.forceSinglePass = !0), this.wireframe === !0 && (i.wireframe = !0), this.wireframeLinewidth > 1 && (i.wireframeLinewidth = this.wireframeLinewidth), this.wireframeLinecap !== "round" && (i.wireframeLinecap = this.wireframeLinecap), this.wireframeLinejoin !== "round" && (i.wireframeLinejoin = this.wireframeLinejoin), this.flatShading === !0 && (i.flatShading = !0), this.visible === !1 && (i.visible = !1), this.toneMapped === !1 && (i.toneMapped = !1), this.fog === !1 && (i.fog = !1), Object.keys(this.userData).length > 0 && (i.userData = this.userData);
 
             function n(a) {
                 let o = [];
                 for (let s in a) {
                     let l = a[s];
                     delete l.metadata, o.push(l)
                 }
@@ -3516,20 +3516,20 @@
         constructor(e) {
             super(), this.isMeshBasicMaterial = !0, this.type = "MeshBasicMaterial", this.color = new Ye(16777215), this.map = null, this.lightMap = null, this.lightMapIntensity = 1, this.aoMap = null, this.aoMapIntensity = 1, this.specularMap = null, this.alphaMap = null, this.envMap = null, this.envMapRotation = new ei, this.combine = Po, this.reflectivity = 1, this.refractionRatio = .98, this.wireframe = !1, this.wireframeLinewidth = 1, this.wireframeLinecap = "round", this.wireframeLinejoin = "round", this.fog = !0, this.setValues(e)
         }
         copy(e) {
             return super.copy(e), this.color.copy(e.color), this.map = e.map, this.lightMap = e.lightMap, this.lightMapIntensity = e.lightMapIntensity, this.aoMap = e.aoMap, this.aoMapIntensity = e.aoMapIntensity, this.specularMap = e.specularMap, this.alphaMap = e.alphaMap, this.envMap = e.envMap, this.envMapRotation.copy(e.envMapRotation), this.combine = e.combine, this.reflectivity = e.reflectivity, this.refractionRatio = e.refractionRatio, this.wireframe = e.wireframe, this.wireframeLinewidth = e.wireframeLinewidth, this.wireframeLinecap = e.wireframeLinecap, this.wireframeLinejoin = e.wireframeLinejoin, this.fog = e.fog, this
         }
     },
-    it = new D,
-    Or = new De,
+    it = new U,
+    Or = new Ue,
     Lt = class {
         constructor(e, t, i = !1) {
             if (Array.isArray(e)) throw new TypeError("THREE.BufferAttribute: array should be a Typed Array.");
-            this.isBufferAttribute = !0, this.name = "", this.array = e, this.itemSize = t, this.count = e !== void 0 ? e.length / t : 0, this.normalized = i, this.usage = Us, this._updateRange = {
+            this.isBufferAttribute = !0, this.name = "", this.array = e, this.itemSize = t, this.count = e !== void 0 ? e.length / t : 0, this.normalized = i, this.usage = Ds, this._updateRange = {
                 offset: 0,
                 count: -1
             }, this.updateRanges = [], this.gpuType = Zt, this.version = 0
         }
         onUploadCallback() {}
         set needsUpdate(e) {
             e === !0 && this.version++
@@ -3635,15 +3635,15 @@
         toJSON() {
             let e = {
                 itemSize: this.itemSize,
                 type: this.array.constructor.name,
                 array: Array.from(this.array),
                 normalized: this.normalized
             };
-            return this.name !== "" && (e.name = this.name), this.usage !== Us && (e.usage = this.usage), e
+            return this.name !== "" && (e.name = this.name), this.usage !== Ds && (e.usage = this.usage), e
         }
     },
     dn = class extends Lt {
         constructor(e, t, i) {
             super(new Uint16Array(e), t, i)
         }
     },
@@ -3656,32 +3656,32 @@
         constructor(e, t, i) {
             super(new Float32Array(e), t, i)
         }
     },
     Pc = 0,
     Ct = new at,
     ea = new wt,
-    Vi = new D,
-    Tt = new Li,
+    Vi = new U,
+    bt = new Li,
     _r = new Li,
-    lt = new D,
-    St = class r extends Jt {
+    lt = new U,
+    Et = class r extends Jt {
         constructor() {
             super(), this.isBufferGeometry = !0, Object.defineProperty(this, "id", {
                 value: Pc++
             }), this.uuid = hr(), this.name = "", this.type = "BufferGeometry", this.index = null, this.attributes = {}, this.morphAttributes = {}, this.morphTargetsRelative = !1, this.groups = [], this.boundingBox = null, this.boundingSphere = null, this.drawRange = {
                 start: 0,
                 count: 1 / 0
             }, this.userData = {}
         }
         getIndex() {
             return this.index
         }
         setIndex(e) {
-            return Array.isArray(e) ? this.index = new(Ho(e) ? pn : dn)(e, 1) : this.index = e, this
+            return Array.isArray(e) ? this.index = new(Go(e) ? pn : dn)(e, 1) : this.index = e, this
         }
         getAttribute(e) {
             return this.attributes[e]
         }
         setAttribute(e, t) {
             return this.attributes[e] = t, this
         }
@@ -3705,15 +3705,15 @@
             this.drawRange.start = e, this.drawRange.count = t
         }
         applyMatrix4(e) {
             let t = this.attributes.position;
             t !== void 0 && (t.applyMatrix4(e), t.needsUpdate = !0);
             let i = this.attributes.normal;
             if (i !== void 0) {
-                let a = new Be().getNormalMatrix(e);
+                let a = new ze().getNormalMatrix(e);
                 i.applyNormalMatrix(a), i.needsUpdate = !0
             }
             let n = this.attributes.tangent;
             return n !== void 0 && (n.transformDirection(e), n.needsUpdate = !0), this.boundingBox !== null && this.computeBoundingBox(), this.boundingSphere !== null && this.computeBoundingSphere(), this
         }
         applyQuaternion(e) {
             return Ct.makeRotationFromQuaternion(e), this.applyMatrix4(Ct), this
@@ -3748,49 +3748,49 @@
             return this.setAttribute("position", new rt(t, 3)), this
         }
         computeBoundingBox() {
             this.boundingBox === null && (this.boundingBox = new Li);
             let e = this.attributes.position,
                 t = this.morphAttributes.position;
             if (e && e.isGLBufferAttribute) {
-                console.error("THREE.BufferGeometry.computeBoundingBox(): GLBufferAttribute requires a manual bounding box.", this), this.boundingBox.set(new D(-1 / 0, -1 / 0, -1 / 0), new D(1 / 0, 1 / 0, 1 / 0));
+                console.error("THREE.BufferGeometry.computeBoundingBox(): GLBufferAttribute requires a manual bounding box.", this), this.boundingBox.set(new U(-1 / 0, -1 / 0, -1 / 0), new U(1 / 0, 1 / 0, 1 / 0));
                 return
             }
             if (e !== void 0) {
                 if (this.boundingBox.setFromBufferAttribute(e), t)
                     for (let i = 0, n = t.length; i < n; i++) {
                         let a = t[i];
-                        Tt.setFromBufferAttribute(a), this.morphTargetsRelative ? (lt.addVectors(this.boundingBox.min, Tt.min), this.boundingBox.expandByPoint(lt), lt.addVectors(this.boundingBox.max, Tt.max), this.boundingBox.expandByPoint(lt)) : (this.boundingBox.expandByPoint(Tt.min), this.boundingBox.expandByPoint(Tt.max))
+                        bt.setFromBufferAttribute(a), this.morphTargetsRelative ? (lt.addVectors(this.boundingBox.min, bt.min), this.boundingBox.expandByPoint(lt), lt.addVectors(this.boundingBox.max, bt.max), this.boundingBox.expandByPoint(lt)) : (this.boundingBox.expandByPoint(bt.min), this.boundingBox.expandByPoint(bt.max))
                     }
             } else this.boundingBox.makeEmpty();
             (isNaN(this.boundingBox.min.x) || isNaN(this.boundingBox.min.y) || isNaN(this.boundingBox.min.z)) && console.error('THREE.BufferGeometry.computeBoundingBox(): Computed min/max have NaN values. The "position" attribute is likely to have NaN values.', this)
         }
         computeBoundingSphere() {
             this.boundingSphere === null && (this.boundingSphere = new or);
             let e = this.attributes.position,
                 t = this.morphAttributes.position;
             if (e && e.isGLBufferAttribute) {
-                console.error("THREE.BufferGeometry.computeBoundingSphere(): GLBufferAttribute requires a manual bounding sphere.", this), this.boundingSphere.set(new D, 1 / 0);
+                console.error("THREE.BufferGeometry.computeBoundingSphere(): GLBufferAttribute requires a manual bounding sphere.", this), this.boundingSphere.set(new U, 1 / 0);
                 return
             }
             if (e) {
                 let i = this.boundingSphere.center;
-                if (Tt.setFromBufferAttribute(e), t)
+                if (bt.setFromBufferAttribute(e), t)
                     for (let a = 0, o = t.length; a < o; a++) {
                         let s = t[a];
-                        _r.setFromBufferAttribute(s), this.morphTargetsRelative ? (lt.addVectors(Tt.min, _r.min), Tt.expandByPoint(lt), lt.addVectors(Tt.max, _r.max), Tt.expandByPoint(lt)) : (Tt.expandByPoint(_r.min), Tt.expandByPoint(_r.max))
+                        _r.setFromBufferAttribute(s), this.morphTargetsRelative ? (lt.addVectors(bt.min, _r.min), bt.expandByPoint(lt), lt.addVectors(bt.max, _r.max), bt.expandByPoint(lt)) : (bt.expandByPoint(_r.min), bt.expandByPoint(_r.max))
                     }
-                Tt.getCenter(i);
+                bt.getCenter(i);
                 let n = 0;
                 for (let a = 0, o = e.count; a < o; a++) lt.fromBufferAttribute(e, a), n = Math.max(n, i.distanceToSquared(lt));
                 if (t)
                     for (let a = 0, o = t.length; a < o; a++) {
                         let s = t[a],
                             l = this.morphTargetsRelative;
-                        for (let c = 0, u = s.count; c < u; c++) lt.fromBufferAttribute(s, c), l && (Vi.fromBufferAttribute(e, c), lt.add(Vi)), n = Math.max(n, i.distanceToSquared(lt))
+                        for (let c = 0, h = s.count; c < h; c++) lt.fromBufferAttribute(s, c), l && (Vi.fromBufferAttribute(e, c), lt.add(Vi)), n = Math.max(n, i.distanceToSquared(lt))
                     }
                 this.boundingSphere.radius = Math.sqrt(n), isNaN(this.boundingSphere.radius) && console.error('THREE.BufferGeometry.computeBoundingSphere(): Computed radius is NaN. The "position" attribute is likely to have NaN values.', this)
             }
         }
         computeTangents() {
             let e = this.index,
                 t = this.attributes;
@@ -3801,119 +3801,119 @@
             let i = t.position,
                 n = t.normal,
                 a = t.uv;
             this.hasAttribute("tangent") === !1 && this.setAttribute("tangent", new Lt(new Float32Array(4 * i.count), 4));
             let o = this.getAttribute("tangent"),
                 s = [],
                 l = [];
-            for (let C = 0; C < i.count; C++) s[C] = new D, l[C] = new D;
-            let c = new D,
-                u = new D,
-                p = new D,
-                f = new De,
-                m = new De,
-                _ = new De,
-                M = new D,
-                d = new D;
-
-            function h(C, Z, v) {
-                c.fromBufferAttribute(i, C), u.fromBufferAttribute(i, Z), p.fromBufferAttribute(i, v), f.fromBufferAttribute(a, C), m.fromBufferAttribute(a, Z), _.fromBufferAttribute(a, v), u.sub(c), p.sub(c), m.sub(f), _.sub(f);
-                let T = 1 / (m.x * _.y - _.x * m.y);
-                isFinite(T) && (M.copy(u).multiplyScalar(_.y).addScaledVector(p, -m.y).multiplyScalar(T), d.copy(p).multiplyScalar(m.x).addScaledVector(u, -_.x).multiplyScalar(T), s[C].add(M), s[Z].add(M), s[v].add(M), l[C].add(d), l[Z].add(d), l[v].add(d))
+            for (let P = 0; P < i.count; P++) s[P] = new U, l[P] = new U;
+            let c = new U,
+                h = new U,
+                p = new U,
+                f = new Ue,
+                m = new Ue,
+                _ = new Ue,
+                M = new U,
+                d = new U;
+
+            function u(P, I, v) {
+                c.fromBufferAttribute(i, P), h.fromBufferAttribute(i, I), p.fromBufferAttribute(i, v), f.fromBufferAttribute(a, P), m.fromBufferAttribute(a, I), _.fromBufferAttribute(a, v), h.sub(c), p.sub(c), m.sub(f), _.sub(f);
+                let w = 1 / (m.x * _.y - _.x * m.y);
+                isFinite(w) && (M.copy(h).multiplyScalar(_.y).addScaledVector(p, -m.y).multiplyScalar(w), d.copy(p).multiplyScalar(m.x).addScaledVector(h, -_.x).multiplyScalar(w), s[P].add(M), s[I].add(M), s[v].add(M), l[P].add(d), l[I].add(d), l[v].add(d))
             }
-            let w = this.groups;
-            w.length === 0 && (w = [{
+            let T = this.groups;
+            T.length === 0 && (T = [{
                 start: 0,
                 count: e.count
             }]);
-            for (let C = 0, Z = w.length; C < Z; ++C) {
-                let v = w[C],
-                    T = v.start,
-                    V = v.count;
-                for (let K = T, P = T + V; K < P; K += 3) h(e.getX(K + 0), e.getX(K + 1), e.getX(K + 2))
-            }
-            let x = new D,
-                R = new D,
-                U = new D,
-                A = new D;
-
-            function y(C) {
-                U.fromBufferAttribute(n, C), A.copy(U);
-                let Z = s[C];
-                x.copy(Z), x.sub(U.multiplyScalar(U.dot(Z))).normalize(), R.crossVectors(A, Z);
-                let v = R.dot(l[C]) < 0 ? -1 : 1;
-                o.setXYZW(C, x.x, x.y, x.z, v)
-            }
-            for (let C = 0, Z = w.length; C < Z; ++C) {
-                let v = w[C],
-                    T = v.start,
-                    V = v.count;
-                for (let K = T, P = T + V; K < P; K += 3) y(e.getX(K + 0)), y(e.getX(K + 1)), y(e.getX(K + 2))
+            for (let P = 0, I = T.length; P < I; ++P) {
+                let v = T[P],
+                    w = v.start,
+                    W = v.count;
+                for (let K = w, L = w + W; K < L; K += 3) u(e.getX(K + 0), e.getX(K + 1), e.getX(K + 2))
+            }
+            let x = new U,
+                A = new U,
+                D = new U,
+                R = new U;
+
+            function b(P) {
+                D.fromBufferAttribute(n, P), R.copy(D);
+                let I = s[P];
+                x.copy(I), x.sub(D.multiplyScalar(D.dot(I))).normalize(), A.crossVectors(R, I);
+                let v = A.dot(l[P]) < 0 ? -1 : 1;
+                o.setXYZW(P, x.x, x.y, x.z, v)
+            }
+            for (let P = 0, I = T.length; P < I; ++P) {
+                let v = T[P],
+                    w = v.start,
+                    W = v.count;
+                for (let K = w, L = w + W; K < L; K += 3) b(e.getX(K + 0)), b(e.getX(K + 1)), b(e.getX(K + 2))
             }
         }
         computeVertexNormals() {
             let e = this.index,
                 t = this.getAttribute("position");
             if (t !== void 0) {
                 let i = this.getAttribute("normal");
                 if (i === void 0) i = new Lt(new Float32Array(t.count * 3), 3), this.setAttribute("normal", i);
                 else
                     for (let f = 0, m = i.count; f < m; f++) i.setXYZ(f, 0, 0, 0);
-                let n = new D,
-                    a = new D,
-                    o = new D,
-                    s = new D,
-                    l = new D,
-                    c = new D,
-                    u = new D,
-                    p = new D;
+                let n = new U,
+                    a = new U,
+                    o = new U,
+                    s = new U,
+                    l = new U,
+                    c = new U,
+                    h = new U,
+                    p = new U;
                 if (e)
                     for (let f = 0, m = e.count; f < m; f += 3) {
                         let _ = e.getX(f + 0),
                             M = e.getX(f + 1),
                             d = e.getX(f + 2);
-                        n.fromBufferAttribute(t, _), a.fromBufferAttribute(t, M), o.fromBufferAttribute(t, d), u.subVectors(o, a), p.subVectors(n, a), u.cross(p), s.fromBufferAttribute(i, _), l.fromBufferAttribute(i, M), c.fromBufferAttribute(i, d), s.add(u), l.add(u), c.add(u), i.setXYZ(_, s.x, s.y, s.z), i.setXYZ(M, l.x, l.y, l.z), i.setXYZ(d, c.x, c.y, c.z)
+                        n.fromBufferAttribute(t, _), a.fromBufferAttribute(t, M), o.fromBufferAttribute(t, d), h.subVectors(o, a), p.subVectors(n, a), h.cross(p), s.fromBufferAttribute(i, _), l.fromBufferAttribute(i, M), c.fromBufferAttribute(i, d), s.add(h), l.add(h), c.add(h), i.setXYZ(_, s.x, s.y, s.z), i.setXYZ(M, l.x, l.y, l.z), i.setXYZ(d, c.x, c.y, c.z)
                     } else
-                        for (let f = 0, m = t.count; f < m; f += 3) n.fromBufferAttribute(t, f + 0), a.fromBufferAttribute(t, f + 1), o.fromBufferAttribute(t, f + 2), u.subVectors(o, a), p.subVectors(n, a), u.cross(p), i.setXYZ(f + 0, u.x, u.y, u.z), i.setXYZ(f + 1, u.x, u.y, u.z), i.setXYZ(f + 2, u.x, u.y, u.z);
+                        for (let f = 0, m = t.count; f < m; f += 3) n.fromBufferAttribute(t, f + 0), a.fromBufferAttribute(t, f + 1), o.fromBufferAttribute(t, f + 2), h.subVectors(o, a), p.subVectors(n, a), h.cross(p), i.setXYZ(f + 0, h.x, h.y, h.z), i.setXYZ(f + 1, h.x, h.y, h.z), i.setXYZ(f + 2, h.x, h.y, h.z);
                 this.normalizeNormals(), i.needsUpdate = !0
             }
         }
         normalizeNormals() {
             let e = this.attributes.normal;
             for (let t = 0, i = e.count; t < i; t++) lt.fromBufferAttribute(e, t), lt.normalize(), e.setXYZ(t, lt.x, lt.y, lt.z)
         }
         toNonIndexed() {
             function e(s, l) {
                 let c = s.array,
-                    u = s.itemSize,
+                    h = s.itemSize,
                     p = s.normalized,
-                    f = new c.constructor(l.length * u),
+                    f = new c.constructor(l.length * h),
                     m = 0,
                     _ = 0;
                 for (let M = 0, d = l.length; M < d; M++) {
-                    s.isInterleavedBufferAttribute ? m = l[M] * s.data.stride + s.offset : m = l[M] * u;
-                    for (let h = 0; h < u; h++) f[_++] = c[m++]
+                    s.isInterleavedBufferAttribute ? m = l[M] * s.data.stride + s.offset : m = l[M] * h;
+                    for (let u = 0; u < h; u++) f[_++] = c[m++]
                 }
-                return new Lt(f, u, p)
+                return new Lt(f, h, p)
             }
             if (this.index === null) return console.warn("THREE.BufferGeometry.toNonIndexed(): BufferGeometry is already non-indexed."), this;
             let t = new r,
                 i = this.index.array,
                 n = this.attributes;
             for (let s in n) {
                 let l = n[s],
                     c = e(l, i);
                 t.setAttribute(s, c)
             }
             let a = this.morphAttributes;
             for (let s in a) {
                 let l = [],
                     c = a[s];
-                for (let u = 0, p = c.length; u < p; u++) {
-                    let f = c[u],
+                for (let h = 0, p = c.length; h < p; h++) {
+                    let f = c[h],
                         m = e(f, i);
                     l.push(m)
                 }
                 t.morphAttributes[s] = l
             }
             t.morphTargetsRelative = this.morphTargetsRelative;
             let o = this.groups;
@@ -3949,20 +3949,20 @@
                 let c = i[l];
                 e.data.attributes[l] = c.toJSON(e.data)
             }
             let n = {},
                 a = !1;
             for (let l in this.morphAttributes) {
                 let c = this.morphAttributes[l],
-                    u = [];
+                    h = [];
                 for (let p = 0, f = c.length; p < f; p++) {
                     let m = c[p];
-                    u.push(m.toJSON(e.data))
+                    h.push(m.toJSON(e.data))
                 }
-                u.length > 0 && (n[l] = u, a = !0)
+                h.length > 0 && (n[l] = h, a = !0)
             }
             a && (e.data.morphAttributes = n, e.data.morphTargetsRelative = this.morphTargetsRelative);
             let o = this.groups;
             o.length > 0 && (e.data.groups = JSON.parse(JSON.stringify(o)));
             let s = this.boundingSphere;
             return s !== null && (e.data.boundingSphere = {
                 center: s.center.toArray(),
@@ -3976,27 +3976,27 @@
             this.index = null, this.attributes = {}, this.morphAttributes = {}, this.groups = [], this.boundingBox = null, this.boundingSphere = null;
             let t = {};
             this.name = e.name;
             let i = e.index;
             i !== null && this.setIndex(i.clone(t));
             let n = e.attributes;
             for (let c in n) {
-                let u = n[c];
-                this.setAttribute(c, u.clone(t))
+                let h = n[c];
+                this.setAttribute(c, h.clone(t))
             }
             let a = e.morphAttributes;
             for (let c in a) {
-                let u = [],
+                let h = [],
                     p = a[c];
-                for (let f = 0, m = p.length; f < m; f++) u.push(p[f].clone(t));
-                this.morphAttributes[c] = u
+                for (let f = 0, m = p.length; f < m; f++) h.push(p[f].clone(t));
+                this.morphAttributes[c] = h
             }
             this.morphTargetsRelative = e.morphTargetsRelative;
             let o = e.groups;
-            for (let c = 0, u = o.length; c < u; c++) {
+            for (let c = 0, h = o.length; c < h; c++) {
                 let p = o[c];
                 this.addGroup(p.start, p.count, p.materialIndex)
             }
             let s = e.boundingBox;
             s !== null && (this.boundingBox = s.clone());
             let l = e.boundingSphere;
             return l !== null && (this.boundingSphere = l.clone()), this.drawRange.start = e.drawRange.start, this.drawRange.count = e.drawRange.count, this.userData = e.userData, this
@@ -4004,32 +4004,32 @@
         dispose() {
             this.dispatchEvent({
                 type: "dispose"
             })
         }
     },
     js = new at,
-    xi = new Sr,
+    xi = new Er,
     Fr = new or,
-    Ys = new D,
-    Wi = new D,
-    Xi = new D,
-    ji = new D,
-    ta = new D,
-    Br = new D,
-    zr = new De,
-    Gr = new De,
-    Hr = new De,
-    qs = new D,
-    Zs = new D,
-    Ks = new D,
-    kr = new D,
-    Vr = new D,
+    Ys = new U,
+    Wi = new U,
+    Xi = new U,
+    ji = new U,
+    ta = new U,
+    zr = new U,
+    Br = new Ue,
+    Hr = new Ue,
+    Gr = new Ue,
+    qs = new U,
+    Zs = new U,
+    Ks = new U,
+    kr = new U,
+    Vr = new U,
     vt = class extends wt {
-        constructor(e = new St, t = new di) {
+        constructor(e = new Et, t = new di) {
             super(), this.isMesh = !0, this.type = "Mesh", this.geometry = e, this.material = t, this.updateMorphTargets()
         }
         copy(e, t) {
             return super.copy(e, t), e.morphTargetInfluences !== void 0 && (this.morphTargetInfluences = e.morphTargetInfluences.slice()), e.morphTargetDictionary !== void 0 && (this.morphTargetDictionary = Object.assign({}, e.morphTargetDictionary)), this.material = Array.isArray(e.material) ? e.material.slice() : e.material, this.geometry = e.geometry, this
         }
         updateMorphTargets() {
             let e = this.geometry.morphAttributes,
@@ -4049,21 +4049,21 @@
             let i = this.geometry,
                 n = i.attributes.position,
                 a = i.morphAttributes.position,
                 o = i.morphTargetsRelative;
             t.fromBufferAttribute(n, e);
             let s = this.morphTargetInfluences;
             if (a && s) {
-                Br.set(0, 0, 0);
+                zr.set(0, 0, 0);
                 for (let l = 0, c = a.length; l < c; l++) {
-                    let u = s[l],
+                    let h = s[l],
                         p = a[l];
-                    u !== 0 && (ta.fromBufferAttribute(p, e), o ? Br.addScaledVector(ta, u) : Br.addScaledVector(ta.sub(t), u))
+                    h !== 0 && (ta.fromBufferAttribute(p, e), o ? zr.addScaledVector(ta, h) : zr.addScaledVector(ta.sub(t), h))
                 }
-                t.add(Br)
+                t.add(zr)
             }
             return t
         }
         raycast(e, t) {
             let i = this.geometry,
                 n = this.material,
                 a = this.matrixWorld;
@@ -4071,141 +4071,141 @@
         }
         _computeIntersections(e, t, i) {
             let n, a = this.geometry,
                 o = this.material,
                 s = a.index,
                 l = a.attributes.position,
                 c = a.attributes.uv,
-                u = a.attributes.uv1,
+                h = a.attributes.uv1,
                 p = a.attributes.normal,
                 f = a.groups,
                 m = a.drawRange;
             if (s !== null)
                 if (Array.isArray(o))
                     for (let _ = 0, M = f.length; _ < M; _++) {
                         let d = f[_],
-                            h = o[d.materialIndex],
-                            w = Math.max(d.start, m.start),
+                            u = o[d.materialIndex],
+                            T = Math.max(d.start, m.start),
                             x = Math.min(s.count, Math.min(d.start + d.count, m.start + m.count));
-                        for (let R = w, U = x; R < U; R += 3) {
-                            let A = s.getX(R),
-                                y = s.getX(R + 1),
-                                C = s.getX(R + 2);
-                            n = Wr(this, h, e, i, c, u, p, A, y, C), n && (n.faceIndex = Math.floor(R / 3), n.face.materialIndex = d.materialIndex, t.push(n))
+                        for (let A = T, D = x; A < D; A += 3) {
+                            let R = s.getX(A),
+                                b = s.getX(A + 1),
+                                P = s.getX(A + 2);
+                            n = Wr(this, u, e, i, c, h, p, R, b, P), n && (n.faceIndex = Math.floor(A / 3), n.face.materialIndex = d.materialIndex, t.push(n))
                         }
                     } else {
                         let _ = Math.max(0, m.start),
                             M = Math.min(s.count, m.start + m.count);
-                        for (let d = _, h = M; d < h; d += 3) {
-                            let w = s.getX(d),
+                        for (let d = _, u = M; d < u; d += 3) {
+                            let T = s.getX(d),
                                 x = s.getX(d + 1),
-                                R = s.getX(d + 2);
-                            n = Wr(this, o, e, i, c, u, p, w, x, R), n && (n.faceIndex = Math.floor(d / 3), t.push(n))
+                                A = s.getX(d + 2);
+                            n = Wr(this, o, e, i, c, h, p, T, x, A), n && (n.faceIndex = Math.floor(d / 3), t.push(n))
                         }
                     } else if (l !== void 0)
                         if (Array.isArray(o))
                             for (let _ = 0, M = f.length; _ < M; _++) {
                                 let d = f[_],
-                                    h = o[d.materialIndex],
-                                    w = Math.max(d.start, m.start),
+                                    u = o[d.materialIndex],
+                                    T = Math.max(d.start, m.start),
                                     x = Math.min(l.count, Math.min(d.start + d.count, m.start + m.count));
-                                for (let R = w, U = x; R < U; R += 3) {
-                                    let A = R,
-                                        y = R + 1,
-                                        C = R + 2;
-                                    n = Wr(this, h, e, i, c, u, p, A, y, C), n && (n.faceIndex = Math.floor(R / 3), n.face.materialIndex = d.materialIndex, t.push(n))
+                                for (let A = T, D = x; A < D; A += 3) {
+                                    let R = A,
+                                        b = A + 1,
+                                        P = A + 2;
+                                    n = Wr(this, u, e, i, c, h, p, R, b, P), n && (n.faceIndex = Math.floor(A / 3), n.face.materialIndex = d.materialIndex, t.push(n))
                                 }
                             } else {
                                 let _ = Math.max(0, m.start),
                                     M = Math.min(l.count, m.start + m.count);
-                                for (let d = _, h = M; d < h; d += 3) {
-                                    let w = d,
+                                for (let d = _, u = M; d < u; d += 3) {
+                                    let T = d,
                                         x = d + 1,
-                                        R = d + 2;
-                                    n = Wr(this, o, e, i, c, u, p, w, x, R), n && (n.faceIndex = Math.floor(d / 3), t.push(n))
+                                        A = d + 2;
+                                    n = Wr(this, o, e, i, c, h, p, T, x, A), n && (n.faceIndex = Math.floor(d / 3), t.push(n))
                                 }
                             }
         }
     };
 
-function Uc(r, e, t, i, n, a, o, s) {
+function Dc(r, e, t, i, n, a, o, s) {
     let l;
-    if (e.side === Et ? l = i.intersectTriangle(o, a, n, !0, s) : l = i.intersectTriangle(n, a, o, e.side === pi, s), l === null) return null;
+    if (e.side === yt ? l = i.intersectTriangle(o, a, n, !0, s) : l = i.intersectTriangle(n, a, o, e.side === pi, s), l === null) return null;
     Vr.copy(s), Vr.applyMatrix4(r.matrixWorld);
     let c = t.ray.origin.distanceTo(Vr);
     return c < t.near || c > t.far ? null : {
         distance: c,
         point: Vr.clone(),
         object: r
     }
 }
 
 function Wr(r, e, t, i, n, a, o, s, l, c) {
     r.getVertexPosition(s, Wi), r.getVertexPosition(l, Xi), r.getVertexPosition(c, ji);
-    let u = Uc(r, e, t, i, Wi, Xi, ji, kr);
-    if (u) {
-        n && (zr.fromBufferAttribute(n, s), Gr.fromBufferAttribute(n, l), Hr.fromBufferAttribute(n, c), u.uv = Ai.getInterpolation(kr, Wi, Xi, ji, zr, Gr, Hr, new De)), a && (zr.fromBufferAttribute(a, s), Gr.fromBufferAttribute(a, l), Hr.fromBufferAttribute(a, c), u.uv1 = Ai.getInterpolation(kr, Wi, Xi, ji, zr, Gr, Hr, new De)), o && (qs.fromBufferAttribute(o, s), Zs.fromBufferAttribute(o, l), Ks.fromBufferAttribute(o, c), u.normal = Ai.getInterpolation(kr, Wi, Xi, ji, qs, Zs, Ks, new D), u.normal.dot(i.direction) > 0 && u.normal.multiplyScalar(-1));
+    let h = Dc(r, e, t, i, Wi, Xi, ji, kr);
+    if (h) {
+        n && (Br.fromBufferAttribute(n, s), Hr.fromBufferAttribute(n, l), Gr.fromBufferAttribute(n, c), h.uv = Ai.getInterpolation(kr, Wi, Xi, ji, Br, Hr, Gr, new Ue)), a && (Br.fromBufferAttribute(a, s), Hr.fromBufferAttribute(a, l), Gr.fromBufferAttribute(a, c), h.uv1 = Ai.getInterpolation(kr, Wi, Xi, ji, Br, Hr, Gr, new Ue)), o && (qs.fromBufferAttribute(o, s), Zs.fromBufferAttribute(o, l), Ks.fromBufferAttribute(o, c), h.normal = Ai.getInterpolation(kr, Wi, Xi, ji, qs, Zs, Ks, new U), h.normal.dot(i.direction) > 0 && h.normal.multiplyScalar(-1));
         let p = {
             a: s,
             b: l,
             c,
-            normal: new D,
+            normal: new U,
             materialIndex: 0
         };
-        Ai.getNormal(Wi, Xi, ji, p.normal), u.face = p
+        Ai.getNormal(Wi, Xi, ji, p.normal), h.face = p
     }
-    return u
+    return h
 }
-var yr = class r extends St {
+var Sr = class r extends Et {
     constructor(e = 1, t = 1, i = 1, n = 1, a = 1, o = 1) {
         super(), this.type = "BoxGeometry", this.parameters = {
             width: e,
             height: t,
             depth: i,
             widthSegments: n,
             heightSegments: a,
             depthSegments: o
         };
         let s = this;
         n = Math.floor(n), a = Math.floor(a), o = Math.floor(o);
         let l = [],
             c = [],
-            u = [],
+            h = [],
             p = [],
             f = 0,
             m = 0;
-        _("z", "y", "x", -1, -1, i, t, e, o, a, 0), _("z", "y", "x", 1, -1, i, t, -e, o, a, 1), _("x", "z", "y", 1, 1, e, i, t, n, o, 2), _("x", "z", "y", 1, -1, e, i, -t, n, o, 3), _("x", "y", "z", 1, -1, e, t, i, n, a, 4), _("x", "y", "z", -1, -1, e, t, -i, n, a, 5), this.setIndex(l), this.setAttribute("position", new rt(c, 3)), this.setAttribute("normal", new rt(u, 3)), this.setAttribute("uv", new rt(p, 2));
+        _("z", "y", "x", -1, -1, i, t, e, o, a, 0), _("z", "y", "x", 1, -1, i, t, -e, o, a, 1), _("x", "z", "y", 1, 1, e, i, t, n, o, 2), _("x", "z", "y", 1, -1, e, i, -t, n, o, 3), _("x", "y", "z", 1, -1, e, t, i, n, a, 4), _("x", "y", "z", -1, -1, e, t, -i, n, a, 5), this.setIndex(l), this.setAttribute("position", new rt(c, 3)), this.setAttribute("normal", new rt(h, 3)), this.setAttribute("uv", new rt(p, 2));
 
-        function _(M, d, h, w, x, R, U, A, y, C, Z) {
-            let v = R / y,
-                T = U / C,
-                V = R / 2,
-                K = U / 2,
-                P = A / 2,
-                X = y + 1,
-                k = C + 1,
-                j = 0,
+        function _(M, d, u, T, x, A, D, R, b, P, I) {
+            let v = A / b,
+                w = D / P,
+                W = A / 2,
+                K = D / 2,
+                L = R / 2,
+                j = b + 1,
+                k = P + 1,
+                Y = 0,
                 q = 0,
-                W = new D;
-            for (let te = 0; te < k; te++) {
-                let ee = te * T - K;
-                for (let pe = 0; pe < X; pe++) {
-                    let xe = pe * v - V;
-                    W[M] = xe * w, W[d] = ee * x, W[h] = P, c.push(W.x, W.y, W.z), W[M] = 0, W[d] = 0, W[h] = A > 0 ? 1 : -1, u.push(W.x, W.y, W.z), p.push(pe / y), p.push(1 - te / C), j += 1
-                }
-            }
-            for (let te = 0; te < C; te++)
-                for (let ee = 0; ee < y; ee++) {
-                    let pe = f + ee + X * te,
-                        xe = f + ee + X * (te + 1),
-                        H = f + (ee + 1) + X * (te + 1),
-                        ie = f + (ee + 1) + X * te;
-                    l.push(pe, xe, ie), l.push(xe, H, ie), q += 6
+                Z = new U;
+            for (let ee = 0; ee < k; ee++) {
+                let ie = ee * w - K;
+                for (let de = 0; de < j; de++) {
+                    let ge = de * v - W;
+                    Z[M] = ge * T, Z[d] = ie * x, Z[u] = L, c.push(Z.x, Z.y, Z.z), Z[M] = 0, Z[d] = 0, Z[u] = R > 0 ? 1 : -1, h.push(Z.x, Z.y, Z.z), p.push(de / b), p.push(1 - ee / P), Y += 1
+                }
+            }
+            for (let ee = 0; ee < P; ee++)
+                for (let ie = 0; ie < b; ie++) {
+                    let de = f + ie + j * ee,
+                        ge = f + ie + j * (ee + 1),
+                        V = f + (ie + 1) + j * (ee + 1),
+                        te = f + (ie + 1) + j * ee;
+                    l.push(de, ge, te), l.push(ge, V, te), q += 6
                 }
-            s.addGroup(m, q, Z), m += q, f += j
+            s.addGroup(m, q, I), m += q, f += Y
         }
     }
     copy(e) {
         return super.copy(e), this.parameters = Object.assign({}, e.parameters), this
     }
     static fromJSON(e) {
         return new r(e.width, e.height, e.depth, e.widthSegments, e.heightSegments, e.depthSegments)
@@ -4229,50 +4229,50 @@
     for (let t = 0; t < r.length; t++) {
         let i = lr(r[t]);
         for (let n in i) e[n] = i[n]
     }
     return e
 }
 
-function Dc(r) {
+function Uc(r) {
     let e = [];
     for (let t = 0; t < r.length; t++) e.push(r[t].clone());
     return e
 }
 
 function Vo(r) {
     return r.getRenderTarget() === null ? r.outputColorSpace : qe.workingColorSpace
 }
-var Nc = {
+var Ic = {
         clone: lr,
         merge: gt
     },
-    Ic = `void main() {
+    Nc = `void main() {
 	gl_Position = projectionMatrix * modelViewMatrix * vec4( position, 1.0 );
 }`,
     Oc = `void main() {
 	gl_FragColor = vec4( 1.0, 0.0, 0.0, 1.0 );
 }`,
-    Gt = class extends Pi {
+    Ht = class extends Pi {
         constructor(e) {
-            super(), this.isShaderMaterial = !0, this.type = "ShaderMaterial", this.defines = {}, this.uniforms = {}, this.uniformsGroups = [], this.vertexShader = Ic, this.fragmentShader = Oc, this.linewidth = 1, this.wireframe = !1, this.wireframeLinewidth = 1, this.fog = !1, this.lights = !1, this.clipping = !1, this.forceSinglePass = !0, this.extensions = {
+            super(), this.isShaderMaterial = !0, this.type = "ShaderMaterial", this.defines = {}, this.uniforms = {}, this.uniformsGroups = [], this.vertexShader = Nc, this.fragmentShader = Oc, this.linewidth = 1, this.wireframe = !1, this.wireframeLinewidth = 1, this.fog = !1, this.lights = !1, this.clipping = !1, this.forceSinglePass = !0, this.extensions = {
                 derivatives: !1,
                 fragDepth: !1,
                 drawBuffers: !1,
                 shaderTextureLOD: !1,
                 clipCullDistance: !1,
                 multiDraw: !1
             }, this.defaultAttributeValues = {
                 color: [1, 1, 1],
                 uv: [0, 0],
                 uv1: [0, 0]
             }, this.index0AttributeName = void 0, this.uniformsNeedUpdate = !1, this.glslVersion = null, e !== void 0 && this.setValues(e)
         }
         copy(e) {
-            return super.copy(e), this.fragmentShader = e.fragmentShader, this.vertexShader = e.vertexShader, this.uniforms = lr(e.uniforms), this.uniformsGroups = Dc(e.uniformsGroups), this.defines = Object.assign({}, e.defines), this.wireframe = e.wireframe, this.wireframeLinewidth = e.wireframeLinewidth, this.fog = e.fog, this.lights = e.lights, this.clipping = e.clipping, this.extensions = Object.assign({}, e.extensions), this.glslVersion = e.glslVersion, this
+            return super.copy(e), this.fragmentShader = e.fragmentShader, this.vertexShader = e.vertexShader, this.uniforms = lr(e.uniforms), this.uniformsGroups = Uc(e.uniformsGroups), this.defines = Object.assign({}, e.defines), this.wireframe = e.wireframe, this.wireframeLinewidth = e.wireframeLinewidth, this.fog = e.fog, this.lights = e.lights, this.clipping = e.clipping, this.extensions = Object.assign({}, e.extensions), this.glslVersion = e.glslVersion, this
         }
         toJSON(e) {
             let t = super.toJSON(e);
             t.glslVersion = this.glslVersion, t.uniforms = {};
             for (let n in this.uniforms) {
                 let a = this.uniforms[n].value;
                 a && a.isTexture ? t.uniforms[n] = {
@@ -4322,34 +4322,34 @@
         updateWorldMatrix(e, t) {
             super.updateWorldMatrix(e, t), this.matrixWorldInverse.copy(this.matrixWorld).invert()
         }
         clone() {
             return new this.constructor().copy(this)
         }
     },
-    si = new D,
-    Js = new De,
-    $s = new De,
+    si = new U,
+    Js = new Ue,
+    $s = new Ue,
     Mt = class extends fn {
         constructor(e = 50, t = 1, i = .1, n = 2e3) {
             super(), this.isPerspectiveCamera = !0, this.type = "PerspectiveCamera", this.fov = e, this.zoom = 1, this.near = i, this.far = n, this.focus = 10, this.aspect = t, this.view = null, this.filmGauge = 35, this.filmOffset = 0, this.updateProjectionMatrix()
         }
         copy(e, t) {
             return super.copy(e, t), this.fov = e.fov, this.zoom = e.zoom, this.near = e.near, this.far = e.far, this.focus = e.focus, this.aspect = e.aspect, this.view = e.view === null ? null : Object.assign({}, e.view), this.filmGauge = e.filmGauge, this.filmOffset = e.filmOffset, this
         }
         setFocalLength(e) {
             let t = .5 * this.getFilmHeight() / e;
-            this.fov = Er * 2 * Math.atan(t), this.updateProjectionMatrix()
+            this.fov = yr * 2 * Math.atan(t), this.updateProjectionMatrix()
         }
         getFocalLength() {
             let e = Math.tan(tr * .5 * this.fov);
             return .5 * this.getFilmHeight() / e
         }
         getEffectiveFOV() {
-            return Er * 2 * Math.atan(Math.tan(tr * .5 * this.fov) / this.zoom)
+            return yr * 2 * Math.atan(Math.tan(tr * .5 * this.fov) / this.zoom)
         }
         getFilmWidth() {
             return this.filmGauge * Math.min(this.aspect, 1)
         }
         getFilmHeight() {
             return this.filmGauge / Math.max(this.aspect, 1)
         }
@@ -4391,15 +4391,15 @@
         toJSON(e) {
             let t = super.toJSON(e);
             return t.object.fov = this.fov, t.object.zoom = this.zoom, t.object.near = this.near, t.object.far = this.far, t.object.focus = this.focus, t.object.aspect = this.aspect, this.view !== null && (t.object.view = Object.assign({}, this.view)), t.object.filmGauge = this.filmGauge, t.object.filmOffset = this.filmOffset, t
         }
     },
     Yi = -90,
     qi = 1,
-    Sa = class extends wt {
+    Ea = class extends wt {
         constructor(e, t, i) {
             super(), this.type = "CubeCamera", this.renderTarget = i, this.coordinateSystem = null, this.activeMipmapLevel = 0;
             let n = new Mt(Yi, qi, e, t);
             n.layers = this.layers, this.add(n);
             let a = new Mt(Yi, qi, e, t);
             a.layers = this.layers, this.add(a);
             let o = new Mt(Yi, qi, e, t);
@@ -4424,32 +4424,32 @@
         update(e, t) {
             this.parent === null && this.updateMatrixWorld();
             let {
                 renderTarget: i,
                 activeMipmapLevel: n
             } = this;
             this.coordinateSystem !== e.coordinateSystem && (this.coordinateSystem = e.coordinateSystem, this.updateCoordinateSystem());
-            let [a, o, s, l, c, u] = this.children, p = e.getRenderTarget(), f = e.getActiveCubeFace(), m = e.getActiveMipmapLevel(), _ = e.xr.enabled;
+            let [a, o, s, l, c, h] = this.children, p = e.getRenderTarget(), f = e.getActiveCubeFace(), m = e.getActiveMipmapLevel(), _ = e.xr.enabled;
             e.xr.enabled = !1;
             let M = i.texture.generateMipmaps;
-            i.texture.generateMipmaps = !1, e.setRenderTarget(i, 0, n), e.render(t, a), e.setRenderTarget(i, 1, n), e.render(t, o), e.setRenderTarget(i, 2, n), e.render(t, s), e.setRenderTarget(i, 3, n), e.render(t, l), e.setRenderTarget(i, 4, n), e.render(t, c), i.texture.generateMipmaps = M, e.setRenderTarget(i, 5, n), e.render(t, u), e.setRenderTarget(p, f, m), e.xr.enabled = _, i.texture.needsPMREMUpdate = !0
+            i.texture.generateMipmaps = !1, e.setRenderTarget(i, 0, n), e.render(t, a), e.setRenderTarget(i, 1, n), e.render(t, o), e.setRenderTarget(i, 2, n), e.render(t, s), e.setRenderTarget(i, 3, n), e.render(t, l), e.setRenderTarget(i, 4, n), e.render(t, c), i.texture.generateMipmaps = M, e.setRenderTarget(i, 5, n), e.render(t, h), e.setRenderTarget(p, f, m), e.xr.enabled = _, i.texture.needsPMREMUpdate = !0
         }
     },
     mn = class extends Pt {
-        constructor(e, t, i, n, a, o, s, l, c, u) {
-            e = e !== void 0 ? e : [], t = t !== void 0 ? t : nr, super(e, t, i, n, a, o, s, l, c, u), this.isCubeTexture = !0, this.flipY = !1
+        constructor(e, t, i, n, a, o, s, l, c, h) {
+            e = e !== void 0 ? e : [], t = t !== void 0 ? t : nr, super(e, t, i, n, a, o, s, l, c, h), this.isCubeTexture = !0, this.flipY = !1
         }
         get images() {
             return this.image
         }
         set images(e) {
             this.image = e
         }
     },
-    ya = class extends $t {
+    Sa = class extends $t {
         constructor(e = 1, t = {}) {
             super(e, e, t), this.isWebGLCubeRenderTarget = !0;
             let i = {
                     width: e,
                     height: e,
                     depth: 1
                 },
@@ -4498,39 +4498,39 @@
 					vec2 sampleUV = equirectUv( direction );
 
 					gl_FragColor = texture2D( tEquirect, sampleUV );
 
 				}
 			`
                 },
-                n = new yr(5, 5, 5),
-                a = new Gt({
+                n = new Sr(5, 5, 5),
+                a = new Ht({
                     name: "CubemapFromEquirect",
                     uniforms: lr(i.uniforms),
                     vertexShader: i.vertexShader,
                     fragmentShader: i.fragmentShader,
-                    side: Et,
+                    side: yt,
                     blending: ci
                 });
             a.uniforms.tEquirect.value = t;
             let o = new vt(n, a),
                 s = t.minFilter;
-            return t.minFilter === wi && (t.minFilter = xt), new Sa(1, 10, this).update(e, o), t.minFilter = s, o.geometry.dispose(), o.material.dispose(), this
+            return t.minFilter === wi && (t.minFilter = xt), new Ea(1, 10, this).update(e, o), t.minFilter = s, o.geometry.dispose(), o.material.dispose(), this
         }
         clear(e, t, i, n) {
             let a = e.getRenderTarget();
             for (let o = 0; o < 6; o++) e.setRenderTarget(this, o), e.clear(t, i, n);
             e.setRenderTarget(a)
         }
     },
-    ia = new D,
-    Fc = new D,
-    Bc = new Be,
-    Bt = class {
-        constructor(e = new D(1, 0, 0), t = 0) {
+    ia = new U,
+    Fc = new U,
+    zc = new ze,
+    zt = class {
+        constructor(e = new U(1, 0, 0), t = 0) {
             this.isPlane = !0, this.normal = e, this.constant = t
         }
         set(e, t) {
             return this.normal.copy(e), this.constant = t, this
         }
         setComponents(e, t, i, n) {
             return this.normal.set(e, t, i), this.constant = n, this
@@ -4579,15 +4579,15 @@
         intersectsSphere(e) {
             return e.intersectsPlane(this)
         }
         coplanarPoint(e) {
             return e.copy(this.normal).multiplyScalar(-this.constant)
         }
         applyMatrix4(e, t) {
-            let i = t || Bc.getNormalMatrix(e),
+            let i = t || zc.getNormalMatrix(e),
                 n = this.coplanarPoint(ia).applyMatrix4(e),
                 a = this.normal.applyMatrix3(i).normalize();
             return this.constant = -n.dot(a), this
         }
         translate(e) {
             return this.constant -= e.dot(this.normal), this
         }
@@ -4595,17 +4595,17 @@
             return e.normal.equals(this.normal) && e.constant === this.constant
         }
         clone() {
             return new this.constructor().copy(this)
         }
     },
     Mi = new or,
-    Xr = new D,
+    Xr = new U,
     gn = class {
-        constructor(e = new Bt, t = new Bt, i = new Bt, n = new Bt, a = new Bt, o = new Bt) {
+        constructor(e = new zt, t = new zt, i = new zt, n = new zt, a = new zt, o = new zt) {
             this.planes = [e, t, i, n, a, o]
         }
         set(e, t, i, n, a, o) {
             let s = this.planes;
             return s[0].copy(e), s[1].copy(t), s[2].copy(i), s[3].copy(n), s[4].copy(a), s[5].copy(o), this
         }
         copy(e) {
@@ -4617,26 +4617,26 @@
             let i = this.planes,
                 n = e.elements,
                 a = n[0],
                 o = n[1],
                 s = n[2],
                 l = n[3],
                 c = n[4],
-                u = n[5],
+                h = n[5],
                 p = n[6],
                 f = n[7],
                 m = n[8],
                 _ = n[9],
                 M = n[10],
                 d = n[11],
-                h = n[12],
-                w = n[13],
+                u = n[12],
+                T = n[13],
                 x = n[14],
-                R = n[15];
-            if (i[0].setComponents(l - a, f - c, d - m, R - h).normalize(), i[1].setComponents(l + a, f + c, d + m, R + h).normalize(), i[2].setComponents(l + o, f + u, d + _, R + w).normalize(), i[3].setComponents(l - o, f - u, d - _, R - w).normalize(), i[4].setComponents(l - s, f - p, d - M, R - x).normalize(), t === Kt) i[5].setComponents(l + s, f + p, d + M, R + x).normalize();
+                A = n[15];
+            if (i[0].setComponents(l - a, f - c, d - m, A - u).normalize(), i[1].setComponents(l + a, f + c, d + m, A + u).normalize(), i[2].setComponents(l + o, f + h, d + _, A + T).normalize(), i[3].setComponents(l - o, f - h, d - _, A - T).normalize(), i[4].setComponents(l - s, f - p, d - M, A - x).normalize(), t === Kt) i[5].setComponents(l + s, f + p, d + M, A + x).normalize();
             else if (t === an) i[5].setComponents(s, p, M, x).normalize();
             else throw new Error("THREE.Frustum.setFromProjectionMatrix(): Invalid coordinate system: " + t);
             return this
         }
         intersectsObject(e) {
             if (e.boundingSphere !== void 0) e.boundingSphere === null && e.computeBoundingSphere(), Mi.copy(e.boundingSphere).applyMatrix4(e.matrixWorld);
             else {
@@ -4696,24 +4696,24 @@
         },
         setContext: function(a) {
             r = a
         }
     }
 }
 
-function zc(r, e) {
+function Bc(r, e) {
     let t = e.isWebGL2,
         i = new WeakMap;
 
-    function n(c, u) {
+    function n(c, h) {
         let p = c.array,
             f = c.usage,
             m = p.byteLength,
             _ = r.createBuffer();
-        r.bindBuffer(u, _), r.bufferData(u, p, f), c.onUploadCallback();
+        r.bindBuffer(h, _), r.bufferData(h, p, f), c.onUploadCallback();
         let M;
         if (p instanceof Float32Array) M = r.FLOAT;
         else if (p instanceof Uint16Array)
             if (c.isFloat16BufferAttribute)
                 if (t) M = r.HALF_FLOAT;
                 else throw new Error("THREE.WebGLAttributes: Usage of Float16BufferAttribute requires WebGL2.");
         else M = r.UNSIGNED_SHORT;
@@ -4729,111 +4729,111 @@
             type: M,
             bytesPerElement: p.BYTES_PER_ELEMENT,
             version: c.version,
             size: m
         }
     }
 
-    function a(c, u, p) {
-        let f = u.array,
-            m = u._updateRange,
-            _ = u.updateRanges;
+    function a(c, h, p) {
+        let f = h.array,
+            m = h._updateRange,
+            _ = h.updateRanges;
         if (r.bindBuffer(p, c), m.count === -1 && _.length === 0 && r.bufferSubData(p, 0, f), _.length !== 0) {
             for (let M = 0, d = _.length; M < d; M++) {
-                let h = _[M];
-                t ? r.bufferSubData(p, h.start * f.BYTES_PER_ELEMENT, f, h.start, h.count) : r.bufferSubData(p, h.start * f.BYTES_PER_ELEMENT, f.subarray(h.start, h.start + h.count))
+                let u = _[M];
+                t ? r.bufferSubData(p, u.start * f.BYTES_PER_ELEMENT, f, u.start, u.count) : r.bufferSubData(p, u.start * f.BYTES_PER_ELEMENT, f.subarray(u.start, u.start + u.count))
             }
-            u.clearUpdateRanges()
+            h.clearUpdateRanges()
         }
-        m.count !== -1 && (t ? r.bufferSubData(p, m.offset * f.BYTES_PER_ELEMENT, f, m.offset, m.count) : r.bufferSubData(p, m.offset * f.BYTES_PER_ELEMENT, f.subarray(m.offset, m.offset + m.count)), m.count = -1), u.onUploadCallback()
+        m.count !== -1 && (t ? r.bufferSubData(p, m.offset * f.BYTES_PER_ELEMENT, f, m.offset, m.count) : r.bufferSubData(p, m.offset * f.BYTES_PER_ELEMENT, f.subarray(m.offset, m.offset + m.count)), m.count = -1), h.onUploadCallback()
     }
 
     function o(c) {
         return c.isInterleavedBufferAttribute && (c = c.data), i.get(c)
     }
 
     function s(c) {
         c.isInterleavedBufferAttribute && (c = c.data);
-        let u = i.get(c);
-        u && (r.deleteBuffer(u.buffer), i.delete(c))
+        let h = i.get(c);
+        h && (r.deleteBuffer(h.buffer), i.delete(c))
     }
 
-    function l(c, u) {
+    function l(c, h) {
         if (c.isGLBufferAttribute) {
             let f = i.get(c);
             (!f || f.version < c.version) && i.set(c, {
                 buffer: c.buffer,
                 type: c.type,
                 bytesPerElement: c.elementSize,
                 version: c.version
             });
             return
         }
         c.isInterleavedBufferAttribute && (c = c.data);
         let p = i.get(c);
-        if (p === void 0) i.set(c, n(c, u));
+        if (p === void 0) i.set(c, n(c, h));
         else if (p.version < c.version) {
             if (p.size !== c.array.byteLength) throw new Error("THREE.WebGLAttributes: The size of the buffer attribute's array buffer does not match the original size. Resizing buffer attributes is not supported.");
-            a(p.buffer, c, u), p.version = c.version
+            a(p.buffer, c, h), p.version = c.version
         }
     }
     return {
         get: o,
         remove: s,
         update: l
     }
 }
-var _n = class r extends St {
+var _n = class r extends Et {
         constructor(e = 1, t = 1, i = 1, n = 1) {
             super(), this.type = "PlaneGeometry", this.parameters = {
                 width: e,
                 height: t,
                 widthSegments: i,
                 heightSegments: n
             };
             let a = e / 2,
                 o = t / 2,
                 s = Math.floor(i),
                 l = Math.floor(n),
                 c = s + 1,
-                u = l + 1,
+                h = l + 1,
                 p = e / s,
                 f = t / l,
                 m = [],
                 _ = [],
                 M = [],
                 d = [];
-            for (let h = 0; h < u; h++) {
-                let w = h * f - o;
+            for (let u = 0; u < h; u++) {
+                let T = u * f - o;
                 for (let x = 0; x < c; x++) {
-                    let R = x * p - a;
-                    _.push(R, -w, 0), M.push(0, 0, 1), d.push(x / s), d.push(1 - h / l)
+                    let A = x * p - a;
+                    _.push(A, -T, 0), M.push(0, 0, 1), d.push(x / s), d.push(1 - u / l)
                 }
             }
-            for (let h = 0; h < l; h++)
-                for (let w = 0; w < s; w++) {
-                    let x = w + c * h,
-                        R = w + c * (h + 1),
-                        U = w + 1 + c * (h + 1),
-                        A = w + 1 + c * h;
-                    m.push(x, R, A), m.push(R, U, A)
+            for (let u = 0; u < l; u++)
+                for (let T = 0; T < s; T++) {
+                    let x = T + c * u,
+                        A = T + c * (u + 1),
+                        D = T + 1 + c * (u + 1),
+                        R = T + 1 + c * u;
+                    m.push(x, A, R), m.push(A, D, R)
                 }
             this.setIndex(m), this.setAttribute("position", new rt(_, 3)), this.setAttribute("normal", new rt(M, 3)), this.setAttribute("uv", new rt(d, 2))
         }
         copy(e) {
             return super.copy(e), this.parameters = Object.assign({}, e.parameters), this
         }
         static fromJSON(e) {
             return new r(e.width, e.height, e.widthSegments, e.heightSegments)
         }
     },
-    Gc = `#ifdef USE_ALPHAHASH
+    Hc = `#ifdef USE_ALPHAHASH
 	if ( diffuseColor.a < getAlphaHashThreshold( vPosition ) ) discard;
 #endif`,
-    Hc = `#ifdef USE_ALPHAHASH
+    Gc = `#ifdef USE_ALPHAHASH
 	const float ALPHA_HASH_SCALE = 0.05;
 	float hash2D( vec2 value ) {
 		return fract( 1.0e4 * sin( 17.0 * value.x + 0.1 * value.y ) * ( 0.1 + abs( sin( 13.0 * value.y + value.x ) ) ) );
 	}
 	float hash3D( vec3 value ) {
 		return hash2D( vec2( hash2D( value.xy ), value.z ) );
 	}
@@ -5407,27 +5407,27 @@
 	#ifdef ENV_WORLDPOS
 		varying vec3 vWorldPosition;
 		uniform float refractionRatio;
 	#else
 		varying vec3 vReflect;
 	#endif
 #endif`,
-    Eh = `#ifdef USE_ENVMAP
+    yh = `#ifdef USE_ENVMAP
 	#if defined( USE_BUMPMAP ) || defined( USE_NORMALMAP ) || defined( PHONG ) || defined( LAMBERT )
 		#define ENV_WORLDPOS
 	#endif
 	#ifdef ENV_WORLDPOS
 		
 		varying vec3 vWorldPosition;
 	#else
 		varying vec3 vReflect;
 		uniform float refractionRatio;
 	#endif
 #endif`,
-    Sh = `#ifdef USE_ENVMAP
+    Eh = `#ifdef USE_ENVMAP
 	#ifdef ENV_WORLDPOS
 		vWorldPosition = worldPosition.xyz;
 	#else
 		vec3 cameraToVertex;
 		if ( isOrthographic ) {
 			cameraToVertex = normalize( vec3( - viewMatrix[ 0 ][ 2 ], - viewMatrix[ 1 ][ 2 ], - viewMatrix[ 2 ][ 2 ] ) );
 		} else {
@@ -5437,21 +5437,21 @@
 		#ifdef ENVMAP_MODE_REFLECTION
 			vReflect = reflect( cameraToVertex, worldNormal );
 		#else
 			vReflect = refract( cameraToVertex, worldNormal, refractionRatio );
 		#endif
 	#endif
 #endif`,
-    yh = `#ifdef USE_FOG
+    Sh = `#ifdef USE_FOG
 	vFogDepth = - mvPosition.z;
 #endif`,
-    bh = `#ifdef USE_FOG
+    Th = `#ifdef USE_FOG
 	varying float vFogDepth;
 #endif`,
-    Th = `#ifdef USE_FOG
+    bh = `#ifdef USE_FOG
 	#ifdef FOG_EXP2
 		float fogFactor = 1.0 - exp( - fogDensity * fogDensity * vFogDepth * vFogDepth );
 	#else
 		float fogFactor = smoothstep( fogNear, fogFar, vFogDepth );
 	#endif
 	gl_FragColor.rgb = mix( gl_FragColor.rgb, fogColor, fogFactor );
 #endif`,
@@ -5501,15 +5501,15 @@
 	reflectedLight.directDiffuse += irradiance * BRDF_Lambert( material.diffuseColor );
 }
 void RE_IndirectDiffuse_Lambert( const in vec3 irradiance, const in vec3 geometryPosition, const in vec3 geometryNormal, const in vec3 geometryViewDir, const in vec3 geometryClearcoatNormal, const in LambertMaterial material, inout ReflectedLight reflectedLight ) {
 	reflectedLight.indirectDiffuse += irradiance * BRDF_Lambert( material.diffuseColor );
 }
 #define RE_Direct				RE_Direct_Lambert
 #define RE_IndirectDiffuse		RE_IndirectDiffuse_Lambert`,
-    Uh = `uniform bool receiveShadow;
+    Dh = `uniform bool receiveShadow;
 uniform vec3 ambientLightColor;
 #if defined( USE_LIGHT_PROBES )
 	uniform vec3 lightProbe[ 9 ];
 #endif
 vec3 shGetIrradianceAt( in vec3 normal, in vec3 shCoefficients[ 9 ] ) {
 	float x = normal.x, y = normal.y, z = normal.z;
 	vec3 result = shCoefficients[ 0 ] * 0.886227;
@@ -5625,15 +5625,15 @@
 	vec3 getHemisphereLightIrradiance( const in HemisphereLight hemiLight, const in vec3 normal ) {
 		float dotNL = dot( normal, hemiLight.direction );
 		float hemiDiffuseWeight = 0.5 * dotNL + 0.5;
 		vec3 irradiance = mix( hemiLight.groundColor, hemiLight.skyColor, hemiDiffuseWeight );
 		return irradiance;
 	}
 #endif`,
-    Dh = `#ifdef USE_ENVMAP
+    Uh = `#ifdef USE_ENVMAP
 	vec3 getIBLIrradiance( const in vec3 normal ) {
 		#ifdef ENVMAP_TYPE_CUBE_UV
 			vec3 worldNormal = inverseTransformDirection( normal, viewMatrix );
 			vec4 envMapColor = textureCubeUV( envMap, envMapRotation * worldNormal, 1.0 );
 			return PI * envMapColor.rgb * envMapIntensity;
 		#else
 			return vec3( 0.0 );
@@ -5659,17 +5659,17 @@
 				return getIBLRadiance( viewDir, bentNormal, roughness );
 			#else
 				return vec3( 0.0 );
 			#endif
 		}
 	#endif
 #endif`,
-    Nh = `ToonMaterial material;
+    Ih = `ToonMaterial material;
 material.diffuseColor = diffuseColor.rgb;`,
-    Ih = `varying vec3 vViewPosition;
+    Nh = `varying vec3 vViewPosition;
 struct ToonMaterial {
 	vec3 diffuseColor;
 };
 void RE_Direct_Toon( const in IncidentLight directLight, const in vec3 geometryPosition, const in vec3 geometryNormal, const in vec3 geometryViewDir, const in vec3 geometryClearcoatNormal, const in ToonMaterial material, inout ReflectedLight reflectedLight ) {
 	vec3 irradiance = getGradientIrradiance( geometryNormal, directLight.direction ) * directLight.color;
 	reflectedLight.directDiffuse += irradiance * BRDF_Lambert( material.diffuseColor );
 }
@@ -5697,15 +5697,15 @@
 	reflectedLight.directSpecular += irradiance * BRDF_BlinnPhong( directLight.direction, geometryViewDir, geometryNormal, material.specularColor, material.specularShininess ) * material.specularStrength;
 }
 void RE_IndirectDiffuse_BlinnPhong( const in vec3 irradiance, const in vec3 geometryPosition, const in vec3 geometryNormal, const in vec3 geometryViewDir, const in vec3 geometryClearcoatNormal, const in BlinnPhongMaterial material, inout ReflectedLight reflectedLight ) {
 	reflectedLight.indirectDiffuse += irradiance * BRDF_Lambert( material.diffuseColor );
 }
 #define RE_Direct				RE_Direct_BlinnPhong
 #define RE_IndirectDiffuse		RE_IndirectDiffuse_BlinnPhong`,
-    Bh = `PhysicalMaterial material;
+    zh = `PhysicalMaterial material;
 material.diffuseColor = diffuseColor.rgb * ( 1.0 - metalnessFactor );
 vec3 dxy = max( abs( dFdx( nonPerturbedNormal ) ), abs( dFdy( nonPerturbedNormal ) ) );
 float geometryRoughness = max( max( dxy.x, dxy.y ), dxy.z );
 material.roughness = max( roughnessFactor, 0.0525 );material.roughness += geometryRoughness;
 material.roughness = min( material.roughness, 1.0 );
 #ifdef IOR
 	material.ior = ior;
@@ -5781,15 +5781,15 @@
 		anisotropyV /= material.anisotropy;
 		material.anisotropy = saturate( material.anisotropy );
 	}
 	material.alphaT = mix( pow2( material.roughness ), 1.0, pow2( material.anisotropy ) );
 	material.anisotropyT = tbn[ 0 ] * anisotropyV.x + tbn[ 1 ] * anisotropyV.y;
 	material.anisotropyB = tbn[ 1 ] * anisotropyV.x - tbn[ 0 ] * anisotropyV.y;
 #endif`,
-    zh = `struct PhysicalMaterial {
+    Bh = `struct PhysicalMaterial {
 	vec3 diffuseColor;
 	float roughness;
 	vec3 specularColor;
 	float specularF90;
 	#ifdef USE_CLEARCOAT
 		float clearcoat;
 		float clearcoatRoughness;
@@ -6082,15 +6082,15 @@
 #define RE_Direct				RE_Direct_Physical
 #define RE_Direct_RectArea		RE_Direct_RectArea_Physical
 #define RE_IndirectDiffuse		RE_IndirectDiffuse_Physical
 #define RE_IndirectSpecular		RE_IndirectSpecular_Physical
 float computeSpecularOcclusion( const in float dotNV, const in float ambientOcclusion, const in float roughness ) {
 	return saturate( pow( dotNV + ambientOcclusion, exp2( - 16.0 * roughness - 1.0 ) ) - 1.0 + ambientOcclusion );
 }`,
-    Gh = `
+    Hh = `
 vec3 geometryPosition = - vViewPosition;
 vec3 geometryNormal = normal;
 vec3 geometryViewDir = ( isOrthographic ) ? vec3( 0, 0, 1 ) : normalize( vViewPosition );
 vec3 geometryClearcoatNormal = vec3( 0.0 );
 #ifdef USE_CLEARCOAT
 	geometryClearcoatNormal = clearcoatNormal;
 #endif
@@ -6198,15 +6198,15 @@
 		#pragma unroll_loop_end
 	#endif
 #endif
 #if defined( RE_IndirectSpecular )
 	vec3 radiance = vec3( 0.0 );
 	vec3 clearcoatRadiance = vec3( 0.0 );
 #endif`,
-    Hh = `#if defined( RE_IndirectDiffuse )
+    Gh = `#if defined( RE_IndirectDiffuse )
 	#ifdef USE_LIGHTMAP
 		vec4 lightMapTexel = texture2D( lightMap, vLightMapUv );
 		vec3 lightMapIrradiance = lightMapTexel.rgb * lightMapIntensity;
 		irradiance += lightMapIrradiance;
 	#endif
 	#if defined( USE_ENVMAP ) && defined( STANDARD ) && defined( ENVMAP_TYPE_CUBE_UV )
 		iblIrradiance += getIBLIrradiance( geometryNormal );
@@ -6573,18 +6573,18 @@
 	}
 #endif`,
     Mu = `float roughnessFactor = roughness;
 #ifdef USE_ROUGHNESSMAP
 	vec4 texelRoughness = texture2D( roughnessMap, vRoughnessMapUv );
 	roughnessFactor *= texelRoughness.g;
 #endif`,
-    Eu = `#ifdef USE_ROUGHNESSMAP
+    yu = `#ifdef USE_ROUGHNESSMAP
 	uniform sampler2D roughnessMap;
 #endif`,
-    Su = `#if NUM_SPOT_LIGHT_COORDS > 0
+    Eu = `#if NUM_SPOT_LIGHT_COORDS > 0
 	varying vec4 vSpotLightCoord[ NUM_SPOT_LIGHT_COORDS ];
 #endif
 #if NUM_SPOT_LIGHT_MAPS > 0
 	uniform sampler2D spotLightMap[ NUM_SPOT_LIGHT_MAPS ];
 #endif
 #ifdef USE_SHADOWMAP
 	#if NUM_DIR_LIGHT_SHADOWS > 0
@@ -6754,15 +6754,15 @@
 				texture2DCompare( shadowMap, cubeToUV( bd3D + offset.yxx, texelSize.y ), dp )
 			) * ( 1.0 / 9.0 );
 		#else
 			return texture2DCompare( shadowMap, cubeToUV( bd3D, texelSize.y ), dp );
 		#endif
 	}
 #endif`,
-    yu = `#if NUM_SPOT_LIGHT_COORDS > 0
+    Su = `#if NUM_SPOT_LIGHT_COORDS > 0
 	uniform mat4 spotLightMatrix[ NUM_SPOT_LIGHT_COORDS ];
 	varying vec4 vSpotLightCoord[ NUM_SPOT_LIGHT_COORDS ];
 #endif
 #ifdef USE_SHADOWMAP
 	#if NUM_DIR_LIGHT_SHADOWS > 0
 		uniform mat4 directionalShadowMatrix[ NUM_DIR_LIGHT_SHADOWS ];
 		varying vec4 vDirectionalShadowCoord[ NUM_DIR_LIGHT_SHADOWS ];
@@ -6793,15 +6793,15 @@
 			vec2 shadowMapSize;
 			float shadowCameraNear;
 			float shadowCameraFar;
 		};
 		uniform PointLightShadow pointLightShadows[ NUM_POINT_LIGHT_SHADOWS ];
 	#endif
 #endif`,
-    bu = `#if ( defined( USE_SHADOWMAP ) && ( NUM_DIR_LIGHT_SHADOWS > 0 || NUM_POINT_LIGHT_SHADOWS > 0 ) ) || ( NUM_SPOT_LIGHT_COORDS > 0 )
+    Tu = `#if ( defined( USE_SHADOWMAP ) && ( NUM_DIR_LIGHT_SHADOWS > 0 || NUM_POINT_LIGHT_SHADOWS > 0 ) ) || ( NUM_SPOT_LIGHT_COORDS > 0 )
 	vec3 shadowWorldNormal = inverseTransformDirection( transformedNormal, viewMatrix );
 	vec4 shadowWorldPosition;
 #endif
 #if defined( USE_SHADOWMAP )
 	#if NUM_DIR_LIGHT_SHADOWS > 0
 		#pragma unroll_loop_start
 		for ( int i = 0; i < NUM_DIR_LIGHT_SHADOWS; i ++ ) {
@@ -6826,15 +6826,15 @@
 		#if ( defined( USE_SHADOWMAP ) && UNROLLED_LOOP_INDEX < NUM_SPOT_LIGHT_SHADOWS )
 			shadowWorldPosition.xyz += shadowWorldNormal * spotLightShadows[ i ].shadowNormalBias;
 		#endif
 		vSpotLightCoord[ i ] = spotLightMatrix[ i ] * shadowWorldPosition;
 	}
 	#pragma unroll_loop_end
 #endif`,
-    Tu = `float getShadowMask() {
+    bu = `float getShadowMask() {
 	float shadow = 1.0;
 	#ifdef USE_SHADOWMAP
 	#if NUM_DIR_LIGHT_SHADOWS > 0
 	DirectionalLightShadow directionalLight;
 	#pragma unroll_loop_start
 	for ( int i = 0; i < NUM_DIR_LIGHT_SHADOWS; i ++ ) {
 		directionalLight = directionalLightShadows[ i ];
@@ -6912,18 +6912,18 @@
 	specularStrength = texelSpecular.r;
 #else
 	specularStrength = 1.0;
 #endif`,
     Pu = `#ifdef USE_SPECULARMAP
 	uniform sampler2D specularMap;
 #endif`,
-    Uu = `#if defined( TONE_MAPPING )
+    Du = `#if defined( TONE_MAPPING )
 	gl_FragColor.rgb = toneMapping( gl_FragColor.rgb );
 #endif`,
-    Du = `#ifndef saturate
+    Uu = `#ifndef saturate
 #define saturate( a ) clamp( a, 0.0, 1.0 )
 #endif
 uniform float toneMappingExposure;
 vec3 LinearToneMapping( vec3 color ) {
 	return saturate( toneMappingExposure * color );
 }
 vec3 ReinhardToneMapping( vec3 color ) {
@@ -7013,15 +7013,15 @@
 	float d = 1. - startCompression;
 	float newPeak = 1. - d * d / (peak + d - startCompression);
 	color *= newPeak / peak;
 	float g = 1. - 1. / (desaturation * (peak - newPeak) + 1.);
 	return mix(color, vec3(1, 1, 1), g);
 }
 vec3 CustomToneMapping( vec3 color ) { return color; }`,
-    Nu = `#ifdef USE_TRANSMISSION
+    Iu = `#ifdef USE_TRANSMISSION
 	material.transmission = transmission;
 	material.transmissionAlpha = 1.0;
 	material.thickness = thickness;
 	material.attenuationDistance = attenuationDistance;
 	material.attenuationColor = attenuationColor;
 	#ifdef USE_TRANSMISSIONMAP
 		material.transmission *= texture2D( transmissionMap, vTransmissionMapUv ).r;
@@ -7035,15 +7035,15 @@
 	vec4 transmitted = getIBLVolumeRefraction(
 		n, v, material.roughness, material.diffuseColor, material.specularColor, material.specularF90,
 		pos, modelMatrix, viewMatrix, projectionMatrix, material.ior, material.thickness,
 		material.attenuationColor, material.attenuationDistance );
 	material.transmissionAlpha = mix( material.transmissionAlpha, transmitted.a, material.transmission );
 	totalDiffuse = mix( totalDiffuse, transmitted.rgb, material.transmission );
 #endif`,
-    Iu = `#ifdef USE_TRANSMISSION
+    Nu = `#ifdef USE_TRANSMISSION
 	uniform float transmission;
 	uniform float thickness;
 	uniform float attenuationDistance;
 	uniform vec3 attenuationColor;
 	#ifdef USE_TRANSMISSIONMAP
 		uniform sampler2D transmissionMap;
 	#endif
@@ -7308,15 +7308,15 @@
 	uniform mat3 transmissionMapTransform;
 	varying vec2 vTransmissionMapUv;
 #endif
 #ifdef USE_THICKNESSMAP
 	uniform mat3 thicknessMapTransform;
 	varying vec2 vThicknessMapUv;
 #endif`,
-    Bu = `#if defined( USE_UV ) || defined( USE_ANISOTROPY )
+    zu = `#if defined( USE_UV ) || defined( USE_ANISOTROPY )
 	vUv = vec3( uv, 1 ).xy;
 #endif
 #ifdef USE_MAP
 	vMapUv = ( mapTransform * vec3( MAP_UV, 1 ) ).xy;
 #endif
 #ifdef USE_ALPHAMAP
 	vAlphaMapUv = ( alphaMapTransform * vec3( ALPHAMAP_UV, 1 ) ).xy;
@@ -7380,31 +7380,31 @@
 #endif
 #ifdef USE_TRANSMISSIONMAP
 	vTransmissionMapUv = ( transmissionMapTransform * vec3( TRANSMISSIONMAP_UV, 1 ) ).xy;
 #endif
 #ifdef USE_THICKNESSMAP
 	vThicknessMapUv = ( thicknessMapTransform * vec3( THICKNESSMAP_UV, 1 ) ).xy;
 #endif`,
-    zu = `#if defined( USE_ENVMAP ) || defined( DISTANCE ) || defined ( USE_SHADOWMAP ) || defined ( USE_TRANSMISSION ) || NUM_SPOT_LIGHT_COORDS > 0
+    Bu = `#if defined( USE_ENVMAP ) || defined( DISTANCE ) || defined ( USE_SHADOWMAP ) || defined ( USE_TRANSMISSION ) || NUM_SPOT_LIGHT_COORDS > 0
 	vec4 worldPosition = vec4( transformed, 1.0 );
 	#ifdef USE_BATCHING
 		worldPosition = batchingMatrix * worldPosition;
 	#endif
 	#ifdef USE_INSTANCING
 		worldPosition = instanceMatrix * worldPosition;
 	#endif
 	worldPosition = modelMatrix * worldPosition;
 #endif`,
-    Gu = `varying vec2 vUv;
+    Hu = `varying vec2 vUv;
 uniform mat3 uvTransform;
 void main() {
 	vUv = ( uvTransform * vec3( uv, 1 ) ).xy;
 	gl_Position = vec4( position.xy, 1.0, 1.0 );
 }`,
-    Hu = `uniform sampler2D t2D;
+    Gu = `uniform sampler2D t2D;
 uniform float backgroundIntensity;
 varying vec2 vUv;
 void main() {
 	vec4 texColor = texture2D( t2D, vUv );
 	#ifdef DECODE_VIDEO_TEXTURE
 		texColor = vec4( mix( pow( texColor.rgb * 0.9478672986 + vec3( 0.0521327014 ), vec3( 2.4 ) ), texColor.rgb * 0.0773993808, vec3( lessThanEqual( texColor.rgb, vec3( 0.04045 ) ) ) ), texColor.w );
 	#endif
@@ -8472,16 +8472,16 @@
 	outgoingLight = diffuseColor.rgb;
 	#include <opaque_fragment>
 	#include <tonemapping_fragment>
 	#include <colorspace_fragment>
 	#include <fog_fragment>
 }`,
     Fe = {
-        alphahash_fragment: Gc,
-        alphahash_pars_fragment: Hc,
+        alphahash_fragment: Hc,
+        alphahash_pars_fragment: Gc,
         alphamap_fragment: kc,
         alphamap_pars_fragment: Vc,
         alphatest_fragment: Wc,
         alphatest_pars_fragment: Xc,
         aomap_fragment: jc,
         aomap_pars_fragment: Yc,
         batching_pars_vertex: qc,
@@ -8507,35 +8507,35 @@
         emissivemap_fragment: fh,
         emissivemap_pars_fragment: mh,
         colorspace_fragment: gh,
         colorspace_pars_fragment: _h,
         envmap_fragment: vh,
         envmap_common_pars_fragment: xh,
         envmap_pars_fragment: Mh,
-        envmap_pars_vertex: Eh,
-        envmap_physical_pars_fragment: Dh,
-        envmap_vertex: Sh,
-        fog_vertex: yh,
-        fog_pars_vertex: bh,
-        fog_fragment: Th,
+        envmap_pars_vertex: yh,
+        envmap_physical_pars_fragment: Uh,
+        envmap_vertex: Eh,
+        fog_vertex: Sh,
+        fog_pars_vertex: Th,
+        fog_fragment: bh,
         fog_pars_fragment: wh,
         gradientmap_pars_fragment: Ah,
         lightmap_fragment: Rh,
         lightmap_pars_fragment: Ch,
         lights_lambert_fragment: Lh,
         lights_lambert_pars_fragment: Ph,
-        lights_pars_begin: Uh,
-        lights_toon_fragment: Nh,
-        lights_toon_pars_fragment: Ih,
+        lights_pars_begin: Dh,
+        lights_toon_fragment: Ih,
+        lights_toon_pars_fragment: Nh,
         lights_phong_fragment: Oh,
         lights_phong_pars_fragment: Fh,
-        lights_physical_fragment: Bh,
-        lights_physical_pars_fragment: zh,
-        lights_fragment_begin: Gh,
-        lights_fragment_maps: Hh,
+        lights_physical_fragment: zh,
+        lights_physical_pars_fragment: Bh,
+        lights_fragment_begin: Hh,
+        lights_fragment_maps: Gh,
         lights_fragment_end: kh,
         logdepthbuf_fragment: Vh,
         logdepthbuf_pars_fragment: Wh,
         logdepthbuf_pars_vertex: Xh,
         logdepthbuf_vertex: jh,
         map_fragment: Yh,
         map_pars_fragment: qh,
@@ -8561,35 +8561,35 @@
         opaque_fragment: fu,
         packing: mu,
         premultiplied_alpha_fragment: gu,
         project_vertex: _u,
         dithering_fragment: vu,
         dithering_pars_fragment: xu,
         roughnessmap_fragment: Mu,
-        roughnessmap_pars_fragment: Eu,
-        shadowmap_pars_fragment: Su,
-        shadowmap_pars_vertex: yu,
-        shadowmap_vertex: bu,
-        shadowmask_pars_fragment: Tu,
+        roughnessmap_pars_fragment: yu,
+        shadowmap_pars_fragment: Eu,
+        shadowmap_pars_vertex: Su,
+        shadowmap_vertex: Tu,
+        shadowmask_pars_fragment: bu,
         skinbase_vertex: wu,
         skinning_pars_vertex: Au,
         skinning_vertex: Ru,
         skinnormal_vertex: Cu,
         specularmap_fragment: Lu,
         specularmap_pars_fragment: Pu,
-        tonemapping_fragment: Uu,
-        tonemapping_pars_fragment: Du,
-        transmission_fragment: Nu,
-        transmission_pars_fragment: Iu,
+        tonemapping_fragment: Du,
+        tonemapping_pars_fragment: Uu,
+        transmission_fragment: Iu,
+        transmission_pars_fragment: Nu,
         uv_pars_fragment: Ou,
         uv_pars_vertex: Fu,
-        uv_vertex: Bu,
-        worldpos_vertex: zu,
-        background_vert: Gu,
-        background_frag: Hu,
+        uv_vertex: zu,
+        worldpos_vertex: Bu,
+        background_vert: Hu,
+        background_frag: Gu,
         backgroundCube_vert: ku,
         backgroundCube_frag: Vu,
         cube_vert: Wu,
         cube_frag: Xu,
         depth_vert: ju,
         depth_frag: Yu,
         distanceRGBA_vert: qu,
@@ -8627,40 +8627,40 @@
             opacity: {
                 value: 1
             },
             map: {
                 value: null
             },
             mapTransform: {
-                value: new Be
+                value: new ze
             },
             alphaMap: {
                 value: null
             },
             alphaMapTransform: {
-                value: new Be
+                value: new ze
             },
             alphaTest: {
                 value: 0
             }
         },
         specularmap: {
             specularMap: {
                 value: null
             },
             specularMapTransform: {
-                value: new Be
+                value: new ze
             }
         },
         envmap: {
             envMap: {
                 value: null
             },
             envMapRotation: {
-                value: new Be
+                value: new ze
             },
             flipEnvMap: {
                 value: -1
             },
             reflectivity: {
                 value: 1
             },
@@ -8675,86 +8675,86 @@
             aoMap: {
                 value: null
             },
             aoMapIntensity: {
                 value: 1
             },
             aoMapTransform: {
-                value: new Be
+                value: new ze
             }
         },
         lightmap: {
             lightMap: {
                 value: null
             },
             lightMapIntensity: {
                 value: 1
             },
             lightMapTransform: {
-                value: new Be
+                value: new ze
             }
         },
         bumpmap: {
             bumpMap: {
                 value: null
             },
             bumpMapTransform: {
-                value: new Be
+                value: new ze
             },
             bumpScale: {
                 value: 1
             }
         },
         normalmap: {
             normalMap: {
                 value: null
             },
             normalMapTransform: {
-                value: new Be
+                value: new ze
             },
             normalScale: {
-                value: new De(1, 1)
+                value: new Ue(1, 1)
             }
         },
         displacementmap: {
             displacementMap: {
                 value: null
             },
             displacementMapTransform: {
-                value: new Be
+                value: new ze
             },
             displacementScale: {
                 value: 1
             },
             displacementBias: {
                 value: 0
             }
         },
         emissivemap: {
             emissiveMap: {
                 value: null
             },
             emissiveMapTransform: {
-                value: new Be
+                value: new ze
             }
         },
         metalnessmap: {
             metalnessMap: {
                 value: null
             },
             metalnessMapTransform: {
-                value: new Be
+                value: new ze
             }
         },
         roughnessmap: {
             roughnessMap: {
                 value: null
             },
             roughnessMapTransform: {
-                value: new Be
+                value: new ze
             }
         },
         gradientmap: {
             gradientMap: {
                 value: null
             }
         },
@@ -8897,54 +8897,54 @@
             map: {
                 value: null
             },
             alphaMap: {
                 value: null
             },
             alphaMapTransform: {
-                value: new Be
+                value: new ze
             },
             alphaTest: {
                 value: 0
             },
             uvTransform: {
-                value: new Be
+                value: new ze
             }
         },
         sprite: {
             diffuse: {
                 value: new Ye(16777215)
             },
             opacity: {
                 value: 1
             },
             center: {
-                value: new De(.5, .5)
+                value: new Ue(.5, .5)
             },
             rotation: {
                 value: 0
             },
             map: {
                 value: null
             },
             mapTransform: {
-                value: new Be
+                value: new ze
             },
             alphaMap: {
                 value: null
             },
             alphaMapTransform: {
-                value: new Be
+                value: new ze
             },
             alphaTest: {
                 value: 0
             }
         }
     },
-    zt = {
+    Bt = {
         basic: {
             uniforms: gt([ce.common, ce.specularmap, ce.envmap, ce.aomap, ce.lightmap, ce.fog]),
             vertexShader: Fe.meshbasic_vert,
             fragmentShader: Fe.meshbasic_frag
         },
         lambert: {
             uniforms: gt([ce.common, ce.specularmap, ce.envmap, ce.aomap, ce.lightmap, ce.emissivemap, ce.bumpmap, ce.normalmap, ce.displacementmap, ce.fog, ce.lights, {
@@ -9044,15 +9044,15 @@
             uniforms: gt([ce.sprite, ce.fog]),
             vertexShader: Fe.sprite_vert,
             fragmentShader: Fe.sprite_frag
         },
         background: {
             uniforms: {
                 uvTransform: {
-                    value: new Be
+                    value: new ze
                 },
                 t2D: {
                     value: null
                 },
                 backgroundIntensity: {
                     value: 1
                 }
@@ -9071,15 +9071,15 @@
                 backgroundBlurriness: {
                     value: 0
                 },
                 backgroundIntensity: {
                     value: 1
                 },
                 backgroundRotation: {
-                    value: new Be
+                    value: new ze
                 }
             },
             vertexShader: Fe.backgroundCube_vert,
             fragmentShader: Fe.backgroundCube_frag
         },
         cube: {
             uniforms: {
@@ -9104,15 +9104,15 @@
             },
             vertexShader: Fe.equirect_vert,
             fragmentShader: Fe.equirect_frag
         },
         distanceRGBA: {
             uniforms: gt([ce.common, ce.displacementmap, {
                 referencePosition: {
-                    value: new D
+                    value: new U
                 },
                 nearDistance: {
                     value: 1
                 },
                 farDistance: {
                     value: 1e3
                 }
@@ -9129,596 +9129,596 @@
                     value: 1
                 }
             }]),
             vertexShader: Fe.shadow_vert,
             fragmentShader: Fe.shadow_frag
         }
     };
-zt.physical = {
-    uniforms: gt([zt.standard.uniforms, {
+Bt.physical = {
+    uniforms: gt([Bt.standard.uniforms, {
         clearcoat: {
             value: 0
         },
         clearcoatMap: {
             value: null
         },
         clearcoatMapTransform: {
-            value: new Be
+            value: new ze
         },
         clearcoatNormalMap: {
             value: null
         },
         clearcoatNormalMapTransform: {
-            value: new Be
+            value: new ze
         },
         clearcoatNormalScale: {
-            value: new De(1, 1)
+            value: new Ue(1, 1)
         },
         clearcoatRoughness: {
             value: 0
         },
         clearcoatRoughnessMap: {
             value: null
         },
         clearcoatRoughnessMapTransform: {
-            value: new Be
+            value: new ze
         },
         iridescence: {
             value: 0
         },
         iridescenceMap: {
             value: null
         },
         iridescenceMapTransform: {
-            value: new Be
+            value: new ze
         },
         iridescenceIOR: {
             value: 1.3
         },
         iridescenceThicknessMinimum: {
             value: 100
         },
         iridescenceThicknessMaximum: {
             value: 400
         },
         iridescenceThicknessMap: {
             value: null
         },
         iridescenceThicknessMapTransform: {
-            value: new Be
+            value: new ze
         },
         sheen: {
             value: 0
         },
         sheenColor: {
             value: new Ye(0)
         },
         sheenColorMap: {
             value: null
         },
         sheenColorMapTransform: {
-            value: new Be
+            value: new ze
         },
         sheenRoughness: {
             value: 1
         },
         sheenRoughnessMap: {
             value: null
         },
         sheenRoughnessMapTransform: {
-            value: new Be
+            value: new ze
         },
         transmission: {
             value: 0
         },
         transmissionMap: {
             value: null
         },
         transmissionMapTransform: {
-            value: new Be
+            value: new ze
         },
         transmissionSamplerSize: {
-            value: new De
+            value: new Ue
         },
         transmissionSamplerMap: {
             value: null
         },
         thickness: {
             value: 0
         },
         thicknessMap: {
             value: null
         },
         thicknessMapTransform: {
-            value: new Be
+            value: new ze
         },
         attenuationDistance: {
             value: 0
         },
         attenuationColor: {
             value: new Ye(0)
         },
         specularColor: {
             value: new Ye(1, 1, 1)
         },
         specularColorMap: {
             value: null
         },
         specularColorMapTransform: {
-            value: new Be
+            value: new ze
         },
         specularIntensity: {
             value: 1
         },
         specularIntensityMap: {
             value: null
         },
         specularIntensityMapTransform: {
-            value: new Be
+            value: new ze
         },
         anisotropyVector: {
-            value: new De
+            value: new Ue
         },
         anisotropyMap: {
             value: null
         },
         anisotropyMapTransform: {
-            value: new Be
+            value: new ze
         }
     }]),
     vertexShader: Fe.meshphysical_vert,
     fragmentShader: Fe.meshphysical_frag
 };
 var jr = {
         r: 0,
         b: 0,
         g: 0
     },
-    Ei = new ei,
+    yi = new ei,
     Md = new at;
 
-function Ed(r, e, t, i, n, a, o) {
+function yd(r, e, t, i, n, a, o) {
     let s = new Ye(0),
         l = a === !0 ? 0 : 1,
-        c, u, p = null,
+        c, h, p = null,
         f = 0,
         m = null;
 
-    function _(d, h) {
-        let w = !1,
-            x = h.isScene === !0 ? h.background : null;
-        x && x.isTexture && (x = (h.backgroundBlurriness > 0 ? t : e).get(x)), x === null ? M(s, l) : x && x.isColor && (M(x, 1), w = !0);
-        let R = r.xr.getEnvironmentBlendMode();
-        R === "additive" ? i.buffers.color.setClear(0, 0, 0, 1, o) : R === "alpha-blend" && i.buffers.color.setClear(0, 0, 0, 0, o), (r.autoClear || w) && r.clear(r.autoClearColor, r.autoClearDepth, r.autoClearStencil), x && (x.isCubeTexture || x.mapping === bn) ? (u === void 0 && (u = new vt(new yr(1, 1, 1), new Gt({
+    function _(d, u) {
+        let T = !1,
+            x = u.isScene === !0 ? u.background : null;
+        x && x.isTexture && (x = (u.backgroundBlurriness > 0 ? t : e).get(x)), x === null ? M(s, l) : x && x.isColor && (M(x, 1), T = !0);
+        let A = r.xr.getEnvironmentBlendMode();
+        A === "additive" ? i.buffers.color.setClear(0, 0, 0, 1, o) : A === "alpha-blend" && i.buffers.color.setClear(0, 0, 0, 0, o), (r.autoClear || T) && r.clear(r.autoClearColor, r.autoClearDepth, r.autoClearStencil), x && (x.isCubeTexture || x.mapping === Tn) ? (h === void 0 && (h = new vt(new Sr(1, 1, 1), new Ht({
             name: "BackgroundCubeMaterial",
-            uniforms: lr(zt.backgroundCube.uniforms),
-            vertexShader: zt.backgroundCube.vertexShader,
-            fragmentShader: zt.backgroundCube.fragmentShader,
-            side: Et,
+            uniforms: lr(Bt.backgroundCube.uniforms),
+            vertexShader: Bt.backgroundCube.vertexShader,
+            fragmentShader: Bt.backgroundCube.fragmentShader,
+            side: yt,
             depthTest: !1,
             depthWrite: !1,
             fog: !1
-        })), u.geometry.deleteAttribute("normal"), u.geometry.deleteAttribute("uv"), u.onBeforeRender = function(U, A, y) {
-            this.matrixWorld.copyPosition(y.matrixWorld)
-        }, Object.defineProperty(u.material, "envMap", {
+        })), h.geometry.deleteAttribute("normal"), h.geometry.deleteAttribute("uv"), h.onBeforeRender = function(D, R, b) {
+            this.matrixWorld.copyPosition(b.matrixWorld)
+        }, Object.defineProperty(h.material, "envMap", {
             get: function() {
                 return this.uniforms.envMap.value
             }
-        }), n.update(u)), Ei.copy(h.backgroundRotation), Ei.x *= -1, Ei.y *= -1, Ei.z *= -1, x.isCubeTexture && x.isRenderTargetTexture === !1 && (Ei.y *= -1, Ei.z *= -1), u.material.uniforms.envMap.value = x, u.material.uniforms.flipEnvMap.value = x.isCubeTexture && x.isRenderTargetTexture === !1 ? -1 : 1, u.material.uniforms.backgroundBlurriness.value = h.backgroundBlurriness, u.material.uniforms.backgroundIntensity.value = h.backgroundIntensity, u.material.uniforms.backgroundRotation.value.setFromMatrix4(Md.makeRotationFromEuler(Ei)), u.material.toneMapped = qe.getTransfer(x.colorSpace) !== Ze, (p !== x || f !== x.version || m !== r.toneMapping) && (u.material.needsUpdate = !0, p = x, f = x.version, m = r.toneMapping), u.layers.enableAll(), d.unshift(u, u.geometry, u.material, 0, 0, null)) : x && x.isTexture && (c === void 0 && (c = new vt(new _n(2, 2), new Gt({
+        }), n.update(h)), yi.copy(u.backgroundRotation), yi.x *= -1, yi.y *= -1, yi.z *= -1, x.isCubeTexture && x.isRenderTargetTexture === !1 && (yi.y *= -1, yi.z *= -1), h.material.uniforms.envMap.value = x, h.material.uniforms.flipEnvMap.value = x.isCubeTexture && x.isRenderTargetTexture === !1 ? -1 : 1, h.material.uniforms.backgroundBlurriness.value = u.backgroundBlurriness, h.material.uniforms.backgroundIntensity.value = u.backgroundIntensity, h.material.uniforms.backgroundRotation.value.setFromMatrix4(Md.makeRotationFromEuler(yi)), h.material.toneMapped = qe.getTransfer(x.colorSpace) !== Ze, (p !== x || f !== x.version || m !== r.toneMapping) && (h.material.needsUpdate = !0, p = x, f = x.version, m = r.toneMapping), h.layers.enableAll(), d.unshift(h, h.geometry, h.material, 0, 0, null)) : x && x.isTexture && (c === void 0 && (c = new vt(new _n(2, 2), new Ht({
             name: "BackgroundMaterial",
-            uniforms: lr(zt.background.uniforms),
-            vertexShader: zt.background.vertexShader,
-            fragmentShader: zt.background.fragmentShader,
+            uniforms: lr(Bt.background.uniforms),
+            vertexShader: Bt.background.vertexShader,
+            fragmentShader: Bt.background.fragmentShader,
             side: pi,
             depthTest: !1,
             depthWrite: !1,
             fog: !1
         })), c.geometry.deleteAttribute("normal"), Object.defineProperty(c.material, "map", {
             get: function() {
                 return this.uniforms.t2D.value
             }
-        }), n.update(c)), c.material.uniforms.t2D.value = x, c.material.uniforms.backgroundIntensity.value = h.backgroundIntensity, c.material.toneMapped = qe.getTransfer(x.colorSpace) !== Ze, x.matrixAutoUpdate === !0 && x.updateMatrix(), c.material.uniforms.uvTransform.value.copy(x.matrix), (p !== x || f !== x.version || m !== r.toneMapping) && (c.material.needsUpdate = !0, p = x, f = x.version, m = r.toneMapping), c.layers.enableAll(), d.unshift(c, c.geometry, c.material, 0, 0, null))
+        }), n.update(c)), c.material.uniforms.t2D.value = x, c.material.uniforms.backgroundIntensity.value = u.backgroundIntensity, c.material.toneMapped = qe.getTransfer(x.colorSpace) !== Ze, x.matrixAutoUpdate === !0 && x.updateMatrix(), c.material.uniforms.uvTransform.value.copy(x.matrix), (p !== x || f !== x.version || m !== r.toneMapping) && (c.material.needsUpdate = !0, p = x, f = x.version, m = r.toneMapping), c.layers.enableAll(), d.unshift(c, c.geometry, c.material, 0, 0, null))
     }
 
-    function M(d, h) {
-        d.getRGB(jr, Vo(r)), i.buffers.color.setClear(jr.r, jr.g, jr.b, h, o)
+    function M(d, u) {
+        d.getRGB(jr, Vo(r)), i.buffers.color.setClear(jr.r, jr.g, jr.b, u, o)
     }
     return {
         getClearColor: function() {
             return s
         },
-        setClearColor: function(d, h = 1) {
-            s.set(d), l = h, M(s, l)
+        setClearColor: function(d, u = 1) {
+            s.set(d), l = u, M(s, l)
         },
         getClearAlpha: function() {
             return l
         },
         setClearAlpha: function(d) {
             l = d, M(s, l)
         },
         render: _
     }
 }
 
-function Sd(r, e, t, i) {
+function Ed(r, e, t, i) {
     let n = r.getParameter(r.MAX_VERTEX_ATTRIBS),
         a = i.isWebGL2 ? null : e.get("OES_vertex_array_object"),
         o = i.isWebGL2 || a !== null,
         s = {},
         l = d(null),
         c = l,
-        u = !1;
+        h = !1;
 
-    function p(P, X, k, j, q) {
-        let W = !1;
+    function p(L, j, k, Y, q) {
+        let Z = !1;
         if (o) {
-            let te = M(j, k, X);
-            c !== te && (c = te, m(c.object)), W = h(P, j, k, q), W && w(P, j, k, q)
+            let ee = M(Y, k, j);
+            c !== ee && (c = ee, m(c.object)), Z = u(L, Y, k, q), Z && T(L, Y, k, q)
         } else {
-            let te = X.wireframe === !0;
-            (c.geometry !== j.id || c.program !== k.id || c.wireframe !== te) && (c.geometry = j.id, c.program = k.id, c.wireframe = te, W = !0)
+            let ee = j.wireframe === !0;
+            (c.geometry !== Y.id || c.program !== k.id || c.wireframe !== ee) && (c.geometry = Y.id, c.program = k.id, c.wireframe = ee, Z = !0)
         }
-        q !== null && t.update(q, r.ELEMENT_ARRAY_BUFFER), (W || u) && (u = !1, C(P, X, k, j), q !== null && r.bindBuffer(r.ELEMENT_ARRAY_BUFFER, t.get(q).buffer))
+        q !== null && t.update(q, r.ELEMENT_ARRAY_BUFFER), (Z || h) && (h = !1, P(L, j, k, Y), q !== null && r.bindBuffer(r.ELEMENT_ARRAY_BUFFER, t.get(q).buffer))
     }
 
     function f() {
         return i.isWebGL2 ? r.createVertexArray() : a.createVertexArrayOES()
     }
 
-    function m(P) {
-        return i.isWebGL2 ? r.bindVertexArray(P) : a.bindVertexArrayOES(P)
+    function m(L) {
+        return i.isWebGL2 ? r.bindVertexArray(L) : a.bindVertexArrayOES(L)
     }
 
-    function _(P) {
-        return i.isWebGL2 ? r.deleteVertexArray(P) : a.deleteVertexArrayOES(P)
+    function _(L) {
+        return i.isWebGL2 ? r.deleteVertexArray(L) : a.deleteVertexArrayOES(L)
     }
 
-    function M(P, X, k) {
-        let j = k.wireframe === !0,
-            q = s[P.id];
-        q === void 0 && (q = {}, s[P.id] = q);
-        let W = q[X.id];
-        W === void 0 && (W = {}, q[X.id] = W);
-        let te = W[j];
-        return te === void 0 && (te = d(f()), W[j] = te), te
+    function M(L, j, k) {
+        let Y = k.wireframe === !0,
+            q = s[L.id];
+        q === void 0 && (q = {}, s[L.id] = q);
+        let Z = q[j.id];
+        Z === void 0 && (Z = {}, q[j.id] = Z);
+        let ee = Z[Y];
+        return ee === void 0 && (ee = d(f()), Z[Y] = ee), ee
     }
 
-    function d(P) {
-        let X = [],
+    function d(L) {
+        let j = [],
             k = [],
-            j = [];
-        for (let q = 0; q < n; q++) X[q] = 0, k[q] = 0, j[q] = 0;
+            Y = [];
+        for (let q = 0; q < n; q++) j[q] = 0, k[q] = 0, Y[q] = 0;
         return {
             geometry: null,
             program: null,
             wireframe: !1,
-            newAttributes: X,
+            newAttributes: j,
             enabledAttributes: k,
-            attributeDivisors: j,
-            object: P,
+            attributeDivisors: Y,
+            object: L,
             attributes: {},
             index: null
         }
     }
 
-    function h(P, X, k, j) {
+    function u(L, j, k, Y) {
         let q = c.attributes,
-            W = X.attributes,
-            te = 0,
-            ee = k.getAttributes();
-        for (let pe in ee)
-            if (ee[pe].location >= 0) {
-                let xe = q[pe],
-                    H = W[pe];
-                if (H === void 0 && (pe === "instanceMatrix" && P.instanceMatrix && (H = P.instanceMatrix), pe === "instanceColor" && P.instanceColor && (H = P.instanceColor)), xe === void 0 || xe.attribute !== H || H && xe.data !== H.data) return !0;
-                te++
-            } return c.attributesNum !== te || c.index !== j
+            Z = j.attributes,
+            ee = 0,
+            ie = k.getAttributes();
+        for (let de in ie)
+            if (ie[de].location >= 0) {
+                let ge = q[de],
+                    V = Z[de];
+                if (V === void 0 && (de === "instanceMatrix" && L.instanceMatrix && (V = L.instanceMatrix), de === "instanceColor" && L.instanceColor && (V = L.instanceColor)), ge === void 0 || ge.attribute !== V || V && ge.data !== V.data) return !0;
+                ee++
+            } return c.attributesNum !== ee || c.index !== Y
     }
 
-    function w(P, X, k, j) {
+    function T(L, j, k, Y) {
         let q = {},
-            W = X.attributes,
-            te = 0,
-            ee = k.getAttributes();
-        for (let pe in ee)
-            if (ee[pe].location >= 0) {
-                let xe = W[pe];
-                xe === void 0 && (pe === "instanceMatrix" && P.instanceMatrix && (xe = P.instanceMatrix), pe === "instanceColor" && P.instanceColor && (xe = P.instanceColor));
-                let H = {};
-                H.attribute = xe, xe && xe.data && (H.data = xe.data), q[pe] = H, te++
-            } c.attributes = q, c.attributesNum = te, c.index = j
+            Z = j.attributes,
+            ee = 0,
+            ie = k.getAttributes();
+        for (let de in ie)
+            if (ie[de].location >= 0) {
+                let ge = Z[de];
+                ge === void 0 && (de === "instanceMatrix" && L.instanceMatrix && (ge = L.instanceMatrix), de === "instanceColor" && L.instanceColor && (ge = L.instanceColor));
+                let V = {};
+                V.attribute = ge, ge && ge.data && (V.data = ge.data), q[de] = V, ee++
+            } c.attributes = q, c.attributesNum = ee, c.index = Y
     }
 
     function x() {
-        let P = c.newAttributes;
-        for (let X = 0, k = P.length; X < k; X++) P[X] = 0
+        let L = c.newAttributes;
+        for (let j = 0, k = L.length; j < k; j++) L[j] = 0
     }
 
-    function R(P) {
-        U(P, 0)
+    function A(L) {
+        D(L, 0)
     }
 
-    function U(P, X) {
+    function D(L, j) {
         let k = c.newAttributes,
-            j = c.enabledAttributes,
+            Y = c.enabledAttributes,
             q = c.attributeDivisors;
-        k[P] = 1, j[P] === 0 && (r.enableVertexAttribArray(P), j[P] = 1), q[P] !== X && ((i.isWebGL2 ? r : e.get("ANGLE_instanced_arrays"))[i.isWebGL2 ? "vertexAttribDivisor" : "vertexAttribDivisorANGLE"](P, X), q[P] = X)
+        k[L] = 1, Y[L] === 0 && (r.enableVertexAttribArray(L), Y[L] = 1), q[L] !== j && ((i.isWebGL2 ? r : e.get("ANGLE_instanced_arrays"))[i.isWebGL2 ? "vertexAttribDivisor" : "vertexAttribDivisorANGLE"](L, j), q[L] = j)
     }
 
-    function A() {
-        let P = c.newAttributes,
-            X = c.enabledAttributes;
-        for (let k = 0, j = X.length; k < j; k++) X[k] !== P[k] && (r.disableVertexAttribArray(k), X[k] = 0)
+    function R() {
+        let L = c.newAttributes,
+            j = c.enabledAttributes;
+        for (let k = 0, Y = j.length; k < Y; k++) j[k] !== L[k] && (r.disableVertexAttribArray(k), j[k] = 0)
     }
 
-    function y(P, X, k, j, q, W, te) {
-        te === !0 ? r.vertexAttribIPointer(P, X, k, q, W) : r.vertexAttribPointer(P, X, k, j, q, W)
+    function b(L, j, k, Y, q, Z, ee) {
+        ee === !0 ? r.vertexAttribIPointer(L, j, k, q, Z) : r.vertexAttribPointer(L, j, k, Y, q, Z)
     }
 
-    function C(P, X, k, j) {
-        if (i.isWebGL2 === !1 && (P.isInstancedMesh || j.isInstancedBufferGeometry) && e.get("ANGLE_instanced_arrays") === null) return;
+    function P(L, j, k, Y) {
+        if (i.isWebGL2 === !1 && (L.isInstancedMesh || Y.isInstancedBufferGeometry) && e.get("ANGLE_instanced_arrays") === null) return;
         x();
-        let q = j.attributes,
-            W = k.getAttributes(),
-            te = X.defaultAttributeValues;
-        for (let ee in W) {
-            let pe = W[ee];
-            if (pe.location >= 0) {
-                let xe = q[ee];
-                if (xe === void 0 && (ee === "instanceMatrix" && P.instanceMatrix && (xe = P.instanceMatrix), ee === "instanceColor" && P.instanceColor && (xe = P.instanceColor)), xe !== void 0) {
-                    let H = xe.normalized,
-                        ie = xe.itemSize,
-                        fe = t.get(xe);
-                    if (fe === void 0) continue;
-                    let Te = fe.buffer,
-                        _e = fe.type,
-                        me = fe.bytesPerElement,
-                        Xe = i.isWebGL2 === !0 && (_e === r.INT || _e === r.UNSIGNED_INT || xe.gpuType === Do);
-                    if (xe.isInterleavedBufferAttribute) {
-                        let we = xe.data,
-                            I = we.stride,
-                            Qe = xe.offset;
-                        if (we.isInstancedInterleavedBuffer) {
-                            for (let ve = 0; ve < pe.locationSize; ve++) U(pe.location + ve, we.meshPerAttribute);
-                            P.isInstancedMesh !== !0 && j._maxInstanceCount === void 0 && (j._maxInstanceCount = we.meshPerAttribute * we.count)
+        let q = Y.attributes,
+            Z = k.getAttributes(),
+            ee = j.defaultAttributeValues;
+        for (let ie in Z) {
+            let de = Z[ie];
+            if (de.location >= 0) {
+                let ge = q[ie];
+                if (ge === void 0 && (ie === "instanceMatrix" && L.instanceMatrix && (ge = L.instanceMatrix), ie === "instanceColor" && L.instanceColor && (ge = L.instanceColor)), ge !== void 0) {
+                    let V = ge.normalized,
+                        te = ge.itemSize,
+                        pe = t.get(ge);
+                    if (pe === void 0) continue;
+                    let we = pe.buffer,
+                        _e = pe.type,
+                        fe = pe.bytesPerElement,
+                        Xe = i.isWebGL2 === !0 && (_e === r.INT || _e === r.UNSIGNED_INT || ge.gpuType === Uo);
+                    if (ge.isInterleavedBufferAttribute) {
+                        let Ae = ge.data,
+                            O = Ae.stride,
+                            Je = ge.offset;
+                        if (Ae.isInstancedInterleavedBuffer) {
+                            for (let ve = 0; ve < de.locationSize; ve++) D(de.location + ve, Ae.meshPerAttribute);
+                            L.isInstancedMesh !== !0 && Y._maxInstanceCount === void 0 && (Y._maxInstanceCount = Ae.meshPerAttribute * Ae.count)
                         } else
-                            for (let ve = 0; ve < pe.locationSize; ve++) R(pe.location + ve);
-                        r.bindBuffer(r.ARRAY_BUFFER, Te);
-                        for (let ve = 0; ve < pe.locationSize; ve++) y(pe.location + ve, ie / pe.locationSize, _e, H, I * me, (Qe + ie / pe.locationSize * ve) * me, Xe)
+                            for (let ve = 0; ve < de.locationSize; ve++) A(de.location + ve);
+                        r.bindBuffer(r.ARRAY_BUFFER, we);
+                        for (let ve = 0; ve < de.locationSize; ve++) b(de.location + ve, te / de.locationSize, _e, V, O * fe, (Je + te / de.locationSize * ve) * fe, Xe)
                     } else {
-                        if (xe.isInstancedBufferAttribute) {
-                            for (let we = 0; we < pe.locationSize; we++) U(pe.location + we, xe.meshPerAttribute);
-                            P.isInstancedMesh !== !0 && j._maxInstanceCount === void 0 && (j._maxInstanceCount = xe.meshPerAttribute * xe.count)
+                        if (ge.isInstancedBufferAttribute) {
+                            for (let Ae = 0; Ae < de.locationSize; Ae++) D(de.location + Ae, ge.meshPerAttribute);
+                            L.isInstancedMesh !== !0 && Y._maxInstanceCount === void 0 && (Y._maxInstanceCount = ge.meshPerAttribute * ge.count)
                         } else
-                            for (let we = 0; we < pe.locationSize; we++) R(pe.location + we);
-                        r.bindBuffer(r.ARRAY_BUFFER, Te);
-                        for (let we = 0; we < pe.locationSize; we++) y(pe.location + we, ie / pe.locationSize, _e, H, ie * me, ie / pe.locationSize * we * me, Xe)
+                            for (let Ae = 0; Ae < de.locationSize; Ae++) A(de.location + Ae);
+                        r.bindBuffer(r.ARRAY_BUFFER, we);
+                        for (let Ae = 0; Ae < de.locationSize; Ae++) b(de.location + Ae, te / de.locationSize, _e, V, te * fe, te / de.locationSize * Ae * fe, Xe)
                     }
-                } else if (te !== void 0) {
-                    let H = te[ee];
-                    if (H !== void 0) switch (H.length) {
+                } else if (ee !== void 0) {
+                    let V = ee[ie];
+                    if (V !== void 0) switch (V.length) {
                         case 2:
-                            r.vertexAttrib2fv(pe.location, H);
+                            r.vertexAttrib2fv(de.location, V);
                             break;
                         case 3:
-                            r.vertexAttrib3fv(pe.location, H);
+                            r.vertexAttrib3fv(de.location, V);
                             break;
                         case 4:
-                            r.vertexAttrib4fv(pe.location, H);
+                            r.vertexAttrib4fv(de.location, V);
                             break;
                         default:
-                            r.vertexAttrib1fv(pe.location, H)
+                            r.vertexAttrib1fv(de.location, V)
                     }
                 }
             }
         }
-        A()
+        R()
     }
 
-    function Z() {
-        V();
-        for (let P in s) {
-            let X = s[P];
-            for (let k in X) {
-                let j = X[k];
-                for (let q in j) _(j[q].object), delete j[q];
-                delete X[k]
+    function I() {
+        W();
+        for (let L in s) {
+            let j = s[L];
+            for (let k in j) {
+                let Y = j[k];
+                for (let q in Y) _(Y[q].object), delete Y[q];
+                delete j[k]
             }
-            delete s[P]
+            delete s[L]
         }
     }
 
-    function v(P) {
-        if (s[P.id] === void 0) return;
-        let X = s[P.id];
-        for (let k in X) {
-            let j = X[k];
-            for (let q in j) _(j[q].object), delete j[q];
-            delete X[k]
+    function v(L) {
+        if (s[L.id] === void 0) return;
+        let j = s[L.id];
+        for (let k in j) {
+            let Y = j[k];
+            for (let q in Y) _(Y[q].object), delete Y[q];
+            delete j[k]
         }
-        delete s[P.id]
+        delete s[L.id]
     }
 
-    function T(P) {
-        for (let X in s) {
-            let k = s[X];
-            if (k[P.id] === void 0) continue;
-            let j = k[P.id];
-            for (let q in j) _(j[q].object), delete j[q];
-            delete k[P.id]
+    function w(L) {
+        for (let j in s) {
+            let k = s[j];
+            if (k[L.id] === void 0) continue;
+            let Y = k[L.id];
+            for (let q in Y) _(Y[q].object), delete Y[q];
+            delete k[L.id]
         }
     }
 
-    function V() {
-        K(), u = !0, c !== l && (c = l, m(c.object))
+    function W() {
+        K(), h = !0, c !== l && (c = l, m(c.object))
     }
 
     function K() {
         l.geometry = null, l.program = null, l.wireframe = !1
     }
     return {
         setup: p,
-        reset: V,
+        reset: W,
         resetDefaultState: K,
-        dispose: Z,
+        dispose: I,
         releaseStatesOfGeometry: v,
-        releaseStatesOfProgram: T,
+        releaseStatesOfProgram: w,
         initAttributes: x,
-        enableAttribute: R,
-        disableUnusedAttributes: A
+        enableAttribute: A,
+        disableUnusedAttributes: R
     }
 }
 
-function yd(r, e, t, i) {
+function Sd(r, e, t, i) {
     let n = i.isWebGL2,
         a;
 
-    function o(u) {
-        a = u
+    function o(h) {
+        a = h
     }
 
-    function s(u, p) {
-        r.drawArrays(a, u, p), t.update(p, a, 1)
+    function s(h, p) {
+        r.drawArrays(a, h, p), t.update(p, a, 1)
     }
 
-    function l(u, p, f) {
+    function l(h, p, f) {
         if (f === 0) return;
         let m, _;
         if (n) m = r, _ = "drawArraysInstanced";
         else if (m = e.get("ANGLE_instanced_arrays"), _ = "drawArraysInstancedANGLE", m === null) {
             console.error("THREE.WebGLBufferRenderer: using THREE.InstancedBufferGeometry but hardware does not support extension ANGLE_instanced_arrays.");
             return
         }
-        m[_](a, u, p, f), t.update(p, a, f)
+        m[_](a, h, p, f), t.update(p, a, f)
     }
 
-    function c(u, p, f) {
+    function c(h, p, f) {
         if (f === 0) return;
         let m = e.get("WEBGL_multi_draw");
         if (m === null)
-            for (let _ = 0; _ < f; _++) this.render(u[_], p[_]);
+            for (let _ = 0; _ < f; _++) this.render(h[_], p[_]);
         else {
-            m.multiDrawArraysWEBGL(a, u, 0, p, 0, f);
+            m.multiDrawArraysWEBGL(a, h, 0, p, 0, f);
             let _ = 0;
             for (let M = 0; M < f; M++) _ += p[M];
             t.update(_, a, 1)
         }
     }
     this.setMode = o, this.render = s, this.renderInstances = l, this.renderMultiDraw = c
 }
 
-function bd(r, e, t) {
+function Td(r, e, t) {
     let i;
 
     function n() {
         if (i !== void 0) return i;
         if (e.has("EXT_texture_filter_anisotropic") === !0) {
-            let y = e.get("EXT_texture_filter_anisotropic");
-            i = r.getParameter(y.MAX_TEXTURE_MAX_ANISOTROPY_EXT)
+            let b = e.get("EXT_texture_filter_anisotropic");
+            i = r.getParameter(b.MAX_TEXTURE_MAX_ANISOTROPY_EXT)
         } else i = 0;
         return i
     }
 
-    function a(y) {
-        if (y === "highp") {
+    function a(b) {
+        if (b === "highp") {
             if (r.getShaderPrecisionFormat(r.VERTEX_SHADER, r.HIGH_FLOAT).precision > 0 && r.getShaderPrecisionFormat(r.FRAGMENT_SHADER, r.HIGH_FLOAT).precision > 0) return "highp";
-            y = "mediump"
+            b = "mediump"
         }
-        return y === "mediump" && r.getShaderPrecisionFormat(r.VERTEX_SHADER, r.MEDIUM_FLOAT).precision > 0 && r.getShaderPrecisionFormat(r.FRAGMENT_SHADER, r.MEDIUM_FLOAT).precision > 0 ? "mediump" : "lowp"
+        return b === "mediump" && r.getShaderPrecisionFormat(r.VERTEX_SHADER, r.MEDIUM_FLOAT).precision > 0 && r.getShaderPrecisionFormat(r.FRAGMENT_SHADER, r.MEDIUM_FLOAT).precision > 0 ? "mediump" : "lowp"
     }
     let o = typeof WebGL2RenderingContext < "u" && r.constructor.name === "WebGL2RenderingContext",
         s = t.precision !== void 0 ? t.precision : "highp",
         l = a(s);
     l !== s && (console.warn("THREE.WebGLRenderer:", s, "not supported, using", l, "instead."), s = l);
     let c = o || e.has("WEBGL_draw_buffers"),
-        u = t.logarithmicDepthBuffer === !0,
+        h = t.logarithmicDepthBuffer === !0,
         p = r.getParameter(r.MAX_TEXTURE_IMAGE_UNITS),
         f = r.getParameter(r.MAX_VERTEX_TEXTURE_IMAGE_UNITS),
         m = r.getParameter(r.MAX_TEXTURE_SIZE),
         _ = r.getParameter(r.MAX_CUBE_MAP_TEXTURE_SIZE),
         M = r.getParameter(r.MAX_VERTEX_ATTRIBS),
         d = r.getParameter(r.MAX_VERTEX_UNIFORM_VECTORS),
-        h = r.getParameter(r.MAX_VARYING_VECTORS),
-        w = r.getParameter(r.MAX_FRAGMENT_UNIFORM_VECTORS),
+        u = r.getParameter(r.MAX_VARYING_VECTORS),
+        T = r.getParameter(r.MAX_FRAGMENT_UNIFORM_VECTORS),
         x = f > 0,
-        R = o || e.has("OES_texture_float"),
-        U = x && R,
-        A = o ? r.getParameter(r.MAX_SAMPLES) : 0;
+        A = o || e.has("OES_texture_float"),
+        D = x && A,
+        R = o ? r.getParameter(r.MAX_SAMPLES) : 0;
     return {
         isWebGL2: o,
         drawBuffers: c,
         getMaxAnisotropy: n,
         getMaxPrecision: a,
         precision: s,
-        logarithmicDepthBuffer: u,
+        logarithmicDepthBuffer: h,
         maxTextures: p,
         maxVertexTextures: f,
         maxTextureSize: m,
         maxCubemapSize: _,
         maxAttributes: M,
         maxVertexUniforms: d,
-        maxVaryings: h,
-        maxFragmentUniforms: w,
+        maxVaryings: u,
+        maxFragmentUniforms: T,
         vertexTextures: x,
-        floatFragmentTextures: R,
-        floatVertexTextures: U,
-        maxSamples: A
+        floatFragmentTextures: A,
+        floatVertexTextures: D,
+        maxSamples: R
     }
 }
 
-function Td(r) {
+function bd(r) {
     let e = this,
         t = null,
         i = 0,
         n = !1,
         a = !1,
-        o = new Bt,
-        s = new Be,
+        o = new zt,
+        s = new ze,
         l = {
             value: null,
             needsUpdate: !1
         };
     this.uniform = l, this.numPlanes = 0, this.numIntersection = 0, this.init = function(p, f) {
         let m = p.length !== 0 || f || i !== 0 || n;
         return n = f, i = p.length, m
     }, this.beginShadows = function() {
-        a = !0, u(null)
+        a = !0, h(null)
     }, this.endShadows = function() {
         a = !1
     }, this.setGlobalState = function(p, f) {
-        t = u(p, f, 0)
+        t = h(p, f, 0)
     }, this.setState = function(p, f, m) {
         let _ = p.clippingPlanes,
             M = p.clipIntersection,
             d = p.clipShadows,
-            h = r.get(p);
-        if (!n || _ === null || _.length === 0 || a && !d) a ? u(null) : c();
+            u = r.get(p);
+        if (!n || _ === null || _.length === 0 || a && !d) a ? h(null) : c();
         else {
-            let w = a ? 0 : i,
-                x = w * 4,
-                R = h.clippingState || null;
-            l.value = R, R = u(_, f, x, m);
-            for (let U = 0; U !== x; ++U) R[U] = t[U];
-            h.clippingState = R, this.numIntersection = M ? this.numPlanes : 0, this.numPlanes += w
+            let T = a ? 0 : i,
+                x = T * 4,
+                A = u.clippingState || null;
+            l.value = A, A = h(_, f, x, m);
+            for (let D = 0; D !== x; ++D) A[D] = t[D];
+            u.clippingState = A, this.numIntersection = M ? this.numPlanes : 0, this.numPlanes += T
         }
     };
 
     function c() {
         l.value !== t && (l.value = t, l.needsUpdate = i > 0), e.numPlanes = i, e.numIntersection = 0
     }
 
-    function u(p, f, m, _) {
+    function h(p, f, m, _) {
         let M = p !== null ? p.length : 0,
             d = null;
         if (M !== 0) {
             if (d = l.value, _ !== !0 || d === null) {
-                let h = m + M * 4,
-                    w = f.matrixWorldInverse;
-                s.getNormalMatrix(w), (d === null || d.length < h) && (d = new Float32Array(h));
-                for (let x = 0, R = m; x !== M; ++x, R += 4) o.copy(p[x]).applyMatrix4(w, s), o.normal.toArray(d, R), d[R + 3] = o.constant
+                let u = m + M * 4,
+                    T = f.matrixWorldInverse;
+                s.getNormalMatrix(T), (d === null || d.length < u) && (d = new Float32Array(u));
+                for (let x = 0, A = m; x !== M; ++x, A += 4) o.copy(p[x]).applyMatrix4(T, s), o.normal.toArray(d, A), d[A + 3] = o.constant
             }
             l.value = d, l.needsUpdate = !0
         }
         return e.numPlanes = M, e.numIntersection = 0, d
     }
 }
 
@@ -9735,15 +9735,15 @@
             if (s === fa || s === ma)
                 if (e.has(o)) {
                     let l = e.get(o).texture;
                     return t(l, o.mapping)
                 } else {
                     let l = o.image;
                     if (l && l.height > 0) {
-                        let c = new ya(l.height);
+                        let c = new Sa(l.height);
                         return c.fromEquirectangularTexture(r, o), e.set(o, c), o.addEventListener("dispose", n), t(c.texture, o.mapping)
                     } else return null
                 }
         }
         return o
     }
 
@@ -9758,15 +9758,15 @@
         e = new WeakMap
     }
     return {
         get: i,
         dispose: a
     }
 }
-var ba = class extends fn {
+var Ta = class extends fn {
         constructor(e = -1, t = 1, i = 1, n = -1, a = .1, o = 2e3) {
             super(), this.isOrthographicCamera = !0, this.type = "OrthographicCamera", this.zoom = 1, this.view = null, this.left = e, this.right = t, this.top = i, this.bottom = n, this.near = a, this.far = o, this.updateProjectionMatrix()
         }
         copy(e, t) {
             return super.copy(e, t), this.left = e.left, this.right = e.right, this.top = e.top, this.bottom = e.bottom, this.near = e.near, this.far = e.far, this.zoom = e.zoom, this.view = e.view === null ? null : Object.assign({}, e.view), this
         }
         setViewOffset(e, t, i, n, a, o) {
@@ -9790,35 +9790,35 @@
                 n = (this.top + this.bottom) / 2,
                 a = i - e,
                 o = i + e,
                 s = n + t,
                 l = n - t;
             if (this.view !== null && this.view.enabled) {
                 let c = (this.right - this.left) / this.view.fullWidth / this.zoom,
-                    u = (this.top - this.bottom) / this.view.fullHeight / this.zoom;
-                a += c * this.view.offsetX, o = a + c * this.view.width, s -= u * this.view.offsetY, l = s - u * this.view.height
+                    h = (this.top - this.bottom) / this.view.fullHeight / this.zoom;
+                a += c * this.view.offsetX, o = a + c * this.view.width, s -= h * this.view.offsetY, l = s - h * this.view.height
             }
             this.projectionMatrix.makeOrthographic(a, o, s, l, this.near, this.far, this.coordinateSystem), this.projectionMatrixInverse.copy(this.projectionMatrix).invert()
         }
         toJSON(e) {
             let t = super.toJSON(e);
             return t.object.zoom = this.zoom, t.object.left = this.left, t.object.right = this.right, t.object.top = this.top, t.object.bottom = this.bottom, t.object.near = this.near, t.object.far = this.far, this.view !== null && (t.object.view = Object.assign({}, this.view)), t
         }
     },
     Ji = 4,
     Qs = [.125, .215, .35, .446, .526, .582],
-    Ti = 20,
-    ra = new ba,
+    bi = 20,
+    ra = new Ta,
     eo = new Ye,
     na = null,
     aa = 0,
     sa = 0,
-    yi = (1 + Math.sqrt(5)) / 2,
-    Zi = 1 / yi,
-    to = [new D(1, 1, 1), new D(-1, 1, 1), new D(1, 1, -1), new D(-1, 1, -1), new D(0, yi, Zi), new D(0, yi, -Zi), new D(Zi, 0, yi), new D(-Zi, 0, yi), new D(yi, Zi, 0), new D(-yi, Zi, 0)],
+    Si = (1 + Math.sqrt(5)) / 2,
+    Zi = 1 / Si,
+    to = [new U(1, 1, 1), new U(-1, 1, 1), new U(1, 1, -1), new U(-1, 1, -1), new U(0, Si, Zi), new U(0, Si, -Zi), new U(Zi, 0, Si), new U(-Zi, 0, Si), new U(Si, Zi, 0), new U(-Si, Zi, 0)],
     vn = class {
         constructor(e) {
             this._renderer = e, this._pingPongRenderTarget = null, this._lodMax = 0, this._cubeSize = 0, this._lodPlanes = [], this._sizeLods = [], this._sigmas = [], this._blurMaterial = null, this._cubemapMaterial = null, this._equirectMaterial = null, this._compileMaterial(this._blurMaterial)
         }
         fromScene(e, t = 0, i = .1, n = 100) {
             na = this._renderer.getRenderTarget(), aa = this._renderer.getActiveCubeFace(), sa = this._renderer.getActiveMipmapLevel(), this._setSize(256);
             let a = this._allocateTargets();
@@ -9886,33 +9886,33 @@
         }
         _sceneToCubeUV(e, t, i, n) {
             let a = new Mt(90, 1, t, i),
                 o = [1, -1, 1, 1, 1, 1],
                 s = [1, 1, 1, -1, -1, -1],
                 l = this._renderer,
                 c = l.autoClear,
-                u = l.toneMapping;
+                h = l.toneMapping;
             l.getClearColor(eo), l.toneMapping = hi, l.autoClear = !1;
             let p = new di({
                     name: "PMREM.Background",
-                    side: Et,
+                    side: yt,
                     depthWrite: !1,
                     depthTest: !1
                 }),
-                f = new vt(new yr, p),
+                f = new vt(new Sr, p),
                 m = !1,
                 _ = e.background;
             _ ? _.isColor && (p.color.copy(_), e.background = null, m = !0) : (p.color.copy(eo), m = !0);
             for (let M = 0; M < 6; M++) {
                 let d = M % 3;
                 d === 0 ? (a.up.set(0, o[M], 0), a.lookAt(s[M], 0, 0)) : d === 1 ? (a.up.set(0, 0, o[M]), a.lookAt(0, s[M], 0)) : (a.up.set(0, o[M], 0), a.lookAt(0, 0, s[M]));
-                let h = this._cubeSize;
-                Yr(n, d * h, M > 2 ? h : 0, h, h), l.setRenderTarget(n), m && l.render(f, a), l.render(e, a)
+                let u = this._cubeSize;
+                Yr(n, d * u, M > 2 ? u : 0, u, u), l.setRenderTarget(n), m && l.render(f, a), l.render(e, a)
             }
-            f.geometry.dispose(), f.material.dispose(), l.toneMapping = u, l.autoClear = c, e.background = _
+            f.geometry.dispose(), f.material.dispose(), l.toneMapping = h, l.autoClear = c, e.background = _
         }
         _textureToCubeUV(e, t) {
             let i = this._renderer,
                 n = e.mapping === nr || e.mapping === ar;
             n ? (this._cubemapMaterial === null && (this._cubemapMaterial = no()), this._cubemapMaterial.uniforms.flipEnvMap.value = e.isRenderTargetTexture === !1 ? -1 : 1) : this._equirectMaterial === null && (this._equirectMaterial = ro());
             let a = n ? this._cubemapMaterial : this._equirectMaterial,
                 o = new vt(this._lodPlanes[0], a),
@@ -9936,39 +9936,39 @@
             let o = this._pingPongRenderTarget;
             this._halfBlur(e, o, t, i, n, "latitudinal", a), this._halfBlur(o, e, i, i, n, "longitudinal", a)
         }
         _halfBlur(e, t, i, n, a, o, s) {
             let l = this._renderer,
                 c = this._blurMaterial;
             o !== "latitudinal" && o !== "longitudinal" && console.error("blur direction must be either latitudinal or longitudinal!");
-            let u = 3,
+            let h = 3,
                 p = new vt(this._lodPlanes[n], c),
                 f = c.uniforms,
                 m = this._sizeLods[i] - 1,
-                _ = isFinite(a) ? Math.PI / (2 * m) : 2 * Math.PI / (2 * Ti - 1),
+                _ = isFinite(a) ? Math.PI / (2 * m) : 2 * Math.PI / (2 * bi - 1),
                 M = a / _,
-                d = isFinite(a) ? 1 + Math.floor(u * M) : Ti;
-            d > Ti && console.warn(`sigmaRadians, ${a}, is too large and will clip, as it requested ${d} samples when the maximum is set to ${Ti}`);
-            let h = [],
-                w = 0;
-            for (let y = 0; y < Ti; ++y) {
-                let C = y / M,
-                    Z = Math.exp(-C * C / 2);
-                h.push(Z), y === 0 ? w += Z : y < d && (w += 2 * Z)
+                d = isFinite(a) ? 1 + Math.floor(h * M) : bi;
+            d > bi && console.warn(`sigmaRadians, ${a}, is too large and will clip, as it requested ${d} samples when the maximum is set to ${bi}`);
+            let u = [],
+                T = 0;
+            for (let b = 0; b < bi; ++b) {
+                let P = b / M,
+                    I = Math.exp(-P * P / 2);
+                u.push(I), b === 0 ? T += I : b < d && (T += 2 * I)
             }
-            for (let y = 0; y < h.length; y++) h[y] = h[y] / w;
-            f.envMap.value = e.texture, f.samples.value = d, f.weights.value = h, f.latitudinal.value = o === "latitudinal", s && (f.poleAxis.value = s);
+            for (let b = 0; b < u.length; b++) u[b] = u[b] / T;
+            f.envMap.value = e.texture, f.samples.value = d, f.weights.value = u, f.latitudinal.value = o === "latitudinal", s && (f.poleAxis.value = s);
             let {
                 _lodMax: x
             } = this;
             f.dTheta.value = _, f.mipInt.value = x - i;
-            let R = this._sizeLods[n],
-                U = 3 * R * (n > x - Ji ? n - x + Ji : 0),
-                A = 4 * (this._cubeSize - R);
-            Yr(t, U, A, 3 * R, 2 * R), l.setRenderTarget(t), l.render(p, ra)
+            let A = this._sizeLods[n],
+                D = 3 * A * (n > x - Ji ? n - x + Ji : 0),
+                R = 4 * (this._cubeSize - A);
+            Yr(t, D, R, 3 * A, 2 * A), l.setRenderTarget(t), l.render(p, ra)
         }
     };
 
 function Ad(r) {
     let e = [],
         t = [],
         i = [],
@@ -9976,59 +9976,59 @@
         a = r - Ji + 1 + Qs.length;
     for (let o = 0; o < a; o++) {
         let s = Math.pow(2, n);
         t.push(s);
         let l = 1 / s;
         o > r - Ji ? l = Qs[o - r + Ji - 1] : o === 0 && (l = 0), i.push(l);
         let c = 1 / (s - 2),
-            u = -c,
+            h = -c,
             p = 1 + c,
-            f = [u, u, p, u, p, p, u, u, p, p, u, p],
+            f = [h, h, p, h, p, p, h, h, p, p, h, p],
             m = 6,
             _ = 6,
             M = 3,
             d = 2,
-            h = 1,
-            w = new Float32Array(M * _ * m),
+            u = 1,
+            T = new Float32Array(M * _ * m),
             x = new Float32Array(d * _ * m),
-            R = new Float32Array(h * _ * m);
-        for (let A = 0; A < m; A++) {
-            let y = A % 3 * 2 / 3 - 1,
-                C = A > 2 ? 0 : -1,
-                Z = [y, C, 0, y + 2 / 3, C, 0, y + 2 / 3, C + 1, 0, y, C, 0, y + 2 / 3, C + 1, 0, y, C + 1, 0];
-            w.set(Z, M * _ * A), x.set(f, d * _ * A);
-            let v = [A, A, A, A, A, A];
-            R.set(v, h * _ * A)
+            A = new Float32Array(u * _ * m);
+        for (let R = 0; R < m; R++) {
+            let b = R % 3 * 2 / 3 - 1,
+                P = R > 2 ? 0 : -1,
+                I = [b, P, 0, b + 2 / 3, P, 0, b + 2 / 3, P + 1, 0, b, P, 0, b + 2 / 3, P + 1, 0, b, P + 1, 0];
+            T.set(I, M * _ * R), x.set(f, d * _ * R);
+            let v = [R, R, R, R, R, R];
+            A.set(v, u * _ * R)
         }
-        let U = new St;
-        U.setAttribute("position", new Lt(w, M)), U.setAttribute("uv", new Lt(x, d)), U.setAttribute("faceIndex", new Lt(R, h)), e.push(U), n > Ji && n--
+        let D = new Et;
+        D.setAttribute("position", new Lt(T, M)), D.setAttribute("uv", new Lt(x, d)), D.setAttribute("faceIndex", new Lt(A, u)), e.push(D), n > Ji && n--
     }
     return {
         lodPlanes: e,
         sizeLods: t,
         sigmas: i
     }
 }
 
 function io(r, e, t) {
     let i = new $t(r, e, t);
-    return i.texture.mapping = bn, i.texture.name = "PMREM.cubeUv", i.scissorTest = !0, i
+    return i.texture.mapping = Tn, i.texture.name = "PMREM.cubeUv", i.scissorTest = !0, i
 }
 
 function Yr(r, e, t, i, n) {
     r.viewport.set(e, t, i, n), r.scissor.set(e, t, i, n)
 }
 
 function Rd(r, e, t) {
-    let i = new Float32Array(Ti),
-        n = new D(0, 1, 0);
-    return new Gt({
+    let i = new Float32Array(bi),
+        n = new U(0, 1, 0);
+    return new Ht({
         name: "SphericalGaussianBlur",
         defines: {
-            n: Ti,
+            n: bi,
             CUBEUV_TEXEL_WIDTH: 1 / e,
             CUBEUV_TEXEL_HEIGHT: 1 / t,
             CUBEUV_MAX_MIP: `${r}.0`
         },
         uniforms: {
             envMap: {
                 value: null
@@ -10117,15 +10117,15 @@
         blending: ci,
         depthTest: !1,
         depthWrite: !1
     })
 }
 
 function ro() {
-    return new Gt({
+    return new Ht({
         name: "EquirectangularToCubeUV",
         uniforms: {
             envMap: {
                 value: null
             }
         },
         vertexShader: ja(),
@@ -10152,15 +10152,15 @@
         blending: ci,
         depthTest: !1,
         depthWrite: !1
     })
 }
 
 function no() {
-    return new Gt({
+    return new Ht({
         name: "CubemapToCubeUV",
         uniforms: {
             envMap: {
                 value: null
             },
             flipEnvMap: {
                 value: -1
@@ -10253,39 +10253,39 @@
     let e = new WeakMap,
         t = null;
 
     function i(s) {
         if (s && s.isTexture) {
             let l = s.mapping,
                 c = l === fa || l === ma,
-                u = l === nr || l === ar;
-            if (c || u)
+                h = l === nr || l === ar;
+            if (c || h)
                 if (s.isRenderTargetTexture && s.needsPMREMUpdate === !0) {
                     s.needsPMREMUpdate = !1;
                     let p = e.get(s);
                     return t === null && (t = new vn(r)), p = c ? t.fromEquirectangular(s, p) : t.fromCubemap(s, p), e.set(s, p), p.texture
                 } else {
                     if (e.has(s)) return e.get(s).texture;
                     {
                         let p = s.image;
-                        if (c && p && p.height > 0 || u && p && n(p)) {
+                        if (c && p && p.height > 0 || h && p && n(p)) {
                             t === null && (t = new vn(r));
                             let f = c ? t.fromEquirectangular(s) : t.fromCubemap(s);
                             return e.set(s, f), s.addEventListener("dispose", a), f.texture
                         } else return null
                     }
                 }
         }
         return s
     }
 
     function n(s) {
         let l = 0,
             c = 6;
-        for (let u = 0; u < c; u++) s[u] !== void 0 && l++;
+        for (let h = 0; h < c; h++) s[h] !== void 0 && l++;
         return l === c
     }
 
     function a(s) {
         let l = s.target;
         l.removeEventListener("dispose", a);
         let c = e.get(l);
@@ -10345,15 +10345,15 @@
 
     function o(p) {
         let f = p.target;
         f.index !== null && e.remove(f.index);
         for (let _ in f.attributes) e.remove(f.attributes[_]);
         for (let _ in f.morphAttributes) {
             let M = f.morphAttributes[_];
-            for (let d = 0, h = M.length; d < h; d++) e.remove(M[d])
+            for (let d = 0, u = M.length; d < u; d++) e.remove(M[d])
         }
         f.removeEventListener("dispose", o), delete n[f.id];
         let m = a.get(f);
         m && (e.remove(m), a.delete(f)), i.releaseStatesOfGeometry(f), f.isInstancedBufferGeometry === !0 && delete f._maxInstanceCount, t.memory.geometries--
     }
 
     function s(p, f) {
@@ -10362,107 +10362,107 @@
 
     function l(p) {
         let f = p.attributes;
         for (let _ in f) e.update(f[_], r.ARRAY_BUFFER);
         let m = p.morphAttributes;
         for (let _ in m) {
             let M = m[_];
-            for (let d = 0, h = M.length; d < h; d++) e.update(M[d], r.ARRAY_BUFFER)
+            for (let d = 0, u = M.length; d < u; d++) e.update(M[d], r.ARRAY_BUFFER)
         }
     }
 
     function c(p) {
         let f = [],
             m = p.index,
             _ = p.attributes.position,
             M = 0;
         if (m !== null) {
-            let w = m.array;
+            let T = m.array;
             M = m.version;
-            for (let x = 0, R = w.length; x < R; x += 3) {
-                let U = w[x + 0],
-                    A = w[x + 1],
-                    y = w[x + 2];
-                f.push(U, A, A, y, y, U)
+            for (let x = 0, A = T.length; x < A; x += 3) {
+                let D = T[x + 0],
+                    R = T[x + 1],
+                    b = T[x + 2];
+                f.push(D, R, R, b, b, D)
             }
         } else if (_ !== void 0) {
-            let w = _.array;
+            let T = _.array;
             M = _.version;
-            for (let x = 0, R = w.length / 3 - 1; x < R; x += 3) {
-                let U = x + 0,
-                    A = x + 1,
-                    y = x + 2;
-                f.push(U, A, A, y, y, U)
+            for (let x = 0, A = T.length / 3 - 1; x < A; x += 3) {
+                let D = x + 0,
+                    R = x + 1,
+                    b = x + 2;
+                f.push(D, R, R, b, b, D)
             }
         } else return;
-        let d = new(Ho(f) ? pn : dn)(f, 1);
+        let d = new(Go(f) ? pn : dn)(f, 1);
         d.version = M;
-        let h = a.get(p);
-        h && e.remove(h), a.set(p, d)
+        let u = a.get(p);
+        u && e.remove(u), a.set(p, d)
     }
 
-    function u(p) {
+    function h(p) {
         let f = a.get(p);
         if (f) {
             let m = p.index;
             m !== null && f.version < m.version && c(p)
         } else c(p);
         return a.get(p)
     }
     return {
         get: s,
         update: l,
-        getWireframeAttribute: u
+        getWireframeAttribute: h
     }
 }
 
-function Ud(r, e, t, i) {
+function Dd(r, e, t, i) {
     let n = i.isWebGL2,
         a;
 
     function o(m) {
         a = m
     }
     let s, l;
 
     function c(m) {
         s = m.type, l = m.bytesPerElement
     }
 
-    function u(m, _) {
+    function h(m, _) {
         r.drawElements(a, _, s, m * l), t.update(_, a, 1)
     }
 
     function p(m, _, M) {
         if (M === 0) return;
-        let d, h;
-        if (n) d = r, h = "drawElementsInstanced";
-        else if (d = e.get("ANGLE_instanced_arrays"), h = "drawElementsInstancedANGLE", d === null) {
+        let d, u;
+        if (n) d = r, u = "drawElementsInstanced";
+        else if (d = e.get("ANGLE_instanced_arrays"), u = "drawElementsInstancedANGLE", d === null) {
             console.error("THREE.WebGLIndexedBufferRenderer: using THREE.InstancedBufferGeometry but hardware does not support extension ANGLE_instanced_arrays.");
             return
         }
-        d[h](a, _, s, m * l, M), t.update(_, a, M)
+        d[u](a, _, s, m * l, M), t.update(_, a, M)
     }
 
     function f(m, _, M) {
         if (M === 0) return;
         let d = e.get("WEBGL_multi_draw");
         if (d === null)
-            for (let h = 0; h < M; h++) this.render(m[h] / l, _[h]);
+            for (let u = 0; u < M; u++) this.render(m[u] / l, _[u]);
         else {
             d.multiDrawElementsWEBGL(a, _, 0, s, m, 0, M);
-            let h = 0;
-            for (let w = 0; w < M; w++) h += _[w];
-            t.update(h, a, 1)
+            let u = 0;
+            for (let T = 0; T < M; T++) u += _[T];
+            t.update(u, a, 1)
         }
     }
-    this.setMode = o, this.setIndex = c, this.render = u, this.renderInstances = p, this.renderMultiDraw = f
+    this.setMode = o, this.setIndex = c, this.render = h, this.renderInstances = p, this.renderMultiDraw = f
 }
 
-function Dd(r) {
+function Ud(r) {
     let e = {
             geometries: 0,
             textures: 0
         },
         t = {
             frame: 0,
             calls: 0,
@@ -10503,120 +10503,120 @@
         programs: null,
         autoReset: !0,
         reset: n,
         update: i
     }
 }
 
-function Nd(r, e) {
+function Id(r, e) {
     return r[0] - e[0]
 }
 
-function Id(r, e) {
+function Nd(r, e) {
     return Math.abs(e[1]) - Math.abs(r[1])
 }
 
 function Od(r, e, t) {
     let i = {},
         n = new Float32Array(8),
         a = new WeakMap,
         o = new ct,
         s = [];
     for (let c = 0; c < 8; c++) s[c] = [c, 0];
 
-    function l(c, u, p) {
+    function l(c, h, p) {
         let f = c.morphTargetInfluences;
         if (e.isWebGL2 === !0) {
-            let m = u.morphAttributes.position || u.morphAttributes.normal || u.morphAttributes.color,
+            let m = h.morphAttributes.position || h.morphAttributes.normal || h.morphAttributes.color,
                 _ = m !== void 0 ? m.length : 0,
-                M = a.get(u);
+                M = a.get(h);
             if (M === void 0 || M.count !== _) {
                 let d = function() {
-                    T.dispose(), a.delete(u), u.removeEventListener("dispose", d)
+                    w.dispose(), a.delete(h), h.removeEventListener("dispose", d)
                 };
                 M !== void 0 && M.texture.dispose();
-                let h = u.morphAttributes.position !== void 0,
-                    w = u.morphAttributes.normal !== void 0,
-                    x = u.morphAttributes.color !== void 0,
-                    R = u.morphAttributes.position || [],
-                    U = u.morphAttributes.normal || [],
-                    A = u.morphAttributes.color || [],
-                    y = 0;
-                h === !0 && (y = 1), w === !0 && (y = 2), x === !0 && (y = 3);
-                let C = u.attributes.position.count * y,
-                    Z = 1;
-                C > e.maxTextureSize && (Z = Math.ceil(C / e.maxTextureSize), C = e.maxTextureSize);
-                let v = new Float32Array(C * Z * 4 * _),
-                    T = new hn(v, C, Z, _);
-                T.type = Zt, T.needsUpdate = !0;
-                let V = y * 4;
+                let u = h.morphAttributes.position !== void 0,
+                    T = h.morphAttributes.normal !== void 0,
+                    x = h.morphAttributes.color !== void 0,
+                    A = h.morphAttributes.position || [],
+                    D = h.morphAttributes.normal || [],
+                    R = h.morphAttributes.color || [],
+                    b = 0;
+                u === !0 && (b = 1), T === !0 && (b = 2), x === !0 && (b = 3);
+                let P = h.attributes.position.count * b,
+                    I = 1;
+                P > e.maxTextureSize && (I = Math.ceil(P / e.maxTextureSize), P = e.maxTextureSize);
+                let v = new Float32Array(P * I * 4 * _),
+                    w = new hn(v, P, I, _);
+                w.type = Zt, w.needsUpdate = !0;
+                let W = b * 4;
                 for (let K = 0; K < _; K++) {
-                    let P = R[K],
-                        X = U[K],
-                        k = A[K],
-                        j = C * Z * 4 * K;
-                    for (let q = 0; q < P.count; q++) {
-                        let W = q * V;
-                        h === !0 && (o.fromBufferAttribute(P, q), v[j + W + 0] = o.x, v[j + W + 1] = o.y, v[j + W + 2] = o.z, v[j + W + 3] = 0), w === !0 && (o.fromBufferAttribute(X, q), v[j + W + 4] = o.x, v[j + W + 5] = o.y, v[j + W + 6] = o.z, v[j + W + 7] = 0), x === !0 && (o.fromBufferAttribute(k, q), v[j + W + 8] = o.x, v[j + W + 9] = o.y, v[j + W + 10] = o.z, v[j + W + 11] = k.itemSize === 4 ? o.w : 1)
+                    let L = A[K],
+                        j = D[K],
+                        k = R[K],
+                        Y = P * I * 4 * K;
+                    for (let q = 0; q < L.count; q++) {
+                        let Z = q * W;
+                        u === !0 && (o.fromBufferAttribute(L, q), v[Y + Z + 0] = o.x, v[Y + Z + 1] = o.y, v[Y + Z + 2] = o.z, v[Y + Z + 3] = 0), T === !0 && (o.fromBufferAttribute(j, q), v[Y + Z + 4] = o.x, v[Y + Z + 5] = o.y, v[Y + Z + 6] = o.z, v[Y + Z + 7] = 0), x === !0 && (o.fromBufferAttribute(k, q), v[Y + Z + 8] = o.x, v[Y + Z + 9] = o.y, v[Y + Z + 10] = o.z, v[Y + Z + 11] = k.itemSize === 4 ? o.w : 1)
                     }
                 }
                 M = {
                     count: _,
-                    texture: T,
-                    size: new De(C, Z)
-                }, a.set(u, M), u.addEventListener("dispose", d)
+                    texture: w,
+                    size: new Ue(P, I)
+                }, a.set(h, M), h.addEventListener("dispose", d)
             }
             if (c.isInstancedMesh === !0 && c.morphTexture !== null) p.getUniforms().setValue(r, "morphTexture", c.morphTexture, t);
             else {
                 let d = 0;
-                for (let w = 0; w < f.length; w++) d += f[w];
-                let h = u.morphTargetsRelative ? 1 : 1 - d;
-                p.getUniforms().setValue(r, "morphTargetBaseInfluence", h), p.getUniforms().setValue(r, "morphTargetInfluences", f)
+                for (let T = 0; T < f.length; T++) d += f[T];
+                let u = h.morphTargetsRelative ? 1 : 1 - d;
+                p.getUniforms().setValue(r, "morphTargetBaseInfluence", u), p.getUniforms().setValue(r, "morphTargetInfluences", f)
             }
             p.getUniforms().setValue(r, "morphTargetsTexture", M.texture, t), p.getUniforms().setValue(r, "morphTargetsTextureSize", M.size)
         } else {
             let m = f === void 0 ? 0 : f.length,
-                _ = i[u.id];
+                _ = i[h.id];
             if (_ === void 0 || _.length !== m) {
                 _ = [];
                 for (let x = 0; x < m; x++) _[x] = [x, 0];
-                i[u.id] = _
+                i[h.id] = _
             }
             for (let x = 0; x < m; x++) {
-                let R = _[x];
-                R[0] = x, R[1] = f[x]
+                let A = _[x];
+                A[0] = x, A[1] = f[x]
             }
-            _.sort(Id);
+            _.sort(Nd);
             for (let x = 0; x < 8; x++) x < m && _[x][1] ? (s[x][0] = _[x][0], s[x][1] = _[x][1]) : (s[x][0] = Number.MAX_SAFE_INTEGER, s[x][1] = 0);
-            s.sort(Nd);
-            let M = u.morphAttributes.position,
-                d = u.morphAttributes.normal,
-                h = 0;
+            s.sort(Id);
+            let M = h.morphAttributes.position,
+                d = h.morphAttributes.normal,
+                u = 0;
             for (let x = 0; x < 8; x++) {
-                let R = s[x],
-                    U = R[0],
-                    A = R[1];
-                U !== Number.MAX_SAFE_INTEGER && A ? (M && u.getAttribute("morphTarget" + x) !== M[U] && u.setAttribute("morphTarget" + x, M[U]), d && u.getAttribute("morphNormal" + x) !== d[U] && u.setAttribute("morphNormal" + x, d[U]), n[x] = A, h += A) : (M && u.hasAttribute("morphTarget" + x) === !0 && u.deleteAttribute("morphTarget" + x), d && u.hasAttribute("morphNormal" + x) === !0 && u.deleteAttribute("morphNormal" + x), n[x] = 0)
+                let A = s[x],
+                    D = A[0],
+                    R = A[1];
+                D !== Number.MAX_SAFE_INTEGER && R ? (M && h.getAttribute("morphTarget" + x) !== M[D] && h.setAttribute("morphTarget" + x, M[D]), d && h.getAttribute("morphNormal" + x) !== d[D] && h.setAttribute("morphNormal" + x, d[D]), n[x] = R, u += R) : (M && h.hasAttribute("morphTarget" + x) === !0 && h.deleteAttribute("morphTarget" + x), d && h.hasAttribute("morphNormal" + x) === !0 && h.deleteAttribute("morphNormal" + x), n[x] = 0)
             }
-            let w = u.morphTargetsRelative ? 1 : 1 - h;
-            p.getUniforms().setValue(r, "morphTargetBaseInfluence", w), p.getUniforms().setValue(r, "morphTargetInfluences", n)
+            let T = h.morphTargetsRelative ? 1 : 1 - u;
+            p.getUniforms().setValue(r, "morphTargetBaseInfluence", T), p.getUniforms().setValue(r, "morphTargetInfluences", n)
         }
     }
     return {
         update: l
     }
 }
 
 function Fd(r, e, t, i) {
     let n = new WeakMap;
 
     function a(l) {
         let c = i.render.frame,
-            u = l.geometry,
-            p = e.get(l, u);
+            h = l.geometry,
+            p = e.get(l, h);
         if (n.get(p) !== c && (e.update(p), n.set(p, c)), l.isInstancedMesh && (l.hasEventListener("dispose", s) === !1 && l.addEventListener("dispose", s), n.get(l) !== c && (t.update(l.instanceMatrix, r.ARRAY_BUFFER), l.instanceColor !== null && t.update(l.instanceColor, r.ARRAY_BUFFER), n.set(l, c))), l.isSkinnedMesh) {
             let f = l.skeleton;
             n.get(f) !== c && (f.update(), n.set(f, c))
         }
         return p
     }
 
@@ -10630,34 +10630,34 @@
     }
     return {
         update: a,
         dispose: o
     }
 }
 var xn = class extends Pt {
-        constructor(e, t, i, n, a, o, s, l, c, u) {
-            if (u = u !== void 0 ? u : Ci, u !== Ci && u !== sr) throw new Error("DepthTexture format must be either THREE.DepthFormat or THREE.DepthStencilFormat");
-            i === void 0 && u === Ci && (i = li), i === void 0 && u === sr && (i = Ri), super(null, n, a, o, s, l, u, i, c), this.isDepthTexture = !0, this.image = {
+        constructor(e, t, i, n, a, o, s, l, c, h) {
+            if (h = h !== void 0 ? h : Ci, h !== Ci && h !== sr) throw new Error("DepthTexture format must be either THREE.DepthFormat or THREE.DepthStencilFormat");
+            i === void 0 && h === Ci && (i = li), i === void 0 && h === sr && (i = Ri), super(null, n, a, o, s, l, h, i, c), this.isDepthTexture = !0, this.image = {
                 width: e,
                 height: t
             }, this.magFilter = s !== void 0 ? s : _t, this.minFilter = l !== void 0 ? l : _t, this.flipY = !1, this.generateMipmaps = !1, this.compareFunction = null
         }
         copy(e) {
             return super.copy(e), this.compareFunction = e.compareFunction, this
         }
         toJSON(e) {
             let t = super.toJSON(e);
             return this.compareFunction !== null && (t.compareFunction = this.compareFunction), t
         }
     },
     Xo = new Pt,
     jo = new xn(1, 1);
-jo.compareFunction = Go;
+jo.compareFunction = Ho;
 var Yo = new hn,
-    qo = new Ea,
+    qo = new ya,
     Zo = new mn,
     ao = [],
     so = [],
     oo = new Float32Array(16),
     lo = new Float32Array(9),
     co = new Float32Array(4);
 
@@ -10687,39 +10687,39 @@
 function wn(r, e) {
     let t = so[e];
     t === void 0 && (t = new Int32Array(e), so[e] = t);
     for (let i = 0; i !== e; ++i) t[i] = r.allocateTextureUnit();
     return t
 }
 
-function Bd(r, e) {
+function zd(r, e) {
     let t = this.cache;
     t[0] !== e && (r.uniform1f(this.addr, e), t[0] = e)
 }
 
-function zd(r, e) {
+function Bd(r, e) {
     let t = this.cache;
     if (e.x !== void 0)(t[0] !== e.x || t[1] !== e.y) && (r.uniform2f(this.addr, e.x, e.y), t[0] = e.x, t[1] = e.y);
     else {
         if (st(t, e)) return;
         r.uniform2fv(this.addr, e), ot(t, e)
     }
 }
 
-function Gd(r, e) {
+function Hd(r, e) {
     let t = this.cache;
     if (e.x !== void 0)(t[0] !== e.x || t[1] !== e.y || t[2] !== e.z) && (r.uniform3f(this.addr, e.x, e.y, e.z), t[0] = e.x, t[1] = e.y, t[2] = e.z);
     else if (e.r !== void 0)(t[0] !== e.r || t[1] !== e.g || t[2] !== e.b) && (r.uniform3f(this.addr, e.r, e.g, e.b), t[0] = e.r, t[1] = e.g, t[2] = e.b);
     else {
         if (st(t, e)) return;
         r.uniform3fv(this.addr, e), ot(t, e)
     }
 }
 
-function Hd(r, e) {
+function Gd(r, e) {
     let t = this.cache;
     if (e.x !== void 0)(t[0] !== e.x || t[1] !== e.y || t[2] !== e.z || t[3] !== e.w) && (r.uniform4f(this.addr, e.x, e.y, e.z, e.w), t[0] = e.x, t[1] = e.y, t[2] = e.z, t[3] = e.w);
     else {
         if (st(t, e)) return;
         r.uniform4fv(this.addr, e), ot(t, e)
     }
 }
@@ -10849,21 +10849,21 @@
         n = t.allocateTextureUnit();
     i[0] !== n && (r.uniform1i(this.addr, n), i[0] = n), t.setTexture2DArray(e || Yo, n)
 }
 
 function rp(r) {
     switch (r) {
         case 5126:
-            return Bd;
-        case 35664:
             return zd;
+        case 35664:
+            return Bd;
         case 35665:
-            return Gd;
-        case 35666:
             return Hd;
+        case 35666:
+            return Gd;
         case 35674:
             return kd;
         case 35675:
             return Vd;
         case 35676:
             return Wd;
         case 5124:
@@ -10987,31 +10987,31 @@
     let i = this.cache,
         n = e.length,
         a = wn(t, n);
     st(i, a) || (r.uniform1iv(this.addr, a), ot(i, a));
     for (let o = 0; o !== n; ++o) t.setTexture3D(e[o] || qo, a[o])
 }
 
-function Ep(r, e, t) {
+function yp(r, e, t) {
     let i = this.cache,
         n = e.length,
         a = wn(t, n);
     st(i, a) || (r.uniform1iv(this.addr, a), ot(i, a));
     for (let o = 0; o !== n; ++o) t.setTextureCube(e[o] || Zo, a[o])
 }
 
-function Sp(r, e, t) {
+function Ep(r, e, t) {
     let i = this.cache,
         n = e.length,
         a = wn(t, n);
     st(i, a) || (r.uniform1iv(this.addr, a), ot(i, a));
     for (let o = 0; o !== n; ++o) t.setTexture2DArray(e[o] || Yo, a[o])
 }
 
-function yp(r) {
+function Sp(r) {
     switch (r) {
         case 5126:
             return np;
         case 35664:
             return ap;
         case 35665:
             return sp;
@@ -11053,30 +11053,30 @@
         case 36299:
         case 36307:
             return Mp;
         case 35680:
         case 36300:
         case 36308:
         case 36293:
-            return Ep;
+            return yp;
         case 36289:
         case 36303:
         case 36311:
         case 36292:
-            return Sp
+            return Ep
     }
 }
-var Ta = class {
+var ba = class {
         constructor(e, t, i) {
             this.id = e, this.addr = i, this.cache = [], this.type = t.type, this.setValue = rp(t.type)
         }
     },
     wa = class {
         constructor(e, t, i) {
-            this.id = e, this.addr = i, this.cache = [], this.type = t.type, this.size = t.size, this.setValue = yp(t.type)
+            this.id = e, this.addr = i, this.cache = [], this.type = t.type, this.size = t.size, this.setValue = Sp(t.type)
         }
     },
     Aa = class {
         constructor(e) {
             this.id = e, this.seq = [], this.map = {}
         }
         setValue(e, t, i) {
@@ -11089,40 +11089,40 @@
     },
     oa = /(\w+)(\])?(\[|\.)?/g;
 
 function ho(r, e) {
     r.seq.push(e), r.map[e.id] = e
 }
 
-function bp(r, e, t) {
+function Tp(r, e, t) {
     let i = r.name,
         n = i.length;
     for (oa.lastIndex = 0;;) {
         let a = oa.exec(i),
             o = oa.lastIndex,
             s = a[1],
             l = a[2] === "]",
             c = a[3];
         if (l && (s = s | 0), c === void 0 || c === "[" && o + 2 === n) {
-            ho(t, c === void 0 ? new Ta(s, r, e) : new wa(s, r, e));
+            ho(t, c === void 0 ? new ba(s, r, e) : new wa(s, r, e));
             break
         } else {
-            let u = t.map[s];
-            u === void 0 && (u = new Aa(s), ho(t, u)), t = u
+            let h = t.map[s];
+            h === void 0 && (h = new Aa(s), ho(t, h)), t = h
         }
     }
 }
 var rr = class {
     constructor(e, t) {
         this.seq = [], this.map = {};
         let i = e.getProgramParameter(t, e.ACTIVE_UNIFORMS);
         for (let n = 0; n < i; ++n) {
             let a = e.getActiveUniform(t, n),
                 o = e.getUniformLocation(t, a.name);
-            bp(a, o, this)
+            Tp(a, o, this)
         }
     }
     setValue(e, t, i, n) {
         let a = this.map[t];
         a !== void 0 && a.setValue(e, i, n)
     }
     setOptional(e, t, i) {
@@ -11146,15 +11146,15 @@
     }
 };
 
 function uo(r, e, t) {
     let i = r.createShader(e);
     return r.shaderSource(i, t), r.compileShader(i), i
 }
-var Tp = 37297,
+var bp = 37297,
     wp = 0;
 
 function Ap(r, e) {
     let t = r.split(`
 `),
         i = [],
         n = Math.max(e - 6, 0),
@@ -11169,15 +11169,15 @@
 
 function Rp(r) {
     let e = qe.getPrimaries(qe.workingColorSpace),
         t = qe.getPrimaries(r),
         i;
     switch (e === t ? i = "" : e === nn && t === rn ? i = "LinearDisplayP3ToLinearSRGB" : e === rn && t === nn && (i = "LinearSRGBToLinearDisplayP3"), r) {
         case fi:
-        case Tn:
+        case bn:
             return [i, "LinearTransferOETF"];
         case Ft:
         case Wa:
             return [i, "sRGBTransferOETF"];
         default:
             return console.warn("THREE.WebGLProgram: Unsupported color space:", r), [i, "LinearTransferOETF"]
     }
@@ -11208,56 +11208,56 @@
     switch (e) {
         case Ll:
             t = "Linear";
             break;
         case Pl:
             t = "Reinhard";
             break;
-        case Ul:
+        case Dl:
             t = "OptimizedCineon";
             break;
-        case Dl:
+        case Ul:
             t = "ACESFilmic";
             break;
-        case Il:
+        case Nl:
             t = "AgX";
             break;
         case Ol:
             t = "Neutral";
             break;
-        case Nl:
+        case Il:
             t = "Custom";
             break;
         default:
             console.warn("THREE.WebGLProgram: Unsupported toneMapping:", e), t = "Linear"
     }
     return "vec3 " + r + "( vec3 color ) { return " + t + "ToneMapping( color ); }"
 }
 
 function Pp(r) {
     return [r.extensionDerivatives || r.envMapCubeUVHeight || r.bumpMap || r.normalMapTangentSpace || r.clearcoatNormalMap || r.flatShading || r.alphaToCoverage || r.shaderID === "physical" ? "#extension GL_OES_standard_derivatives : enable" : "", (r.extensionFragDepth || r.logarithmicDepthBuffer) && r.rendererExtensionFragDepth ? "#extension GL_EXT_frag_depth : enable" : "", r.extensionDrawBuffers && r.rendererExtensionDrawBuffers ? "#extension GL_EXT_draw_buffers : require" : "", (r.extensionShaderTextureLOD || r.envMap || r.transmission) && r.rendererExtensionShaderTextureLod ? "#extension GL_EXT_shader_texture_lod : enable" : ""].filter($i).join(`
 `)
 }
 
-function Up(r) {
+function Dp(r) {
     return [r.extensionClipCullDistance ? "#extension GL_ANGLE_clip_cull_distance : require" : "", r.extensionMultiDraw ? "#extension GL_ANGLE_multi_draw : require" : ""].filter($i).join(`
 `)
 }
 
-function Dp(r) {
+function Up(r) {
     let e = [];
     for (let t in r) {
         let i = r[t];
         i !== !1 && e.push("#define " + t + " " + i)
     }
     return e.join(`
 `)
 }
 
-function Np(r, e) {
+function Ip(r, e) {
     let t = {},
         i = r.getProgramParameter(e, r.ACTIVE_ATTRIBUTES);
     for (let n = 0; n < i; n++) {
         let a = r.getActiveAttrib(e, n),
             o = a.name,
             s = 1;
         a.type === r.FLOAT_MAT2 && (s = 2), a.type === r.FLOAT_MAT3 && (s = 3), a.type === r.FLOAT_MAT4 && (s = 4), t[o] = {
@@ -11277,18 +11277,18 @@
     let t = e.numSpotLightShadows + e.numSpotLightMaps - e.numSpotLightShadowsWithMaps;
     return r.replace(/NUM_DIR_LIGHTS/g, e.numDirLights).replace(/NUM_SPOT_LIGHTS/g, e.numSpotLights).replace(/NUM_SPOT_LIGHT_MAPS/g, e.numSpotLightMaps).replace(/NUM_SPOT_LIGHT_COORDS/g, t).replace(/NUM_RECT_AREA_LIGHTS/g, e.numRectAreaLights).replace(/NUM_POINT_LIGHTS/g, e.numPointLights).replace(/NUM_HEMI_LIGHTS/g, e.numHemiLights).replace(/NUM_DIR_LIGHT_SHADOWS/g, e.numDirLightShadows).replace(/NUM_SPOT_LIGHT_SHADOWS_WITH_MAPS/g, e.numSpotLightShadowsWithMaps).replace(/NUM_SPOT_LIGHT_SHADOWS/g, e.numSpotLightShadows).replace(/NUM_POINT_LIGHT_SHADOWS/g, e.numPointLightShadows)
 }
 
 function mo(r, e) {
     return r.replace(/NUM_CLIPPING_PLANES/g, e.numClippingPlanes).replace(/UNION_CLIPPING_PLANES/g, e.numClippingPlanes - e.numClipIntersection)
 }
-var Ip = /^[ \t]*#include +<([\w\d./]+)>/gm;
+var Np = /^[ \t]*#include +<([\w\d./]+)>/gm;
 
 function Ra(r) {
-    return r.replace(Ip, Fp)
+    return r.replace(Np, Fp)
 }
 var Op = new Map([
     ["encodings_fragment", "colorspace_fragment"],
     ["encodings_pars_fragment", "colorspace_pars_fragment"],
     ["output_fragment", "opaque_fragment"]
 ]);
 
@@ -11297,21 +11297,21 @@
     if (t === void 0) {
         let i = Op.get(e);
         if (i !== void 0) t = Fe[i], console.warn('THREE.WebGLRenderer: Shader chunk "%s" has been deprecated. Use "%s" instead.', e, i);
         else throw new Error("Can not resolve #include <" + e + ">")
     }
     return Ra(t)
 }
-var Bp = /#pragma unroll_loop_start\s+for\s*\(\s*int\s+i\s*=\s*(\d+)\s*;\s*i\s*<\s*(\d+)\s*;\s*i\s*\+\+\s*\)\s*{([\s\S]+?)}\s+#pragma unroll_loop_end/g;
+var zp = /#pragma unroll_loop_start\s+for\s*\(\s*int\s+i\s*=\s*(\d+)\s*;\s*i\s*<\s*(\d+)\s*;\s*i\s*\+\+\s*\)\s*{([\s\S]+?)}\s+#pragma unroll_loop_end/g;
 
 function go(r) {
-    return r.replace(Bp, zp)
+    return r.replace(zp, Bp)
 }
 
-function zp(r, e, t, i) {
+function Bp(r, e, t, i) {
     let n = "";
     for (let a = parseInt(e); a < parseInt(t); a++) n += i.replace(/\[\s*i\s*\]/g, "[ " + a + " ]").replace(/UNROLLED_LOOP_INDEX/g, a);
     return n
 }
 
 function _o(r) {
     let e = `precision ${r.precision} float;
@@ -11334,27 +11334,27 @@
 		precision ${r.precision} usampler2DArray;
 		`), r.precision === "highp" ? e += `
 #define HIGH_PRECISION` : r.precision === "mediump" ? e += `
 #define MEDIUM_PRECISION` : r.precision === "lowp" && (e += `
 #define LOW_PRECISION`), e
 }
 
-function Gp(r) {
+function Hp(r) {
     let e = "SHADOWMAP_TYPE_BASIC";
     return r.shadowMapType === Lo ? e = "SHADOWMAP_TYPE_PCF" : r.shadowMapType === nl ? e = "SHADOWMAP_TYPE_PCF_SOFT" : r.shadowMapType === Yt && (e = "SHADOWMAP_TYPE_VSM"), e
 }
 
-function Hp(r) {
+function Gp(r) {
     let e = "ENVMAP_TYPE_CUBE";
     if (r.envMap) switch (r.envMapMode) {
         case nr:
         case ar:
             e = "ENVMAP_TYPE_CUBE";
             break;
-        case bn:
+        case Tn:
             e = "ENVMAP_TYPE_CUBE_UV";
             break
     }
     return e
 }
 
 function kp(r) {
@@ -11396,96 +11396,96 @@
 }
 
 function Xp(r, e, t, i) {
     let n = r.getContext(),
         a = t.defines,
         o = t.vertexShader,
         s = t.fragmentShader,
-        l = Gp(t),
-        c = Hp(t),
-        u = kp(t),
+        l = Hp(t),
+        c = Gp(t),
+        h = kp(t),
         p = Vp(t),
         f = Wp(t),
         m = t.isWebGL2 ? "" : Pp(t),
-        _ = Up(t),
-        M = Dp(a),
+        _ = Dp(t),
+        M = Up(a),
         d = n.createProgram(),
-        h, w, x = t.glslVersion ? "#version " + t.glslVersion + `
+        u, T, x = t.glslVersion ? "#version " + t.glslVersion + `
 ` : "";
-    t.isRawShaderMaterial ? (h = ["#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M].filter($i).join(`
-`), h.length > 0 && (h += `
-`), w = [m, "#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M].filter($i).join(`
-`), w.length > 0 && (w += `
-`)) : (h = [_o(t), "#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M, t.extensionClipCullDistance ? "#define USE_CLIP_DISTANCE" : "", t.batching ? "#define USE_BATCHING" : "", t.instancing ? "#define USE_INSTANCING" : "", t.instancingColor ? "#define USE_INSTANCING_COLOR" : "", t.instancingMorph ? "#define USE_INSTANCING_MORPH" : "", t.useFog && t.fog ? "#define USE_FOG" : "", t.useFog && t.fogExp2 ? "#define FOG_EXP2" : "", t.map ? "#define USE_MAP" : "", t.envMap ? "#define USE_ENVMAP" : "", t.envMap ? "#define " + u : "", t.lightMap ? "#define USE_LIGHTMAP" : "", t.aoMap ? "#define USE_AOMAP" : "", t.bumpMap ? "#define USE_BUMPMAP" : "", t.normalMap ? "#define USE_NORMALMAP" : "", t.normalMapObjectSpace ? "#define USE_NORMALMAP_OBJECTSPACE" : "", t.normalMapTangentSpace ? "#define USE_NORMALMAP_TANGENTSPACE" : "", t.displacementMap ? "#define USE_DISPLACEMENTMAP" : "", t.emissiveMap ? "#define USE_EMISSIVEMAP" : "", t.anisotropy ? "#define USE_ANISOTROPY" : "", t.anisotropyMap ? "#define USE_ANISOTROPYMAP" : "", t.clearcoatMap ? "#define USE_CLEARCOATMAP" : "", t.clearcoatRoughnessMap ? "#define USE_CLEARCOAT_ROUGHNESSMAP" : "", t.clearcoatNormalMap ? "#define USE_CLEARCOAT_NORMALMAP" : "", t.iridescenceMap ? "#define USE_IRIDESCENCEMAP" : "", t.iridescenceThicknessMap ? "#define USE_IRIDESCENCE_THICKNESSMAP" : "", t.specularMap ? "#define USE_SPECULARMAP" : "", t.specularColorMap ? "#define USE_SPECULAR_COLORMAP" : "", t.specularIntensityMap ? "#define USE_SPECULAR_INTENSITYMAP" : "", t.roughnessMap ? "#define USE_ROUGHNESSMAP" : "", t.metalnessMap ? "#define USE_METALNESSMAP" : "", t.alphaMap ? "#define USE_ALPHAMAP" : "", t.alphaHash ? "#define USE_ALPHAHASH" : "", t.transmission ? "#define USE_TRANSMISSION" : "", t.transmissionMap ? "#define USE_TRANSMISSIONMAP" : "", t.thicknessMap ? "#define USE_THICKNESSMAP" : "", t.sheenColorMap ? "#define USE_SHEEN_COLORMAP" : "", t.sheenRoughnessMap ? "#define USE_SHEEN_ROUGHNESSMAP" : "", t.mapUv ? "#define MAP_UV " + t.mapUv : "", t.alphaMapUv ? "#define ALPHAMAP_UV " + t.alphaMapUv : "", t.lightMapUv ? "#define LIGHTMAP_UV " + t.lightMapUv : "", t.aoMapUv ? "#define AOMAP_UV " + t.aoMapUv : "", t.emissiveMapUv ? "#define EMISSIVEMAP_UV " + t.emissiveMapUv : "", t.bumpMapUv ? "#define BUMPMAP_UV " + t.bumpMapUv : "", t.normalMapUv ? "#define NORMALMAP_UV " + t.normalMapUv : "", t.displacementMapUv ? "#define DISPLACEMENTMAP_UV " + t.displacementMapUv : "", t.metalnessMapUv ? "#define METALNESSMAP_UV " + t.metalnessMapUv : "", t.roughnessMapUv ? "#define ROUGHNESSMAP_UV " + t.roughnessMapUv : "", t.anisotropyMapUv ? "#define ANISOTROPYMAP_UV " + t.anisotropyMapUv : "", t.clearcoatMapUv ? "#define CLEARCOATMAP_UV " + t.clearcoatMapUv : "", t.clearcoatNormalMapUv ? "#define CLEARCOAT_NORMALMAP_UV " + t.clearcoatNormalMapUv : "", t.clearcoatRoughnessMapUv ? "#define CLEARCOAT_ROUGHNESSMAP_UV " + t.clearcoatRoughnessMapUv : "", t.iridescenceMapUv ? "#define IRIDESCENCEMAP_UV " + t.iridescenceMapUv : "", t.iridescenceThicknessMapUv ? "#define IRIDESCENCE_THICKNESSMAP_UV " + t.iridescenceThicknessMapUv : "", t.sheenColorMapUv ? "#define SHEEN_COLORMAP_UV " + t.sheenColorMapUv : "", t.sheenRoughnessMapUv ? "#define SHEEN_ROUGHNESSMAP_UV " + t.sheenRoughnessMapUv : "", t.specularMapUv ? "#define SPECULARMAP_UV " + t.specularMapUv : "", t.specularColorMapUv ? "#define SPECULAR_COLORMAP_UV " + t.specularColorMapUv : "", t.specularIntensityMapUv ? "#define SPECULAR_INTENSITYMAP_UV " + t.specularIntensityMapUv : "", t.transmissionMapUv ? "#define TRANSMISSIONMAP_UV " + t.transmissionMapUv : "", t.thicknessMapUv ? "#define THICKNESSMAP_UV " + t.thicknessMapUv : "", t.vertexTangents && t.flatShading === !1 ? "#define USE_TANGENT" : "", t.vertexColors ? "#define USE_COLOR" : "", t.vertexAlphas ? "#define USE_COLOR_ALPHA" : "", t.vertexUv1s ? "#define USE_UV1" : "", t.vertexUv2s ? "#define USE_UV2" : "", t.vertexUv3s ? "#define USE_UV3" : "", t.pointsUvs ? "#define USE_POINTS_UV" : "", t.flatShading ? "#define FLAT_SHADED" : "", t.skinning ? "#define USE_SKINNING" : "", t.morphTargets ? "#define USE_MORPHTARGETS" : "", t.morphNormals && t.flatShading === !1 ? "#define USE_MORPHNORMALS" : "", t.morphColors && t.isWebGL2 ? "#define USE_MORPHCOLORS" : "", t.morphTargetsCount > 0 && t.isWebGL2 ? "#define MORPHTARGETS_TEXTURE" : "", t.morphTargetsCount > 0 && t.isWebGL2 ? "#define MORPHTARGETS_TEXTURE_STRIDE " + t.morphTextureStride : "", t.morphTargetsCount > 0 && t.isWebGL2 ? "#define MORPHTARGETS_COUNT " + t.morphTargetsCount : "", t.doubleSided ? "#define DOUBLE_SIDED" : "", t.flipSided ? "#define FLIP_SIDED" : "", t.shadowMapEnabled ? "#define USE_SHADOWMAP" : "", t.shadowMapEnabled ? "#define " + l : "", t.sizeAttenuation ? "#define USE_SIZEATTENUATION" : "", t.numLightProbes > 0 ? "#define USE_LIGHT_PROBES" : "", t.useLegacyLights ? "#define LEGACY_LIGHTS" : "", t.logarithmicDepthBuffer ? "#define USE_LOGDEPTHBUF" : "", t.logarithmicDepthBuffer && t.rendererExtensionFragDepth ? "#define USE_LOGDEPTHBUF_EXT" : "", "uniform mat4 modelMatrix;", "uniform mat4 modelViewMatrix;", "uniform mat4 projectionMatrix;", "uniform mat4 viewMatrix;", "uniform mat3 normalMatrix;", "uniform vec3 cameraPosition;", "uniform bool isOrthographic;", "#ifdef USE_INSTANCING", "	attribute mat4 instanceMatrix;", "#endif", "#ifdef USE_INSTANCING_COLOR", "	attribute vec3 instanceColor;", "#endif", "#ifdef USE_INSTANCING_MORPH", "	uniform sampler2D morphTexture;", "#endif", "attribute vec3 position;", "attribute vec3 normal;", "attribute vec2 uv;", "#ifdef USE_UV1", "	attribute vec2 uv1;", "#endif", "#ifdef USE_UV2", "	attribute vec2 uv2;", "#endif", "#ifdef USE_UV3", "	attribute vec2 uv3;", "#endif", "#ifdef USE_TANGENT", "	attribute vec4 tangent;", "#endif", "#if defined( USE_COLOR_ALPHA )", "	attribute vec4 color;", "#elif defined( USE_COLOR )", "	attribute vec3 color;", "#endif", "#if ( defined( USE_MORPHTARGETS ) && ! defined( MORPHTARGETS_TEXTURE ) )", "	attribute vec3 morphTarget0;", "	attribute vec3 morphTarget1;", "	attribute vec3 morphTarget2;", "	attribute vec3 morphTarget3;", "	#ifdef USE_MORPHNORMALS", "		attribute vec3 morphNormal0;", "		attribute vec3 morphNormal1;", "		attribute vec3 morphNormal2;", "		attribute vec3 morphNormal3;", "	#else", "		attribute vec3 morphTarget4;", "		attribute vec3 morphTarget5;", "		attribute vec3 morphTarget6;", "		attribute vec3 morphTarget7;", "	#endif", "#endif", "#ifdef USE_SKINNING", "	attribute vec4 skinIndex;", "	attribute vec4 skinWeight;", "#endif", `
+    t.isRawShaderMaterial ? (u = ["#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M].filter($i).join(`
+`), u.length > 0 && (u += `
+`), T = [m, "#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M].filter($i).join(`
+`), T.length > 0 && (T += `
+`)) : (u = [_o(t), "#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M, t.extensionClipCullDistance ? "#define USE_CLIP_DISTANCE" : "", t.batching ? "#define USE_BATCHING" : "", t.instancing ? "#define USE_INSTANCING" : "", t.instancingColor ? "#define USE_INSTANCING_COLOR" : "", t.instancingMorph ? "#define USE_INSTANCING_MORPH" : "", t.useFog && t.fog ? "#define USE_FOG" : "", t.useFog && t.fogExp2 ? "#define FOG_EXP2" : "", t.map ? "#define USE_MAP" : "", t.envMap ? "#define USE_ENVMAP" : "", t.envMap ? "#define " + h : "", t.lightMap ? "#define USE_LIGHTMAP" : "", t.aoMap ? "#define USE_AOMAP" : "", t.bumpMap ? "#define USE_BUMPMAP" : "", t.normalMap ? "#define USE_NORMALMAP" : "", t.normalMapObjectSpace ? "#define USE_NORMALMAP_OBJECTSPACE" : "", t.normalMapTangentSpace ? "#define USE_NORMALMAP_TANGENTSPACE" : "", t.displacementMap ? "#define USE_DISPLACEMENTMAP" : "", t.emissiveMap ? "#define USE_EMISSIVEMAP" : "", t.anisotropy ? "#define USE_ANISOTROPY" : "", t.anisotropyMap ? "#define USE_ANISOTROPYMAP" : "", t.clearcoatMap ? "#define USE_CLEARCOATMAP" : "", t.clearcoatRoughnessMap ? "#define USE_CLEARCOAT_ROUGHNESSMAP" : "", t.clearcoatNormalMap ? "#define USE_CLEARCOAT_NORMALMAP" : "", t.iridescenceMap ? "#define USE_IRIDESCENCEMAP" : "", t.iridescenceThicknessMap ? "#define USE_IRIDESCENCE_THICKNESSMAP" : "", t.specularMap ? "#define USE_SPECULARMAP" : "", t.specularColorMap ? "#define USE_SPECULAR_COLORMAP" : "", t.specularIntensityMap ? "#define USE_SPECULAR_INTENSITYMAP" : "", t.roughnessMap ? "#define USE_ROUGHNESSMAP" : "", t.metalnessMap ? "#define USE_METALNESSMAP" : "", t.alphaMap ? "#define USE_ALPHAMAP" : "", t.alphaHash ? "#define USE_ALPHAHASH" : "", t.transmission ? "#define USE_TRANSMISSION" : "", t.transmissionMap ? "#define USE_TRANSMISSIONMAP" : "", t.thicknessMap ? "#define USE_THICKNESSMAP" : "", t.sheenColorMap ? "#define USE_SHEEN_COLORMAP" : "", t.sheenRoughnessMap ? "#define USE_SHEEN_ROUGHNESSMAP" : "", t.mapUv ? "#define MAP_UV " + t.mapUv : "", t.alphaMapUv ? "#define ALPHAMAP_UV " + t.alphaMapUv : "", t.lightMapUv ? "#define LIGHTMAP_UV " + t.lightMapUv : "", t.aoMapUv ? "#define AOMAP_UV " + t.aoMapUv : "", t.emissiveMapUv ? "#define EMISSIVEMAP_UV " + t.emissiveMapUv : "", t.bumpMapUv ? "#define BUMPMAP_UV " + t.bumpMapUv : "", t.normalMapUv ? "#define NORMALMAP_UV " + t.normalMapUv : "", t.displacementMapUv ? "#define DISPLACEMENTMAP_UV " + t.displacementMapUv : "", t.metalnessMapUv ? "#define METALNESSMAP_UV " + t.metalnessMapUv : "", t.roughnessMapUv ? "#define ROUGHNESSMAP_UV " + t.roughnessMapUv : "", t.anisotropyMapUv ? "#define ANISOTROPYMAP_UV " + t.anisotropyMapUv : "", t.clearcoatMapUv ? "#define CLEARCOATMAP_UV " + t.clearcoatMapUv : "", t.clearcoatNormalMapUv ? "#define CLEARCOAT_NORMALMAP_UV " + t.clearcoatNormalMapUv : "", t.clearcoatRoughnessMapUv ? "#define CLEARCOAT_ROUGHNESSMAP_UV " + t.clearcoatRoughnessMapUv : "", t.iridescenceMapUv ? "#define IRIDESCENCEMAP_UV " + t.iridescenceMapUv : "", t.iridescenceThicknessMapUv ? "#define IRIDESCENCE_THICKNESSMAP_UV " + t.iridescenceThicknessMapUv : "", t.sheenColorMapUv ? "#define SHEEN_COLORMAP_UV " + t.sheenColorMapUv : "", t.sheenRoughnessMapUv ? "#define SHEEN_ROUGHNESSMAP_UV " + t.sheenRoughnessMapUv : "", t.specularMapUv ? "#define SPECULARMAP_UV " + t.specularMapUv : "", t.specularColorMapUv ? "#define SPECULAR_COLORMAP_UV " + t.specularColorMapUv : "", t.specularIntensityMapUv ? "#define SPECULAR_INTENSITYMAP_UV " + t.specularIntensityMapUv : "", t.transmissionMapUv ? "#define TRANSMISSIONMAP_UV " + t.transmissionMapUv : "", t.thicknessMapUv ? "#define THICKNESSMAP_UV " + t.thicknessMapUv : "", t.vertexTangents && t.flatShading === !1 ? "#define USE_TANGENT" : "", t.vertexColors ? "#define USE_COLOR" : "", t.vertexAlphas ? "#define USE_COLOR_ALPHA" : "", t.vertexUv1s ? "#define USE_UV1" : "", t.vertexUv2s ? "#define USE_UV2" : "", t.vertexUv3s ? "#define USE_UV3" : "", t.pointsUvs ? "#define USE_POINTS_UV" : "", t.flatShading ? "#define FLAT_SHADED" : "", t.skinning ? "#define USE_SKINNING" : "", t.morphTargets ? "#define USE_MORPHTARGETS" : "", t.morphNormals && t.flatShading === !1 ? "#define USE_MORPHNORMALS" : "", t.morphColors && t.isWebGL2 ? "#define USE_MORPHCOLORS" : "", t.morphTargetsCount > 0 && t.isWebGL2 ? "#define MORPHTARGETS_TEXTURE" : "", t.morphTargetsCount > 0 && t.isWebGL2 ? "#define MORPHTARGETS_TEXTURE_STRIDE " + t.morphTextureStride : "", t.morphTargetsCount > 0 && t.isWebGL2 ? "#define MORPHTARGETS_COUNT " + t.morphTargetsCount : "", t.doubleSided ? "#define DOUBLE_SIDED" : "", t.flipSided ? "#define FLIP_SIDED" : "", t.shadowMapEnabled ? "#define USE_SHADOWMAP" : "", t.shadowMapEnabled ? "#define " + l : "", t.sizeAttenuation ? "#define USE_SIZEATTENUATION" : "", t.numLightProbes > 0 ? "#define USE_LIGHT_PROBES" : "", t.useLegacyLights ? "#define LEGACY_LIGHTS" : "", t.logarithmicDepthBuffer ? "#define USE_LOGDEPTHBUF" : "", t.logarithmicDepthBuffer && t.rendererExtensionFragDepth ? "#define USE_LOGDEPTHBUF_EXT" : "", "uniform mat4 modelMatrix;", "uniform mat4 modelViewMatrix;", "uniform mat4 projectionMatrix;", "uniform mat4 viewMatrix;", "uniform mat3 normalMatrix;", "uniform vec3 cameraPosition;", "uniform bool isOrthographic;", "#ifdef USE_INSTANCING", "	attribute mat4 instanceMatrix;", "#endif", "#ifdef USE_INSTANCING_COLOR", "	attribute vec3 instanceColor;", "#endif", "#ifdef USE_INSTANCING_MORPH", "	uniform sampler2D morphTexture;", "#endif", "attribute vec3 position;", "attribute vec3 normal;", "attribute vec2 uv;", "#ifdef USE_UV1", "	attribute vec2 uv1;", "#endif", "#ifdef USE_UV2", "	attribute vec2 uv2;", "#endif", "#ifdef USE_UV3", "	attribute vec2 uv3;", "#endif", "#ifdef USE_TANGENT", "	attribute vec4 tangent;", "#endif", "#if defined( USE_COLOR_ALPHA )", "	attribute vec4 color;", "#elif defined( USE_COLOR )", "	attribute vec3 color;", "#endif", "#if ( defined( USE_MORPHTARGETS ) && ! defined( MORPHTARGETS_TEXTURE ) )", "	attribute vec3 morphTarget0;", "	attribute vec3 morphTarget1;", "	attribute vec3 morphTarget2;", "	attribute vec3 morphTarget3;", "	#ifdef USE_MORPHNORMALS", "		attribute vec3 morphNormal0;", "		attribute vec3 morphNormal1;", "		attribute vec3 morphNormal2;", "		attribute vec3 morphNormal3;", "	#else", "		attribute vec3 morphTarget4;", "		attribute vec3 morphTarget5;", "		attribute vec3 morphTarget6;", "		attribute vec3 morphTarget7;", "	#endif", "#endif", "#ifdef USE_SKINNING", "	attribute vec4 skinIndex;", "	attribute vec4 skinWeight;", "#endif", `
 `].filter($i).join(`
-`), w = [m, _o(t), "#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M, t.useFog && t.fog ? "#define USE_FOG" : "", t.useFog && t.fogExp2 ? "#define FOG_EXP2" : "", t.alphaToCoverage ? "#define ALPHA_TO_COVERAGE" : "", t.map ? "#define USE_MAP" : "", t.matcap ? "#define USE_MATCAP" : "", t.envMap ? "#define USE_ENVMAP" : "", t.envMap ? "#define " + c : "", t.envMap ? "#define " + u : "", t.envMap ? "#define " + p : "", f ? "#define CUBEUV_TEXEL_WIDTH " + f.texelWidth : "", f ? "#define CUBEUV_TEXEL_HEIGHT " + f.texelHeight : "", f ? "#define CUBEUV_MAX_MIP " + f.maxMip + ".0" : "", t.lightMap ? "#define USE_LIGHTMAP" : "", t.aoMap ? "#define USE_AOMAP" : "", t.bumpMap ? "#define USE_BUMPMAP" : "", t.normalMap ? "#define USE_NORMALMAP" : "", t.normalMapObjectSpace ? "#define USE_NORMALMAP_OBJECTSPACE" : "", t.normalMapTangentSpace ? "#define USE_NORMALMAP_TANGENTSPACE" : "", t.emissiveMap ? "#define USE_EMISSIVEMAP" : "", t.anisotropy ? "#define USE_ANISOTROPY" : "", t.anisotropyMap ? "#define USE_ANISOTROPYMAP" : "", t.clearcoat ? "#define USE_CLEARCOAT" : "", t.clearcoatMap ? "#define USE_CLEARCOATMAP" : "", t.clearcoatRoughnessMap ? "#define USE_CLEARCOAT_ROUGHNESSMAP" : "", t.clearcoatNormalMap ? "#define USE_CLEARCOAT_NORMALMAP" : "", t.iridescence ? "#define USE_IRIDESCENCE" : "", t.iridescenceMap ? "#define USE_IRIDESCENCEMAP" : "", t.iridescenceThicknessMap ? "#define USE_IRIDESCENCE_THICKNESSMAP" : "", t.specularMap ? "#define USE_SPECULARMAP" : "", t.specularColorMap ? "#define USE_SPECULAR_COLORMAP" : "", t.specularIntensityMap ? "#define USE_SPECULAR_INTENSITYMAP" : "", t.roughnessMap ? "#define USE_ROUGHNESSMAP" : "", t.metalnessMap ? "#define USE_METALNESSMAP" : "", t.alphaMap ? "#define USE_ALPHAMAP" : "", t.alphaTest ? "#define USE_ALPHATEST" : "", t.alphaHash ? "#define USE_ALPHAHASH" : "", t.sheen ? "#define USE_SHEEN" : "", t.sheenColorMap ? "#define USE_SHEEN_COLORMAP" : "", t.sheenRoughnessMap ? "#define USE_SHEEN_ROUGHNESSMAP" : "", t.transmission ? "#define USE_TRANSMISSION" : "", t.transmissionMap ? "#define USE_TRANSMISSIONMAP" : "", t.thicknessMap ? "#define USE_THICKNESSMAP" : "", t.vertexTangents && t.flatShading === !1 ? "#define USE_TANGENT" : "", t.vertexColors || t.instancingColor ? "#define USE_COLOR" : "", t.vertexAlphas ? "#define USE_COLOR_ALPHA" : "", t.vertexUv1s ? "#define USE_UV1" : "", t.vertexUv2s ? "#define USE_UV2" : "", t.vertexUv3s ? "#define USE_UV3" : "", t.pointsUvs ? "#define USE_POINTS_UV" : "", t.gradientMap ? "#define USE_GRADIENTMAP" : "", t.flatShading ? "#define FLAT_SHADED" : "", t.doubleSided ? "#define DOUBLE_SIDED" : "", t.flipSided ? "#define FLIP_SIDED" : "", t.shadowMapEnabled ? "#define USE_SHADOWMAP" : "", t.shadowMapEnabled ? "#define " + l : "", t.premultipliedAlpha ? "#define PREMULTIPLIED_ALPHA" : "", t.numLightProbes > 0 ? "#define USE_LIGHT_PROBES" : "", t.useLegacyLights ? "#define LEGACY_LIGHTS" : "", t.decodeVideoTexture ? "#define DECODE_VIDEO_TEXTURE" : "", t.logarithmicDepthBuffer ? "#define USE_LOGDEPTHBUF" : "", t.logarithmicDepthBuffer && t.rendererExtensionFragDepth ? "#define USE_LOGDEPTHBUF_EXT" : "", "uniform mat4 viewMatrix;", "uniform vec3 cameraPosition;", "uniform bool isOrthographic;", t.toneMapping !== hi ? "#define TONE_MAPPING" : "", t.toneMapping !== hi ? Fe.tonemapping_pars_fragment : "", t.toneMapping !== hi ? Lp("toneMapping", t.toneMapping) : "", t.dithering ? "#define DITHERING" : "", t.opaque ? "#define OPAQUE" : "", Fe.colorspace_pars_fragment, Cp("linearToOutputTexel", t.outputColorSpace), t.useDepthPacking ? "#define DEPTH_PACKING " + t.depthPacking : "", `
+`), T = [m, _o(t), "#define SHADER_TYPE " + t.shaderType, "#define SHADER_NAME " + t.shaderName, M, t.useFog && t.fog ? "#define USE_FOG" : "", t.useFog && t.fogExp2 ? "#define FOG_EXP2" : "", t.alphaToCoverage ? "#define ALPHA_TO_COVERAGE" : "", t.map ? "#define USE_MAP" : "", t.matcap ? "#define USE_MATCAP" : "", t.envMap ? "#define USE_ENVMAP" : "", t.envMap ? "#define " + c : "", t.envMap ? "#define " + h : "", t.envMap ? "#define " + p : "", f ? "#define CUBEUV_TEXEL_WIDTH " + f.texelWidth : "", f ? "#define CUBEUV_TEXEL_HEIGHT " + f.texelHeight : "", f ? "#define CUBEUV_MAX_MIP " + f.maxMip + ".0" : "", t.lightMap ? "#define USE_LIGHTMAP" : "", t.aoMap ? "#define USE_AOMAP" : "", t.bumpMap ? "#define USE_BUMPMAP" : "", t.normalMap ? "#define USE_NORMALMAP" : "", t.normalMapObjectSpace ? "#define USE_NORMALMAP_OBJECTSPACE" : "", t.normalMapTangentSpace ? "#define USE_NORMALMAP_TANGENTSPACE" : "", t.emissiveMap ? "#define USE_EMISSIVEMAP" : "", t.anisotropy ? "#define USE_ANISOTROPY" : "", t.anisotropyMap ? "#define USE_ANISOTROPYMAP" : "", t.clearcoat ? "#define USE_CLEARCOAT" : "", t.clearcoatMap ? "#define USE_CLEARCOATMAP" : "", t.clearcoatRoughnessMap ? "#define USE_CLEARCOAT_ROUGHNESSMAP" : "", t.clearcoatNormalMap ? "#define USE_CLEARCOAT_NORMALMAP" : "", t.iridescence ? "#define USE_IRIDESCENCE" : "", t.iridescenceMap ? "#define USE_IRIDESCENCEMAP" : "", t.iridescenceThicknessMap ? "#define USE_IRIDESCENCE_THICKNESSMAP" : "", t.specularMap ? "#define USE_SPECULARMAP" : "", t.specularColorMap ? "#define USE_SPECULAR_COLORMAP" : "", t.specularIntensityMap ? "#define USE_SPECULAR_INTENSITYMAP" : "", t.roughnessMap ? "#define USE_ROUGHNESSMAP" : "", t.metalnessMap ? "#define USE_METALNESSMAP" : "", t.alphaMap ? "#define USE_ALPHAMAP" : "", t.alphaTest ? "#define USE_ALPHATEST" : "", t.alphaHash ? "#define USE_ALPHAHASH" : "", t.sheen ? "#define USE_SHEEN" : "", t.sheenColorMap ? "#define USE_SHEEN_COLORMAP" : "", t.sheenRoughnessMap ? "#define USE_SHEEN_ROUGHNESSMAP" : "", t.transmission ? "#define USE_TRANSMISSION" : "", t.transmissionMap ? "#define USE_TRANSMISSIONMAP" : "", t.thicknessMap ? "#define USE_THICKNESSMAP" : "", t.vertexTangents && t.flatShading === !1 ? "#define USE_TANGENT" : "", t.vertexColors || t.instancingColor ? "#define USE_COLOR" : "", t.vertexAlphas ? "#define USE_COLOR_ALPHA" : "", t.vertexUv1s ? "#define USE_UV1" : "", t.vertexUv2s ? "#define USE_UV2" : "", t.vertexUv3s ? "#define USE_UV3" : "", t.pointsUvs ? "#define USE_POINTS_UV" : "", t.gradientMap ? "#define USE_GRADIENTMAP" : "", t.flatShading ? "#define FLAT_SHADED" : "", t.doubleSided ? "#define DOUBLE_SIDED" : "", t.flipSided ? "#define FLIP_SIDED" : "", t.shadowMapEnabled ? "#define USE_SHADOWMAP" : "", t.shadowMapEnabled ? "#define " + l : "", t.premultipliedAlpha ? "#define PREMULTIPLIED_ALPHA" : "", t.numLightProbes > 0 ? "#define USE_LIGHT_PROBES" : "", t.useLegacyLights ? "#define LEGACY_LIGHTS" : "", t.decodeVideoTexture ? "#define DECODE_VIDEO_TEXTURE" : "", t.logarithmicDepthBuffer ? "#define USE_LOGDEPTHBUF" : "", t.logarithmicDepthBuffer && t.rendererExtensionFragDepth ? "#define USE_LOGDEPTHBUF_EXT" : "", "uniform mat4 viewMatrix;", "uniform vec3 cameraPosition;", "uniform bool isOrthographic;", t.toneMapping !== hi ? "#define TONE_MAPPING" : "", t.toneMapping !== hi ? Fe.tonemapping_pars_fragment : "", t.toneMapping !== hi ? Lp("toneMapping", t.toneMapping) : "", t.dithering ? "#define DITHERING" : "", t.opaque ? "#define OPAQUE" : "", Fe.colorspace_pars_fragment, Cp("linearToOutputTexel", t.outputColorSpace), t.useDepthPacking ? "#define DEPTH_PACKING " + t.depthPacking : "", `
 `].filter($i).join(`
 `)), o = Ra(o), o = fo(o, t), o = mo(o, t), s = Ra(s), s = fo(s, t), s = mo(s, t), o = go(o), s = go(s), t.isWebGL2 && t.isRawShaderMaterial !== !0 && (x = `#version 300 es
-`, h = [_, "precision mediump sampler2DArray;", "#define attribute in", "#define varying out", "#define texture2D texture"].join(`
+`, u = [_, "precision mediump sampler2DArray;", "#define attribute in", "#define varying out", "#define texture2D texture"].join(`
 `) + `
-` + h, w = ["precision mediump sampler2DArray;", "#define varying in", t.glslVersion === Ds ? "" : "layout(location = 0) out highp vec4 pc_fragColor;", t.glslVersion === Ds ? "" : "#define gl_FragColor pc_fragColor", "#define gl_FragDepthEXT gl_FragDepth", "#define texture2D texture", "#define textureCube texture", "#define texture2DProj textureProj", "#define texture2DLodEXT textureLod", "#define texture2DProjLodEXT textureProjLod", "#define textureCubeLodEXT textureLod", "#define texture2DGradEXT textureGrad", "#define texture2DProjGradEXT textureProjGrad", "#define textureCubeGradEXT textureGrad"].join(`
+` + u, T = ["precision mediump sampler2DArray;", "#define varying in", t.glslVersion === Us ? "" : "layout(location = 0) out highp vec4 pc_fragColor;", t.glslVersion === Us ? "" : "#define gl_FragColor pc_fragColor", "#define gl_FragDepthEXT gl_FragDepth", "#define texture2D texture", "#define textureCube texture", "#define texture2DProj textureProj", "#define texture2DLodEXT textureLod", "#define texture2DProjLodEXT textureProjLod", "#define textureCubeLodEXT textureLod", "#define texture2DGradEXT textureGrad", "#define texture2DProjGradEXT textureProjGrad", "#define textureCubeGradEXT textureGrad"].join(`
 `) + `
-` + w);
-    let R = x + h + o,
-        U = x + w + s,
-        A = uo(n, n.VERTEX_SHADER, R),
-        y = uo(n, n.FRAGMENT_SHADER, U);
-    n.attachShader(d, A), n.attachShader(d, y), t.index0AttributeName !== void 0 ? n.bindAttribLocation(d, 0, t.index0AttributeName) : t.morphTargets === !0 && n.bindAttribLocation(d, 0, "position"), n.linkProgram(d);
+` + T);
+    let A = x + u + o,
+        D = x + T + s,
+        R = uo(n, n.VERTEX_SHADER, A),
+        b = uo(n, n.FRAGMENT_SHADER, D);
+    n.attachShader(d, R), n.attachShader(d, b), t.index0AttributeName !== void 0 ? n.bindAttribLocation(d, 0, t.index0AttributeName) : t.morphTargets === !0 && n.bindAttribLocation(d, 0, "position"), n.linkProgram(d);
 
-    function C(V) {
+    function P(W) {
         if (r.debug.checkShaderErrors) {
             let K = n.getProgramInfoLog(d).trim(),
-                P = n.getShaderInfoLog(A).trim(),
-                X = n.getShaderInfoLog(y).trim(),
+                L = n.getShaderInfoLog(R).trim(),
+                j = n.getShaderInfoLog(b).trim(),
                 k = !0,
-                j = !0;
+                Y = !0;
             if (n.getProgramParameter(d, n.LINK_STATUS) === !1)
-                if (k = !1, typeof r.debug.onShaderError == "function") r.debug.onShaderError(n, d, A, y);
+                if (k = !1, typeof r.debug.onShaderError == "function") r.debug.onShaderError(n, d, R, b);
                 else {
-                    let q = po(n, A, "vertex"),
-                        W = po(n, y, "fragment");
+                    let q = po(n, R, "vertex"),
+                        Z = po(n, b, "fragment");
                     console.error("THREE.WebGLProgram: Shader Error " + n.getError() + " - VALIDATE_STATUS " + n.getProgramParameter(d, n.VALIDATE_STATUS) + `
 
-Material Name: ` + V.name + `
-Material Type: ` + V.type + `
+Material Name: ` + W.name + `
+Material Type: ` + W.type + `
 
 Program Info Log: ` + K + `
 ` + q + `
-` + W)
+` + Z)
                 }
-            else K !== "" ? console.warn("THREE.WebGLProgram: Program Info Log:", K) : (P === "" || X === "") && (j = !1);
-            j && (V.diagnostics = {
+            else K !== "" ? console.warn("THREE.WebGLProgram: Program Info Log:", K) : (L === "" || j === "") && (Y = !1);
+            Y && (W.diagnostics = {
                 runnable: k,
                 programLog: K,
                 vertexShader: {
-                    log: P,
-                    prefix: h
+                    log: L,
+                    prefix: u
                 },
                 fragmentShader: {
-                    log: X,
-                    prefix: w
+                    log: j,
+                    prefix: T
                 }
             })
         }
-        n.deleteShader(A), n.deleteShader(y), Z = new rr(n, d), v = Np(n, d)
+        n.deleteShader(R), n.deleteShader(b), I = new rr(n, d), v = Ip(n, d)
     }
-    let Z;
+    let I;
     this.getUniforms = function() {
-        return Z === void 0 && C(this), Z
+        return I === void 0 && P(this), I
     };
     let v;
     this.getAttributes = function() {
-        return v === void 0 && C(this), v
+        return v === void 0 && P(this), v
     };
-    let T = t.rendererExtensionParallelShaderCompile === !1;
+    let w = t.rendererExtensionParallelShaderCompile === !1;
     return this.isReady = function() {
-        return T === !1 && (T = n.getProgramParameter(d, Tp)), T
+        return w === !1 && (w = n.getProgramParameter(d, bp)), w
     }, this.destroy = function() {
         i.releaseStatesOfProgram(this), n.deleteProgram(d), this.program = void 0
-    }, this.type = t.shaderType, this.name = t.shaderName, this.id = wp++, this.cacheKey = e, this.usedTimes = 1, this.program = d, this.vertexShader = A, this.fragmentShader = y, this
+    }, this.type = t.shaderType, this.name = t.shaderName, this.id = wp++, this.cacheKey = e, this.usedTimes = 1, this.program = d, this.vertexShader = R, this.fragmentShader = b, this
 }
 var jp = 0,
     Ca = class {
         constructor() {
             this.shaderCache = new Map, this.materialCache = new Map
         }
         update(e) {
@@ -11527,15 +11527,15 @@
         }
     };
 
 function Yp(r, e, t, i, n, a, o) {
     let s = new un,
         l = new Ca,
         c = new Set,
-        u = [],
+        h = [],
         p = n.isWebGL2,
         f = n.logarithmicDepthBuffer,
         m = n.vertexTextures,
         _ = n.precision,
         M = {
             MeshDepthMaterial: "depth",
             MeshDistanceMaterial: "distanceRGBA",
@@ -11554,190 +11554,190 @@
             SpriteMaterial: "sprite"
         };
 
     function d(v) {
         return c.add(v), v === 0 ? "uv" : `uv${v}`
     }
 
-    function h(v, T, V, K, P) {
-        let X = K.fog,
-            k = P.geometry,
-            j = v.isMeshStandardMaterial ? K.environment : null,
-            q = (v.isMeshStandardMaterial ? t : e).get(v.envMap || j),
-            W = q && q.mapping === bn ? q.image.height : null,
-            te = M[v.type];
+    function u(v, w, W, K, L) {
+        let j = K.fog,
+            k = L.geometry,
+            Y = v.isMeshStandardMaterial ? K.environment : null,
+            q = (v.isMeshStandardMaterial ? t : e).get(v.envMap || Y),
+            Z = q && q.mapping === Tn ? q.image.height : null,
+            ee = M[v.type];
         v.precision !== null && (_ = n.getMaxPrecision(v.precision), _ !== v.precision && console.warn("THREE.WebGLProgram.getParameters:", v.precision, "not supported, using", _, "instead."));
-        let ee = k.morphAttributes.position || k.morphAttributes.normal || k.morphAttributes.color,
-            pe = ee !== void 0 ? ee.length : 0,
-            xe = 0;
-        k.morphAttributes.position !== void 0 && (xe = 1), k.morphAttributes.normal !== void 0 && (xe = 2), k.morphAttributes.color !== void 0 && (xe = 3);
-        let H, ie, fe, Te;
-        if (te) {
-            let Ve = zt[te];
-            H = Ve.vertexShader, ie = Ve.fragmentShader
-        } else H = v.vertexShader, ie = v.fragmentShader, l.update(v), fe = l.getVertexShaderID(v), Te = l.getFragmentShaderID(v);
+        let ie = k.morphAttributes.position || k.morphAttributes.normal || k.morphAttributes.color,
+            de = ie !== void 0 ? ie.length : 0,
+            ge = 0;
+        k.morphAttributes.position !== void 0 && (ge = 1), k.morphAttributes.normal !== void 0 && (ge = 2), k.morphAttributes.color !== void 0 && (ge = 3);
+        let V, te, pe, we;
+        if (ee) {
+            let Ve = Bt[ee];
+            V = Ve.vertexShader, te = Ve.fragmentShader
+        } else V = v.vertexShader, te = v.fragmentShader, l.update(v), pe = l.getVertexShaderID(v), we = l.getFragmentShaderID(v);
         let _e = r.getRenderTarget(),
-            me = P.isInstancedMesh === !0,
-            Xe = P.isBatchedMesh === !0,
-            we = !!v.map,
-            I = !!v.matcap,
-            Qe = !!q,
+            fe = L.isInstancedMesh === !0,
+            Xe = L.isBatchedMesh === !0,
+            Ae = !!v.map,
+            O = !!v.matcap,
+            Je = !!q,
             ve = !!v.aoMap,
-            Ue = !!v.lightMap,
-            Me = !!v.bumpMap,
-            Le = !!v.normalMap,
+            Pe = !!v.lightMap,
+            Se = !!v.bumpMap,
+            Ne = !!v.normalMap,
             be = !!v.displacementMap,
-            de = !!v.emissiveMap,
-            Ne = !!v.metalnessMap,
-            S = !!v.roughnessMap,
+            Re = !!v.emissiveMap,
+            xe = !!v.metalnessMap,
+            E = !!v.roughnessMap,
             g = v.anisotropy > 0,
             B = v.clearcoat > 0,
-            Y = v.iridescence > 0,
+            X = v.iridescence > 0,
             Q = v.sheen > 0,
             J = v.transmission > 0,
-            Ce = g && !!v.anisotropyMap,
-            ye = B && !!v.clearcoatMap,
+            Ee = g && !!v.anisotropyMap,
+            Me = B && !!v.clearcoatMap,
             ae = B && !!v.clearcoatNormalMap,
             he = B && !!v.clearcoatRoughnessMap,
-            Ie = Y && !!v.iridescenceMap,
-            ne = Y && !!v.iridescenceThicknessMap,
-            Je = Q && !!v.sheenColorMap,
-            ze = Q && !!v.sheenRoughnessMap,
-            Ee = !!v.specularMap,
-            ge = !!v.specularColorMap,
-            b = !!v.specularIntensityMap,
+            Ie = X && !!v.iridescenceMap,
+            ne = X && !!v.iridescenceThicknessMap,
+            $e = Q && !!v.sheenColorMap,
+            Be = Q && !!v.sheenRoughnessMap,
+            ye = !!v.specularMap,
+            me = !!v.specularColorMap,
+            S = !!v.specularIntensityMap,
             $ = J && !!v.transmissionMap,
             oe = J && !!v.thicknessMap,
-            Ae = !!v.gradientMap,
-            L = !!v.alphaMap,
+            Ce = !!v.gradientMap,
+            C = !!v.alphaMap,
             re = v.alphaTest > 0,
-            O = !!v.alphaHash,
+            F = !!v.alphaHash,
             le = !!v.extensions,
             se = hi;
         v.toneMapped && (_e === null || _e.isXRRenderTarget === !0) && (se = r.toneMapping);
-        let Ge = {
+        let He = {
             isWebGL2: p,
-            shaderID: te,
+            shaderID: ee,
             shaderType: v.type,
             shaderName: v.name,
-            vertexShader: H,
-            fragmentShader: ie,
+            vertexShader: V,
+            fragmentShader: te,
             defines: v.defines,
-            customVertexShaderID: fe,
-            customFragmentShaderID: Te,
+            customVertexShaderID: pe,
+            customFragmentShaderID: we,
             isRawShaderMaterial: v.isRawShaderMaterial === !0,
             glslVersion: v.glslVersion,
             precision: _,
             batching: Xe,
-            instancing: me,
-            instancingColor: me && P.instanceColor !== null,
-            instancingMorph: me && P.morphTexture !== null,
+            instancing: fe,
+            instancingColor: fe && L.instanceColor !== null,
+            instancingMorph: fe && L.morphTexture !== null,
             supportsVertexTextures: m,
             outputColorSpace: _e === null ? r.outputColorSpace : _e.isXRRenderTarget === !0 ? _e.texture.colorSpace : fi,
             alphaToCoverage: !!v.alphaToCoverage,
-            map: we,
-            matcap: I,
-            envMap: Qe,
-            envMapMode: Qe && q.mapping,
-            envMapCubeUVHeight: W,
+            map: Ae,
+            matcap: O,
+            envMap: Je,
+            envMapMode: Je && q.mapping,
+            envMapCubeUVHeight: Z,
             aoMap: ve,
-            lightMap: Ue,
-            bumpMap: Me,
-            normalMap: Le,
+            lightMap: Pe,
+            bumpMap: Se,
+            normalMap: Ne,
             displacementMap: m && be,
-            emissiveMap: de,
-            normalMapObjectSpace: Le && v.normalMapType === ql,
-            normalMapTangentSpace: Le && v.normalMapType === Yl,
-            metalnessMap: Ne,
-            roughnessMap: S,
+            emissiveMap: Re,
+            normalMapObjectSpace: Ne && v.normalMapType === ql,
+            normalMapTangentSpace: Ne && v.normalMapType === Yl,
+            metalnessMap: xe,
+            roughnessMap: E,
             anisotropy: g,
-            anisotropyMap: Ce,
+            anisotropyMap: Ee,
             clearcoat: B,
-            clearcoatMap: ye,
+            clearcoatMap: Me,
             clearcoatNormalMap: ae,
             clearcoatRoughnessMap: he,
-            iridescence: Y,
+            iridescence: X,
             iridescenceMap: Ie,
             iridescenceThicknessMap: ne,
             sheen: Q,
-            sheenColorMap: Je,
-            sheenRoughnessMap: ze,
-            specularMap: Ee,
-            specularColorMap: ge,
-            specularIntensityMap: b,
+            sheenColorMap: $e,
+            sheenRoughnessMap: Be,
+            specularMap: ye,
+            specularColorMap: me,
+            specularIntensityMap: S,
             transmission: J,
             transmissionMap: $,
             thicknessMap: oe,
-            gradientMap: Ae,
+            gradientMap: Ce,
             opaque: v.transparent === !1 && v.blending === er && v.alphaToCoverage === !1,
-            alphaMap: L,
+            alphaMap: C,
             alphaTest: re,
-            alphaHash: O,
+            alphaHash: F,
             combine: v.combine,
-            mapUv: we && d(v.map.channel),
+            mapUv: Ae && d(v.map.channel),
             aoMapUv: ve && d(v.aoMap.channel),
-            lightMapUv: Ue && d(v.lightMap.channel),
-            bumpMapUv: Me && d(v.bumpMap.channel),
-            normalMapUv: Le && d(v.normalMap.channel),
+            lightMapUv: Pe && d(v.lightMap.channel),
+            bumpMapUv: Se && d(v.bumpMap.channel),
+            normalMapUv: Ne && d(v.normalMap.channel),
             displacementMapUv: be && d(v.displacementMap.channel),
-            emissiveMapUv: de && d(v.emissiveMap.channel),
-            metalnessMapUv: Ne && d(v.metalnessMap.channel),
-            roughnessMapUv: S && d(v.roughnessMap.channel),
-            anisotropyMapUv: Ce && d(v.anisotropyMap.channel),
-            clearcoatMapUv: ye && d(v.clearcoatMap.channel),
+            emissiveMapUv: Re && d(v.emissiveMap.channel),
+            metalnessMapUv: xe && d(v.metalnessMap.channel),
+            roughnessMapUv: E && d(v.roughnessMap.channel),
+            anisotropyMapUv: Ee && d(v.anisotropyMap.channel),
+            clearcoatMapUv: Me && d(v.clearcoatMap.channel),
             clearcoatNormalMapUv: ae && d(v.clearcoatNormalMap.channel),
             clearcoatRoughnessMapUv: he && d(v.clearcoatRoughnessMap.channel),
             iridescenceMapUv: Ie && d(v.iridescenceMap.channel),
             iridescenceThicknessMapUv: ne && d(v.iridescenceThicknessMap.channel),
-            sheenColorMapUv: Je && d(v.sheenColorMap.channel),
-            sheenRoughnessMapUv: ze && d(v.sheenRoughnessMap.channel),
-            specularMapUv: Ee && d(v.specularMap.channel),
-            specularColorMapUv: ge && d(v.specularColorMap.channel),
-            specularIntensityMapUv: b && d(v.specularIntensityMap.channel),
+            sheenColorMapUv: $e && d(v.sheenColorMap.channel),
+            sheenRoughnessMapUv: Be && d(v.sheenRoughnessMap.channel),
+            specularMapUv: ye && d(v.specularMap.channel),
+            specularColorMapUv: me && d(v.specularColorMap.channel),
+            specularIntensityMapUv: S && d(v.specularIntensityMap.channel),
             transmissionMapUv: $ && d(v.transmissionMap.channel),
             thicknessMapUv: oe && d(v.thicknessMap.channel),
-            alphaMapUv: L && d(v.alphaMap.channel),
-            vertexTangents: !!k.attributes.tangent && (Le || g),
+            alphaMapUv: C && d(v.alphaMap.channel),
+            vertexTangents: !!k.attributes.tangent && (Ne || g),
             vertexColors: v.vertexColors,
             vertexAlphas: v.vertexColors === !0 && !!k.attributes.color && k.attributes.color.itemSize === 4,
-            pointsUvs: P.isPoints === !0 && !!k.attributes.uv && (we || L),
-            fog: !!X,
+            pointsUvs: L.isPoints === !0 && !!k.attributes.uv && (Ae || C),
+            fog: !!j,
             useFog: v.fog === !0,
-            fogExp2: !!X && X.isFogExp2,
+            fogExp2: !!j && j.isFogExp2,
             flatShading: v.flatShading === !0,
             sizeAttenuation: v.sizeAttenuation === !0,
             logarithmicDepthBuffer: f,
-            skinning: P.isSkinnedMesh === !0,
+            skinning: L.isSkinnedMesh === !0,
             morphTargets: k.morphAttributes.position !== void 0,
             morphNormals: k.morphAttributes.normal !== void 0,
             morphColors: k.morphAttributes.color !== void 0,
-            morphTargetsCount: pe,
-            morphTextureStride: xe,
-            numDirLights: T.directional.length,
-            numPointLights: T.point.length,
-            numSpotLights: T.spot.length,
-            numSpotLightMaps: T.spotLightMap.length,
-            numRectAreaLights: T.rectArea.length,
-            numHemiLights: T.hemi.length,
-            numDirLightShadows: T.directionalShadowMap.length,
-            numPointLightShadows: T.pointShadowMap.length,
-            numSpotLightShadows: T.spotShadowMap.length,
-            numSpotLightShadowsWithMaps: T.numSpotLightShadowsWithMaps,
-            numLightProbes: T.numLightProbes,
+            morphTargetsCount: de,
+            morphTextureStride: ge,
+            numDirLights: w.directional.length,
+            numPointLights: w.point.length,
+            numSpotLights: w.spot.length,
+            numSpotLightMaps: w.spotLightMap.length,
+            numRectAreaLights: w.rectArea.length,
+            numHemiLights: w.hemi.length,
+            numDirLightShadows: w.directionalShadowMap.length,
+            numPointLightShadows: w.pointShadowMap.length,
+            numSpotLightShadows: w.spotShadowMap.length,
+            numSpotLightShadowsWithMaps: w.numSpotLightShadowsWithMaps,
+            numLightProbes: w.numLightProbes,
             numClippingPlanes: o.numPlanes,
             numClipIntersection: o.numIntersection,
             dithering: v.dithering,
-            shadowMapEnabled: r.shadowMap.enabled && V.length > 0,
+            shadowMapEnabled: r.shadowMap.enabled && W.length > 0,
             shadowMapType: r.shadowMap.type,
             toneMapping: se,
             useLegacyLights: r._useLegacyLights,
-            decodeVideoTexture: we && v.map.isVideoTexture === !0 && qe.getTransfer(v.map.colorSpace) === Ze,
+            decodeVideoTexture: Ae && v.map.isVideoTexture === !0 && qe.getTransfer(v.map.colorSpace) === Ze,
             premultipliedAlpha: v.premultipliedAlpha,
             doubleSided: v.side === qt,
-            flipSided: v.side === Et,
+            flipSided: v.side === yt,
             useDepthPacking: v.depthPacking >= 0,
             depthPacking: v.depthPacking || 0,
             index0AttributeName: v.index0AttributeName,
             extensionDerivatives: le && v.extensions.derivatives === !0,
             extensionFragDepth: le && v.extensions.fragDepth === !0,
             extensionDrawBuffers: le && v.extensions.drawBuffers === !0,
             extensionShaderTextureLOD: le && v.extensions.shaderTextureLOD === !0,
@@ -11745,77 +11745,77 @@
             extensionMultiDraw: le && v.extensions.multiDraw === !0 && i.has("WEBGL_multi_draw"),
             rendererExtensionFragDepth: p || i.has("EXT_frag_depth"),
             rendererExtensionDrawBuffers: p || i.has("WEBGL_draw_buffers"),
             rendererExtensionShaderTextureLod: p || i.has("EXT_shader_texture_lod"),
             rendererExtensionParallelShaderCompile: i.has("KHR_parallel_shader_compile"),
             customProgramCacheKey: v.customProgramCacheKey()
         };
-        return Ge.vertexUv1s = c.has(1), Ge.vertexUv2s = c.has(2), Ge.vertexUv3s = c.has(3), c.clear(), Ge
+        return He.vertexUv1s = c.has(1), He.vertexUv2s = c.has(2), He.vertexUv3s = c.has(3), c.clear(), He
     }
 
-    function w(v) {
-        let T = [];
-        if (v.shaderID ? T.push(v.shaderID) : (T.push(v.customVertexShaderID), T.push(v.customFragmentShaderID)), v.defines !== void 0)
-            for (let V in v.defines) T.push(V), T.push(v.defines[V]);
-        return v.isRawShaderMaterial === !1 && (x(T, v), R(T, v), T.push(r.outputColorSpace)), T.push(v.customProgramCacheKey), T.join()
+    function T(v) {
+        let w = [];
+        if (v.shaderID ? w.push(v.shaderID) : (w.push(v.customVertexShaderID), w.push(v.customFragmentShaderID)), v.defines !== void 0)
+            for (let W in v.defines) w.push(W), w.push(v.defines[W]);
+        return v.isRawShaderMaterial === !1 && (x(w, v), A(w, v), w.push(r.outputColorSpace)), w.push(v.customProgramCacheKey), w.join()
     }
 
-    function x(v, T) {
-        v.push(T.precision), v.push(T.outputColorSpace), v.push(T.envMapMode), v.push(T.envMapCubeUVHeight), v.push(T.mapUv), v.push(T.alphaMapUv), v.push(T.lightMapUv), v.push(T.aoMapUv), v.push(T.bumpMapUv), v.push(T.normalMapUv), v.push(T.displacementMapUv), v.push(T.emissiveMapUv), v.push(T.metalnessMapUv), v.push(T.roughnessMapUv), v.push(T.anisotropyMapUv), v.push(T.clearcoatMapUv), v.push(T.clearcoatNormalMapUv), v.push(T.clearcoatRoughnessMapUv), v.push(T.iridescenceMapUv), v.push(T.iridescenceThicknessMapUv), v.push(T.sheenColorMapUv), v.push(T.sheenRoughnessMapUv), v.push(T.specularMapUv), v.push(T.specularColorMapUv), v.push(T.specularIntensityMapUv), v.push(T.transmissionMapUv), v.push(T.thicknessMapUv), v.push(T.combine), v.push(T.fogExp2), v.push(T.sizeAttenuation), v.push(T.morphTargetsCount), v.push(T.morphAttributeCount), v.push(T.numDirLights), v.push(T.numPointLights), v.push(T.numSpotLights), v.push(T.numSpotLightMaps), v.push(T.numHemiLights), v.push(T.numRectAreaLights), v.push(T.numDirLightShadows), v.push(T.numPointLightShadows), v.push(T.numSpotLightShadows), v.push(T.numSpotLightShadowsWithMaps), v.push(T.numLightProbes), v.push(T.shadowMapType), v.push(T.toneMapping), v.push(T.numClippingPlanes), v.push(T.numClipIntersection), v.push(T.depthPacking)
+    function x(v, w) {
+        v.push(w.precision), v.push(w.outputColorSpace), v.push(w.envMapMode), v.push(w.envMapCubeUVHeight), v.push(w.mapUv), v.push(w.alphaMapUv), v.push(w.lightMapUv), v.push(w.aoMapUv), v.push(w.bumpMapUv), v.push(w.normalMapUv), v.push(w.displacementMapUv), v.push(w.emissiveMapUv), v.push(w.metalnessMapUv), v.push(w.roughnessMapUv), v.push(w.anisotropyMapUv), v.push(w.clearcoatMapUv), v.push(w.clearcoatNormalMapUv), v.push(w.clearcoatRoughnessMapUv), v.push(w.iridescenceMapUv), v.push(w.iridescenceThicknessMapUv), v.push(w.sheenColorMapUv), v.push(w.sheenRoughnessMapUv), v.push(w.specularMapUv), v.push(w.specularColorMapUv), v.push(w.specularIntensityMapUv), v.push(w.transmissionMapUv), v.push(w.thicknessMapUv), v.push(w.combine), v.push(w.fogExp2), v.push(w.sizeAttenuation), v.push(w.morphTargetsCount), v.push(w.morphAttributeCount), v.push(w.numDirLights), v.push(w.numPointLights), v.push(w.numSpotLights), v.push(w.numSpotLightMaps), v.push(w.numHemiLights), v.push(w.numRectAreaLights), v.push(w.numDirLightShadows), v.push(w.numPointLightShadows), v.push(w.numSpotLightShadows), v.push(w.numSpotLightShadowsWithMaps), v.push(w.numLightProbes), v.push(w.shadowMapType), v.push(w.toneMapping), v.push(w.numClippingPlanes), v.push(w.numClipIntersection), v.push(w.depthPacking)
     }
 
-    function R(v, T) {
-        s.disableAll(), T.isWebGL2 && s.enable(0), T.supportsVertexTextures && s.enable(1), T.instancing && s.enable(2), T.instancingColor && s.enable(3), T.instancingMorph && s.enable(4), T.matcap && s.enable(5), T.envMap && s.enable(6), T.normalMapObjectSpace && s.enable(7), T.normalMapTangentSpace && s.enable(8), T.clearcoat && s.enable(9), T.iridescence && s.enable(10), T.alphaTest && s.enable(11), T.vertexColors && s.enable(12), T.vertexAlphas && s.enable(13), T.vertexUv1s && s.enable(14), T.vertexUv2s && s.enable(15), T.vertexUv3s && s.enable(16), T.vertexTangents && s.enable(17), T.anisotropy && s.enable(18), T.alphaHash && s.enable(19), T.batching && s.enable(20), v.push(s.mask), s.disableAll(), T.fog && s.enable(0), T.useFog && s.enable(1), T.flatShading && s.enable(2), T.logarithmicDepthBuffer && s.enable(3), T.skinning && s.enable(4), T.morphTargets && s.enable(5), T.morphNormals && s.enable(6), T.morphColors && s.enable(7), T.premultipliedAlpha && s.enable(8), T.shadowMapEnabled && s.enable(9), T.useLegacyLights && s.enable(10), T.doubleSided && s.enable(11), T.flipSided && s.enable(12), T.useDepthPacking && s.enable(13), T.dithering && s.enable(14), T.transmission && s.enable(15), T.sheen && s.enable(16), T.opaque && s.enable(17), T.pointsUvs && s.enable(18), T.decodeVideoTexture && s.enable(19), T.alphaToCoverage && s.enable(20), v.push(s.mask)
+    function A(v, w) {
+        s.disableAll(), w.isWebGL2 && s.enable(0), w.supportsVertexTextures && s.enable(1), w.instancing && s.enable(2), w.instancingColor && s.enable(3), w.instancingMorph && s.enable(4), w.matcap && s.enable(5), w.envMap && s.enable(6), w.normalMapObjectSpace && s.enable(7), w.normalMapTangentSpace && s.enable(8), w.clearcoat && s.enable(9), w.iridescence && s.enable(10), w.alphaTest && s.enable(11), w.vertexColors && s.enable(12), w.vertexAlphas && s.enable(13), w.vertexUv1s && s.enable(14), w.vertexUv2s && s.enable(15), w.vertexUv3s && s.enable(16), w.vertexTangents && s.enable(17), w.anisotropy && s.enable(18), w.alphaHash && s.enable(19), w.batching && s.enable(20), v.push(s.mask), s.disableAll(), w.fog && s.enable(0), w.useFog && s.enable(1), w.flatShading && s.enable(2), w.logarithmicDepthBuffer && s.enable(3), w.skinning && s.enable(4), w.morphTargets && s.enable(5), w.morphNormals && s.enable(6), w.morphColors && s.enable(7), w.premultipliedAlpha && s.enable(8), w.shadowMapEnabled && s.enable(9), w.useLegacyLights && s.enable(10), w.doubleSided && s.enable(11), w.flipSided && s.enable(12), w.useDepthPacking && s.enable(13), w.dithering && s.enable(14), w.transmission && s.enable(15), w.sheen && s.enable(16), w.opaque && s.enable(17), w.pointsUvs && s.enable(18), w.decodeVideoTexture && s.enable(19), w.alphaToCoverage && s.enable(20), v.push(s.mask)
     }
 
-    function U(v) {
-        let T = M[v.type],
-            V;
-        if (T) {
-            let K = zt[T];
-            V = Nc.clone(K.uniforms)
-        } else V = v.uniforms;
-        return V
+    function D(v) {
+        let w = M[v.type],
+            W;
+        if (w) {
+            let K = Bt[w];
+            W = Ic.clone(K.uniforms)
+        } else W = v.uniforms;
+        return W
     }
 
-    function A(v, T) {
-        let V;
-        for (let K = 0, P = u.length; K < P; K++) {
-            let X = u[K];
-            if (X.cacheKey === T) {
-                V = X, ++V.usedTimes;
+    function R(v, w) {
+        let W;
+        for (let K = 0, L = h.length; K < L; K++) {
+            let j = h[K];
+            if (j.cacheKey === w) {
+                W = j, ++W.usedTimes;
                 break
             }
         }
-        return V === void 0 && (V = new Xp(r, T, v, a), u.push(V)), V
+        return W === void 0 && (W = new Xp(r, w, v, a), h.push(W)), W
     }
 
-    function y(v) {
+    function b(v) {
         if (--v.usedTimes === 0) {
-            let T = u.indexOf(v);
-            u[T] = u[u.length - 1], u.pop(), v.destroy()
+            let w = h.indexOf(v);
+            h[w] = h[h.length - 1], h.pop(), v.destroy()
         }
     }
 
-    function C(v) {
+    function P(v) {
         l.remove(v)
     }
 
-    function Z() {
+    function I() {
         l.dispose()
     }
     return {
-        getParameters: h,
-        getProgramCacheKey: w,
-        getUniforms: U,
-        acquireProgram: A,
-        releaseProgram: y,
-        releaseShaderCache: C,
-        programs: u,
-        dispose: Z
+        getParameters: u,
+        getProgramCacheKey: T,
+        getUniforms: D,
+        acquireProgram: R,
+        releaseProgram: b,
+        releaseShaderCache: P,
+        programs: h,
+        dispose: I
     }
 }
 
 function qp() {
     let r = new WeakMap;
 
     function e(a) {
@@ -11858,56 +11858,56 @@
         n = [];
 
     function a() {
         e = 0, t.length = 0, i.length = 0, n.length = 0
     }
 
     function o(p, f, m, _, M, d) {
-        let h = r[e];
-        return h === void 0 ? (h = {
+        let u = r[e];
+        return u === void 0 ? (u = {
             id: p.id,
             object: p,
             geometry: f,
             material: m,
             groupOrder: _,
             renderOrder: p.renderOrder,
             z: M,
             group: d
-        }, r[e] = h) : (h.id = p.id, h.object = p, h.geometry = f, h.material = m, h.groupOrder = _, h.renderOrder = p.renderOrder, h.z = M, h.group = d), e++, h
+        }, r[e] = u) : (u.id = p.id, u.object = p, u.geometry = f, u.material = m, u.groupOrder = _, u.renderOrder = p.renderOrder, u.z = M, u.group = d), e++, u
     }
 
     function s(p, f, m, _, M, d) {
-        let h = o(p, f, m, _, M, d);
-        m.transmission > 0 ? i.push(h) : m.transparent === !0 ? n.push(h) : t.push(h)
+        let u = o(p, f, m, _, M, d);
+        m.transmission > 0 ? i.push(u) : m.transparent === !0 ? n.push(u) : t.push(u)
     }
 
     function l(p, f, m, _, M, d) {
-        let h = o(p, f, m, _, M, d);
-        m.transmission > 0 ? i.unshift(h) : m.transparent === !0 ? n.unshift(h) : t.unshift(h)
+        let u = o(p, f, m, _, M, d);
+        m.transmission > 0 ? i.unshift(u) : m.transparent === !0 ? n.unshift(u) : t.unshift(u)
     }
 
     function c(p, f) {
         t.length > 1 && t.sort(p || Zp), i.length > 1 && i.sort(f || vo), n.length > 1 && n.sort(f || vo)
     }
 
-    function u() {
+    function h() {
         for (let p = e, f = r.length; p < f; p++) {
             let m = r[p];
             if (m.id === null) break;
             m.id = null, m.object = null, m.geometry = null, m.material = null, m.group = null
         }
     }
     return {
         opaque: t,
         transmissive: i,
         transparent: n,
         init: a,
         push: s,
         unshift: l,
-        finish: u,
+        finish: h,
         sort: c
     }
 }
 
 function Kp() {
     let r = new WeakMap;
 
@@ -11931,50 +11931,50 @@
     return {
         get: function(e) {
             if (r[e.id] !== void 0) return r[e.id];
             let t;
             switch (e.type) {
                 case "DirectionalLight":
                     t = {
-                        direction: new D,
+                        direction: new U,
                         color: new Ye
                     };
                     break;
                 case "SpotLight":
                     t = {
-                        position: new D,
-                        direction: new D,
+                        position: new U,
+                        direction: new U,
                         color: new Ye,
                         distance: 0,
                         coneCos: 0,
                         penumbraCos: 0,
                         decay: 0
                     };
                     break;
                 case "PointLight":
                     t = {
-                        position: new D,
+                        position: new U,
                         color: new Ye,
                         distance: 0,
                         decay: 0
                     };
                     break;
                 case "HemisphereLight":
                     t = {
-                        direction: new D,
+                        direction: new U,
                         skyColor: new Ye,
                         groundColor: new Ye
                     };
                     break;
                 case "RectAreaLight":
                     t = {
                         color: new Ye,
-                        position: new D,
-                        halfWidth: new D,
-                        halfHeight: new D
+                        position: new U,
+                        halfWidth: new U,
+                        halfHeight: new U
                     };
                     break
             }
             return r[e.id] = t, t
         }
     }
 }
@@ -11987,31 +11987,31 @@
             let t;
             switch (e.type) {
                 case "DirectionalLight":
                     t = {
                         shadowBias: 0,
                         shadowNormalBias: 0,
                         shadowRadius: 1,
-                        shadowMapSize: new De
+                        shadowMapSize: new Ue
                     };
                     break;
                 case "SpotLight":
                     t = {
                         shadowBias: 0,
                         shadowNormalBias: 0,
                         shadowRadius: 1,
-                        shadowMapSize: new De
+                        shadowMapSize: new Ue
                     };
                     break;
                 case "PointLight":
                     t = {
                         shadowBias: 0,
                         shadowNormalBias: 0,
                         shadowRadius: 1,
-                        shadowMapSize: new De,
+                        shadowMapSize: new Ue,
                         shadowCameraNear: 1,
                         shadowCameraFar: 1e3
                     };
                     break
             }
             return r[e.id] = t, t
         }
@@ -12058,109 +12058,109 @@
             pointShadow: [],
             pointShadowMap: [],
             pointShadowMatrix: [],
             hemi: [],
             numSpotLightShadowsWithMaps: 0,
             numLightProbes: 0
         };
-    for (let u = 0; u < 9; u++) n.probe.push(new D);
-    let a = new D,
+    for (let h = 0; h < 9; h++) n.probe.push(new U);
+    let a = new U,
         o = new at,
         s = new at;
 
-    function l(u, p) {
+    function l(h, p) {
         let f = 0,
             m = 0,
             _ = 0;
-        for (let V = 0; V < 9; V++) n.probe[V].set(0, 0, 0);
+        for (let W = 0; W < 9; W++) n.probe[W].set(0, 0, 0);
         let M = 0,
             d = 0,
-            h = 0,
-            w = 0,
+            u = 0,
+            T = 0,
             x = 0,
-            R = 0,
-            U = 0,
             A = 0,
-            y = 0,
-            C = 0,
-            Z = 0;
-        u.sort(ef);
+            D = 0,
+            R = 0,
+            b = 0,
+            P = 0,
+            I = 0;
+        h.sort(ef);
         let v = p === !0 ? Math.PI : 1;
-        for (let V = 0, K = u.length; V < K; V++) {
-            let P = u[V],
-                X = P.color,
-                k = P.intensity,
-                j = P.distance,
-                q = P.shadow && P.shadow.map ? P.shadow.map.texture : null;
-            if (P.isAmbientLight) f += X.r * k * v, m += X.g * k * v, _ += X.b * k * v;
-            else if (P.isLightProbe) {
-                for (let W = 0; W < 9; W++) n.probe[W].addScaledVector(P.sh.coefficients[W], k);
-                Z++
-            } else if (P.isDirectionalLight) {
-                let W = t.get(P);
-                if (W.color.copy(P.color).multiplyScalar(P.intensity * v), P.castShadow) {
-                    let te = P.shadow,
-                        ee = i.get(P);
-                    ee.shadowBias = te.bias, ee.shadowNormalBias = te.normalBias, ee.shadowRadius = te.radius, ee.shadowMapSize = te.mapSize, n.directionalShadow[M] = ee, n.directionalShadowMap[M] = q, n.directionalShadowMatrix[M] = P.shadow.matrix, R++
-                }
-                n.directional[M] = W, M++
-            } else if (P.isSpotLight) {
-                let W = t.get(P);
-                W.position.setFromMatrixPosition(P.matrixWorld), W.color.copy(X).multiplyScalar(k * v), W.distance = j, W.coneCos = Math.cos(P.angle), W.penumbraCos = Math.cos(P.angle * (1 - P.penumbra)), W.decay = P.decay, n.spot[h] = W;
-                let te = P.shadow;
-                if (P.map && (n.spotLightMap[y] = P.map, y++, te.updateMatrices(P), P.castShadow && C++), n.spotLightMatrix[h] = te.matrix, P.castShadow) {
-                    let ee = i.get(P);
-                    ee.shadowBias = te.bias, ee.shadowNormalBias = te.normalBias, ee.shadowRadius = te.radius, ee.shadowMapSize = te.mapSize, n.spotShadow[h] = ee, n.spotShadowMap[h] = q, A++
-                }
-                h++
-            } else if (P.isRectAreaLight) {
-                let W = t.get(P);
-                W.color.copy(X).multiplyScalar(k), W.halfWidth.set(P.width * .5, 0, 0), W.halfHeight.set(0, P.height * .5, 0), n.rectArea[w] = W, w++
-            } else if (P.isPointLight) {
-                let W = t.get(P);
-                if (W.color.copy(P.color).multiplyScalar(P.intensity * v), W.distance = P.distance, W.decay = P.decay, P.castShadow) {
-                    let te = P.shadow,
-                        ee = i.get(P);
-                    ee.shadowBias = te.bias, ee.shadowNormalBias = te.normalBias, ee.shadowRadius = te.radius, ee.shadowMapSize = te.mapSize, ee.shadowCameraNear = te.camera.near, ee.shadowCameraFar = te.camera.far, n.pointShadow[d] = ee, n.pointShadowMap[d] = q, n.pointShadowMatrix[d] = P.shadow.matrix, U++
-                }
-                n.point[d] = W, d++
-            } else if (P.isHemisphereLight) {
-                let W = t.get(P);
-                W.skyColor.copy(P.color).multiplyScalar(k * v), W.groundColor.copy(P.groundColor).multiplyScalar(k * v), n.hemi[x] = W, x++
-            }
-        }
-        w > 0 && (e.isWebGL2 ? r.has("OES_texture_float_linear") === !0 ? (n.rectAreaLTC1 = ce.LTC_FLOAT_1, n.rectAreaLTC2 = ce.LTC_FLOAT_2) : (n.rectAreaLTC1 = ce.LTC_HALF_1, n.rectAreaLTC2 = ce.LTC_HALF_2) : r.has("OES_texture_float_linear") === !0 ? (n.rectAreaLTC1 = ce.LTC_FLOAT_1, n.rectAreaLTC2 = ce.LTC_FLOAT_2) : r.has("OES_texture_half_float_linear") === !0 ? (n.rectAreaLTC1 = ce.LTC_HALF_1, n.rectAreaLTC2 = ce.LTC_HALF_2) : console.error("THREE.WebGLRenderer: Unable to use RectAreaLight. Missing WebGL extensions.")), n.ambient[0] = f, n.ambient[1] = m, n.ambient[2] = _;
-        let T = n.hash;
-        (T.directionalLength !== M || T.pointLength !== d || T.spotLength !== h || T.rectAreaLength !== w || T.hemiLength !== x || T.numDirectionalShadows !== R || T.numPointShadows !== U || T.numSpotShadows !== A || T.numSpotMaps !== y || T.numLightProbes !== Z) && (n.directional.length = M, n.spot.length = h, n.rectArea.length = w, n.point.length = d, n.hemi.length = x, n.directionalShadow.length = R, n.directionalShadowMap.length = R, n.pointShadow.length = U, n.pointShadowMap.length = U, n.spotShadow.length = A, n.spotShadowMap.length = A, n.directionalShadowMatrix.length = R, n.pointShadowMatrix.length = U, n.spotLightMatrix.length = A + y - C, n.spotLightMap.length = y, n.numSpotLightShadowsWithMaps = C, n.numLightProbes = Z, T.directionalLength = M, T.pointLength = d, T.spotLength = h, T.rectAreaLength = w, T.hemiLength = x, T.numDirectionalShadows = R, T.numPointShadows = U, T.numSpotShadows = A, T.numSpotMaps = y, T.numLightProbes = Z, n.version = Qp++)
+        for (let W = 0, K = h.length; W < K; W++) {
+            let L = h[W],
+                j = L.color,
+                k = L.intensity,
+                Y = L.distance,
+                q = L.shadow && L.shadow.map ? L.shadow.map.texture : null;
+            if (L.isAmbientLight) f += j.r * k * v, m += j.g * k * v, _ += j.b * k * v;
+            else if (L.isLightProbe) {
+                for (let Z = 0; Z < 9; Z++) n.probe[Z].addScaledVector(L.sh.coefficients[Z], k);
+                I++
+            } else if (L.isDirectionalLight) {
+                let Z = t.get(L);
+                if (Z.color.copy(L.color).multiplyScalar(L.intensity * v), L.castShadow) {
+                    let ee = L.shadow,
+                        ie = i.get(L);
+                    ie.shadowBias = ee.bias, ie.shadowNormalBias = ee.normalBias, ie.shadowRadius = ee.radius, ie.shadowMapSize = ee.mapSize, n.directionalShadow[M] = ie, n.directionalShadowMap[M] = q, n.directionalShadowMatrix[M] = L.shadow.matrix, A++
+                }
+                n.directional[M] = Z, M++
+            } else if (L.isSpotLight) {
+                let Z = t.get(L);
+                Z.position.setFromMatrixPosition(L.matrixWorld), Z.color.copy(j).multiplyScalar(k * v), Z.distance = Y, Z.coneCos = Math.cos(L.angle), Z.penumbraCos = Math.cos(L.angle * (1 - L.penumbra)), Z.decay = L.decay, n.spot[u] = Z;
+                let ee = L.shadow;
+                if (L.map && (n.spotLightMap[b] = L.map, b++, ee.updateMatrices(L), L.castShadow && P++), n.spotLightMatrix[u] = ee.matrix, L.castShadow) {
+                    let ie = i.get(L);
+                    ie.shadowBias = ee.bias, ie.shadowNormalBias = ee.normalBias, ie.shadowRadius = ee.radius, ie.shadowMapSize = ee.mapSize, n.spotShadow[u] = ie, n.spotShadowMap[u] = q, R++
+                }
+                u++
+            } else if (L.isRectAreaLight) {
+                let Z = t.get(L);
+                Z.color.copy(j).multiplyScalar(k), Z.halfWidth.set(L.width * .5, 0, 0), Z.halfHeight.set(0, L.height * .5, 0), n.rectArea[T] = Z, T++
+            } else if (L.isPointLight) {
+                let Z = t.get(L);
+                if (Z.color.copy(L.color).multiplyScalar(L.intensity * v), Z.distance = L.distance, Z.decay = L.decay, L.castShadow) {
+                    let ee = L.shadow,
+                        ie = i.get(L);
+                    ie.shadowBias = ee.bias, ie.shadowNormalBias = ee.normalBias, ie.shadowRadius = ee.radius, ie.shadowMapSize = ee.mapSize, ie.shadowCameraNear = ee.camera.near, ie.shadowCameraFar = ee.camera.far, n.pointShadow[d] = ie, n.pointShadowMap[d] = q, n.pointShadowMatrix[d] = L.shadow.matrix, D++
+                }
+                n.point[d] = Z, d++
+            } else if (L.isHemisphereLight) {
+                let Z = t.get(L);
+                Z.skyColor.copy(L.color).multiplyScalar(k * v), Z.groundColor.copy(L.groundColor).multiplyScalar(k * v), n.hemi[x] = Z, x++
+            }
+        }
+        T > 0 && (e.isWebGL2 ? r.has("OES_texture_float_linear") === !0 ? (n.rectAreaLTC1 = ce.LTC_FLOAT_1, n.rectAreaLTC2 = ce.LTC_FLOAT_2) : (n.rectAreaLTC1 = ce.LTC_HALF_1, n.rectAreaLTC2 = ce.LTC_HALF_2) : r.has("OES_texture_float_linear") === !0 ? (n.rectAreaLTC1 = ce.LTC_FLOAT_1, n.rectAreaLTC2 = ce.LTC_FLOAT_2) : r.has("OES_texture_half_float_linear") === !0 ? (n.rectAreaLTC1 = ce.LTC_HALF_1, n.rectAreaLTC2 = ce.LTC_HALF_2) : console.error("THREE.WebGLRenderer: Unable to use RectAreaLight. Missing WebGL extensions.")), n.ambient[0] = f, n.ambient[1] = m, n.ambient[2] = _;
+        let w = n.hash;
+        (w.directionalLength !== M || w.pointLength !== d || w.spotLength !== u || w.rectAreaLength !== T || w.hemiLength !== x || w.numDirectionalShadows !== A || w.numPointShadows !== D || w.numSpotShadows !== R || w.numSpotMaps !== b || w.numLightProbes !== I) && (n.directional.length = M, n.spot.length = u, n.rectArea.length = T, n.point.length = d, n.hemi.length = x, n.directionalShadow.length = A, n.directionalShadowMap.length = A, n.pointShadow.length = D, n.pointShadowMap.length = D, n.spotShadow.length = R, n.spotShadowMap.length = R, n.directionalShadowMatrix.length = A, n.pointShadowMatrix.length = D, n.spotLightMatrix.length = R + b - P, n.spotLightMap.length = b, n.numSpotLightShadowsWithMaps = P, n.numLightProbes = I, w.directionalLength = M, w.pointLength = d, w.spotLength = u, w.rectAreaLength = T, w.hemiLength = x, w.numDirectionalShadows = A, w.numPointShadows = D, w.numSpotShadows = R, w.numSpotMaps = b, w.numLightProbes = I, n.version = Qp++)
     }
 
-    function c(u, p) {
+    function c(h, p) {
         let f = 0,
             m = 0,
             _ = 0,
             M = 0,
             d = 0,
-            h = p.matrixWorldInverse;
-        for (let w = 0, x = u.length; w < x; w++) {
-            let R = u[w];
-            if (R.isDirectionalLight) {
-                let U = n.directional[f];
-                U.direction.setFromMatrixPosition(R.matrixWorld), a.setFromMatrixPosition(R.target.matrixWorld), U.direction.sub(a), U.direction.transformDirection(h), f++
-            } else if (R.isSpotLight) {
-                let U = n.spot[_];
-                U.position.setFromMatrixPosition(R.matrixWorld), U.position.applyMatrix4(h), U.direction.setFromMatrixPosition(R.matrixWorld), a.setFromMatrixPosition(R.target.matrixWorld), U.direction.sub(a), U.direction.transformDirection(h), _++
-            } else if (R.isRectAreaLight) {
-                let U = n.rectArea[M];
-                U.position.setFromMatrixPosition(R.matrixWorld), U.position.applyMatrix4(h), s.identity(), o.copy(R.matrixWorld), o.premultiply(h), s.extractRotation(o), U.halfWidth.set(R.width * .5, 0, 0), U.halfHeight.set(0, R.height * .5, 0), U.halfWidth.applyMatrix4(s), U.halfHeight.applyMatrix4(s), M++
-            } else if (R.isPointLight) {
-                let U = n.point[m];
-                U.position.setFromMatrixPosition(R.matrixWorld), U.position.applyMatrix4(h), m++
-            } else if (R.isHemisphereLight) {
-                let U = n.hemi[d];
-                U.direction.setFromMatrixPosition(R.matrixWorld), U.direction.transformDirection(h), d++
+            u = p.matrixWorldInverse;
+        for (let T = 0, x = h.length; T < x; T++) {
+            let A = h[T];
+            if (A.isDirectionalLight) {
+                let D = n.directional[f];
+                D.direction.setFromMatrixPosition(A.matrixWorld), a.setFromMatrixPosition(A.target.matrixWorld), D.direction.sub(a), D.direction.transformDirection(u), f++
+            } else if (A.isSpotLight) {
+                let D = n.spot[_];
+                D.position.setFromMatrixPosition(A.matrixWorld), D.position.applyMatrix4(u), D.direction.setFromMatrixPosition(A.matrixWorld), a.setFromMatrixPosition(A.target.matrixWorld), D.direction.sub(a), D.direction.transformDirection(u), _++
+            } else if (A.isRectAreaLight) {
+                let D = n.rectArea[M];
+                D.position.setFromMatrixPosition(A.matrixWorld), D.position.applyMatrix4(u), s.identity(), o.copy(A.matrixWorld), o.premultiply(u), s.extractRotation(o), D.halfWidth.set(A.width * .5, 0, 0), D.halfHeight.set(0, A.height * .5, 0), D.halfWidth.applyMatrix4(s), D.halfHeight.applyMatrix4(s), M++
+            } else if (A.isPointLight) {
+                let D = n.point[m];
+                D.position.setFromMatrixPosition(A.matrixWorld), D.position.applyMatrix4(u), m++
+            } else if (A.isHemisphereLight) {
+                let D = n.hemi[d];
+                D.direction.setFromMatrixPosition(A.matrixWorld), D.direction.transformDirection(u), d++
             }
         }
     }
     return {
         setup: l,
         setupView: c,
         state: n
@@ -12172,28 +12172,28 @@
         i = [],
         n = [];
 
     function a() {
         i.length = 0, n.length = 0
     }
 
-    function o(u) {
-        i.push(u)
+    function o(h) {
+        i.push(h)
     }
 
-    function s(u) {
-        n.push(u)
+    function s(h) {
+        n.push(h)
     }
 
-    function l(u) {
-        t.setup(i, u)
+    function l(h) {
+        t.setup(i, h)
     }
 
-    function c(u) {
-        t.setupView(i, u)
+    function c(h) {
+        t.setupView(i, h)
     }
     return {
         init: a,
         state: {
             lightsArray: i,
             shadowsArray: n,
             lights: t
@@ -12226,15 +12226,15 @@
         constructor(e) {
             super(), this.isMeshDepthMaterial = !0, this.type = "MeshDepthMaterial", this.depthPacking = Xl, this.map = null, this.alphaMap = null, this.displacementMap = null, this.displacementScale = 1, this.displacementBias = 0, this.wireframe = !1, this.wireframeLinewidth = 1, this.setValues(e)
         }
         copy(e) {
             return super.copy(e), this.depthPacking = e.depthPacking, this.map = e.map, this.alphaMap = e.alphaMap, this.displacementMap = e.displacementMap, this.displacementScale = e.displacementScale, this.displacementBias = e.displacementBias, this.wireframe = e.wireframe, this.wireframeLinewidth = e.wireframeLinewidth, this
         }
     },
-    Ua = class extends Pi {
+    Da = class extends Pi {
         constructor(e) {
             super(), this.isMeshDistanceMaterial = !0, this.type = "MeshDistanceMaterial", this.map = null, this.alphaMap = null, this.displacementMap = null, this.displacementScale = 1, this.displacementBias = 0, this.setValues(e)
         }
         copy(e) {
             return super.copy(e), this.map = e.map, this.alphaMap = e.alphaMap, this.displacementMap = e.displacementMap, this.displacementScale = e.displacementScale, this.displacementBias = e.displacementBias, this
         }
     },
@@ -12267,356 +12267,356 @@
 	squared_mean = squared_mean / samples;
 	float std_dev = sqrt( squared_mean - mean * mean );
 	gl_FragColor = pack2HalfToRGBA( vec2( mean, std_dev ) );
 }`;
 
 function sf(r, e, t) {
     let i = new gn,
-        n = new De,
-        a = new De,
+        n = new Ue,
+        a = new Ue,
         o = new ct,
         s = new Pa({
             depthPacking: jl
         }),
-        l = new Ua,
+        l = new Da,
         c = {},
-        u = t.maxTextureSize,
+        h = t.maxTextureSize,
         p = {
-            [pi]: Et,
-            [Et]: pi,
+            [pi]: yt,
+            [yt]: pi,
             [qt]: qt
         },
-        f = new Gt({
+        f = new Ht({
             defines: {
                 VSM_SAMPLES: 8
             },
             uniforms: {
                 shadow_pass: {
                     value: null
                 },
                 resolution: {
-                    value: new De
+                    value: new Ue
                 },
                 radius: {
                     value: 4
                 }
             },
             vertexShader: nf,
             fragmentShader: af
         }),
         m = f.clone();
     m.defines.HORIZONTAL_PASS = 1;
-    let _ = new St;
+    let _ = new Et;
     _.setAttribute("position", new Lt(new Float32Array([-1, -1, .5, 3, -1, .5, -1, 3, .5]), 3));
     let M = new vt(_, f),
         d = this;
     this.enabled = !1, this.autoUpdate = !0, this.needsUpdate = !1, this.type = Lo;
-    let h = this.type;
-    this.render = function(A, y, C) {
-        if (d.enabled === !1 || d.autoUpdate === !1 && d.needsUpdate === !1 || A.length === 0) return;
-        let Z = r.getRenderTarget(),
+    let u = this.type;
+    this.render = function(R, b, P) {
+        if (d.enabled === !1 || d.autoUpdate === !1 && d.needsUpdate === !1 || R.length === 0) return;
+        let I = r.getRenderTarget(),
             v = r.getActiveCubeFace(),
-            T = r.getActiveMipmapLevel(),
-            V = r.state;
-        V.setBlending(ci), V.buffers.color.setClear(1, 1, 1, 1), V.buffers.depth.setTest(!0), V.setScissorTest(!1);
-        let K = h !== Yt && this.type === Yt,
-            P = h === Yt && this.type !== Yt;
-        for (let X = 0, k = A.length; X < k; X++) {
-            let j = A[X],
-                q = j.shadow;
+            w = r.getActiveMipmapLevel(),
+            W = r.state;
+        W.setBlending(ci), W.buffers.color.setClear(1, 1, 1, 1), W.buffers.depth.setTest(!0), W.setScissorTest(!1);
+        let K = u !== Yt && this.type === Yt,
+            L = u === Yt && this.type !== Yt;
+        for (let j = 0, k = R.length; j < k; j++) {
+            let Y = R[j],
+                q = Y.shadow;
             if (q === void 0) {
-                console.warn("THREE.WebGLShadowMap:", j, "has no shadow.");
+                console.warn("THREE.WebGLShadowMap:", Y, "has no shadow.");
                 continue
             }
             if (q.autoUpdate === !1 && q.needsUpdate === !1) continue;
             n.copy(q.mapSize);
-            let W = q.getFrameExtents();
-            if (n.multiply(W), a.copy(q.mapSize), (n.x > u || n.y > u) && (n.x > u && (a.x = Math.floor(u / W.x), n.x = a.x * W.x, q.mapSize.x = a.x), n.y > u && (a.y = Math.floor(u / W.y), n.y = a.y * W.y, q.mapSize.y = a.y)), q.map === null || K === !0 || P === !0) {
-                let ee = this.type !== Yt ? {
+            let Z = q.getFrameExtents();
+            if (n.multiply(Z), a.copy(q.mapSize), (n.x > h || n.y > h) && (n.x > h && (a.x = Math.floor(h / Z.x), n.x = a.x * Z.x, q.mapSize.x = a.x), n.y > h && (a.y = Math.floor(h / Z.y), n.y = a.y * Z.y, q.mapSize.y = a.y)), q.map === null || K === !0 || L === !0) {
+                let ie = this.type !== Yt ? {
                     minFilter: _t,
                     magFilter: _t
                 } : {};
-                q.map !== null && q.map.dispose(), q.map = new $t(n.x, n.y, ee), q.map.texture.name = j.name + ".shadowMap", q.camera.updateProjectionMatrix()
+                q.map !== null && q.map.dispose(), q.map = new $t(n.x, n.y, ie), q.map.texture.name = Y.name + ".shadowMap", q.camera.updateProjectionMatrix()
             }
             r.setRenderTarget(q.map), r.clear();
-            let te = q.getViewportCount();
-            for (let ee = 0; ee < te; ee++) {
-                let pe = q.getViewport(ee);
-                o.set(a.x * pe.x, a.y * pe.y, a.x * pe.z, a.y * pe.w), V.viewport(o), q.updateMatrices(j, ee), i = q.getFrustum(), R(y, C, q.camera, j, this.type)
+            let ee = q.getViewportCount();
+            for (let ie = 0; ie < ee; ie++) {
+                let de = q.getViewport(ie);
+                o.set(a.x * de.x, a.y * de.y, a.x * de.z, a.y * de.w), W.viewport(o), q.updateMatrices(Y, ie), i = q.getFrustum(), A(b, P, q.camera, Y, this.type)
             }
-            q.isPointLightShadow !== !0 && this.type === Yt && w(q, C), q.needsUpdate = !1
+            q.isPointLightShadow !== !0 && this.type === Yt && T(q, P), q.needsUpdate = !1
         }
-        h = this.type, d.needsUpdate = !1, r.setRenderTarget(Z, v, T)
+        u = this.type, d.needsUpdate = !1, r.setRenderTarget(I, v, w)
     };
 
-    function w(A, y) {
-        let C = e.update(M);
-        f.defines.VSM_SAMPLES !== A.blurSamples && (f.defines.VSM_SAMPLES = A.blurSamples, m.defines.VSM_SAMPLES = A.blurSamples, f.needsUpdate = !0, m.needsUpdate = !0), A.mapPass === null && (A.mapPass = new $t(n.x, n.y)), f.uniforms.shadow_pass.value = A.map.texture, f.uniforms.resolution.value = A.mapSize, f.uniforms.radius.value = A.radius, r.setRenderTarget(A.mapPass), r.clear(), r.renderBufferDirect(y, null, C, f, M, null), m.uniforms.shadow_pass.value = A.mapPass.texture, m.uniforms.resolution.value = A.mapSize, m.uniforms.radius.value = A.radius, r.setRenderTarget(A.map), r.clear(), r.renderBufferDirect(y, null, C, m, M, null)
+    function T(R, b) {
+        let P = e.update(M);
+        f.defines.VSM_SAMPLES !== R.blurSamples && (f.defines.VSM_SAMPLES = R.blurSamples, m.defines.VSM_SAMPLES = R.blurSamples, f.needsUpdate = !0, m.needsUpdate = !0), R.mapPass === null && (R.mapPass = new $t(n.x, n.y)), f.uniforms.shadow_pass.value = R.map.texture, f.uniforms.resolution.value = R.mapSize, f.uniforms.radius.value = R.radius, r.setRenderTarget(R.mapPass), r.clear(), r.renderBufferDirect(b, null, P, f, M, null), m.uniforms.shadow_pass.value = R.mapPass.texture, m.uniforms.resolution.value = R.mapSize, m.uniforms.radius.value = R.radius, r.setRenderTarget(R.map), r.clear(), r.renderBufferDirect(b, null, P, m, M, null)
     }
 
-    function x(A, y, C, Z) {
+    function x(R, b, P, I) {
         let v = null,
-            T = C.isPointLight === !0 ? A.customDistanceMaterial : A.customDepthMaterial;
-        if (T !== void 0) v = T;
-        else if (v = C.isPointLight === !0 ? l : s, r.localClippingEnabled && y.clipShadows === !0 && Array.isArray(y.clippingPlanes) && y.clippingPlanes.length !== 0 || y.displacementMap && y.displacementScale !== 0 || y.alphaMap && y.alphaTest > 0 || y.map && y.alphaTest > 0) {
-            let V = v.uuid,
-                K = y.uuid,
-                P = c[V];
-            P === void 0 && (P = {}, c[V] = P);
-            let X = P[K];
-            X === void 0 && (X = v.clone(), P[K] = X, y.addEventListener("dispose", U)), v = X
-        }
-        if (v.visible = y.visible, v.wireframe = y.wireframe, Z === Yt ? v.side = y.shadowSide !== null ? y.shadowSide : y.side : v.side = y.shadowSide !== null ? y.shadowSide : p[y.side], v.alphaMap = y.alphaMap, v.alphaTest = y.alphaTest, v.map = y.map, v.clipShadows = y.clipShadows, v.clippingPlanes = y.clippingPlanes, v.clipIntersection = y.clipIntersection, v.displacementMap = y.displacementMap, v.displacementScale = y.displacementScale, v.displacementBias = y.displacementBias, v.wireframeLinewidth = y.wireframeLinewidth, v.linewidth = y.linewidth, C.isPointLight === !0 && v.isMeshDistanceMaterial === !0) {
-            let V = r.properties.get(v);
-            V.light = C
+            w = P.isPointLight === !0 ? R.customDistanceMaterial : R.customDepthMaterial;
+        if (w !== void 0) v = w;
+        else if (v = P.isPointLight === !0 ? l : s, r.localClippingEnabled && b.clipShadows === !0 && Array.isArray(b.clippingPlanes) && b.clippingPlanes.length !== 0 || b.displacementMap && b.displacementScale !== 0 || b.alphaMap && b.alphaTest > 0 || b.map && b.alphaTest > 0) {
+            let W = v.uuid,
+                K = b.uuid,
+                L = c[W];
+            L === void 0 && (L = {}, c[W] = L);
+            let j = L[K];
+            j === void 0 && (j = v.clone(), L[K] = j, b.addEventListener("dispose", D)), v = j
+        }
+        if (v.visible = b.visible, v.wireframe = b.wireframe, I === Yt ? v.side = b.shadowSide !== null ? b.shadowSide : b.side : v.side = b.shadowSide !== null ? b.shadowSide : p[b.side], v.alphaMap = b.alphaMap, v.alphaTest = b.alphaTest, v.map = b.map, v.clipShadows = b.clipShadows, v.clippingPlanes = b.clippingPlanes, v.clipIntersection = b.clipIntersection, v.displacementMap = b.displacementMap, v.displacementScale = b.displacementScale, v.displacementBias = b.displacementBias, v.wireframeLinewidth = b.wireframeLinewidth, v.linewidth = b.linewidth, P.isPointLight === !0 && v.isMeshDistanceMaterial === !0) {
+            let W = r.properties.get(v);
+            W.light = P
         }
         return v
     }
 
-    function R(A, y, C, Z, v) {
-        if (A.visible === !1) return;
-        if (A.layers.test(y.layers) && (A.isMesh || A.isLine || A.isPoints) && (A.castShadow || A.receiveShadow && v === Yt) && (!A.frustumCulled || i.intersectsObject(A))) {
-            A.modelViewMatrix.multiplyMatrices(C.matrixWorldInverse, A.matrixWorld);
-            let V = e.update(A),
-                K = A.material;
+    function A(R, b, P, I, v) {
+        if (R.visible === !1) return;
+        if (R.layers.test(b.layers) && (R.isMesh || R.isLine || R.isPoints) && (R.castShadow || R.receiveShadow && v === Yt) && (!R.frustumCulled || i.intersectsObject(R))) {
+            R.modelViewMatrix.multiplyMatrices(P.matrixWorldInverse, R.matrixWorld);
+            let W = e.update(R),
+                K = R.material;
             if (Array.isArray(K)) {
-                let P = V.groups;
-                for (let X = 0, k = P.length; X < k; X++) {
-                    let j = P[X],
-                        q = K[j.materialIndex];
+                let L = W.groups;
+                for (let j = 0, k = L.length; j < k; j++) {
+                    let Y = L[j],
+                        q = K[Y.materialIndex];
                     if (q && q.visible) {
-                        let W = x(A, q, Z, v);
-                        A.onBeforeShadow(r, A, y, C, V, W, j), r.renderBufferDirect(C, null, V, W, A, j), A.onAfterShadow(r, A, y, C, V, W, j)
+                        let Z = x(R, q, I, v);
+                        R.onBeforeShadow(r, R, b, P, W, Z, Y), r.renderBufferDirect(P, null, W, Z, R, Y), R.onAfterShadow(r, R, b, P, W, Z, Y)
                     }
                 }
             } else if (K.visible) {
-                let P = x(A, K, Z, v);
-                A.onBeforeShadow(r, A, y, C, V, P, null), r.renderBufferDirect(C, null, V, P, A, null), A.onAfterShadow(r, A, y, C, V, P, null)
+                let L = x(R, K, I, v);
+                R.onBeforeShadow(r, R, b, P, W, L, null), r.renderBufferDirect(P, null, W, L, R, null), R.onAfterShadow(r, R, b, P, W, L, null)
             }
         }
-        let T = A.children;
-        for (let V = 0, K = T.length; V < K; V++) R(T[V], y, C, Z, v)
+        let w = R.children;
+        for (let W = 0, K = w.length; W < K; W++) A(w[W], b, P, I, v)
     }
 
-    function U(A) {
-        A.target.removeEventListener("dispose", U);
-        for (let y in c) {
-            let C = c[y],
-                Z = A.target.uuid;
-            Z in C && (C[Z].dispose(), delete C[Z])
+    function D(R) {
+        R.target.removeEventListener("dispose", D);
+        for (let b in c) {
+            let P = c[b],
+                I = R.target.uuid;
+            I in P && (P[I].dispose(), delete P[I])
         }
     }
 }
 
 function of(r, e, t) {
     let i = t.isWebGL2;
 
     function n() {
-        let L = !1,
+        let C = !1,
             re = new ct,
-            O = null,
+            F = null,
             le = new ct(0, 0, 0, 0);
         return {
             setMask: function(se) {
-                O !== se && !L && (r.colorMask(se, se, se, se), O = se)
+                F !== se && !C && (r.colorMask(se, se, se, se), F = se)
             },
             setLocked: function(se) {
-                L = se
+                C = se
             },
-            setClear: function(se, Ge, Ve, Ke, $e) {
-                $e === !0 && (se *= Ke, Ge *= Ke, Ve *= Ke), re.set(se, Ge, Ve, Ke), le.equals(re) === !1 && (r.clearColor(se, Ge, Ve, Ke), le.copy(re))
+            setClear: function(se, He, Ve, Ke, Qe) {
+                Qe === !0 && (se *= Ke, He *= Ke, Ve *= Ke), re.set(se, He, Ve, Ke), le.equals(re) === !1 && (r.clearColor(se, He, Ve, Ke), le.copy(re))
             },
             reset: function() {
-                L = !1, O = null, le.set(-1, 0, 0, 0)
+                C = !1, F = null, le.set(-1, 0, 0, 0)
             }
         }
     }
 
     function a() {
-        let L = !1,
+        let C = !1,
             re = null,
-            O = null,
+            F = null,
             le = null;
         return {
             setTest: function(se) {
-                se ? me(r.DEPTH_TEST) : Xe(r.DEPTH_TEST)
+                se ? fe(r.DEPTH_TEST) : Xe(r.DEPTH_TEST)
             },
             setMask: function(se) {
-                re !== se && !L && (r.depthMask(se), re = se)
+                re !== se && !C && (r.depthMask(se), re = se)
             },
             setFunc: function(se) {
-                if (O !== se) {
+                if (F !== se) {
                     switch (se) {
-                        case El:
+                        case yl:
                             r.depthFunc(r.NEVER);
                             break;
-                        case Sl:
+                        case El:
                             r.depthFunc(r.ALWAYS);
                             break;
-                        case yl:
+                        case Sl:
                             r.depthFunc(r.LESS);
                             break;
                         case en:
                             r.depthFunc(r.LEQUAL);
                             break;
-                        case bl:
+                        case Tl:
                             r.depthFunc(r.EQUAL);
                             break;
-                        case Tl:
+                        case bl:
                             r.depthFunc(r.GEQUAL);
                             break;
                         case wl:
                             r.depthFunc(r.GREATER);
                             break;
                         case Al:
                             r.depthFunc(r.NOTEQUAL);
                             break;
                         default:
                             r.depthFunc(r.LEQUAL)
                     }
-                    O = se
+                    F = se
                 }
             },
             setLocked: function(se) {
-                L = se
+                C = se
             },
             setClear: function(se) {
                 le !== se && (r.clearDepth(se), le = se)
             },
             reset: function() {
-                L = !1, re = null, O = null, le = null
+                C = !1, re = null, F = null, le = null
             }
         }
     }
 
     function o() {
-        let L = !1,
+        let C = !1,
             re = null,
-            O = null,
+            F = null,
             le = null,
             se = null,
-            Ge = null,
+            He = null,
             Ve = null,
             Ke = null,
-            $e = null;
+            Qe = null;
         return {
             setTest: function(je) {
-                L || (je ? me(r.STENCIL_TEST) : Xe(r.STENCIL_TEST))
+                C || (je ? fe(r.STENCIL_TEST) : Xe(r.STENCIL_TEST))
             },
             setMask: function(je) {
-                re !== je && !L && (r.stencilMask(je), re = je)
+                re !== je && !C && (r.stencilMask(je), re = je)
             },
-            setFunc: function(je, tt, yt) {
-                (O !== je || le !== tt || se !== yt) && (r.stencilFunc(je, tt, yt), O = je, le = tt, se = yt)
+            setFunc: function(je, tt, St) {
+                (F !== je || le !== tt || se !== St) && (r.stencilFunc(je, tt, St), F = je, le = tt, se = St)
             },
-            setOp: function(je, tt, yt) {
-                (Ge !== je || Ve !== tt || Ke !== yt) && (r.stencilOp(je, tt, yt), Ge = je, Ve = tt, Ke = yt)
+            setOp: function(je, tt, St) {
+                (He !== je || Ve !== tt || Ke !== St) && (r.stencilOp(je, tt, St), He = je, Ve = tt, Ke = St)
             },
             setLocked: function(je) {
-                L = je
+                C = je
             },
             setClear: function(je) {
-                $e !== je && (r.clearStencil(je), $e = je)
+                Qe !== je && (r.clearStencil(je), Qe = je)
             },
             reset: function() {
-                L = !1, re = null, O = null, le = null, se = null, Ge = null, Ve = null, Ke = null, $e = null
+                C = !1, re = null, F = null, le = null, se = null, He = null, Ve = null, Ke = null, Qe = null
             }
         }
     }
     let s = new n,
         l = new a,
         c = new o,
-        u = new WeakMap,
+        h = new WeakMap,
         p = new WeakMap,
         f = {},
         m = {},
         _ = new WeakMap,
         M = [],
         d = null,
-        h = !1,
-        w = null,
+        u = !1,
+        T = null,
         x = null,
-        R = null,
-        U = null,
         A = null,
-        y = null,
-        C = null,
-        Z = new Ye(0, 0, 0),
+        D = null,
+        R = null,
+        b = null,
+        P = null,
+        I = new Ye(0, 0, 0),
         v = 0,
-        T = !1,
-        V = null,
+        w = !1,
+        W = null,
         K = null,
-        P = null,
-        X = null,
+        L = null,
+        j = null,
         k = null,
-        j = r.getParameter(r.MAX_COMBINED_TEXTURE_IMAGE_UNITS),
+        Y = r.getParameter(r.MAX_COMBINED_TEXTURE_IMAGE_UNITS),
         q = !1,
-        W = 0,
-        te = r.getParameter(r.VERSION);
-    te.indexOf("WebGL") !== -1 ? (W = parseFloat(/^WebGL (\d)/.exec(te)[1]), q = W >= 1) : te.indexOf("OpenGL ES") !== -1 && (W = parseFloat(/^OpenGL ES (\d)/.exec(te)[1]), q = W >= 2);
-    let ee = null,
-        pe = {},
-        xe = r.getParameter(r.SCISSOR_BOX),
-        H = r.getParameter(r.VIEWPORT),
-        ie = new ct().fromArray(xe),
-        fe = new ct().fromArray(H);
+        Z = 0,
+        ee = r.getParameter(r.VERSION);
+    ee.indexOf("WebGL") !== -1 ? (Z = parseFloat(/^WebGL (\d)/.exec(ee)[1]), q = Z >= 1) : ee.indexOf("OpenGL ES") !== -1 && (Z = parseFloat(/^OpenGL ES (\d)/.exec(ee)[1]), q = Z >= 2);
+    let ie = null,
+        de = {},
+        ge = r.getParameter(r.SCISSOR_BOX),
+        V = r.getParameter(r.VIEWPORT),
+        te = new ct().fromArray(ge),
+        pe = new ct().fromArray(V);
 
-    function Te(L, re, O, le) {
+    function we(C, re, F, le) {
         let se = new Uint8Array(4),
-            Ge = r.createTexture();
-        r.bindTexture(L, Ge), r.texParameteri(L, r.TEXTURE_MIN_FILTER, r.NEAREST), r.texParameteri(L, r.TEXTURE_MAG_FILTER, r.NEAREST);
-        for (let Ve = 0; Ve < O; Ve++) i && (L === r.TEXTURE_3D || L === r.TEXTURE_2D_ARRAY) ? r.texImage3D(re, 0, r.RGBA, 1, 1, le, 0, r.RGBA, r.UNSIGNED_BYTE, se) : r.texImage2D(re + Ve, 0, r.RGBA, 1, 1, 0, r.RGBA, r.UNSIGNED_BYTE, se);
-        return Ge
+            He = r.createTexture();
+        r.bindTexture(C, He), r.texParameteri(C, r.TEXTURE_MIN_FILTER, r.NEAREST), r.texParameteri(C, r.TEXTURE_MAG_FILTER, r.NEAREST);
+        for (let Ve = 0; Ve < F; Ve++) i && (C === r.TEXTURE_3D || C === r.TEXTURE_2D_ARRAY) ? r.texImage3D(re, 0, r.RGBA, 1, 1, le, 0, r.RGBA, r.UNSIGNED_BYTE, se) : r.texImage2D(re + Ve, 0, r.RGBA, 1, 1, 0, r.RGBA, r.UNSIGNED_BYTE, se);
+        return He
     }
     let _e = {};
-    _e[r.TEXTURE_2D] = Te(r.TEXTURE_2D, r.TEXTURE_2D, 1), _e[r.TEXTURE_CUBE_MAP] = Te(r.TEXTURE_CUBE_MAP, r.TEXTURE_CUBE_MAP_POSITIVE_X, 6), i && (_e[r.TEXTURE_2D_ARRAY] = Te(r.TEXTURE_2D_ARRAY, r.TEXTURE_2D_ARRAY, 1, 1), _e[r.TEXTURE_3D] = Te(r.TEXTURE_3D, r.TEXTURE_3D, 1, 1)), s.setClear(0, 0, 0, 1), l.setClear(1), c.setClear(0), me(r.DEPTH_TEST), l.setFunc(en), be(!1), de(Qa), me(r.CULL_FACE), Me(ci);
+    _e[r.TEXTURE_2D] = we(r.TEXTURE_2D, r.TEXTURE_2D, 1), _e[r.TEXTURE_CUBE_MAP] = we(r.TEXTURE_CUBE_MAP, r.TEXTURE_CUBE_MAP_POSITIVE_X, 6), i && (_e[r.TEXTURE_2D_ARRAY] = we(r.TEXTURE_2D_ARRAY, r.TEXTURE_2D_ARRAY, 1, 1), _e[r.TEXTURE_3D] = we(r.TEXTURE_3D, r.TEXTURE_3D, 1, 1)), s.setClear(0, 0, 0, 1), l.setClear(1), c.setClear(0), fe(r.DEPTH_TEST), l.setFunc(en), be(!1), Re(Qa), fe(r.CULL_FACE), Se(ci);
 
-    function me(L) {
-        f[L] !== !0 && (r.enable(L), f[L] = !0)
+    function fe(C) {
+        f[C] !== !0 && (r.enable(C), f[C] = !0)
     }
 
-    function Xe(L) {
-        f[L] !== !1 && (r.disable(L), f[L] = !1)
+    function Xe(C) {
+        f[C] !== !1 && (r.disable(C), f[C] = !1)
     }
 
-    function we(L, re) {
-        return m[L] !== re ? (r.bindFramebuffer(L, re), m[L] = re, i && (L === r.DRAW_FRAMEBUFFER && (m[r.FRAMEBUFFER] = re), L === r.FRAMEBUFFER && (m[r.DRAW_FRAMEBUFFER] = re)), !0) : !1
+    function Ae(C, re) {
+        return m[C] !== re ? (r.bindFramebuffer(C, re), m[C] = re, i && (C === r.DRAW_FRAMEBUFFER && (m[r.FRAMEBUFFER] = re), C === r.FRAMEBUFFER && (m[r.DRAW_FRAMEBUFFER] = re)), !0) : !1
     }
 
-    function I(L, re) {
-        let O = M,
+    function O(C, re) {
+        let F = M,
             le = !1;
-        if (L) {
-            O = _.get(re), O === void 0 && (O = [], _.set(re, O));
-            let se = L.textures;
-            if (O.length !== se.length || O[0] !== r.COLOR_ATTACHMENT0) {
-                for (let Ge = 0, Ve = se.length; Ge < Ve; Ge++) O[Ge] = r.COLOR_ATTACHMENT0 + Ge;
-                O.length = se.length, le = !0
+        if (C) {
+            F = _.get(re), F === void 0 && (F = [], _.set(re, F));
+            let se = C.textures;
+            if (F.length !== se.length || F[0] !== r.COLOR_ATTACHMENT0) {
+                for (let He = 0, Ve = se.length; He < Ve; He++) F[He] = r.COLOR_ATTACHMENT0 + He;
+                F.length = se.length, le = !0
             }
-        } else O[0] !== r.BACK && (O[0] = r.BACK, le = !0);
+        } else F[0] !== r.BACK && (F[0] = r.BACK, le = !0);
         if (le)
-            if (t.isWebGL2) r.drawBuffers(O);
-            else if (e.has("WEBGL_draw_buffers") === !0) e.get("WEBGL_draw_buffers").drawBuffersWEBGL(O);
+            if (t.isWebGL2) r.drawBuffers(F);
+            else if (e.has("WEBGL_draw_buffers") === !0) e.get("WEBGL_draw_buffers").drawBuffersWEBGL(F);
         else throw new Error("THREE.WebGLState: Usage of gl.drawBuffers() require WebGL2 or WEBGL_draw_buffers extension")
     }
 
-    function Qe(L) {
-        return d !== L ? (r.useProgram(L), d = L, !0) : !1
+    function Je(C) {
+        return d !== C ? (r.useProgram(C), d = C, !0) : !1
     }
     let ve = {
-        [bi]: r.FUNC_ADD,
+        [Ti]: r.FUNC_ADD,
         [sl]: r.FUNC_SUBTRACT,
         [ol]: r.FUNC_REVERSE_SUBTRACT
     };
     if (i) ve[rs] = r.MIN, ve[ns] = r.MAX;
     else {
-        let L = e.get("EXT_blend_minmax");
-        L !== null && (ve[rs] = L.MIN_EXT, ve[ns] = L.MAX_EXT)
+        let C = e.get("EXT_blend_minmax");
+        C !== null && (ve[rs] = C.MIN_EXT, ve[ns] = C.MAX_EXT)
     }
-    let Ue = {
+    let Pe = {
         [ll]: r.ZERO,
         [cl]: r.ONE,
         [hl]: r.SRC_COLOR,
         [da]: r.SRC_ALPHA,
         [gl]: r.SRC_ALPHA_SATURATE,
         [fl]: r.DST_COLOR,
         [dl]: r.DST_ALPHA,
@@ -12626,887 +12626,887 @@
         [pl]: r.ONE_MINUS_DST_ALPHA,
         [_l]: r.CONSTANT_COLOR,
         [vl]: r.ONE_MINUS_CONSTANT_COLOR,
         [xl]: r.CONSTANT_ALPHA,
         [Ml]: r.ONE_MINUS_CONSTANT_ALPHA
     };
 
-    function Me(L, re, O, le, se, Ge, Ve, Ke, $e, je) {
-        if (L === ci) {
-            h === !0 && (Xe(r.BLEND), h = !1);
+    function Se(C, re, F, le, se, He, Ve, Ke, Qe, je) {
+        if (C === ci) {
+            u === !0 && (Xe(r.BLEND), u = !1);
             return
         }
-        if (h === !1 && (me(r.BLEND), h = !0), L !== al) {
-            if (L !== w || je !== T) {
-                if ((x !== bi || A !== bi) && (r.blendEquation(r.FUNC_ADD), x = bi, A = bi), je) switch (L) {
+        if (u === !1 && (fe(r.BLEND), u = !0), C !== al) {
+            if (C !== T || je !== w) {
+                if ((x !== Ti || R !== Ti) && (r.blendEquation(r.FUNC_ADD), x = Ti, R = Ti), je) switch (C) {
                     case er:
                         r.blendFuncSeparate(r.ONE, r.ONE_MINUS_SRC_ALPHA, r.ONE, r.ONE_MINUS_SRC_ALPHA);
                         break;
                     case es:
                         r.blendFunc(r.ONE, r.ONE);
                         break;
                     case ts:
                         r.blendFuncSeparate(r.ZERO, r.ONE_MINUS_SRC_COLOR, r.ZERO, r.ONE);
                         break;
                     case is:
                         r.blendFuncSeparate(r.ZERO, r.SRC_COLOR, r.ZERO, r.SRC_ALPHA);
                         break;
                     default:
-                        console.error("THREE.WebGLState: Invalid blending: ", L);
+                        console.error("THREE.WebGLState: Invalid blending: ", C);
                         break
-                } else switch (L) {
+                } else switch (C) {
                     case er:
                         r.blendFuncSeparate(r.SRC_ALPHA, r.ONE_MINUS_SRC_ALPHA, r.ONE, r.ONE_MINUS_SRC_ALPHA);
                         break;
                     case es:
                         r.blendFunc(r.SRC_ALPHA, r.ONE);
                         break;
                     case ts:
                         r.blendFuncSeparate(r.ZERO, r.ONE_MINUS_SRC_COLOR, r.ZERO, r.ONE);
                         break;
                     case is:
                         r.blendFunc(r.ZERO, r.SRC_COLOR);
                         break;
                     default:
-                        console.error("THREE.WebGLState: Invalid blending: ", L);
+                        console.error("THREE.WebGLState: Invalid blending: ", C);
                         break
                 }
-                R = null, U = null, y = null, C = null, Z.set(0, 0, 0), v = 0, w = L, T = je
+                A = null, D = null, b = null, P = null, I.set(0, 0, 0), v = 0, T = C, w = je
             }
             return
         }
-        se = se || re, Ge = Ge || O, Ve = Ve || le, (re !== x || se !== A) && (r.blendEquationSeparate(ve[re], ve[se]), x = re, A = se), (O !== R || le !== U || Ge !== y || Ve !== C) && (r.blendFuncSeparate(Ue[O], Ue[le], Ue[Ge], Ue[Ve]), R = O, U = le, y = Ge, C = Ve), (Ke.equals(Z) === !1 || $e !== v) && (r.blendColor(Ke.r, Ke.g, Ke.b, $e), Z.copy(Ke), v = $e), w = L, T = !1
+        se = se || re, He = He || F, Ve = Ve || le, (re !== x || se !== R) && (r.blendEquationSeparate(ve[re], ve[se]), x = re, R = se), (F !== A || le !== D || He !== b || Ve !== P) && (r.blendFuncSeparate(Pe[F], Pe[le], Pe[He], Pe[Ve]), A = F, D = le, b = He, P = Ve), (Ke.equals(I) === !1 || Qe !== v) && (r.blendColor(Ke.r, Ke.g, Ke.b, Qe), I.copy(Ke), v = Qe), T = C, w = !1
     }
 
-    function Le(L, re) {
-        L.side === qt ? Xe(r.CULL_FACE) : me(r.CULL_FACE);
-        let O = L.side === Et;
-        re && (O = !O), be(O), L.blending === er && L.transparent === !1 ? Me(ci) : Me(L.blending, L.blendEquation, L.blendSrc, L.blendDst, L.blendEquationAlpha, L.blendSrcAlpha, L.blendDstAlpha, L.blendColor, L.blendAlpha, L.premultipliedAlpha), l.setFunc(L.depthFunc), l.setTest(L.depthTest), l.setMask(L.depthWrite), s.setMask(L.colorWrite);
-        let le = L.stencilWrite;
-        c.setTest(le), le && (c.setMask(L.stencilWriteMask), c.setFunc(L.stencilFunc, L.stencilRef, L.stencilFuncMask), c.setOp(L.stencilFail, L.stencilZFail, L.stencilZPass)), S(L.polygonOffset, L.polygonOffsetFactor, L.polygonOffsetUnits), L.alphaToCoverage === !0 ? me(r.SAMPLE_ALPHA_TO_COVERAGE) : Xe(r.SAMPLE_ALPHA_TO_COVERAGE)
+    function Ne(C, re) {
+        C.side === qt ? Xe(r.CULL_FACE) : fe(r.CULL_FACE);
+        let F = C.side === yt;
+        re && (F = !F), be(F), C.blending === er && C.transparent === !1 ? Se(ci) : Se(C.blending, C.blendEquation, C.blendSrc, C.blendDst, C.blendEquationAlpha, C.blendSrcAlpha, C.blendDstAlpha, C.blendColor, C.blendAlpha, C.premultipliedAlpha), l.setFunc(C.depthFunc), l.setTest(C.depthTest), l.setMask(C.depthWrite), s.setMask(C.colorWrite);
+        let le = C.stencilWrite;
+        c.setTest(le), le && (c.setMask(C.stencilWriteMask), c.setFunc(C.stencilFunc, C.stencilRef, C.stencilFuncMask), c.setOp(C.stencilFail, C.stencilZFail, C.stencilZPass)), E(C.polygonOffset, C.polygonOffsetFactor, C.polygonOffsetUnits), C.alphaToCoverage === !0 ? fe(r.SAMPLE_ALPHA_TO_COVERAGE) : Xe(r.SAMPLE_ALPHA_TO_COVERAGE)
     }
 
-    function be(L) {
-        V !== L && (L ? r.frontFace(r.CW) : r.frontFace(r.CCW), V = L)
+    function be(C) {
+        W !== C && (C ? r.frontFace(r.CW) : r.frontFace(r.CCW), W = C)
     }
 
-    function de(L) {
-        L !== il ? (me(r.CULL_FACE), L !== K && (L === Qa ? r.cullFace(r.BACK) : L === rl ? r.cullFace(r.FRONT) : r.cullFace(r.FRONT_AND_BACK))) : Xe(r.CULL_FACE), K = L
+    function Re(C) {
+        C !== il ? (fe(r.CULL_FACE), C !== K && (C === Qa ? r.cullFace(r.BACK) : C === rl ? r.cullFace(r.FRONT) : r.cullFace(r.FRONT_AND_BACK))) : Xe(r.CULL_FACE), K = C
     }
 
-    function Ne(L) {
-        L !== P && (q && r.lineWidth(L), P = L)
+    function xe(C) {
+        C !== L && (q && r.lineWidth(C), L = C)
     }
 
-    function S(L, re, O) {
-        L ? (me(r.POLYGON_OFFSET_FILL), (X !== re || k !== O) && (r.polygonOffset(re, O), X = re, k = O)) : Xe(r.POLYGON_OFFSET_FILL)
+    function E(C, re, F) {
+        C ? (fe(r.POLYGON_OFFSET_FILL), (j !== re || k !== F) && (r.polygonOffset(re, F), j = re, k = F)) : Xe(r.POLYGON_OFFSET_FILL)
     }
 
-    function g(L) {
-        L ? me(r.SCISSOR_TEST) : Xe(r.SCISSOR_TEST)
+    function g(C) {
+        C ? fe(r.SCISSOR_TEST) : Xe(r.SCISSOR_TEST)
     }
 
-    function B(L) {
-        L === void 0 && (L = r.TEXTURE0 + j - 1), ee !== L && (r.activeTexture(L), ee = L)
+    function B(C) {
+        C === void 0 && (C = r.TEXTURE0 + Y - 1), ie !== C && (r.activeTexture(C), ie = C)
     }
 
-    function Y(L, re, O) {
-        O === void 0 && (ee === null ? O = r.TEXTURE0 + j - 1 : O = ee);
-        let le = pe[O];
+    function X(C, re, F) {
+        F === void 0 && (ie === null ? F = r.TEXTURE0 + Y - 1 : F = ie);
+        let le = de[F];
         le === void 0 && (le = {
             type: void 0,
             texture: void 0
-        }, pe[O] = le), (le.type !== L || le.texture !== re) && (ee !== O && (r.activeTexture(O), ee = O), r.bindTexture(L, re || _e[L]), le.type = L, le.texture = re)
+        }, de[F] = le), (le.type !== C || le.texture !== re) && (ie !== F && (r.activeTexture(F), ie = F), r.bindTexture(C, re || _e[C]), le.type = C, le.texture = re)
     }
 
     function Q() {
-        let L = pe[ee];
-        L !== void 0 && L.type !== void 0 && (r.bindTexture(L.type, null), L.type = void 0, L.texture = void 0)
+        let C = de[ie];
+        C !== void 0 && C.type !== void 0 && (r.bindTexture(C.type, null), C.type = void 0, C.texture = void 0)
     }
 
     function J() {
         try {
             r.compressedTexImage2D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
-    function Ce() {
+    function Ee() {
         try {
             r.compressedTexImage3D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
-    function ye() {
+    function Me() {
         try {
             r.texSubImage2D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
     function ae() {
         try {
             r.texSubImage3D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
     function he() {
         try {
             r.compressedTexSubImage2D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
     function Ie() {
         try {
             r.compressedTexSubImage3D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
     function ne() {
         try {
             r.texStorage2D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
-    function Je() {
+    function $e() {
         try {
             r.texStorage3D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
-    function ze() {
+    function Be() {
         try {
             r.texImage2D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
-    function Ee() {
+    function ye() {
         try {
             r.texImage3D.apply(r, arguments)
-        } catch (L) {
-            console.error("THREE.WebGLState:", L)
+        } catch (C) {
+            console.error("THREE.WebGLState:", C)
         }
     }
 
-    function ge(L) {
-        ie.equals(L) === !1 && (r.scissor(L.x, L.y, L.z, L.w), ie.copy(L))
+    function me(C) {
+        te.equals(C) === !1 && (r.scissor(C.x, C.y, C.z, C.w), te.copy(C))
     }
 
-    function b(L) {
-        fe.equals(L) === !1 && (r.viewport(L.x, L.y, L.z, L.w), fe.copy(L))
+    function S(C) {
+        pe.equals(C) === !1 && (r.viewport(C.x, C.y, C.z, C.w), pe.copy(C))
     }
 
-    function $(L, re) {
-        let O = p.get(re);
-        O === void 0 && (O = new WeakMap, p.set(re, O));
-        let le = O.get(L);
-        le === void 0 && (le = r.getUniformBlockIndex(re, L.name), O.set(L, le))
+    function $(C, re) {
+        let F = p.get(re);
+        F === void 0 && (F = new WeakMap, p.set(re, F));
+        let le = F.get(C);
+        le === void 0 && (le = r.getUniformBlockIndex(re, C.name), F.set(C, le))
     }
 
-    function oe(L, re) {
-        let O = p.get(re).get(L);
-        u.get(re) !== O && (r.uniformBlockBinding(re, O, L.__bindingPointIndex), u.set(re, O))
+    function oe(C, re) {
+        let F = p.get(re).get(C);
+        h.get(re) !== F && (r.uniformBlockBinding(re, F, C.__bindingPointIndex), h.set(re, F))
     }
 
-    function Ae() {
-        r.disable(r.BLEND), r.disable(r.CULL_FACE), r.disable(r.DEPTH_TEST), r.disable(r.POLYGON_OFFSET_FILL), r.disable(r.SCISSOR_TEST), r.disable(r.STENCIL_TEST), r.disable(r.SAMPLE_ALPHA_TO_COVERAGE), r.blendEquation(r.FUNC_ADD), r.blendFunc(r.ONE, r.ZERO), r.blendFuncSeparate(r.ONE, r.ZERO, r.ONE, r.ZERO), r.blendColor(0, 0, 0, 0), r.colorMask(!0, !0, !0, !0), r.clearColor(0, 0, 0, 0), r.depthMask(!0), r.depthFunc(r.LESS), r.clearDepth(1), r.stencilMask(4294967295), r.stencilFunc(r.ALWAYS, 0, 4294967295), r.stencilOp(r.KEEP, r.KEEP, r.KEEP), r.clearStencil(0), r.cullFace(r.BACK), r.frontFace(r.CCW), r.polygonOffset(0, 0), r.activeTexture(r.TEXTURE0), r.bindFramebuffer(r.FRAMEBUFFER, null), i === !0 && (r.bindFramebuffer(r.DRAW_FRAMEBUFFER, null), r.bindFramebuffer(r.READ_FRAMEBUFFER, null)), r.useProgram(null), r.lineWidth(1), r.scissor(0, 0, r.canvas.width, r.canvas.height), r.viewport(0, 0, r.canvas.width, r.canvas.height), f = {}, ee = null, pe = {}, m = {}, _ = new WeakMap, M = [], d = null, h = !1, w = null, x = null, R = null, U = null, A = null, y = null, C = null, Z = new Ye(0, 0, 0), v = 0, T = !1, V = null, K = null, P = null, X = null, k = null, ie.set(0, 0, r.canvas.width, r.canvas.height), fe.set(0, 0, r.canvas.width, r.canvas.height), s.reset(), l.reset(), c.reset()
+    function Ce() {
+        r.disable(r.BLEND), r.disable(r.CULL_FACE), r.disable(r.DEPTH_TEST), r.disable(r.POLYGON_OFFSET_FILL), r.disable(r.SCISSOR_TEST), r.disable(r.STENCIL_TEST), r.disable(r.SAMPLE_ALPHA_TO_COVERAGE), r.blendEquation(r.FUNC_ADD), r.blendFunc(r.ONE, r.ZERO), r.blendFuncSeparate(r.ONE, r.ZERO, r.ONE, r.ZERO), r.blendColor(0, 0, 0, 0), r.colorMask(!0, !0, !0, !0), r.clearColor(0, 0, 0, 0), r.depthMask(!0), r.depthFunc(r.LESS), r.clearDepth(1), r.stencilMask(4294967295), r.stencilFunc(r.ALWAYS, 0, 4294967295), r.stencilOp(r.KEEP, r.KEEP, r.KEEP), r.clearStencil(0), r.cullFace(r.BACK), r.frontFace(r.CCW), r.polygonOffset(0, 0), r.activeTexture(r.TEXTURE0), r.bindFramebuffer(r.FRAMEBUFFER, null), i === !0 && (r.bindFramebuffer(r.DRAW_FRAMEBUFFER, null), r.bindFramebuffer(r.READ_FRAMEBUFFER, null)), r.useProgram(null), r.lineWidth(1), r.scissor(0, 0, r.canvas.width, r.canvas.height), r.viewport(0, 0, r.canvas.width, r.canvas.height), f = {}, ie = null, de = {}, m = {}, _ = new WeakMap, M = [], d = null, u = !1, T = null, x = null, A = null, D = null, R = null, b = null, P = null, I = new Ye(0, 0, 0), v = 0, w = !1, W = null, K = null, L = null, j = null, k = null, te.set(0, 0, r.canvas.width, r.canvas.height), pe.set(0, 0, r.canvas.width, r.canvas.height), s.reset(), l.reset(), c.reset()
     }
     return {
         buffers: {
             color: s,
             depth: l,
             stencil: c
         },
-        enable: me,
+        enable: fe,
         disable: Xe,
-        bindFramebuffer: we,
-        drawBuffers: I,
-        useProgram: Qe,
-        setBlending: Me,
-        setMaterial: Le,
+        bindFramebuffer: Ae,
+        drawBuffers: O,
+        useProgram: Je,
+        setBlending: Se,
+        setMaterial: Ne,
         setFlipSided: be,
-        setCullFace: de,
-        setLineWidth: Ne,
-        setPolygonOffset: S,
+        setCullFace: Re,
+        setLineWidth: xe,
+        setPolygonOffset: E,
         setScissorTest: g,
         activeTexture: B,
-        bindTexture: Y,
+        bindTexture: X,
         unbindTexture: Q,
         compressedTexImage2D: J,
-        compressedTexImage3D: Ce,
-        texImage2D: ze,
-        texImage3D: Ee,
+        compressedTexImage3D: Ee,
+        texImage2D: Be,
+        texImage3D: ye,
         updateUBOMapping: $,
         uniformBlockBinding: oe,
         texStorage2D: ne,
-        texStorage3D: Je,
-        texSubImage2D: ye,
+        texStorage3D: $e,
+        texSubImage2D: Me,
         texSubImage3D: ae,
         compressedTexSubImage2D: he,
         compressedTexSubImage3D: Ie,
-        scissor: ge,
-        viewport: b,
-        reset: Ae
+        scissor: me,
+        viewport: S,
+        reset: Ce
     }
 }
 
 function lf(r, e, t, i, n, a, o) {
     let s = n.isWebGL2,
         l = e.has("WEBGL_multisampled_render_to_texture") ? e.get("WEBGL_multisampled_render_to_texture") : null,
         c = typeof navigator > "u" ? !1 : /OculusBrowser/g.test(navigator.userAgent),
-        u = new De,
+        h = new Ue,
         p = new WeakMap,
         f, m = new WeakMap,
         _ = !1;
     try {
         _ = typeof OffscreenCanvas < "u" && new OffscreenCanvas(1, 1).getContext("2d") !== null
     } catch {}
 
-    function M(S, g) {
-        return _ ? new OffscreenCanvas(S, g) : on("canvas")
+    function M(E, g) {
+        return _ ? new OffscreenCanvas(E, g) : on("canvas")
     }
 
-    function d(S, g, B, Y) {
+    function d(E, g, B, X) {
         let Q = 1,
-            J = Ne(S);
-        if ((J.width > Y || J.height > Y) && (Q = Y / Math.max(J.width, J.height)), Q < 1 || g === !0)
-            if (typeof HTMLImageElement < "u" && S instanceof HTMLImageElement || typeof HTMLCanvasElement < "u" && S instanceof HTMLCanvasElement || typeof ImageBitmap < "u" && S instanceof ImageBitmap || typeof VideoFrame < "u" && S instanceof VideoFrame) {
-                let Ce = g ? sn : Math.floor,
-                    ye = Ce(Q * J.width),
-                    ae = Ce(Q * J.height);
-                f === void 0 && (f = M(ye, ae));
-                let he = B ? M(ye, ae) : f;
-                return he.width = ye, he.height = ae, he.getContext("2d").drawImage(S, 0, 0, ye, ae), console.warn("THREE.WebGLRenderer: Texture has been resized from (" + J.width + "x" + J.height + ") to (" + ye + "x" + ae + ")."), he
-            } else return "data" in S && console.warn("THREE.WebGLRenderer: Image in DataTexture is too big (" + J.width + "x" + J.height + ")."), S;
-        return S
+            J = xe(E);
+        if ((J.width > X || J.height > X) && (Q = X / Math.max(J.width, J.height)), Q < 1 || g === !0)
+            if (typeof HTMLImageElement < "u" && E instanceof HTMLImageElement || typeof HTMLCanvasElement < "u" && E instanceof HTMLCanvasElement || typeof ImageBitmap < "u" && E instanceof ImageBitmap || typeof VideoFrame < "u" && E instanceof VideoFrame) {
+                let Ee = g ? sn : Math.floor,
+                    Me = Ee(Q * J.width),
+                    ae = Ee(Q * J.height);
+                f === void 0 && (f = M(Me, ae));
+                let he = B ? M(Me, ae) : f;
+                return he.width = Me, he.height = ae, he.getContext("2d").drawImage(E, 0, 0, Me, ae), console.warn("THREE.WebGLRenderer: Texture has been resized from (" + J.width + "x" + J.height + ") to (" + Me + "x" + ae + ")."), he
+            } else return "data" in E && console.warn("THREE.WebGLRenderer: Image in DataTexture is too big (" + J.width + "x" + J.height + ")."), E;
+        return E
     }
 
-    function h(S) {
-        let g = Ne(S);
+    function u(E) {
+        let g = xe(E);
         return xa(g.width) && xa(g.height)
     }
 
-    function w(S) {
-        return s ? !1 : S.wrapS !== It || S.wrapT !== It || S.minFilter !== _t && S.minFilter !== xt
+    function T(E) {
+        return s ? !1 : E.wrapS !== Nt || E.wrapT !== Nt || E.minFilter !== _t && E.minFilter !== xt
     }
 
-    function x(S, g) {
-        return S.generateMipmaps && g && S.minFilter !== _t && S.minFilter !== xt
+    function x(E, g) {
+        return E.generateMipmaps && g && E.minFilter !== _t && E.minFilter !== xt
     }
 
-    function R(S) {
-        r.generateMipmap(S)
+    function A(E) {
+        r.generateMipmap(E)
     }
 
-    function U(S, g, B, Y, Q = !1) {
+    function D(E, g, B, X, Q = !1) {
         if (s === !1) return g;
-        if (S !== null) {
-            if (r[S] !== void 0) return r[S];
-            console.warn("THREE.WebGLRenderer: Attempt to use non-existing WebGL internal format '" + S + "'")
+        if (E !== null) {
+            if (r[E] !== void 0) return r[E];
+            console.warn("THREE.WebGLRenderer: Attempt to use non-existing WebGL internal format '" + E + "'")
         }
         let J = g;
         if (g === r.RED && (B === r.FLOAT && (J = r.R32F), B === r.HALF_FLOAT && (J = r.R16F), B === r.UNSIGNED_BYTE && (J = r.R8)), g === r.RED_INTEGER && (B === r.UNSIGNED_BYTE && (J = r.R8UI), B === r.UNSIGNED_SHORT && (J = r.R16UI), B === r.UNSIGNED_INT && (J = r.R32UI), B === r.BYTE && (J = r.R8I), B === r.SHORT && (J = r.R16I), B === r.INT && (J = r.R32I)), g === r.RG && (B === r.FLOAT && (J = r.RG32F), B === r.HALF_FLOAT && (J = r.RG16F), B === r.UNSIGNED_BYTE && (J = r.RG8)), g === r.RG_INTEGER && (B === r.UNSIGNED_BYTE && (J = r.RG8UI), B === r.UNSIGNED_SHORT && (J = r.RG16UI), B === r.UNSIGNED_INT && (J = r.RG32UI), B === r.BYTE && (J = r.RG8I), B === r.SHORT && (J = r.RG16I), B === r.INT && (J = r.RG32I)), g === r.RGBA) {
-            let Ce = Q ? tn : qe.getTransfer(Y);
-            B === r.FLOAT && (J = r.RGBA32F), B === r.HALF_FLOAT && (J = r.RGBA16F), B === r.UNSIGNED_BYTE && (J = Ce === Ze ? r.SRGB8_ALPHA8 : r.RGBA8), B === r.UNSIGNED_SHORT_4_4_4_4 && (J = r.RGBA4), B === r.UNSIGNED_SHORT_5_5_5_1 && (J = r.RGB5_A1)
+            let Ee = Q ? tn : qe.getTransfer(X);
+            B === r.FLOAT && (J = r.RGBA32F), B === r.HALF_FLOAT && (J = r.RGBA16F), B === r.UNSIGNED_BYTE && (J = Ee === Ze ? r.SRGB8_ALPHA8 : r.RGBA8), B === r.UNSIGNED_SHORT_4_4_4_4 && (J = r.RGBA4), B === r.UNSIGNED_SHORT_5_5_5_1 && (J = r.RGB5_A1)
         }
         return (J === r.R16F || J === r.R32F || J === r.RG16F || J === r.RG32F || J === r.RGBA16F || J === r.RGBA32F) && e.get("EXT_color_buffer_float"), J
     }
 
-    function A(S, g, B) {
-        return x(S, B) === !0 || S.isFramebufferTexture && S.minFilter !== _t && S.minFilter !== xt ? Math.log2(Math.max(g.width, g.height)) + 1 : S.mipmaps !== void 0 && S.mipmaps.length > 0 ? S.mipmaps.length : S.isCompressedTexture && Array.isArray(S.image) ? g.mipmaps.length : 1
+    function R(E, g, B) {
+        return x(E, B) === !0 || E.isFramebufferTexture && E.minFilter !== _t && E.minFilter !== xt ? Math.log2(Math.max(g.width, g.height)) + 1 : E.mipmaps !== void 0 && E.mipmaps.length > 0 ? E.mipmaps.length : E.isCompressedTexture && Array.isArray(E.image) ? g.mipmaps.length : 1
     }
 
-    function y(S) {
-        return S === _t || S === as || S === pr ? r.NEAREST : r.LINEAR
+    function b(E) {
+        return E === _t || E === as || E === pr ? r.NEAREST : r.LINEAR
     }
 
-    function C(S) {
-        let g = S.target;
-        g.removeEventListener("dispose", C), v(g), g.isVideoTexture && p.delete(g)
+    function P(E) {
+        let g = E.target;
+        g.removeEventListener("dispose", P), v(g), g.isVideoTexture && p.delete(g)
     }
 
-    function Z(S) {
-        let g = S.target;
-        g.removeEventListener("dispose", Z), V(g)
+    function I(E) {
+        let g = E.target;
+        g.removeEventListener("dispose", I), W(g)
     }
 
-    function v(S) {
-        let g = i.get(S);
+    function v(E) {
+        let g = i.get(E);
         if (g.__webglInit === void 0) return;
-        let B = S.source,
-            Y = m.get(B);
-        if (Y) {
-            let Q = Y[g.__cacheKey];
-            Q.usedTimes--, Q.usedTimes === 0 && T(S), Object.keys(Y).length === 0 && m.delete(B)
+        let B = E.source,
+            X = m.get(B);
+        if (X) {
+            let Q = X[g.__cacheKey];
+            Q.usedTimes--, Q.usedTimes === 0 && w(E), Object.keys(X).length === 0 && m.delete(B)
         }
-        i.remove(S)
+        i.remove(E)
     }
 
-    function T(S) {
-        let g = i.get(S);
+    function w(E) {
+        let g = i.get(E);
         r.deleteTexture(g.__webglTexture);
-        let B = S.source,
-            Y = m.get(B);
-        delete Y[g.__cacheKey], o.memory.textures--
+        let B = E.source,
+            X = m.get(B);
+        delete X[g.__cacheKey], o.memory.textures--
     }
 
-    function V(S) {
-        let g = i.get(S);
-        if (S.depthTexture && S.depthTexture.dispose(), S.isWebGLCubeRenderTarget)
-            for (let Y = 0; Y < 6; Y++) {
-                if (Array.isArray(g.__webglFramebuffer[Y]))
-                    for (let Q = 0; Q < g.__webglFramebuffer[Y].length; Q++) r.deleteFramebuffer(g.__webglFramebuffer[Y][Q]);
-                else r.deleteFramebuffer(g.__webglFramebuffer[Y]);
-                g.__webglDepthbuffer && r.deleteRenderbuffer(g.__webglDepthbuffer[Y])
+    function W(E) {
+        let g = i.get(E);
+        if (E.depthTexture && E.depthTexture.dispose(), E.isWebGLCubeRenderTarget)
+            for (let X = 0; X < 6; X++) {
+                if (Array.isArray(g.__webglFramebuffer[X]))
+                    for (let Q = 0; Q < g.__webglFramebuffer[X].length; Q++) r.deleteFramebuffer(g.__webglFramebuffer[X][Q]);
+                else r.deleteFramebuffer(g.__webglFramebuffer[X]);
+                g.__webglDepthbuffer && r.deleteRenderbuffer(g.__webglDepthbuffer[X])
             } else {
                 if (Array.isArray(g.__webglFramebuffer))
-                    for (let Y = 0; Y < g.__webglFramebuffer.length; Y++) r.deleteFramebuffer(g.__webglFramebuffer[Y]);
+                    for (let X = 0; X < g.__webglFramebuffer.length; X++) r.deleteFramebuffer(g.__webglFramebuffer[X]);
                 else r.deleteFramebuffer(g.__webglFramebuffer);
                 if (g.__webglDepthbuffer && r.deleteRenderbuffer(g.__webglDepthbuffer), g.__webglMultisampledFramebuffer && r.deleteFramebuffer(g.__webglMultisampledFramebuffer), g.__webglColorRenderbuffer)
-                    for (let Y = 0; Y < g.__webglColorRenderbuffer.length; Y++) g.__webglColorRenderbuffer[Y] && r.deleteRenderbuffer(g.__webglColorRenderbuffer[Y]);
+                    for (let X = 0; X < g.__webglColorRenderbuffer.length; X++) g.__webglColorRenderbuffer[X] && r.deleteRenderbuffer(g.__webglColorRenderbuffer[X]);
                 g.__webglDepthRenderbuffer && r.deleteRenderbuffer(g.__webglDepthRenderbuffer)
             }
-        let B = S.textures;
-        for (let Y = 0, Q = B.length; Y < Q; Y++) {
-            let J = i.get(B[Y]);
-            J.__webglTexture && (r.deleteTexture(J.__webglTexture), o.memory.textures--), i.remove(B[Y])
+        let B = E.textures;
+        for (let X = 0, Q = B.length; X < Q; X++) {
+            let J = i.get(B[X]);
+            J.__webglTexture && (r.deleteTexture(J.__webglTexture), o.memory.textures--), i.remove(B[X])
         }
-        i.remove(S)
+        i.remove(E)
     }
     let K = 0;
 
-    function P() {
+    function L() {
         K = 0
     }
 
-    function X() {
-        let S = K;
-        return S >= n.maxTextures && console.warn("THREE.WebGLTextures: Trying to use " + S + " texture units while this GPU supports only " + n.maxTextures), K += 1, S
+    function j() {
+        let E = K;
+        return E >= n.maxTextures && console.warn("THREE.WebGLTextures: Trying to use " + E + " texture units while this GPU supports only " + n.maxTextures), K += 1, E
     }
 
-    function k(S) {
+    function k(E) {
         let g = [];
-        return g.push(S.wrapS), g.push(S.wrapT), g.push(S.wrapR || 0), g.push(S.magFilter), g.push(S.minFilter), g.push(S.anisotropy), g.push(S.internalFormat), g.push(S.format), g.push(S.type), g.push(S.generateMipmaps), g.push(S.premultiplyAlpha), g.push(S.flipY), g.push(S.unpackAlignment), g.push(S.colorSpace), g.join()
+        return g.push(E.wrapS), g.push(E.wrapT), g.push(E.wrapR || 0), g.push(E.magFilter), g.push(E.minFilter), g.push(E.anisotropy), g.push(E.internalFormat), g.push(E.format), g.push(E.type), g.push(E.generateMipmaps), g.push(E.premultiplyAlpha), g.push(E.flipY), g.push(E.unpackAlignment), g.push(E.colorSpace), g.join()
     }
 
-    function j(S, g) {
-        let B = i.get(S);
-        if (S.isVideoTexture && be(S), S.isRenderTargetTexture === !1 && S.version > 0 && B.__version !== S.version) {
-            let Y = S.image;
-            if (Y === null) console.warn("THREE.WebGLRenderer: Texture marked for update but no image data found.");
-            else if (Y.complete === !1) console.warn("THREE.WebGLRenderer: Texture marked for update but image is incomplete");
+    function Y(E, g) {
+        let B = i.get(E);
+        if (E.isVideoTexture && be(E), E.isRenderTargetTexture === !1 && E.version > 0 && B.__version !== E.version) {
+            let X = E.image;
+            if (X === null) console.warn("THREE.WebGLRenderer: Texture marked for update but no image data found.");
+            else if (X.complete === !1) console.warn("THREE.WebGLRenderer: Texture marked for update but image is incomplete");
             else {
-                fe(B, S, g);
+                pe(B, E, g);
                 return
             }
         }
         t.bindTexture(r.TEXTURE_2D, B.__webglTexture, r.TEXTURE0 + g)
     }
 
-    function q(S, g) {
-        let B = i.get(S);
-        if (S.version > 0 && B.__version !== S.version) {
-            fe(B, S, g);
+    function q(E, g) {
+        let B = i.get(E);
+        if (E.version > 0 && B.__version !== E.version) {
+            pe(B, E, g);
             return
         }
         t.bindTexture(r.TEXTURE_2D_ARRAY, B.__webglTexture, r.TEXTURE0 + g)
     }
 
-    function W(S, g) {
-        let B = i.get(S);
-        if (S.version > 0 && B.__version !== S.version) {
-            fe(B, S, g);
+    function Z(E, g) {
+        let B = i.get(E);
+        if (E.version > 0 && B.__version !== E.version) {
+            pe(B, E, g);
             return
         }
         t.bindTexture(r.TEXTURE_3D, B.__webglTexture, r.TEXTURE0 + g)
     }
 
-    function te(S, g) {
-        let B = i.get(S);
-        if (S.version > 0 && B.__version !== S.version) {
-            Te(B, S, g);
+    function ee(E, g) {
+        let B = i.get(E);
+        if (E.version > 0 && B.__version !== E.version) {
+            we(B, E, g);
             return
         }
         t.bindTexture(r.TEXTURE_CUBE_MAP, B.__webglTexture, r.TEXTURE0 + g)
     }
-    let ee = {
+    let ie = {
             [ga]: r.REPEAT,
-            [It]: r.CLAMP_TO_EDGE,
+            [Nt]: r.CLAMP_TO_EDGE,
             [_a]: r.MIRRORED_REPEAT
         },
-        pe = {
+        de = {
             [_t]: r.NEAREST,
             [as]: r.NEAREST_MIPMAP_NEAREST,
             [pr]: r.NEAREST_MIPMAP_LINEAR,
             [xt]: r.LINEAR,
-            [Un]: r.LINEAR_MIPMAP_NEAREST,
+            [Dn]: r.LINEAR_MIPMAP_NEAREST,
             [wi]: r.LINEAR_MIPMAP_LINEAR
         },
-        xe = {
+        ge = {
             [Zl]: r.NEVER,
             [tc]: r.ALWAYS,
             [Kl]: r.LESS,
-            [Go]: r.LEQUAL,
+            [Ho]: r.LEQUAL,
             [Jl]: r.EQUAL,
             [ec]: r.GEQUAL,
             [$l]: r.GREATER,
             [Ql]: r.NOTEQUAL
         };
 
-    function H(S, g, B) {
-        if (g.type === Zt && e.has("OES_texture_float_linear") === !1 && (g.magFilter === xt || g.magFilter === Un || g.magFilter === pr || g.magFilter === wi || g.minFilter === xt || g.minFilter === Un || g.minFilter === pr || g.minFilter === wi) && console.warn("THREE.WebGLRenderer: Unable to use linear filtering with floating point textures. OES_texture_float_linear not supported on this device."), B ? (r.texParameteri(S, r.TEXTURE_WRAP_S, ee[g.wrapS]), r.texParameteri(S, r.TEXTURE_WRAP_T, ee[g.wrapT]), (S === r.TEXTURE_3D || S === r.TEXTURE_2D_ARRAY) && r.texParameteri(S, r.TEXTURE_WRAP_R, ee[g.wrapR]), r.texParameteri(S, r.TEXTURE_MAG_FILTER, pe[g.magFilter]), r.texParameteri(S, r.TEXTURE_MIN_FILTER, pe[g.minFilter])) : (r.texParameteri(S, r.TEXTURE_WRAP_S, r.CLAMP_TO_EDGE), r.texParameteri(S, r.TEXTURE_WRAP_T, r.CLAMP_TO_EDGE), (S === r.TEXTURE_3D || S === r.TEXTURE_2D_ARRAY) && r.texParameteri(S, r.TEXTURE_WRAP_R, r.CLAMP_TO_EDGE), (g.wrapS !== It || g.wrapT !== It) && console.warn("THREE.WebGLRenderer: Texture is not power of two. Texture.wrapS and Texture.wrapT should be set to THREE.ClampToEdgeWrapping."), r.texParameteri(S, r.TEXTURE_MAG_FILTER, y(g.magFilter)), r.texParameteri(S, r.TEXTURE_MIN_FILTER, y(g.minFilter)), g.minFilter !== _t && g.minFilter !== xt && console.warn("THREE.WebGLRenderer: Texture is not power of two. Texture.minFilter should be set to THREE.NearestFilter or THREE.LinearFilter.")), g.compareFunction && (r.texParameteri(S, r.TEXTURE_COMPARE_MODE, r.COMPARE_REF_TO_TEXTURE), r.texParameteri(S, r.TEXTURE_COMPARE_FUNC, xe[g.compareFunction])), e.has("EXT_texture_filter_anisotropic") === !0) {
+    function V(E, g, B) {
+        if (g.type === Zt && e.has("OES_texture_float_linear") === !1 && (g.magFilter === xt || g.magFilter === Dn || g.magFilter === pr || g.magFilter === wi || g.minFilter === xt || g.minFilter === Dn || g.minFilter === pr || g.minFilter === wi) && console.warn("THREE.WebGLRenderer: Unable to use linear filtering with floating point textures. OES_texture_float_linear not supported on this device."), B ? (r.texParameteri(E, r.TEXTURE_WRAP_S, ie[g.wrapS]), r.texParameteri(E, r.TEXTURE_WRAP_T, ie[g.wrapT]), (E === r.TEXTURE_3D || E === r.TEXTURE_2D_ARRAY) && r.texParameteri(E, r.TEXTURE_WRAP_R, ie[g.wrapR]), r.texParameteri(E, r.TEXTURE_MAG_FILTER, de[g.magFilter]), r.texParameteri(E, r.TEXTURE_MIN_FILTER, de[g.minFilter])) : (r.texParameteri(E, r.TEXTURE_WRAP_S, r.CLAMP_TO_EDGE), r.texParameteri(E, r.TEXTURE_WRAP_T, r.CLAMP_TO_EDGE), (E === r.TEXTURE_3D || E === r.TEXTURE_2D_ARRAY) && r.texParameteri(E, r.TEXTURE_WRAP_R, r.CLAMP_TO_EDGE), (g.wrapS !== Nt || g.wrapT !== Nt) && console.warn("THREE.WebGLRenderer: Texture is not power of two. Texture.wrapS and Texture.wrapT should be set to THREE.ClampToEdgeWrapping."), r.texParameteri(E, r.TEXTURE_MAG_FILTER, b(g.magFilter)), r.texParameteri(E, r.TEXTURE_MIN_FILTER, b(g.minFilter)), g.minFilter !== _t && g.minFilter !== xt && console.warn("THREE.WebGLRenderer: Texture is not power of two. Texture.minFilter should be set to THREE.NearestFilter or THREE.LinearFilter.")), g.compareFunction && (r.texParameteri(E, r.TEXTURE_COMPARE_MODE, r.COMPARE_REF_TO_TEXTURE), r.texParameteri(E, r.TEXTURE_COMPARE_FUNC, ge[g.compareFunction])), e.has("EXT_texture_filter_anisotropic") === !0) {
             if (g.magFilter === _t || g.minFilter !== pr && g.minFilter !== wi || g.type === Zt && e.has("OES_texture_float_linear") === !1 || s === !1 && g.type === Mr && e.has("OES_texture_half_float_linear") === !1) return;
             if (g.anisotropy > 1 || i.get(g).__currentAnisotropy) {
-                let Y = e.get("EXT_texture_filter_anisotropic");
-                r.texParameterf(S, Y.TEXTURE_MAX_ANISOTROPY_EXT, Math.min(g.anisotropy, n.getMaxAnisotropy())), i.get(g).__currentAnisotropy = g.anisotropy
+                let X = e.get("EXT_texture_filter_anisotropic");
+                r.texParameterf(E, X.TEXTURE_MAX_ANISOTROPY_EXT, Math.min(g.anisotropy, n.getMaxAnisotropy())), i.get(g).__currentAnisotropy = g.anisotropy
             }
         }
     }
 
-    function ie(S, g) {
+    function te(E, g) {
         let B = !1;
-        S.__webglInit === void 0 && (S.__webglInit = !0, g.addEventListener("dispose", C));
-        let Y = g.source,
-            Q = m.get(Y);
-        Q === void 0 && (Q = {}, m.set(Y, Q));
+        E.__webglInit === void 0 && (E.__webglInit = !0, g.addEventListener("dispose", P));
+        let X = g.source,
+            Q = m.get(X);
+        Q === void 0 && (Q = {}, m.set(X, Q));
         let J = k(g);
-        if (J !== S.__cacheKey) {
+        if (J !== E.__cacheKey) {
             Q[J] === void 0 && (Q[J] = {
                 texture: r.createTexture(),
                 usedTimes: 0
             }, o.memory.textures++, B = !0), Q[J].usedTimes++;
-            let Ce = Q[S.__cacheKey];
-            Ce !== void 0 && (Q[S.__cacheKey].usedTimes--, Ce.usedTimes === 0 && T(g)), S.__cacheKey = J, S.__webglTexture = Q[J].texture
+            let Ee = Q[E.__cacheKey];
+            Ee !== void 0 && (Q[E.__cacheKey].usedTimes--, Ee.usedTimes === 0 && w(g)), E.__cacheKey = J, E.__webglTexture = Q[J].texture
         }
         return B
     }
 
-    function fe(S, g, B) {
-        let Y = r.TEXTURE_2D;
-        (g.isDataArrayTexture || g.isCompressedArrayTexture) && (Y = r.TEXTURE_2D_ARRAY), g.isData3DTexture && (Y = r.TEXTURE_3D);
-        let Q = ie(S, g),
+    function pe(E, g, B) {
+        let X = r.TEXTURE_2D;
+        (g.isDataArrayTexture || g.isCompressedArrayTexture) && (X = r.TEXTURE_2D_ARRAY), g.isData3DTexture && (X = r.TEXTURE_3D);
+        let Q = te(E, g),
             J = g.source;
-        t.bindTexture(Y, S.__webglTexture, r.TEXTURE0 + B);
-        let Ce = i.get(J);
-        if (J.version !== Ce.__version || Q === !0) {
+        t.bindTexture(X, E.__webglTexture, r.TEXTURE0 + B);
+        let Ee = i.get(J);
+        if (J.version !== Ee.__version || Q === !0) {
             t.activeTexture(r.TEXTURE0 + B);
-            let ye = qe.getPrimaries(qe.workingColorSpace),
+            let Me = qe.getPrimaries(qe.workingColorSpace),
                 ae = g.colorSpace === oi ? null : qe.getPrimaries(g.colorSpace),
-                he = g.colorSpace === oi || ye === ae ? r.NONE : r.BROWSER_DEFAULT_WEBGL;
+                he = g.colorSpace === oi || Me === ae ? r.NONE : r.BROWSER_DEFAULT_WEBGL;
             r.pixelStorei(r.UNPACK_FLIP_Y_WEBGL, g.flipY), r.pixelStorei(r.UNPACK_PREMULTIPLY_ALPHA_WEBGL, g.premultiplyAlpha), r.pixelStorei(r.UNPACK_ALIGNMENT, g.unpackAlignment), r.pixelStorei(r.UNPACK_COLORSPACE_CONVERSION_WEBGL, he);
-            let Ie = w(g) && h(g.image) === !1,
+            let Ie = T(g) && u(g.image) === !1,
                 ne = d(g.image, Ie, !1, n.maxTextureSize);
-            ne = de(g, ne);
-            let Je = h(ne) || s,
-                ze = a.convert(g.format, g.colorSpace),
-                Ee = a.convert(g.type),
-                ge = U(g.internalFormat, ze, Ee, g.colorSpace, g.isVideoTexture);
-            H(Y, g, Je);
-            let b, $ = g.mipmaps,
-                oe = s && g.isVideoTexture !== !0 && ge !== zo,
-                Ae = Ce.__version === void 0 || Q === !0,
-                L = J.dataReady,
-                re = A(g, ne, Je);
-            if (g.isDepthTexture) ge = r.DEPTH_COMPONENT, s ? g.type === Zt ? ge = r.DEPTH_COMPONENT32F : g.type === li ? ge = r.DEPTH_COMPONENT24 : g.type === Ri ? ge = r.DEPTH24_STENCIL8 : ge = r.DEPTH_COMPONENT16 : g.type === Zt && console.error("WebGLRenderer: Floating point depth texture requires WebGL2."), g.format === Ci && ge === r.DEPTH_COMPONENT && g.type !== Va && g.type !== li && (console.warn("THREE.WebGLRenderer: Use UnsignedShortType or UnsignedIntType for DepthFormat DepthTexture."), g.type = li, Ee = a.convert(g.type)), g.format === sr && ge === r.DEPTH_COMPONENT && (ge = r.DEPTH_STENCIL, g.type !== Ri && (console.warn("THREE.WebGLRenderer: Use UnsignedInt248Type for DepthStencilFormat DepthTexture."), g.type = Ri, Ee = a.convert(g.type))), Ae && (oe ? t.texStorage2D(r.TEXTURE_2D, 1, ge, ne.width, ne.height) : t.texImage2D(r.TEXTURE_2D, 0, ge, ne.width, ne.height, 0, ze, Ee, null));
+            ne = Re(g, ne);
+            let $e = u(ne) || s,
+                Be = a.convert(g.format, g.colorSpace),
+                ye = a.convert(g.type),
+                me = D(g.internalFormat, Be, ye, g.colorSpace, g.isVideoTexture);
+            V(X, g, $e);
+            let S, $ = g.mipmaps,
+                oe = s && g.isVideoTexture !== !0 && me !== Bo,
+                Ce = Ee.__version === void 0 || Q === !0,
+                C = J.dataReady,
+                re = R(g, ne, $e);
+            if (g.isDepthTexture) me = r.DEPTH_COMPONENT, s ? g.type === Zt ? me = r.DEPTH_COMPONENT32F : g.type === li ? me = r.DEPTH_COMPONENT24 : g.type === Ri ? me = r.DEPTH24_STENCIL8 : me = r.DEPTH_COMPONENT16 : g.type === Zt && console.error("WebGLRenderer: Floating point depth texture requires WebGL2."), g.format === Ci && me === r.DEPTH_COMPONENT && g.type !== Va && g.type !== li && (console.warn("THREE.WebGLRenderer: Use UnsignedShortType or UnsignedIntType for DepthFormat DepthTexture."), g.type = li, ye = a.convert(g.type)), g.format === sr && me === r.DEPTH_COMPONENT && (me = r.DEPTH_STENCIL, g.type !== Ri && (console.warn("THREE.WebGLRenderer: Use UnsignedInt248Type for DepthStencilFormat DepthTexture."), g.type = Ri, ye = a.convert(g.type))), Ce && (oe ? t.texStorage2D(r.TEXTURE_2D, 1, me, ne.width, ne.height) : t.texImage2D(r.TEXTURE_2D, 0, me, ne.width, ne.height, 0, Be, ye, null));
             else if (g.isDataTexture)
-                if ($.length > 0 && Je) {
-                    oe && Ae && t.texStorage2D(r.TEXTURE_2D, re, ge, $[0].width, $[0].height);
-                    for (let O = 0, le = $.length; O < le; O++) b = $[O], oe ? L && t.texSubImage2D(r.TEXTURE_2D, O, 0, 0, b.width, b.height, ze, Ee, b.data) : t.texImage2D(r.TEXTURE_2D, O, ge, b.width, b.height, 0, ze, Ee, b.data);
+                if ($.length > 0 && $e) {
+                    oe && Ce && t.texStorage2D(r.TEXTURE_2D, re, me, $[0].width, $[0].height);
+                    for (let F = 0, le = $.length; F < le; F++) S = $[F], oe ? C && t.texSubImage2D(r.TEXTURE_2D, F, 0, 0, S.width, S.height, Be, ye, S.data) : t.texImage2D(r.TEXTURE_2D, F, me, S.width, S.height, 0, Be, ye, S.data);
                     g.generateMipmaps = !1
-                } else oe ? (Ae && t.texStorage2D(r.TEXTURE_2D, re, ge, ne.width, ne.height), L && t.texSubImage2D(r.TEXTURE_2D, 0, 0, 0, ne.width, ne.height, ze, Ee, ne.data)) : t.texImage2D(r.TEXTURE_2D, 0, ge, ne.width, ne.height, 0, ze, Ee, ne.data);
+                } else oe ? (Ce && t.texStorage2D(r.TEXTURE_2D, re, me, ne.width, ne.height), C && t.texSubImage2D(r.TEXTURE_2D, 0, 0, 0, ne.width, ne.height, Be, ye, ne.data)) : t.texImage2D(r.TEXTURE_2D, 0, me, ne.width, ne.height, 0, Be, ye, ne.data);
             else if (g.isCompressedTexture)
                 if (g.isCompressedArrayTexture) {
-                    oe && Ae && t.texStorage3D(r.TEXTURE_2D_ARRAY, re, ge, $[0].width, $[0].height, ne.depth);
-                    for (let O = 0, le = $.length; O < le; O++) b = $[O], g.format !== Ot ? ze !== null ? oe ? L && t.compressedTexSubImage3D(r.TEXTURE_2D_ARRAY, O, 0, 0, 0, b.width, b.height, ne.depth, ze, b.data, 0, 0) : t.compressedTexImage3D(r.TEXTURE_2D_ARRAY, O, ge, b.width, b.height, ne.depth, 0, b.data, 0, 0) : console.warn("THREE.WebGLRenderer: Attempt to load unsupported compressed texture format in .uploadTexture()") : oe ? L && t.texSubImage3D(r.TEXTURE_2D_ARRAY, O, 0, 0, 0, b.width, b.height, ne.depth, ze, Ee, b.data) : t.texImage3D(r.TEXTURE_2D_ARRAY, O, ge, b.width, b.height, ne.depth, 0, ze, Ee, b.data)
+                    oe && Ce && t.texStorage3D(r.TEXTURE_2D_ARRAY, re, me, $[0].width, $[0].height, ne.depth);
+                    for (let F = 0, le = $.length; F < le; F++) S = $[F], g.format !== Ot ? Be !== null ? oe ? C && t.compressedTexSubImage3D(r.TEXTURE_2D_ARRAY, F, 0, 0, 0, S.width, S.height, ne.depth, Be, S.data, 0, 0) : t.compressedTexImage3D(r.TEXTURE_2D_ARRAY, F, me, S.width, S.height, ne.depth, 0, S.data, 0, 0) : console.warn("THREE.WebGLRenderer: Attempt to load unsupported compressed texture format in .uploadTexture()") : oe ? C && t.texSubImage3D(r.TEXTURE_2D_ARRAY, F, 0, 0, 0, S.width, S.height, ne.depth, Be, ye, S.data) : t.texImage3D(r.TEXTURE_2D_ARRAY, F, me, S.width, S.height, ne.depth, 0, Be, ye, S.data)
                 } else {
-                    oe && Ae && t.texStorage2D(r.TEXTURE_2D, re, ge, $[0].width, $[0].height);
-                    for (let O = 0, le = $.length; O < le; O++) b = $[O], g.format !== Ot ? ze !== null ? oe ? L && t.compressedTexSubImage2D(r.TEXTURE_2D, O, 0, 0, b.width, b.height, ze, b.data) : t.compressedTexImage2D(r.TEXTURE_2D, O, ge, b.width, b.height, 0, b.data) : console.warn("THREE.WebGLRenderer: Attempt to load unsupported compressed texture format in .uploadTexture()") : oe ? L && t.texSubImage2D(r.TEXTURE_2D, O, 0, 0, b.width, b.height, ze, Ee, b.data) : t.texImage2D(r.TEXTURE_2D, O, ge, b.width, b.height, 0, ze, Ee, b.data)
+                    oe && Ce && t.texStorage2D(r.TEXTURE_2D, re, me, $[0].width, $[0].height);
+                    for (let F = 0, le = $.length; F < le; F++) S = $[F], g.format !== Ot ? Be !== null ? oe ? C && t.compressedTexSubImage2D(r.TEXTURE_2D, F, 0, 0, S.width, S.height, Be, S.data) : t.compressedTexImage2D(r.TEXTURE_2D, F, me, S.width, S.height, 0, S.data) : console.warn("THREE.WebGLRenderer: Attempt to load unsupported compressed texture format in .uploadTexture()") : oe ? C && t.texSubImage2D(r.TEXTURE_2D, F, 0, 0, S.width, S.height, Be, ye, S.data) : t.texImage2D(r.TEXTURE_2D, F, me, S.width, S.height, 0, Be, ye, S.data)
                 }
-            else if (g.isDataArrayTexture) oe ? (Ae && t.texStorage3D(r.TEXTURE_2D_ARRAY, re, ge, ne.width, ne.height, ne.depth), L && t.texSubImage3D(r.TEXTURE_2D_ARRAY, 0, 0, 0, 0, ne.width, ne.height, ne.depth, ze, Ee, ne.data)) : t.texImage3D(r.TEXTURE_2D_ARRAY, 0, ge, ne.width, ne.height, ne.depth, 0, ze, Ee, ne.data);
-            else if (g.isData3DTexture) oe ? (Ae && t.texStorage3D(r.TEXTURE_3D, re, ge, ne.width, ne.height, ne.depth), L && t.texSubImage3D(r.TEXTURE_3D, 0, 0, 0, 0, ne.width, ne.height, ne.depth, ze, Ee, ne.data)) : t.texImage3D(r.TEXTURE_3D, 0, ge, ne.width, ne.height, ne.depth, 0, ze, Ee, ne.data);
+            else if (g.isDataArrayTexture) oe ? (Ce && t.texStorage3D(r.TEXTURE_2D_ARRAY, re, me, ne.width, ne.height, ne.depth), C && t.texSubImage3D(r.TEXTURE_2D_ARRAY, 0, 0, 0, 0, ne.width, ne.height, ne.depth, Be, ye, ne.data)) : t.texImage3D(r.TEXTURE_2D_ARRAY, 0, me, ne.width, ne.height, ne.depth, 0, Be, ye, ne.data);
+            else if (g.isData3DTexture) oe ? (Ce && t.texStorage3D(r.TEXTURE_3D, re, me, ne.width, ne.height, ne.depth), C && t.texSubImage3D(r.TEXTURE_3D, 0, 0, 0, 0, ne.width, ne.height, ne.depth, Be, ye, ne.data)) : t.texImage3D(r.TEXTURE_3D, 0, me, ne.width, ne.height, ne.depth, 0, Be, ye, ne.data);
             else if (g.isFramebufferTexture) {
-                if (Ae)
-                    if (oe) t.texStorage2D(r.TEXTURE_2D, re, ge, ne.width, ne.height);
+                if (Ce)
+                    if (oe) t.texStorage2D(r.TEXTURE_2D, re, me, ne.width, ne.height);
                     else {
-                        let O = ne.width,
+                        let F = ne.width,
                             le = ne.height;
-                        for (let se = 0; se < re; se++) t.texImage2D(r.TEXTURE_2D, se, ge, O, le, 0, ze, Ee, null), O >>= 1, le >>= 1
+                        for (let se = 0; se < re; se++) t.texImage2D(r.TEXTURE_2D, se, me, F, le, 0, Be, ye, null), F >>= 1, le >>= 1
                     }
-            } else if ($.length > 0 && Je) {
-                if (oe && Ae) {
-                    let O = Ne($[0]);
-                    t.texStorage2D(r.TEXTURE_2D, re, ge, O.width, O.height)
+            } else if ($.length > 0 && $e) {
+                if (oe && Ce) {
+                    let F = xe($[0]);
+                    t.texStorage2D(r.TEXTURE_2D, re, me, F.width, F.height)
                 }
-                for (let O = 0, le = $.length; O < le; O++) b = $[O], oe ? L && t.texSubImage2D(r.TEXTURE_2D, O, 0, 0, ze, Ee, b) : t.texImage2D(r.TEXTURE_2D, O, ge, ze, Ee, b);
+                for (let F = 0, le = $.length; F < le; F++) S = $[F], oe ? C && t.texSubImage2D(r.TEXTURE_2D, F, 0, 0, Be, ye, S) : t.texImage2D(r.TEXTURE_2D, F, me, Be, ye, S);
                 g.generateMipmaps = !1
             } else if (oe) {
-                if (Ae) {
-                    let O = Ne(ne);
-                    t.texStorage2D(r.TEXTURE_2D, re, ge, O.width, O.height)
+                if (Ce) {
+                    let F = xe(ne);
+                    t.texStorage2D(r.TEXTURE_2D, re, me, F.width, F.height)
                 }
-                L && t.texSubImage2D(r.TEXTURE_2D, 0, 0, 0, ze, Ee, ne)
-            } else t.texImage2D(r.TEXTURE_2D, 0, ge, ze, Ee, ne);
-            x(g, Je) && R(Y), Ce.__version = J.version, g.onUpdate && g.onUpdate(g)
+                C && t.texSubImage2D(r.TEXTURE_2D, 0, 0, 0, Be, ye, ne)
+            } else t.texImage2D(r.TEXTURE_2D, 0, me, Be, ye, ne);
+            x(g, $e) && A(X), Ee.__version = J.version, g.onUpdate && g.onUpdate(g)
         }
-        S.__version = g.version
+        E.__version = g.version
     }
 
-    function Te(S, g, B) {
+    function we(E, g, B) {
         if (g.image.length !== 6) return;
-        let Y = ie(S, g),
+        let X = te(E, g),
             Q = g.source;
-        t.bindTexture(r.TEXTURE_CUBE_MAP, S.__webglTexture, r.TEXTURE0 + B);
+        t.bindTexture(r.TEXTURE_CUBE_MAP, E.__webglTexture, r.TEXTURE0 + B);
         let J = i.get(Q);
-        if (Q.version !== J.__version || Y === !0) {
+        if (Q.version !== J.__version || X === !0) {
             t.activeTexture(r.TEXTURE0 + B);
-            let Ce = qe.getPrimaries(qe.workingColorSpace),
-                ye = g.colorSpace === oi ? null : qe.getPrimaries(g.colorSpace),
-                ae = g.colorSpace === oi || Ce === ye ? r.NONE : r.BROWSER_DEFAULT_WEBGL;
+            let Ee = qe.getPrimaries(qe.workingColorSpace),
+                Me = g.colorSpace === oi ? null : qe.getPrimaries(g.colorSpace),
+                ae = g.colorSpace === oi || Ee === Me ? r.NONE : r.BROWSER_DEFAULT_WEBGL;
             r.pixelStorei(r.UNPACK_FLIP_Y_WEBGL, g.flipY), r.pixelStorei(r.UNPACK_PREMULTIPLY_ALPHA_WEBGL, g.premultiplyAlpha), r.pixelStorei(r.UNPACK_ALIGNMENT, g.unpackAlignment), r.pixelStorei(r.UNPACK_COLORSPACE_CONVERSION_WEBGL, ae);
             let he = g.isCompressedTexture || g.image[0].isCompressedTexture,
                 Ie = g.image[0] && g.image[0].isDataTexture,
                 ne = [];
-            for (let O = 0; O < 6; O++) !he && !Ie ? ne[O] = d(g.image[O], !1, !0, n.maxCubemapSize) : ne[O] = Ie ? g.image[O].image : g.image[O], ne[O] = de(g, ne[O]);
-            let Je = ne[0],
-                ze = h(Je) || s,
-                Ee = a.convert(g.format, g.colorSpace),
-                ge = a.convert(g.type),
-                b = U(g.internalFormat, Ee, ge, g.colorSpace),
+            for (let F = 0; F < 6; F++) !he && !Ie ? ne[F] = d(g.image[F], !1, !0, n.maxCubemapSize) : ne[F] = Ie ? g.image[F].image : g.image[F], ne[F] = Re(g, ne[F]);
+            let $e = ne[0],
+                Be = u($e) || s,
+                ye = a.convert(g.format, g.colorSpace),
+                me = a.convert(g.type),
+                S = D(g.internalFormat, ye, me, g.colorSpace),
                 $ = s && g.isVideoTexture !== !0,
-                oe = J.__version === void 0 || Y === !0,
-                Ae = Q.dataReady,
-                L = A(g, Je, ze);
-            H(r.TEXTURE_CUBE_MAP, g, ze);
+                oe = J.__version === void 0 || X === !0,
+                Ce = Q.dataReady,
+                C = R(g, $e, Be);
+            V(r.TEXTURE_CUBE_MAP, g, Be);
             let re;
             if (he) {
-                $ && oe && t.texStorage2D(r.TEXTURE_CUBE_MAP, L, b, Je.width, Je.height);
-                for (let O = 0; O < 6; O++) {
-                    re = ne[O].mipmaps;
+                $ && oe && t.texStorage2D(r.TEXTURE_CUBE_MAP, C, S, $e.width, $e.height);
+                for (let F = 0; F < 6; F++) {
+                    re = ne[F].mipmaps;
                     for (let le = 0; le < re.length; le++) {
                         let se = re[le];
-                        g.format !== Ot ? Ee !== null ? $ ? Ae && t.compressedTexSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le, 0, 0, se.width, se.height, Ee, se.data) : t.compressedTexImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le, b, se.width, se.height, 0, se.data) : console.warn("THREE.WebGLRenderer: Attempt to load unsupported compressed texture format in .setTextureCube()") : $ ? Ae && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le, 0, 0, se.width, se.height, Ee, ge, se.data) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le, b, se.width, se.height, 0, Ee, ge, se.data)
+                        g.format !== Ot ? ye !== null ? $ ? Ce && t.compressedTexSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le, 0, 0, se.width, se.height, ye, se.data) : t.compressedTexImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le, S, se.width, se.height, 0, se.data) : console.warn("THREE.WebGLRenderer: Attempt to load unsupported compressed texture format in .setTextureCube()") : $ ? Ce && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le, 0, 0, se.width, se.height, ye, me, se.data) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le, S, se.width, se.height, 0, ye, me, se.data)
                     }
                 }
             } else {
                 if (re = g.mipmaps, $ && oe) {
-                    re.length > 0 && L++;
-                    let O = Ne(ne[0]);
-                    t.texStorage2D(r.TEXTURE_CUBE_MAP, L, b, O.width, O.height)
+                    re.length > 0 && C++;
+                    let F = xe(ne[0]);
+                    t.texStorage2D(r.TEXTURE_CUBE_MAP, C, S, F.width, F.height)
                 }
-                for (let O = 0; O < 6; O++)
+                for (let F = 0; F < 6; F++)
                     if (Ie) {
-                        $ ? Ae && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, 0, 0, 0, ne[O].width, ne[O].height, Ee, ge, ne[O].data) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, 0, b, ne[O].width, ne[O].height, 0, Ee, ge, ne[O].data);
+                        $ ? Ce && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, 0, 0, 0, ne[F].width, ne[F].height, ye, me, ne[F].data) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, 0, S, ne[F].width, ne[F].height, 0, ye, me, ne[F].data);
                         for (let le = 0; le < re.length; le++) {
-                            let se = re[le].image[O].image;
-                            $ ? Ae && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le + 1, 0, 0, se.width, se.height, Ee, ge, se.data) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le + 1, b, se.width, se.height, 0, Ee, ge, se.data)
+                            let se = re[le].image[F].image;
+                            $ ? Ce && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le + 1, 0, 0, se.width, se.height, ye, me, se.data) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le + 1, S, se.width, se.height, 0, ye, me, se.data)
                         }
                     } else {
-                        $ ? Ae && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, 0, 0, 0, Ee, ge, ne[O]) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, 0, b, Ee, ge, ne[O]);
+                        $ ? Ce && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, 0, 0, 0, ye, me, ne[F]) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, 0, S, ye, me, ne[F]);
                         for (let le = 0; le < re.length; le++) {
                             let se = re[le];
-                            $ ? Ae && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le + 1, 0, 0, Ee, ge, se.image[O]) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + O, le + 1, b, Ee, ge, se.image[O])
+                            $ ? Ce && t.texSubImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le + 1, 0, 0, ye, me, se.image[F]) : t.texImage2D(r.TEXTURE_CUBE_MAP_POSITIVE_X + F, le + 1, S, ye, me, se.image[F])
                         }
                     }
             }
-            x(g, ze) && R(r.TEXTURE_CUBE_MAP), J.__version = Q.version, g.onUpdate && g.onUpdate(g)
+            x(g, Be) && A(r.TEXTURE_CUBE_MAP), J.__version = Q.version, g.onUpdate && g.onUpdate(g)
         }
-        S.__version = g.version
+        E.__version = g.version
     }
 
-    function _e(S, g, B, Y, Q, J) {
-        let Ce = a.convert(B.format, B.colorSpace),
-            ye = a.convert(B.type),
-            ae = U(B.internalFormat, Ce, ye, B.colorSpace);
+    function _e(E, g, B, X, Q, J) {
+        let Ee = a.convert(B.format, B.colorSpace),
+            Me = a.convert(B.type),
+            ae = D(B.internalFormat, Ee, Me, B.colorSpace);
         if (!i.get(g).__hasExternalTextures) {
             let he = Math.max(1, g.width >> J),
                 Ie = Math.max(1, g.height >> J);
-            Q === r.TEXTURE_3D || Q === r.TEXTURE_2D_ARRAY ? t.texImage3D(Q, J, ae, he, Ie, g.depth, 0, Ce, ye, null) : t.texImage2D(Q, J, ae, he, Ie, 0, Ce, ye, null)
+            Q === r.TEXTURE_3D || Q === r.TEXTURE_2D_ARRAY ? t.texImage3D(Q, J, ae, he, Ie, g.depth, 0, Ee, Me, null) : t.texImage2D(Q, J, ae, he, Ie, 0, Ee, Me, null)
         }
-        t.bindFramebuffer(r.FRAMEBUFFER, S), Le(g) ? l.framebufferTexture2DMultisampleEXT(r.FRAMEBUFFER, Y, Q, i.get(B).__webglTexture, 0, Me(g)) : (Q === r.TEXTURE_2D || Q >= r.TEXTURE_CUBE_MAP_POSITIVE_X && Q <= r.TEXTURE_CUBE_MAP_NEGATIVE_Z) && r.framebufferTexture2D(r.FRAMEBUFFER, Y, Q, i.get(B).__webglTexture, J), t.bindFramebuffer(r.FRAMEBUFFER, null)
+        t.bindFramebuffer(r.FRAMEBUFFER, E), Ne(g) ? l.framebufferTexture2DMultisampleEXT(r.FRAMEBUFFER, X, Q, i.get(B).__webglTexture, 0, Se(g)) : (Q === r.TEXTURE_2D || Q >= r.TEXTURE_CUBE_MAP_POSITIVE_X && Q <= r.TEXTURE_CUBE_MAP_NEGATIVE_Z) && r.framebufferTexture2D(r.FRAMEBUFFER, X, Q, i.get(B).__webglTexture, J), t.bindFramebuffer(r.FRAMEBUFFER, null)
     }
 
-    function me(S, g, B) {
-        if (r.bindRenderbuffer(r.RENDERBUFFER, S), g.depthBuffer && !g.stencilBuffer) {
-            let Y = s === !0 ? r.DEPTH_COMPONENT24 : r.DEPTH_COMPONENT16;
-            if (B || Le(g)) {
+    function fe(E, g, B) {
+        if (r.bindRenderbuffer(r.RENDERBUFFER, E), g.depthBuffer && !g.stencilBuffer) {
+            let X = s === !0 ? r.DEPTH_COMPONENT24 : r.DEPTH_COMPONENT16;
+            if (B || Ne(g)) {
                 let Q = g.depthTexture;
-                Q && Q.isDepthTexture && (Q.type === Zt ? Y = r.DEPTH_COMPONENT32F : Q.type === li && (Y = r.DEPTH_COMPONENT24));
-                let J = Me(g);
-                Le(g) ? l.renderbufferStorageMultisampleEXT(r.RENDERBUFFER, J, Y, g.width, g.height) : r.renderbufferStorageMultisample(r.RENDERBUFFER, J, Y, g.width, g.height)
-            } else r.renderbufferStorage(r.RENDERBUFFER, Y, g.width, g.height);
-            r.framebufferRenderbuffer(r.FRAMEBUFFER, r.DEPTH_ATTACHMENT, r.RENDERBUFFER, S)
+                Q && Q.isDepthTexture && (Q.type === Zt ? X = r.DEPTH_COMPONENT32F : Q.type === li && (X = r.DEPTH_COMPONENT24));
+                let J = Se(g);
+                Ne(g) ? l.renderbufferStorageMultisampleEXT(r.RENDERBUFFER, J, X, g.width, g.height) : r.renderbufferStorageMultisample(r.RENDERBUFFER, J, X, g.width, g.height)
+            } else r.renderbufferStorage(r.RENDERBUFFER, X, g.width, g.height);
+            r.framebufferRenderbuffer(r.FRAMEBUFFER, r.DEPTH_ATTACHMENT, r.RENDERBUFFER, E)
         } else if (g.depthBuffer && g.stencilBuffer) {
-            let Y = Me(g);
-            B && Le(g) === !1 ? r.renderbufferStorageMultisample(r.RENDERBUFFER, Y, r.DEPTH24_STENCIL8, g.width, g.height) : Le(g) ? l.renderbufferStorageMultisampleEXT(r.RENDERBUFFER, Y, r.DEPTH24_STENCIL8, g.width, g.height) : r.renderbufferStorage(r.RENDERBUFFER, r.DEPTH_STENCIL, g.width, g.height), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.DEPTH_STENCIL_ATTACHMENT, r.RENDERBUFFER, S)
+            let X = Se(g);
+            B && Ne(g) === !1 ? r.renderbufferStorageMultisample(r.RENDERBUFFER, X, r.DEPTH24_STENCIL8, g.width, g.height) : Ne(g) ? l.renderbufferStorageMultisampleEXT(r.RENDERBUFFER, X, r.DEPTH24_STENCIL8, g.width, g.height) : r.renderbufferStorage(r.RENDERBUFFER, r.DEPTH_STENCIL, g.width, g.height), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.DEPTH_STENCIL_ATTACHMENT, r.RENDERBUFFER, E)
         } else {
-            let Y = g.textures;
-            for (let Q = 0; Q < Y.length; Q++) {
-                let J = Y[Q],
-                    Ce = a.convert(J.format, J.colorSpace),
-                    ye = a.convert(J.type),
-                    ae = U(J.internalFormat, Ce, ye, J.colorSpace),
-                    he = Me(g);
-                B && Le(g) === !1 ? r.renderbufferStorageMultisample(r.RENDERBUFFER, he, ae, g.width, g.height) : Le(g) ? l.renderbufferStorageMultisampleEXT(r.RENDERBUFFER, he, ae, g.width, g.height) : r.renderbufferStorage(r.RENDERBUFFER, ae, g.width, g.height)
+            let X = g.textures;
+            for (let Q = 0; Q < X.length; Q++) {
+                let J = X[Q],
+                    Ee = a.convert(J.format, J.colorSpace),
+                    Me = a.convert(J.type),
+                    ae = D(J.internalFormat, Ee, Me, J.colorSpace),
+                    he = Se(g);
+                B && Ne(g) === !1 ? r.renderbufferStorageMultisample(r.RENDERBUFFER, he, ae, g.width, g.height) : Ne(g) ? l.renderbufferStorageMultisampleEXT(r.RENDERBUFFER, he, ae, g.width, g.height) : r.renderbufferStorage(r.RENDERBUFFER, ae, g.width, g.height)
             }
         }
         r.bindRenderbuffer(r.RENDERBUFFER, null)
     }
 
-    function Xe(S, g) {
+    function Xe(E, g) {
         if (g && g.isWebGLCubeRenderTarget) throw new Error("Depth Texture with cube render targets is not supported");
-        if (t.bindFramebuffer(r.FRAMEBUFFER, S), !(g.depthTexture && g.depthTexture.isDepthTexture)) throw new Error("renderTarget.depthTexture must be an instance of THREE.DepthTexture");
-        (!i.get(g.depthTexture).__webglTexture || g.depthTexture.image.width !== g.width || g.depthTexture.image.height !== g.height) && (g.depthTexture.image.width = g.width, g.depthTexture.image.height = g.height, g.depthTexture.needsUpdate = !0), j(g.depthTexture, 0);
+        if (t.bindFramebuffer(r.FRAMEBUFFER, E), !(g.depthTexture && g.depthTexture.isDepthTexture)) throw new Error("renderTarget.depthTexture must be an instance of THREE.DepthTexture");
+        (!i.get(g.depthTexture).__webglTexture || g.depthTexture.image.width !== g.width || g.depthTexture.image.height !== g.height) && (g.depthTexture.image.width = g.width, g.depthTexture.image.height = g.height, g.depthTexture.needsUpdate = !0), Y(g.depthTexture, 0);
         let B = i.get(g.depthTexture).__webglTexture,
-            Y = Me(g);
-        if (g.depthTexture.format === Ci) Le(g) ? l.framebufferTexture2DMultisampleEXT(r.FRAMEBUFFER, r.DEPTH_ATTACHMENT, r.TEXTURE_2D, B, 0, Y) : r.framebufferTexture2D(r.FRAMEBUFFER, r.DEPTH_ATTACHMENT, r.TEXTURE_2D, B, 0);
-        else if (g.depthTexture.format === sr) Le(g) ? l.framebufferTexture2DMultisampleEXT(r.FRAMEBUFFER, r.DEPTH_STENCIL_ATTACHMENT, r.TEXTURE_2D, B, 0, Y) : r.framebufferTexture2D(r.FRAMEBUFFER, r.DEPTH_STENCIL_ATTACHMENT, r.TEXTURE_2D, B, 0);
+            X = Se(g);
+        if (g.depthTexture.format === Ci) Ne(g) ? l.framebufferTexture2DMultisampleEXT(r.FRAMEBUFFER, r.DEPTH_ATTACHMENT, r.TEXTURE_2D, B, 0, X) : r.framebufferTexture2D(r.FRAMEBUFFER, r.DEPTH_ATTACHMENT, r.TEXTURE_2D, B, 0);
+        else if (g.depthTexture.format === sr) Ne(g) ? l.framebufferTexture2DMultisampleEXT(r.FRAMEBUFFER, r.DEPTH_STENCIL_ATTACHMENT, r.TEXTURE_2D, B, 0, X) : r.framebufferTexture2D(r.FRAMEBUFFER, r.DEPTH_STENCIL_ATTACHMENT, r.TEXTURE_2D, B, 0);
         else throw new Error("Unknown depthTexture format")
     }
 
-    function we(S) {
-        let g = i.get(S),
-            B = S.isWebGLCubeRenderTarget === !0;
-        if (S.depthTexture && !g.__autoAllocateDepthBuffer) {
+    function Ae(E) {
+        let g = i.get(E),
+            B = E.isWebGLCubeRenderTarget === !0;
+        if (E.depthTexture && !g.__autoAllocateDepthBuffer) {
             if (B) throw new Error("target.depthTexture not supported in Cube render targets");
-            Xe(g.__webglFramebuffer, S)
+            Xe(g.__webglFramebuffer, E)
         } else if (B) {
             g.__webglDepthbuffer = [];
-            for (let Y = 0; Y < 6; Y++) t.bindFramebuffer(r.FRAMEBUFFER, g.__webglFramebuffer[Y]), g.__webglDepthbuffer[Y] = r.createRenderbuffer(), me(g.__webglDepthbuffer[Y], S, !1)
-        } else t.bindFramebuffer(r.FRAMEBUFFER, g.__webglFramebuffer), g.__webglDepthbuffer = r.createRenderbuffer(), me(g.__webglDepthbuffer, S, !1);
+            for (let X = 0; X < 6; X++) t.bindFramebuffer(r.FRAMEBUFFER, g.__webglFramebuffer[X]), g.__webglDepthbuffer[X] = r.createRenderbuffer(), fe(g.__webglDepthbuffer[X], E, !1)
+        } else t.bindFramebuffer(r.FRAMEBUFFER, g.__webglFramebuffer), g.__webglDepthbuffer = r.createRenderbuffer(), fe(g.__webglDepthbuffer, E, !1);
         t.bindFramebuffer(r.FRAMEBUFFER, null)
     }
 
-    function I(S, g, B) {
-        let Y = i.get(S);
-        g !== void 0 && _e(Y.__webglFramebuffer, S, S.texture, r.COLOR_ATTACHMENT0, r.TEXTURE_2D, 0), B !== void 0 && we(S)
+    function O(E, g, B) {
+        let X = i.get(E);
+        g !== void 0 && _e(X.__webglFramebuffer, E, E.texture, r.COLOR_ATTACHMENT0, r.TEXTURE_2D, 0), B !== void 0 && Ae(E)
     }
 
-    function Qe(S) {
-        let g = S.texture,
-            B = i.get(S),
-            Y = i.get(g);
-        S.addEventListener("dispose", Z);
-        let Q = S.textures,
-            J = S.isWebGLCubeRenderTarget === !0,
-            Ce = Q.length > 1,
-            ye = h(S) || s;
-        if (Ce || (Y.__webglTexture === void 0 && (Y.__webglTexture = r.createTexture()), Y.__version = g.version, o.memory.textures++), J) {
+    function Je(E) {
+        let g = E.texture,
+            B = i.get(E),
+            X = i.get(g);
+        E.addEventListener("dispose", I);
+        let Q = E.textures,
+            J = E.isWebGLCubeRenderTarget === !0,
+            Ee = Q.length > 1,
+            Me = u(E) || s;
+        if (Ee || (X.__webglTexture === void 0 && (X.__webglTexture = r.createTexture()), X.__version = g.version, o.memory.textures++), J) {
             B.__webglFramebuffer = [];
             for (let ae = 0; ae < 6; ae++)
                 if (s && g.mipmaps && g.mipmaps.length > 0) {
                     B.__webglFramebuffer[ae] = [];
                     for (let he = 0; he < g.mipmaps.length; he++) B.__webglFramebuffer[ae][he] = r.createFramebuffer()
                 } else B.__webglFramebuffer[ae] = r.createFramebuffer()
         } else {
             if (s && g.mipmaps && g.mipmaps.length > 0) {
                 B.__webglFramebuffer = [];
                 for (let ae = 0; ae < g.mipmaps.length; ae++) B.__webglFramebuffer[ae] = r.createFramebuffer()
             } else B.__webglFramebuffer = r.createFramebuffer();
-            if (Ce)
+            if (Ee)
                 if (n.drawBuffers)
                     for (let ae = 0, he = Q.length; ae < he; ae++) {
                         let Ie = i.get(Q[ae]);
                         Ie.__webglTexture === void 0 && (Ie.__webglTexture = r.createTexture(), o.memory.textures++)
                     } else console.warn("THREE.WebGLRenderer: WebGLMultipleRenderTargets can only be used with WebGL2 or WEBGL_draw_buffers extension.");
-            if (s && S.samples > 0 && Le(S) === !1) {
+            if (s && E.samples > 0 && Ne(E) === !1) {
                 B.__webglMultisampledFramebuffer = r.createFramebuffer(), B.__webglColorRenderbuffer = [], t.bindFramebuffer(r.FRAMEBUFFER, B.__webglMultisampledFramebuffer);
                 for (let ae = 0; ae < Q.length; ae++) {
                     let he = Q[ae];
                     B.__webglColorRenderbuffer[ae] = r.createRenderbuffer(), r.bindRenderbuffer(r.RENDERBUFFER, B.__webglColorRenderbuffer[ae]);
                     let Ie = a.convert(he.format, he.colorSpace),
                         ne = a.convert(he.type),
-                        Je = U(he.internalFormat, Ie, ne, he.colorSpace, S.isXRRenderTarget === !0),
-                        ze = Me(S);
-                    r.renderbufferStorageMultisample(r.RENDERBUFFER, ze, Je, S.width, S.height), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.COLOR_ATTACHMENT0 + ae, r.RENDERBUFFER, B.__webglColorRenderbuffer[ae])
+                        $e = D(he.internalFormat, Ie, ne, he.colorSpace, E.isXRRenderTarget === !0),
+                        Be = Se(E);
+                    r.renderbufferStorageMultisample(r.RENDERBUFFER, Be, $e, E.width, E.height), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.COLOR_ATTACHMENT0 + ae, r.RENDERBUFFER, B.__webglColorRenderbuffer[ae])
                 }
-                r.bindRenderbuffer(r.RENDERBUFFER, null), S.depthBuffer && (B.__webglDepthRenderbuffer = r.createRenderbuffer(), me(B.__webglDepthRenderbuffer, S, !0)), t.bindFramebuffer(r.FRAMEBUFFER, null)
+                r.bindRenderbuffer(r.RENDERBUFFER, null), E.depthBuffer && (B.__webglDepthRenderbuffer = r.createRenderbuffer(), fe(B.__webglDepthRenderbuffer, E, !0)), t.bindFramebuffer(r.FRAMEBUFFER, null)
             }
         }
         if (J) {
-            t.bindTexture(r.TEXTURE_CUBE_MAP, Y.__webglTexture), H(r.TEXTURE_CUBE_MAP, g, ye);
+            t.bindTexture(r.TEXTURE_CUBE_MAP, X.__webglTexture), V(r.TEXTURE_CUBE_MAP, g, Me);
             for (let ae = 0; ae < 6; ae++)
                 if (s && g.mipmaps && g.mipmaps.length > 0)
-                    for (let he = 0; he < g.mipmaps.length; he++) _e(B.__webglFramebuffer[ae][he], S, g, r.COLOR_ATTACHMENT0, r.TEXTURE_CUBE_MAP_POSITIVE_X + ae, he);
-                else _e(B.__webglFramebuffer[ae], S, g, r.COLOR_ATTACHMENT0, r.TEXTURE_CUBE_MAP_POSITIVE_X + ae, 0);
-            x(g, ye) && R(r.TEXTURE_CUBE_MAP), t.unbindTexture()
-        } else if (Ce) {
+                    for (let he = 0; he < g.mipmaps.length; he++) _e(B.__webglFramebuffer[ae][he], E, g, r.COLOR_ATTACHMENT0, r.TEXTURE_CUBE_MAP_POSITIVE_X + ae, he);
+                else _e(B.__webglFramebuffer[ae], E, g, r.COLOR_ATTACHMENT0, r.TEXTURE_CUBE_MAP_POSITIVE_X + ae, 0);
+            x(g, Me) && A(r.TEXTURE_CUBE_MAP), t.unbindTexture()
+        } else if (Ee) {
             for (let ae = 0, he = Q.length; ae < he; ae++) {
                 let Ie = Q[ae],
                     ne = i.get(Ie);
-                t.bindTexture(r.TEXTURE_2D, ne.__webglTexture), H(r.TEXTURE_2D, Ie, ye), _e(B.__webglFramebuffer, S, Ie, r.COLOR_ATTACHMENT0 + ae, r.TEXTURE_2D, 0), x(Ie, ye) && R(r.TEXTURE_2D)
+                t.bindTexture(r.TEXTURE_2D, ne.__webglTexture), V(r.TEXTURE_2D, Ie, Me), _e(B.__webglFramebuffer, E, Ie, r.COLOR_ATTACHMENT0 + ae, r.TEXTURE_2D, 0), x(Ie, Me) && A(r.TEXTURE_2D)
             }
             t.unbindTexture()
         } else {
             let ae = r.TEXTURE_2D;
-            if ((S.isWebGL3DRenderTarget || S.isWebGLArrayRenderTarget) && (s ? ae = S.isWebGL3DRenderTarget ? r.TEXTURE_3D : r.TEXTURE_2D_ARRAY : console.error("THREE.WebGLTextures: THREE.Data3DTexture and THREE.DataArrayTexture only supported with WebGL2.")), t.bindTexture(ae, Y.__webglTexture), H(ae, g, ye), s && g.mipmaps && g.mipmaps.length > 0)
-                for (let he = 0; he < g.mipmaps.length; he++) _e(B.__webglFramebuffer[he], S, g, r.COLOR_ATTACHMENT0, ae, he);
-            else _e(B.__webglFramebuffer, S, g, r.COLOR_ATTACHMENT0, ae, 0);
-            x(g, ye) && R(ae), t.unbindTexture()
-        }
-        S.depthBuffer && we(S)
+            if ((E.isWebGL3DRenderTarget || E.isWebGLArrayRenderTarget) && (s ? ae = E.isWebGL3DRenderTarget ? r.TEXTURE_3D : r.TEXTURE_2D_ARRAY : console.error("THREE.WebGLTextures: THREE.Data3DTexture and THREE.DataArrayTexture only supported with WebGL2.")), t.bindTexture(ae, X.__webglTexture), V(ae, g, Me), s && g.mipmaps && g.mipmaps.length > 0)
+                for (let he = 0; he < g.mipmaps.length; he++) _e(B.__webglFramebuffer[he], E, g, r.COLOR_ATTACHMENT0, ae, he);
+            else _e(B.__webglFramebuffer, E, g, r.COLOR_ATTACHMENT0, ae, 0);
+            x(g, Me) && A(ae), t.unbindTexture()
+        }
+        E.depthBuffer && Ae(E)
     }
 
-    function ve(S) {
-        let g = h(S) || s,
-            B = S.textures;
-        for (let Y = 0, Q = B.length; Y < Q; Y++) {
-            let J = B[Y];
+    function ve(E) {
+        let g = u(E) || s,
+            B = E.textures;
+        for (let X = 0, Q = B.length; X < Q; X++) {
+            let J = B[X];
             if (x(J, g)) {
-                let Ce = S.isWebGLCubeRenderTarget ? r.TEXTURE_CUBE_MAP : r.TEXTURE_2D,
-                    ye = i.get(J).__webglTexture;
-                t.bindTexture(Ce, ye), R(Ce), t.unbindTexture()
+                let Ee = E.isWebGLCubeRenderTarget ? r.TEXTURE_CUBE_MAP : r.TEXTURE_2D,
+                    Me = i.get(J).__webglTexture;
+                t.bindTexture(Ee, Me), A(Ee), t.unbindTexture()
             }
         }
     }
 
-    function Ue(S) {
-        if (s && S.samples > 0 && Le(S) === !1) {
-            let g = S.textures,
-                B = S.width,
-                Y = S.height,
+    function Pe(E) {
+        if (s && E.samples > 0 && Ne(E) === !1) {
+            let g = E.textures,
+                B = E.width,
+                X = E.height,
                 Q = r.COLOR_BUFFER_BIT,
                 J = [],
-                Ce = S.stencilBuffer ? r.DEPTH_STENCIL_ATTACHMENT : r.DEPTH_ATTACHMENT,
-                ye = i.get(S),
+                Ee = E.stencilBuffer ? r.DEPTH_STENCIL_ATTACHMENT : r.DEPTH_ATTACHMENT,
+                Me = i.get(E),
                 ae = g.length > 1;
             if (ae)
-                for (let he = 0; he < g.length; he++) t.bindFramebuffer(r.FRAMEBUFFER, ye.__webglMultisampledFramebuffer), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.RENDERBUFFER, null), t.bindFramebuffer(r.FRAMEBUFFER, ye.__webglFramebuffer), r.framebufferTexture2D(r.DRAW_FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.TEXTURE_2D, null, 0);
-            t.bindFramebuffer(r.READ_FRAMEBUFFER, ye.__webglMultisampledFramebuffer), t.bindFramebuffer(r.DRAW_FRAMEBUFFER, ye.__webglFramebuffer);
+                for (let he = 0; he < g.length; he++) t.bindFramebuffer(r.FRAMEBUFFER, Me.__webglMultisampledFramebuffer), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.RENDERBUFFER, null), t.bindFramebuffer(r.FRAMEBUFFER, Me.__webglFramebuffer), r.framebufferTexture2D(r.DRAW_FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.TEXTURE_2D, null, 0);
+            t.bindFramebuffer(r.READ_FRAMEBUFFER, Me.__webglMultisampledFramebuffer), t.bindFramebuffer(r.DRAW_FRAMEBUFFER, Me.__webglFramebuffer);
             for (let he = 0; he < g.length; he++) {
-                J.push(r.COLOR_ATTACHMENT0 + he), S.depthBuffer && J.push(Ce);
-                let Ie = ye.__ignoreDepthValues !== void 0 ? ye.__ignoreDepthValues : !1;
-                if (Ie === !1 && (S.depthBuffer && (Q |= r.DEPTH_BUFFER_BIT), S.stencilBuffer && (Q |= r.STENCIL_BUFFER_BIT)), ae && r.framebufferRenderbuffer(r.READ_FRAMEBUFFER, r.COLOR_ATTACHMENT0, r.RENDERBUFFER, ye.__webglColorRenderbuffer[he]), Ie === !0 && (r.invalidateFramebuffer(r.READ_FRAMEBUFFER, [Ce]), r.invalidateFramebuffer(r.DRAW_FRAMEBUFFER, [Ce])), ae) {
+                J.push(r.COLOR_ATTACHMENT0 + he), E.depthBuffer && J.push(Ee);
+                let Ie = Me.__ignoreDepthValues !== void 0 ? Me.__ignoreDepthValues : !1;
+                if (Ie === !1 && (E.depthBuffer && (Q |= r.DEPTH_BUFFER_BIT), E.stencilBuffer && (Q |= r.STENCIL_BUFFER_BIT)), ae && r.framebufferRenderbuffer(r.READ_FRAMEBUFFER, r.COLOR_ATTACHMENT0, r.RENDERBUFFER, Me.__webglColorRenderbuffer[he]), Ie === !0 && (r.invalidateFramebuffer(r.READ_FRAMEBUFFER, [Ee]), r.invalidateFramebuffer(r.DRAW_FRAMEBUFFER, [Ee])), ae) {
                     let ne = i.get(g[he]).__webglTexture;
                     r.framebufferTexture2D(r.DRAW_FRAMEBUFFER, r.COLOR_ATTACHMENT0, r.TEXTURE_2D, ne, 0)
                 }
-                r.blitFramebuffer(0, 0, B, Y, 0, 0, B, Y, Q, r.NEAREST), c && r.invalidateFramebuffer(r.READ_FRAMEBUFFER, J)
+                r.blitFramebuffer(0, 0, B, X, 0, 0, B, X, Q, r.NEAREST), c && r.invalidateFramebuffer(r.READ_FRAMEBUFFER, J)
             }
             if (t.bindFramebuffer(r.READ_FRAMEBUFFER, null), t.bindFramebuffer(r.DRAW_FRAMEBUFFER, null), ae)
                 for (let he = 0; he < g.length; he++) {
-                    t.bindFramebuffer(r.FRAMEBUFFER, ye.__webglMultisampledFramebuffer), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.RENDERBUFFER, ye.__webglColorRenderbuffer[he]);
+                    t.bindFramebuffer(r.FRAMEBUFFER, Me.__webglMultisampledFramebuffer), r.framebufferRenderbuffer(r.FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.RENDERBUFFER, Me.__webglColorRenderbuffer[he]);
                     let Ie = i.get(g[he]).__webglTexture;
-                    t.bindFramebuffer(r.FRAMEBUFFER, ye.__webglFramebuffer), r.framebufferTexture2D(r.DRAW_FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.TEXTURE_2D, Ie, 0)
+                    t.bindFramebuffer(r.FRAMEBUFFER, Me.__webglFramebuffer), r.framebufferTexture2D(r.DRAW_FRAMEBUFFER, r.COLOR_ATTACHMENT0 + he, r.TEXTURE_2D, Ie, 0)
                 }
-            t.bindFramebuffer(r.DRAW_FRAMEBUFFER, ye.__webglMultisampledFramebuffer)
+            t.bindFramebuffer(r.DRAW_FRAMEBUFFER, Me.__webglMultisampledFramebuffer)
         }
     }
 
-    function Me(S) {
-        return Math.min(n.maxSamples, S.samples)
+    function Se(E) {
+        return Math.min(n.maxSamples, E.samples)
     }
 
-    function Le(S) {
-        let g = i.get(S);
-        return s && S.samples > 0 && e.has("WEBGL_multisampled_render_to_texture") === !0 && g.__useRenderToTexture !== !1
+    function Ne(E) {
+        let g = i.get(E);
+        return s && E.samples > 0 && e.has("WEBGL_multisampled_render_to_texture") === !0 && g.__useRenderToTexture !== !1
     }
 
-    function be(S) {
+    function be(E) {
         let g = o.render.frame;
-        p.get(S) !== g && (p.set(S, g), S.update())
+        p.get(E) !== g && (p.set(E, g), E.update())
     }
 
-    function de(S, g) {
-        let B = S.colorSpace,
-            Y = S.format,
-            Q = S.type;
-        return S.isCompressedTexture === !0 || S.isVideoTexture === !0 || S.format === va || B !== fi && B !== oi && (qe.getTransfer(B) === Ze ? s === !1 ? e.has("EXT_sRGB") === !0 && Y === Ot ? (S.format = va, S.minFilter = xt, S.generateMipmaps = !1) : g = ln.sRGBToLinear(g) : (Y !== Ot || Q !== ui) && console.warn("THREE.WebGLTextures: sRGB encoded textures have to use RGBAFormat and UnsignedByteType.") : console.error("THREE.WebGLTextures: Unsupported texture color space:", B)), g
+    function Re(E, g) {
+        let B = E.colorSpace,
+            X = E.format,
+            Q = E.type;
+        return E.isCompressedTexture === !0 || E.isVideoTexture === !0 || E.format === va || B !== fi && B !== oi && (qe.getTransfer(B) === Ze ? s === !1 ? e.has("EXT_sRGB") === !0 && X === Ot ? (E.format = va, E.minFilter = xt, E.generateMipmaps = !1) : g = ln.sRGBToLinear(g) : (X !== Ot || Q !== ui) && console.warn("THREE.WebGLTextures: sRGB encoded textures have to use RGBAFormat and UnsignedByteType.") : console.error("THREE.WebGLTextures: Unsupported texture color space:", B)), g
     }
 
-    function Ne(S) {
-        return typeof HTMLImageElement < "u" && S instanceof HTMLImageElement ? (u.width = S.naturalWidth || S.width, u.height = S.naturalHeight || S.height) : typeof VideoFrame < "u" && S instanceof VideoFrame ? (u.width = S.displayWidth, u.height = S.displayHeight) : (u.width = S.width, u.height = S.height), u
+    function xe(E) {
+        return typeof HTMLImageElement < "u" && E instanceof HTMLImageElement ? (h.width = E.naturalWidth || E.width, h.height = E.naturalHeight || E.height) : typeof VideoFrame < "u" && E instanceof VideoFrame ? (h.width = E.displayWidth, h.height = E.displayHeight) : (h.width = E.width, h.height = E.height), h
     }
-    this.allocateTextureUnit = X, this.resetTextureUnits = P, this.setTexture2D = j, this.setTexture2DArray = q, this.setTexture3D = W, this.setTextureCube = te, this.rebindTextures = I, this.setupRenderTarget = Qe, this.updateRenderTargetMipmap = ve, this.updateMultisampleRenderTarget = Ue, this.setupDepthRenderbuffer = we, this.setupFrameBufferTexture = _e, this.useMultisampledRTT = Le
+    this.allocateTextureUnit = j, this.resetTextureUnits = L, this.setTexture2D = Y, this.setTexture2DArray = q, this.setTexture3D = Z, this.setTextureCube = ee, this.rebindTextures = O, this.setupRenderTarget = Je, this.updateRenderTargetMipmap = ve, this.updateMultisampleRenderTarget = Pe, this.setupDepthRenderbuffer = Ae, this.setupFrameBufferTexture = _e, this.useMultisampledRTT = Ne
 }
 
 function cf(r, e, t) {
     let i = t.isWebGL2;
 
     function n(a, o = oi) {
         let s, l = qe.getTransfer(o);
         if (a === ui) return r.UNSIGNED_BYTE;
-        if (a === No) return r.UNSIGNED_SHORT_4_4_4_4;
-        if (a === Io) return r.UNSIGNED_SHORT_5_5_5_1;
+        if (a === Io) return r.UNSIGNED_SHORT_4_4_4_4;
+        if (a === No) return r.UNSIGNED_SHORT_5_5_5_1;
         if (a === Fl) return r.BYTE;
-        if (a === Bl) return r.SHORT;
+        if (a === zl) return r.SHORT;
         if (a === Va) return r.UNSIGNED_SHORT;
-        if (a === Do) return r.INT;
+        if (a === Uo) return r.INT;
         if (a === li) return r.UNSIGNED_INT;
         if (a === Zt) return r.FLOAT;
         if (a === Mr) return i ? r.HALF_FLOAT : (s = e.get("OES_texture_half_float"), s !== null ? s.HALF_FLOAT_OES : null);
-        if (a === zl) return r.ALPHA;
+        if (a === Bl) return r.ALPHA;
         if (a === Ot) return r.RGBA;
-        if (a === Gl) return r.LUMINANCE;
-        if (a === Hl) return r.LUMINANCE_ALPHA;
+        if (a === Hl) return r.LUMINANCE;
+        if (a === Gl) return r.LUMINANCE_ALPHA;
         if (a === Ci) return r.DEPTH_COMPONENT;
         if (a === sr) return r.DEPTH_STENCIL;
         if (a === va) return s = e.get("EXT_sRGB"), s !== null ? s.SRGB_ALPHA_EXT : null;
         if (a === kl) return r.RED;
         if (a === Oo) return r.RED_INTEGER;
         if (a === Vl) return r.RG;
         if (a === Fo) return r.RG_INTEGER;
-        if (a === Bo) return r.RGBA_INTEGER;
-        if (a === Dn || a === Nn || a === In || a === On)
+        if (a === zo) return r.RGBA_INTEGER;
+        if (a === Un || a === In || a === Nn || a === On)
             if (l === Ze)
                 if (s = e.get("WEBGL_compressed_texture_s3tc_srgb"), s !== null) {
-                    if (a === Dn) return s.COMPRESSED_SRGB_S3TC_DXT1_EXT;
-                    if (a === Nn) return s.COMPRESSED_SRGB_ALPHA_S3TC_DXT1_EXT;
-                    if (a === In) return s.COMPRESSED_SRGB_ALPHA_S3TC_DXT3_EXT;
+                    if (a === Un) return s.COMPRESSED_SRGB_S3TC_DXT1_EXT;
+                    if (a === In) return s.COMPRESSED_SRGB_ALPHA_S3TC_DXT1_EXT;
+                    if (a === Nn) return s.COMPRESSED_SRGB_ALPHA_S3TC_DXT3_EXT;
                     if (a === On) return s.COMPRESSED_SRGB_ALPHA_S3TC_DXT5_EXT
                 } else return null;
         else if (s = e.get("WEBGL_compressed_texture_s3tc"), s !== null) {
-            if (a === Dn) return s.COMPRESSED_RGB_S3TC_DXT1_EXT;
-            if (a === Nn) return s.COMPRESSED_RGBA_S3TC_DXT1_EXT;
-            if (a === In) return s.COMPRESSED_RGBA_S3TC_DXT3_EXT;
+            if (a === Un) return s.COMPRESSED_RGB_S3TC_DXT1_EXT;
+            if (a === In) return s.COMPRESSED_RGBA_S3TC_DXT1_EXT;
+            if (a === Nn) return s.COMPRESSED_RGBA_S3TC_DXT3_EXT;
             if (a === On) return s.COMPRESSED_RGBA_S3TC_DXT5_EXT
         } else return null;
         if (a === ss || a === os || a === ls || a === cs)
             if (s = e.get("WEBGL_compressed_texture_pvrtc"), s !== null) {
                 if (a === ss) return s.COMPRESSED_RGB_PVRTC_4BPPV1_IMG;
                 if (a === os) return s.COMPRESSED_RGB_PVRTC_2BPPV1_IMG;
                 if (a === ls) return s.COMPRESSED_RGBA_PVRTC_4BPPV1_IMG;
                 if (a === cs) return s.COMPRESSED_RGBA_PVRTC_2BPPV1_IMG
             } else return null;
-        if (a === zo) return s = e.get("WEBGL_compressed_texture_etc1"), s !== null ? s.COMPRESSED_RGB_ETC1_WEBGL : null;
+        if (a === Bo) return s = e.get("WEBGL_compressed_texture_etc1"), s !== null ? s.COMPRESSED_RGB_ETC1_WEBGL : null;
         if (a === hs || a === us)
             if (s = e.get("WEBGL_compressed_texture_etc"), s !== null) {
                 if (a === hs) return l === Ze ? s.COMPRESSED_SRGB8_ETC2 : s.COMPRESSED_RGB8_ETC2;
                 if (a === us) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ETC2_EAC : s.COMPRESSED_RGBA8_ETC2_EAC
             } else return null;
-        if (a === ds || a === ps || a === fs || a === ms || a === gs || a === _s || a === vs || a === xs || a === Ms || a === Es || a === Ss || a === ys || a === bs || a === Ts)
+        if (a === ds || a === ps || a === fs || a === ms || a === gs || a === _s || a === vs || a === xs || a === Ms || a === ys || a === Es || a === Ss || a === Ts || a === bs)
             if (s = e.get("WEBGL_compressed_texture_astc"), s !== null) {
                 if (a === ds) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_4x4_KHR : s.COMPRESSED_RGBA_ASTC_4x4_KHR;
                 if (a === ps) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_5x4_KHR : s.COMPRESSED_RGBA_ASTC_5x4_KHR;
                 if (a === fs) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_5x5_KHR : s.COMPRESSED_RGBA_ASTC_5x5_KHR;
                 if (a === ms) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_6x5_KHR : s.COMPRESSED_RGBA_ASTC_6x5_KHR;
                 if (a === gs) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_6x6_KHR : s.COMPRESSED_RGBA_ASTC_6x6_KHR;
                 if (a === _s) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_8x5_KHR : s.COMPRESSED_RGBA_ASTC_8x5_KHR;
                 if (a === vs) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_8x6_KHR : s.COMPRESSED_RGBA_ASTC_8x6_KHR;
                 if (a === xs) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_8x8_KHR : s.COMPRESSED_RGBA_ASTC_8x8_KHR;
                 if (a === Ms) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x5_KHR : s.COMPRESSED_RGBA_ASTC_10x5_KHR;
-                if (a === Es) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x6_KHR : s.COMPRESSED_RGBA_ASTC_10x6_KHR;
-                if (a === Ss) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x8_KHR : s.COMPRESSED_RGBA_ASTC_10x8_KHR;
-                if (a === ys) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x10_KHR : s.COMPRESSED_RGBA_ASTC_10x10_KHR;
-                if (a === bs) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_12x10_KHR : s.COMPRESSED_RGBA_ASTC_12x10_KHR;
-                if (a === Ts) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_12x12_KHR : s.COMPRESSED_RGBA_ASTC_12x12_KHR
+                if (a === ys) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x6_KHR : s.COMPRESSED_RGBA_ASTC_10x6_KHR;
+                if (a === Es) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x8_KHR : s.COMPRESSED_RGBA_ASTC_10x8_KHR;
+                if (a === Ss) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_10x10_KHR : s.COMPRESSED_RGBA_ASTC_10x10_KHR;
+                if (a === Ts) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_12x10_KHR : s.COMPRESSED_RGBA_ASTC_12x10_KHR;
+                if (a === bs) return l === Ze ? s.COMPRESSED_SRGB8_ALPHA8_ASTC_12x12_KHR : s.COMPRESSED_RGBA_ASTC_12x12_KHR
             } else return null;
         if (a === Fn || a === ws || a === As)
             if (s = e.get("EXT_texture_compression_bptc"), s !== null) {
                 if (a === Fn) return l === Ze ? s.COMPRESSED_SRGB_ALPHA_BPTC_UNORM_EXT : s.COMPRESSED_RGBA_BPTC_UNORM_EXT;
                 if (a === ws) return s.COMPRESSED_RGB_BPTC_SIGNED_FLOAT_EXT;
                 if (a === As) return s.COMPRESSED_RGB_BPTC_UNSIGNED_FLOAT_EXT
             } else return null;
@@ -13519,15 +13519,15 @@
             } else return null;
         return a === Ri ? i ? r.UNSIGNED_INT_24_8 : (s = e.get("WEBGL_depth_texture"), s !== null ? s.UNSIGNED_INT_24_8_WEBGL : null) : r[a] !== void 0 ? r[a] : null
     }
     return {
         convert: n
     }
 }
-var Da = class extends Mt {
+var Ua = class extends Mt {
         constructor(e = []) {
             super(), this.isArrayCamera = !0, this.cameras = e
         }
     },
     Qi = class extends wt {
         constructor() {
             super(), this.isGroup = !0, this.type = "Group"
@@ -13542,18 +13542,18 @@
         }
         getHandSpace() {
             return this._hand === null && (this._hand = new Qi, this._hand.matrixAutoUpdate = !1, this._hand.visible = !1, this._hand.joints = {}, this._hand.inputState = {
                 pinching: !1
             }), this._hand
         }
         getTargetRaySpace() {
-            return this._targetRay === null && (this._targetRay = new Qi, this._targetRay.matrixAutoUpdate = !1, this._targetRay.visible = !1, this._targetRay.hasLinearVelocity = !1, this._targetRay.linearVelocity = new D, this._targetRay.hasAngularVelocity = !1, this._targetRay.angularVelocity = new D), this._targetRay
+            return this._targetRay === null && (this._targetRay = new Qi, this._targetRay.matrixAutoUpdate = !1, this._targetRay.visible = !1, this._targetRay.hasLinearVelocity = !1, this._targetRay.linearVelocity = new U, this._targetRay.hasAngularVelocity = !1, this._targetRay.angularVelocity = new U), this._targetRay
         }
         getGripSpace() {
-            return this._grip === null && (this._grip = new Qi, this._grip.matrixAutoUpdate = !1, this._grip.visible = !1, this._grip.hasLinearVelocity = !1, this._grip.linearVelocity = new D, this._grip.hasAngularVelocity = !1, this._grip.angularVelocity = new D), this._grip
+            return this._grip === null && (this._grip = new Qi, this._grip.matrixAutoUpdate = !1, this._grip.visible = !1, this._grip.hasLinearVelocity = !1, this._grip.linearVelocity = new U, this._grip.hasAngularVelocity = !1, this._grip.angularVelocity = new U), this._grip
         }
         dispatchEvent(e) {
             return this._targetRay !== null && this._targetRay.dispatchEvent(e), this._grip !== null && this._grip.dispatchEvent(e), this._hand !== null && this._hand.dispatchEvent(e), this
         }
         connect(e) {
             if (e && e.hand) {
                 let t = this._hand;
@@ -13579,20 +13579,20 @@
                 l = this._grip,
                 c = this._hand;
             if (e && t.session.visibilityState !== "visible-blurred") {
                 if (c && e.hand) {
                     o = !0;
                     for (let M of e.hand.values()) {
                         let d = t.getJointPose(M, i),
-                            h = this._getHandJoint(c, M);
-                        d !== null && (h.matrix.fromArray(d.transform.matrix), h.matrix.decompose(h.position, h.rotation, h.scale), h.matrixWorldNeedsUpdate = !0, h.jointRadius = d.radius), h.visible = d !== null
+                            u = this._getHandJoint(c, M);
+                        d !== null && (u.matrix.fromArray(d.transform.matrix), u.matrix.decompose(u.position, u.rotation, u.scale), u.matrixWorldNeedsUpdate = !0, u.jointRadius = d.radius), u.visible = d !== null
                     }
-                    let u = c.joints["index-finger-tip"],
+                    let h = c.joints["index-finger-tip"],
                         p = c.joints["thumb-tip"],
-                        f = u.position.distanceTo(p.position),
+                        f = h.position.distanceTo(p.position),
                         m = .02,
                         _ = .005;
                     c.inputState.pinching && f > m + _ ? (c.inputState.pinching = !1, this.dispatchEvent({
                         type: "pinchend",
                         handedness: e.handedness,
                         target: this
                     })) : !c.inputState.pinching && f <= m - _ && (c.inputState.pinching = !0, this.dispatchEvent({
@@ -13635,30 +13635,30 @@
 	} else {
 
 		gl_FragDepthEXT = texture( depthColor, vec3( coord.x, coord.y, 0 ) ).r;
 
 	}
 
 }`,
-    Na = class {
+    Ia = class {
         constructor() {
             this.texture = null, this.mesh = null, this.depthNear = 0, this.depthFar = 0
         }
         init(e, t, i) {
             if (this.texture === null) {
                 let n = new Pt,
                     a = e.properties.get(n);
                 a.__webglTexture = t.texture, (t.depthNear != i.depthNear || t.depthFar != i.depthFar) && (this.depthNear = t.depthNear, this.depthFar = t.depthFar), this.texture = n
             }
         }
         render(e, t) {
             if (this.texture !== null) {
                 if (this.mesh === null) {
                     let i = t.cameras[0].viewport,
-                        n = new Gt({
+                        n = new Ht({
                             extensions: {
                                 fragDepth: !0
                             },
                             vertexShader: uf,
                             fragmentShader: df,
                             uniforms: {
                                 depthColor: {
@@ -13677,1070 +13677,1070 @@
                 e.render(this.mesh, t)
             }
         }
         reset() {
             this.texture = null, this.mesh = null
         }
     },
-    Ia = class extends Jt {
+    Na = class extends Jt {
         constructor(e, t) {
             super();
             let i = this,
                 n = null,
                 a = 1,
                 o = null,
                 s = "local-floor",
                 l = 1,
                 c = null,
-                u = null,
+                h = null,
                 p = null,
                 f = null,
                 m = null,
                 _ = null,
-                M = new Na,
+                M = new Ia,
                 d = t.getContextAttributes(),
-                h = null,
-                w = null,
+                u = null,
+                T = null,
                 x = [],
-                R = [],
-                U = new De,
-                A = null,
-                y = new Mt;
-            y.layers.enable(1), y.viewport = new ct;
-            let C = new Mt;
-            C.layers.enable(2), C.viewport = new ct;
-            let Z = [y, C],
-                v = new Da;
+                A = [],
+                D = new Ue,
+                R = null,
+                b = new Mt;
+            b.layers.enable(1), b.viewport = new ct;
+            let P = new Mt;
+            P.layers.enable(2), P.viewport = new ct;
+            let I = [b, P],
+                v = new Ua;
             v.layers.enable(1), v.layers.enable(2);
-            let T = null,
-                V = null;
-            this.cameraAutoUpdate = !0, this.enabled = !1, this.isPresenting = !1, this.getController = function(H) {
-                let ie = x[H];
-                return ie === void 0 && (ie = new xr, x[H] = ie), ie.getTargetRaySpace()
-            }, this.getControllerGrip = function(H) {
-                let ie = x[H];
-                return ie === void 0 && (ie = new xr, x[H] = ie), ie.getGripSpace()
-            }, this.getHand = function(H) {
-                let ie = x[H];
-                return ie === void 0 && (ie = new xr, x[H] = ie), ie.getHandSpace()
+            let w = null,
+                W = null;
+            this.cameraAutoUpdate = !0, this.enabled = !1, this.isPresenting = !1, this.getController = function(V) {
+                let te = x[V];
+                return te === void 0 && (te = new xr, x[V] = te), te.getTargetRaySpace()
+            }, this.getControllerGrip = function(V) {
+                let te = x[V];
+                return te === void 0 && (te = new xr, x[V] = te), te.getGripSpace()
+            }, this.getHand = function(V) {
+                let te = x[V];
+                return te === void 0 && (te = new xr, x[V] = te), te.getHandSpace()
             };
 
-            function K(H) {
-                let ie = R.indexOf(H.inputSource);
-                if (ie === -1) return;
-                let fe = x[ie];
-                fe !== void 0 && (fe.update(H.inputSource, H.frame, c || o), fe.dispatchEvent({
-                    type: H.type,
-                    data: H.inputSource
+            function K(V) {
+                let te = A.indexOf(V.inputSource);
+                if (te === -1) return;
+                let pe = x[te];
+                pe !== void 0 && (pe.update(V.inputSource, V.frame, c || o), pe.dispatchEvent({
+                    type: V.type,
+                    data: V.inputSource
                 }))
             }
 
-            function P() {
-                n.removeEventListener("select", K), n.removeEventListener("selectstart", K), n.removeEventListener("selectend", K), n.removeEventListener("squeeze", K), n.removeEventListener("squeezestart", K), n.removeEventListener("squeezeend", K), n.removeEventListener("end", P), n.removeEventListener("inputsourceschange", X);
-                for (let H = 0; H < x.length; H++) {
-                    let ie = R[H];
-                    ie !== null && (R[H] = null, x[H].disconnect(ie))
+            function L() {
+                n.removeEventListener("select", K), n.removeEventListener("selectstart", K), n.removeEventListener("selectend", K), n.removeEventListener("squeeze", K), n.removeEventListener("squeezestart", K), n.removeEventListener("squeezeend", K), n.removeEventListener("end", L), n.removeEventListener("inputsourceschange", j);
+                for (let V = 0; V < x.length; V++) {
+                    let te = A[V];
+                    te !== null && (A[V] = null, x[V].disconnect(te))
                 }
-                T = null, V = null, M.reset(), e.setRenderTarget(h), m = null, f = null, p = null, n = null, w = null, xe.stop(), i.isPresenting = !1, e.setPixelRatio(A), e.setSize(U.width, U.height, !1), i.dispatchEvent({
+                w = null, W = null, M.reset(), e.setRenderTarget(u), m = null, f = null, p = null, n = null, T = null, ge.stop(), i.isPresenting = !1, e.setPixelRatio(R), e.setSize(D.width, D.height, !1), i.dispatchEvent({
                     type: "sessionend"
                 })
             }
-            this.setFramebufferScaleFactor = function(H) {
-                a = H, i.isPresenting === !0 && console.warn("THREE.WebXRManager: Cannot change framebuffer scale while presenting.")
-            }, this.setReferenceSpaceType = function(H) {
-                s = H, i.isPresenting === !0 && console.warn("THREE.WebXRManager: Cannot change reference space type while presenting.")
+            this.setFramebufferScaleFactor = function(V) {
+                a = V, i.isPresenting === !0 && console.warn("THREE.WebXRManager: Cannot change framebuffer scale while presenting.")
+            }, this.setReferenceSpaceType = function(V) {
+                s = V, i.isPresenting === !0 && console.warn("THREE.WebXRManager: Cannot change reference space type while presenting.")
             }, this.getReferenceSpace = function() {
                 return c || o
-            }, this.setReferenceSpace = function(H) {
-                c = H
+            }, this.setReferenceSpace = function(V) {
+                c = V
             }, this.getBaseLayer = function() {
                 return f !== null ? f : m
             }, this.getBinding = function() {
                 return p
             }, this.getFrame = function() {
                 return _
             }, this.getSession = function() {
                 return n
-            }, this.setSession = async function(H) {
-                if (n = H, n !== null) {
-                    if (h = e.getRenderTarget(), n.addEventListener("select", K), n.addEventListener("selectstart", K), n.addEventListener("selectend", K), n.addEventListener("squeeze", K), n.addEventListener("squeezestart", K), n.addEventListener("squeezeend", K), n.addEventListener("end", P), n.addEventListener("inputsourceschange", X), d.xrCompatible !== !0 && await t.makeXRCompatible(), A = e.getPixelRatio(), e.getSize(U), n.renderState.layers === void 0 || e.capabilities.isWebGL2 === !1) {
-                        let ie = {
+            }, this.setSession = async function(V) {
+                if (n = V, n !== null) {
+                    if (u = e.getRenderTarget(), n.addEventListener("select", K), n.addEventListener("selectstart", K), n.addEventListener("selectend", K), n.addEventListener("squeeze", K), n.addEventListener("squeezestart", K), n.addEventListener("squeezeend", K), n.addEventListener("end", L), n.addEventListener("inputsourceschange", j), d.xrCompatible !== !0 && await t.makeXRCompatible(), R = e.getPixelRatio(), e.getSize(D), n.renderState.layers === void 0 || e.capabilities.isWebGL2 === !1) {
+                        let te = {
                             antialias: n.renderState.layers === void 0 ? d.antialias : !0,
                             alpha: !0,
                             depth: d.depth,
                             stencil: d.stencil,
                             framebufferScaleFactor: a
                         };
-                        m = new XRWebGLLayer(n, t, ie), n.updateRenderState({
+                        m = new XRWebGLLayer(n, t, te), n.updateRenderState({
                             baseLayer: m
-                        }), e.setPixelRatio(1), e.setSize(m.framebufferWidth, m.framebufferHeight, !1), w = new $t(m.framebufferWidth, m.framebufferHeight, {
+                        }), e.setPixelRatio(1), e.setSize(m.framebufferWidth, m.framebufferHeight, !1), T = new $t(m.framebufferWidth, m.framebufferHeight, {
                             format: Ot,
                             type: ui,
                             colorSpace: e.outputColorSpace,
                             stencilBuffer: d.stencil
                         })
                     } else {
-                        let ie = null,
-                            fe = null,
-                            Te = null;
-                        d.depth && (Te = d.stencil ? t.DEPTH24_STENCIL8 : t.DEPTH_COMPONENT24, ie = d.stencil ? sr : Ci, fe = d.stencil ? Ri : li);
+                        let te = null,
+                            pe = null,
+                            we = null;
+                        d.depth && (we = d.stencil ? t.DEPTH24_STENCIL8 : t.DEPTH_COMPONENT24, te = d.stencil ? sr : Ci, pe = d.stencil ? Ri : li);
                         let _e = {
                             colorFormat: t.RGBA8,
-                            depthFormat: Te,
+                            depthFormat: we,
                             scaleFactor: a
                         };
                         p = new XRWebGLBinding(n, t), f = p.createProjectionLayer(_e), n.updateRenderState({
                             layers: [f]
-                        }), e.setPixelRatio(1), e.setSize(f.textureWidth, f.textureHeight, !1), w = new $t(f.textureWidth, f.textureHeight, {
+                        }), e.setPixelRatio(1), e.setSize(f.textureWidth, f.textureHeight, !1), T = new $t(f.textureWidth, f.textureHeight, {
                             format: Ot,
                             type: ui,
-                            depthTexture: new xn(f.textureWidth, f.textureHeight, fe, void 0, void 0, void 0, void 0, void 0, void 0, ie),
+                            depthTexture: new xn(f.textureWidth, f.textureHeight, pe, void 0, void 0, void 0, void 0, void 0, void 0, te),
                             stencilBuffer: d.stencil,
                             colorSpace: e.outputColorSpace,
                             samples: d.antialias ? 4 : 0
                         });
-                        let me = e.properties.get(w);
-                        me.__ignoreDepthValues = f.ignoreDepthValues
+                        let fe = e.properties.get(T);
+                        fe.__ignoreDepthValues = f.ignoreDepthValues
                     }
-                    w.isXRRenderTarget = !0, this.setFoveation(l), c = null, o = await n.requestReferenceSpace(s), xe.setContext(n), xe.start(), i.isPresenting = !0, i.dispatchEvent({
+                    T.isXRRenderTarget = !0, this.setFoveation(l), c = null, o = await n.requestReferenceSpace(s), ge.setContext(n), ge.start(), i.isPresenting = !0, i.dispatchEvent({
                         type: "sessionstart"
                     })
                 }
             }, this.getEnvironmentBlendMode = function() {
                 if (n !== null) return n.environmentBlendMode
             };
 
-            function X(H) {
-                for (let ie = 0; ie < H.removed.length; ie++) {
-                    let fe = H.removed[ie],
-                        Te = R.indexOf(fe);
-                    Te >= 0 && (R[Te] = null, x[Te].disconnect(fe))
-                }
-                for (let ie = 0; ie < H.added.length; ie++) {
-                    let fe = H.added[ie],
-                        Te = R.indexOf(fe);
-                    if (Te === -1) {
-                        for (let me = 0; me < x.length; me++)
-                            if (me >= R.length) {
-                                R.push(fe), Te = me;
+            function j(V) {
+                for (let te = 0; te < V.removed.length; te++) {
+                    let pe = V.removed[te],
+                        we = A.indexOf(pe);
+                    we >= 0 && (A[we] = null, x[we].disconnect(pe))
+                }
+                for (let te = 0; te < V.added.length; te++) {
+                    let pe = V.added[te],
+                        we = A.indexOf(pe);
+                    if (we === -1) {
+                        for (let fe = 0; fe < x.length; fe++)
+                            if (fe >= A.length) {
+                                A.push(pe), we = fe;
                                 break
-                            } else if (R[me] === null) {
-                            R[me] = fe, Te = me;
+                            } else if (A[fe] === null) {
+                            A[fe] = pe, we = fe;
                             break
                         }
-                        if (Te === -1) break
+                        if (we === -1) break
                     }
-                    let _e = x[Te];
-                    _e && _e.connect(fe)
+                    let _e = x[we];
+                    _e && _e.connect(pe)
                 }
             }
-            let k = new D,
-                j = new D;
+            let k = new U,
+                Y = new U;
 
-            function q(H, ie, fe) {
-                k.setFromMatrixPosition(ie.matrixWorld), j.setFromMatrixPosition(fe.matrixWorld);
-                let Te = k.distanceTo(j),
-                    _e = ie.projectionMatrix.elements,
-                    me = fe.projectionMatrix.elements,
+            function q(V, te, pe) {
+                k.setFromMatrixPosition(te.matrixWorld), Y.setFromMatrixPosition(pe.matrixWorld);
+                let we = k.distanceTo(Y),
+                    _e = te.projectionMatrix.elements,
+                    fe = pe.projectionMatrix.elements,
                     Xe = _e[14] / (_e[10] - 1),
-                    we = _e[14] / (_e[10] + 1),
-                    I = (_e[9] + 1) / _e[5],
-                    Qe = (_e[9] - 1) / _e[5],
+                    Ae = _e[14] / (_e[10] + 1),
+                    O = (_e[9] + 1) / _e[5],
+                    Je = (_e[9] - 1) / _e[5],
                     ve = (_e[8] - 1) / _e[0],
-                    Ue = (me[8] + 1) / me[0],
-                    Me = Xe * ve,
-                    Le = Xe * Ue,
-                    be = Te / (-ve + Ue),
-                    de = be * -ve;
-                ie.matrixWorld.decompose(H.position, H.quaternion, H.scale), H.translateX(de), H.translateZ(be), H.matrixWorld.compose(H.position, H.quaternion, H.scale), H.matrixWorldInverse.copy(H.matrixWorld).invert();
-                let Ne = Xe + be,
-                    S = we + be,
-                    g = Me - de,
-                    B = Le + (Te - de),
-                    Y = I * we / S * Ne,
-                    Q = Qe * we / S * Ne;
-                H.projectionMatrix.makePerspective(g, B, Y, Q, Ne, S), H.projectionMatrixInverse.copy(H.projectionMatrix).invert()
+                    Pe = (fe[8] + 1) / fe[0],
+                    Se = Xe * ve,
+                    Ne = Xe * Pe,
+                    be = we / (-ve + Pe),
+                    Re = be * -ve;
+                te.matrixWorld.decompose(V.position, V.quaternion, V.scale), V.translateX(Re), V.translateZ(be), V.matrixWorld.compose(V.position, V.quaternion, V.scale), V.matrixWorldInverse.copy(V.matrixWorld).invert();
+                let xe = Xe + be,
+                    E = Ae + be,
+                    g = Se - Re,
+                    B = Ne + (we - Re),
+                    X = O * Ae / E * xe,
+                    Q = Je * Ae / E * xe;
+                V.projectionMatrix.makePerspective(g, B, X, Q, xe, E), V.projectionMatrixInverse.copy(V.projectionMatrix).invert()
             }
 
-            function W(H, ie) {
-                ie === null ? H.matrixWorld.copy(H.matrix) : H.matrixWorld.multiplyMatrices(ie.matrixWorld, H.matrix), H.matrixWorldInverse.copy(H.matrixWorld).invert()
+            function Z(V, te) {
+                te === null ? V.matrixWorld.copy(V.matrix) : V.matrixWorld.multiplyMatrices(te.matrixWorld, V.matrix), V.matrixWorldInverse.copy(V.matrixWorld).invert()
             }
-            this.updateCamera = function(H) {
+            this.updateCamera = function(V) {
                 if (n === null) return;
-                M.texture !== null && (H.near = M.depthNear, H.far = M.depthFar), v.near = C.near = y.near = H.near, v.far = C.far = y.far = H.far, (T !== v.near || V !== v.far) && (n.updateRenderState({
+                M.texture !== null && (V.near = M.depthNear, V.far = M.depthFar), v.near = P.near = b.near = V.near, v.far = P.far = b.far = V.far, (w !== v.near || W !== v.far) && (n.updateRenderState({
                     depthNear: v.near,
                     depthFar: v.far
-                }), T = v.near, V = v.far, y.near = T, y.far = V, C.near = T, C.far = V, y.updateProjectionMatrix(), C.updateProjectionMatrix(), H.updateProjectionMatrix());
-                let ie = H.parent,
-                    fe = v.cameras;
-                W(v, ie);
-                for (let Te = 0; Te < fe.length; Te++) W(fe[Te], ie);
-                fe.length === 2 ? q(v, y, C) : v.projectionMatrix.copy(y.projectionMatrix), te(H, v, ie)
+                }), w = v.near, W = v.far, b.near = w, b.far = W, P.near = w, P.far = W, b.updateProjectionMatrix(), P.updateProjectionMatrix(), V.updateProjectionMatrix());
+                let te = V.parent,
+                    pe = v.cameras;
+                Z(v, te);
+                for (let we = 0; we < pe.length; we++) Z(pe[we], te);
+                pe.length === 2 ? q(v, b, P) : v.projectionMatrix.copy(b.projectionMatrix), ee(V, v, te)
             };
 
-            function te(H, ie, fe) {
-                fe === null ? H.matrix.copy(ie.matrixWorld) : (H.matrix.copy(fe.matrixWorld), H.matrix.invert(), H.matrix.multiply(ie.matrixWorld)), H.matrix.decompose(H.position, H.quaternion, H.scale), H.updateMatrixWorld(!0), H.projectionMatrix.copy(ie.projectionMatrix), H.projectionMatrixInverse.copy(ie.projectionMatrixInverse), H.isPerspectiveCamera && (H.fov = Er * 2 * Math.atan(1 / H.projectionMatrix.elements[5]), H.zoom = 1)
+            function ee(V, te, pe) {
+                pe === null ? V.matrix.copy(te.matrixWorld) : (V.matrix.copy(pe.matrixWorld), V.matrix.invert(), V.matrix.multiply(te.matrixWorld)), V.matrix.decompose(V.position, V.quaternion, V.scale), V.updateMatrixWorld(!0), V.projectionMatrix.copy(te.projectionMatrix), V.projectionMatrixInverse.copy(te.projectionMatrixInverse), V.isPerspectiveCamera && (V.fov = yr * 2 * Math.atan(1 / V.projectionMatrix.elements[5]), V.zoom = 1)
             }
             this.getCamera = function() {
                 return v
             }, this.getFoveation = function() {
                 if (!(f === null && m === null)) return l
-            }, this.setFoveation = function(H) {
-                l = H, f !== null && (f.fixedFoveation = H), m !== null && m.fixedFoveation !== void 0 && (m.fixedFoveation = H)
+            }, this.setFoveation = function(V) {
+                l = V, f !== null && (f.fixedFoveation = V), m !== null && m.fixedFoveation !== void 0 && (m.fixedFoveation = V)
             }, this.hasDepthSensing = function() {
                 return M.texture !== null
             };
-            let ee = null;
+            let ie = null;
 
-            function pe(H, ie) {
-                if (u = ie.getViewerPose(c || o), _ = ie, u !== null) {
-                    let fe = u.views;
-                    m !== null && (e.setRenderTargetFramebuffer(w, m.framebuffer), e.setRenderTarget(w));
-                    let Te = !1;
-                    fe.length !== v.cameras.length && (v.cameras.length = 0, Te = !0);
-                    for (let me = 0; me < fe.length; me++) {
-                        let Xe = fe[me],
-                            we = null;
-                        if (m !== null) we = m.getViewport(Xe);
+            function de(V, te) {
+                if (h = te.getViewerPose(c || o), _ = te, h !== null) {
+                    let pe = h.views;
+                    m !== null && (e.setRenderTargetFramebuffer(T, m.framebuffer), e.setRenderTarget(T));
+                    let we = !1;
+                    pe.length !== v.cameras.length && (v.cameras.length = 0, we = !0);
+                    for (let fe = 0; fe < pe.length; fe++) {
+                        let Xe = pe[fe],
+                            Ae = null;
+                        if (m !== null) Ae = m.getViewport(Xe);
                         else {
-                            let Qe = p.getViewSubImage(f, Xe);
-                            we = Qe.viewport, me === 0 && (e.setRenderTargetTextures(w, Qe.colorTexture, f.ignoreDepthValues ? void 0 : Qe.depthStencilTexture), e.setRenderTarget(w))
+                            let Je = p.getViewSubImage(f, Xe);
+                            Ae = Je.viewport, fe === 0 && (e.setRenderTargetTextures(T, Je.colorTexture, f.ignoreDepthValues ? void 0 : Je.depthStencilTexture), e.setRenderTarget(T))
                         }
-                        let I = Z[me];
-                        I === void 0 && (I = new Mt, I.layers.enable(me), I.viewport = new ct, Z[me] = I), I.matrix.fromArray(Xe.transform.matrix), I.matrix.decompose(I.position, I.quaternion, I.scale), I.projectionMatrix.fromArray(Xe.projectionMatrix), I.projectionMatrixInverse.copy(I.projectionMatrix).invert(), I.viewport.set(we.x, we.y, we.width, we.height), me === 0 && (v.matrix.copy(I.matrix), v.matrix.decompose(v.position, v.quaternion, v.scale)), Te === !0 && v.cameras.push(I)
+                        let O = I[fe];
+                        O === void 0 && (O = new Mt, O.layers.enable(fe), O.viewport = new ct, I[fe] = O), O.matrix.fromArray(Xe.transform.matrix), O.matrix.decompose(O.position, O.quaternion, O.scale), O.projectionMatrix.fromArray(Xe.projectionMatrix), O.projectionMatrixInverse.copy(O.projectionMatrix).invert(), O.viewport.set(Ae.x, Ae.y, Ae.width, Ae.height), fe === 0 && (v.matrix.copy(O.matrix), v.matrix.decompose(v.position, v.quaternion, v.scale)), we === !0 && v.cameras.push(O)
                     }
                     let _e = n.enabledFeatures;
                     if (_e && _e.includes("depth-sensing")) {
-                        let me = p.getDepthInformation(fe[0]);
-                        me && me.isValid && me.texture && M.init(e, me, n.renderState)
+                        let fe = p.getDepthInformation(pe[0]);
+                        fe && fe.isValid && fe.texture && M.init(e, fe, n.renderState)
                     }
                 }
-                for (let fe = 0; fe < x.length; fe++) {
-                    let Te = R[fe],
-                        _e = x[fe];
-                    Te !== null && _e !== void 0 && _e.update(Te, ie, c || o)
+                for (let pe = 0; pe < x.length; pe++) {
+                    let we = A[pe],
+                        _e = x[pe];
+                    we !== null && _e !== void 0 && _e.update(we, te, c || o)
                 }
-                M.render(e, v), ee && ee(H, ie), ie.detectedPlanes && i.dispatchEvent({
+                M.render(e, v), ie && ie(V, te), te.detectedPlanes && i.dispatchEvent({
                     type: "planesdetected",
-                    data: ie
+                    data: te
                 }), _ = null
             }
-            let xe = new Wo;
-            xe.setAnimationLoop(pe), this.setAnimationLoop = function(H) {
-                ee = H
+            let ge = new Wo;
+            ge.setAnimationLoop(de), this.setAnimationLoop = function(V) {
+                ie = V
             }, this.dispose = function() {}
         }
     },
-    Si = new ei,
+    Ei = new ei,
     pf = new at;
 
 function ff(r, e) {
-    function t(d, h) {
-        d.matrixAutoUpdate === !0 && d.updateMatrix(), h.value.copy(d.matrix)
+    function t(d, u) {
+        d.matrixAutoUpdate === !0 && d.updateMatrix(), u.value.copy(d.matrix)
     }
 
-    function i(d, h) {
-        h.color.getRGB(d.fogColor.value, Vo(r)), h.isFog ? (d.fogNear.value = h.near, d.fogFar.value = h.far) : h.isFogExp2 && (d.fogDensity.value = h.density)
+    function i(d, u) {
+        u.color.getRGB(d.fogColor.value, Vo(r)), u.isFog ? (d.fogNear.value = u.near, d.fogFar.value = u.far) : u.isFogExp2 && (d.fogDensity.value = u.density)
     }
 
-    function n(d, h, w, x, R) {
-        h.isMeshBasicMaterial || h.isMeshLambertMaterial ? a(d, h) : h.isMeshToonMaterial ? (a(d, h), p(d, h)) : h.isMeshPhongMaterial ? (a(d, h), u(d, h)) : h.isMeshStandardMaterial ? (a(d, h), f(d, h), h.isMeshPhysicalMaterial && m(d, h, R)) : h.isMeshMatcapMaterial ? (a(d, h), _(d, h)) : h.isMeshDepthMaterial ? a(d, h) : h.isMeshDistanceMaterial ? (a(d, h), M(d, h)) : h.isMeshNormalMaterial ? a(d, h) : h.isLineBasicMaterial ? (o(d, h), h.isLineDashedMaterial && s(d, h)) : h.isPointsMaterial ? l(d, h, w, x) : h.isSpriteMaterial ? c(d, h) : h.isShadowMaterial ? (d.color.value.copy(h.color), d.opacity.value = h.opacity) : h.isShaderMaterial && (h.uniformsNeedUpdate = !1)
+    function n(d, u, T, x, A) {
+        u.isMeshBasicMaterial || u.isMeshLambertMaterial ? a(d, u) : u.isMeshToonMaterial ? (a(d, u), p(d, u)) : u.isMeshPhongMaterial ? (a(d, u), h(d, u)) : u.isMeshStandardMaterial ? (a(d, u), f(d, u), u.isMeshPhysicalMaterial && m(d, u, A)) : u.isMeshMatcapMaterial ? (a(d, u), _(d, u)) : u.isMeshDepthMaterial ? a(d, u) : u.isMeshDistanceMaterial ? (a(d, u), M(d, u)) : u.isMeshNormalMaterial ? a(d, u) : u.isLineBasicMaterial ? (o(d, u), u.isLineDashedMaterial && s(d, u)) : u.isPointsMaterial ? l(d, u, T, x) : u.isSpriteMaterial ? c(d, u) : u.isShadowMaterial ? (d.color.value.copy(u.color), d.opacity.value = u.opacity) : u.isShaderMaterial && (u.uniformsNeedUpdate = !1)
     }
 
-    function a(d, h) {
-        d.opacity.value = h.opacity, h.color && d.diffuse.value.copy(h.color), h.emissive && d.emissive.value.copy(h.emissive).multiplyScalar(h.emissiveIntensity), h.map && (d.map.value = h.map, t(h.map, d.mapTransform)), h.alphaMap && (d.alphaMap.value = h.alphaMap, t(h.alphaMap, d.alphaMapTransform)), h.bumpMap && (d.bumpMap.value = h.bumpMap, t(h.bumpMap, d.bumpMapTransform), d.bumpScale.value = h.bumpScale, h.side === Et && (d.bumpScale.value *= -1)), h.normalMap && (d.normalMap.value = h.normalMap, t(h.normalMap, d.normalMapTransform), d.normalScale.value.copy(h.normalScale), h.side === Et && d.normalScale.value.negate()), h.displacementMap && (d.displacementMap.value = h.displacementMap, t(h.displacementMap, d.displacementMapTransform), d.displacementScale.value = h.displacementScale, d.displacementBias.value = h.displacementBias), h.emissiveMap && (d.emissiveMap.value = h.emissiveMap, t(h.emissiveMap, d.emissiveMapTransform)), h.specularMap && (d.specularMap.value = h.specularMap, t(h.specularMap, d.specularMapTransform)), h.alphaTest > 0 && (d.alphaTest.value = h.alphaTest);
-        let w = e.get(h),
-            x = w.envMap,
-            R = w.envMapRotation;
-        if (x && (d.envMap.value = x, Si.copy(R), Si.x *= -1, Si.y *= -1, Si.z *= -1, x.isCubeTexture && x.isRenderTargetTexture === !1 && (Si.y *= -1, Si.z *= -1), d.envMapRotation.value.setFromMatrix4(pf.makeRotationFromEuler(Si)), d.flipEnvMap.value = x.isCubeTexture && x.isRenderTargetTexture === !1 ? -1 : 1, d.reflectivity.value = h.reflectivity, d.ior.value = h.ior, d.refractionRatio.value = h.refractionRatio), h.lightMap) {
-            d.lightMap.value = h.lightMap;
-            let U = r._useLegacyLights === !0 ? Math.PI : 1;
-            d.lightMapIntensity.value = h.lightMapIntensity * U, t(h.lightMap, d.lightMapTransform)
+    function a(d, u) {
+        d.opacity.value = u.opacity, u.color && d.diffuse.value.copy(u.color), u.emissive && d.emissive.value.copy(u.emissive).multiplyScalar(u.emissiveIntensity), u.map && (d.map.value = u.map, t(u.map, d.mapTransform)), u.alphaMap && (d.alphaMap.value = u.alphaMap, t(u.alphaMap, d.alphaMapTransform)), u.bumpMap && (d.bumpMap.value = u.bumpMap, t(u.bumpMap, d.bumpMapTransform), d.bumpScale.value = u.bumpScale, u.side === yt && (d.bumpScale.value *= -1)), u.normalMap && (d.normalMap.value = u.normalMap, t(u.normalMap, d.normalMapTransform), d.normalScale.value.copy(u.normalScale), u.side === yt && d.normalScale.value.negate()), u.displacementMap && (d.displacementMap.value = u.displacementMap, t(u.displacementMap, d.displacementMapTransform), d.displacementScale.value = u.displacementScale, d.displacementBias.value = u.displacementBias), u.emissiveMap && (d.emissiveMap.value = u.emissiveMap, t(u.emissiveMap, d.emissiveMapTransform)), u.specularMap && (d.specularMap.value = u.specularMap, t(u.specularMap, d.specularMapTransform)), u.alphaTest > 0 && (d.alphaTest.value = u.alphaTest);
+        let T = e.get(u),
+            x = T.envMap,
+            A = T.envMapRotation;
+        if (x && (d.envMap.value = x, Ei.copy(A), Ei.x *= -1, Ei.y *= -1, Ei.z *= -1, x.isCubeTexture && x.isRenderTargetTexture === !1 && (Ei.y *= -1, Ei.z *= -1), d.envMapRotation.value.setFromMatrix4(pf.makeRotationFromEuler(Ei)), d.flipEnvMap.value = x.isCubeTexture && x.isRenderTargetTexture === !1 ? -1 : 1, d.reflectivity.value = u.reflectivity, d.ior.value = u.ior, d.refractionRatio.value = u.refractionRatio), u.lightMap) {
+            d.lightMap.value = u.lightMap;
+            let D = r._useLegacyLights === !0 ? Math.PI : 1;
+            d.lightMapIntensity.value = u.lightMapIntensity * D, t(u.lightMap, d.lightMapTransform)
         }
-        h.aoMap && (d.aoMap.value = h.aoMap, d.aoMapIntensity.value = h.aoMapIntensity, t(h.aoMap, d.aoMapTransform))
+        u.aoMap && (d.aoMap.value = u.aoMap, d.aoMapIntensity.value = u.aoMapIntensity, t(u.aoMap, d.aoMapTransform))
     }
 
-    function o(d, h) {
-        d.diffuse.value.copy(h.color), d.opacity.value = h.opacity, h.map && (d.map.value = h.map, t(h.map, d.mapTransform))
+    function o(d, u) {
+        d.diffuse.value.copy(u.color), d.opacity.value = u.opacity, u.map && (d.map.value = u.map, t(u.map, d.mapTransform))
     }
 
-    function s(d, h) {
-        d.dashSize.value = h.dashSize, d.totalSize.value = h.dashSize + h.gapSize, d.scale.value = h.scale
+    function s(d, u) {
+        d.dashSize.value = u.dashSize, d.totalSize.value = u.dashSize + u.gapSize, d.scale.value = u.scale
     }
 
-    function l(d, h, w, x) {
-        d.diffuse.value.copy(h.color), d.opacity.value = h.opacity, d.size.value = h.size * w, d.scale.value = x * .5, h.map && (d.map.value = h.map, t(h.map, d.uvTransform)), h.alphaMap && (d.alphaMap.value = h.alphaMap, t(h.alphaMap, d.alphaMapTransform)), h.alphaTest > 0 && (d.alphaTest.value = h.alphaTest)
+    function l(d, u, T, x) {
+        d.diffuse.value.copy(u.color), d.opacity.value = u.opacity, d.size.value = u.size * T, d.scale.value = x * .5, u.map && (d.map.value = u.map, t(u.map, d.uvTransform)), u.alphaMap && (d.alphaMap.value = u.alphaMap, t(u.alphaMap, d.alphaMapTransform)), u.alphaTest > 0 && (d.alphaTest.value = u.alphaTest)
     }
 
-    function c(d, h) {
-        d.diffuse.value.copy(h.color), d.opacity.value = h.opacity, d.rotation.value = h.rotation, h.map && (d.map.value = h.map, t(h.map, d.mapTransform)), h.alphaMap && (d.alphaMap.value = h.alphaMap, t(h.alphaMap, d.alphaMapTransform)), h.alphaTest > 0 && (d.alphaTest.value = h.alphaTest)
+    function c(d, u) {
+        d.diffuse.value.copy(u.color), d.opacity.value = u.opacity, d.rotation.value = u.rotation, u.map && (d.map.value = u.map, t(u.map, d.mapTransform)), u.alphaMap && (d.alphaMap.value = u.alphaMap, t(u.alphaMap, d.alphaMapTransform)), u.alphaTest > 0 && (d.alphaTest.value = u.alphaTest)
     }
 
-    function u(d, h) {
-        d.specular.value.copy(h.specular), d.shininess.value = Math.max(h.shininess, 1e-4)
+    function h(d, u) {
+        d.specular.value.copy(u.specular), d.shininess.value = Math.max(u.shininess, 1e-4)
     }
 
-    function p(d, h) {
-        h.gradientMap && (d.gradientMap.value = h.gradientMap)
+    function p(d, u) {
+        u.gradientMap && (d.gradientMap.value = u.gradientMap)
     }
 
-    function f(d, h) {
-        d.metalness.value = h.metalness, h.metalnessMap && (d.metalnessMap.value = h.metalnessMap, t(h.metalnessMap, d.metalnessMapTransform)), d.roughness.value = h.roughness, h.roughnessMap && (d.roughnessMap.value = h.roughnessMap, t(h.roughnessMap, d.roughnessMapTransform)), e.get(h).envMap && (d.envMapIntensity.value = h.envMapIntensity)
+    function f(d, u) {
+        d.metalness.value = u.metalness, u.metalnessMap && (d.metalnessMap.value = u.metalnessMap, t(u.metalnessMap, d.metalnessMapTransform)), d.roughness.value = u.roughness, u.roughnessMap && (d.roughnessMap.value = u.roughnessMap, t(u.roughnessMap, d.roughnessMapTransform)), e.get(u).envMap && (d.envMapIntensity.value = u.envMapIntensity)
     }
 
-    function m(d, h, w) {
-        d.ior.value = h.ior, h.sheen > 0 && (d.sheenColor.value.copy(h.sheenColor).multiplyScalar(h.sheen), d.sheenRoughness.value = h.sheenRoughness, h.sheenColorMap && (d.sheenColorMap.value = h.sheenColorMap, t(h.sheenColorMap, d.sheenColorMapTransform)), h.sheenRoughnessMap && (d.sheenRoughnessMap.value = h.sheenRoughnessMap, t(h.sheenRoughnessMap, d.sheenRoughnessMapTransform))), h.clearcoat > 0 && (d.clearcoat.value = h.clearcoat, d.clearcoatRoughness.value = h.clearcoatRoughness, h.clearcoatMap && (d.clearcoatMap.value = h.clearcoatMap, t(h.clearcoatMap, d.clearcoatMapTransform)), h.clearcoatRoughnessMap && (d.clearcoatRoughnessMap.value = h.clearcoatRoughnessMap, t(h.clearcoatRoughnessMap, d.clearcoatRoughnessMapTransform)), h.clearcoatNormalMap && (d.clearcoatNormalMap.value = h.clearcoatNormalMap, t(h.clearcoatNormalMap, d.clearcoatNormalMapTransform), d.clearcoatNormalScale.value.copy(h.clearcoatNormalScale), h.side === Et && d.clearcoatNormalScale.value.negate())), h.iridescence > 0 && (d.iridescence.value = h.iridescence, d.iridescenceIOR.value = h.iridescenceIOR, d.iridescenceThicknessMinimum.value = h.iridescenceThicknessRange[0], d.iridescenceThicknessMaximum.value = h.iridescenceThicknessRange[1], h.iridescenceMap && (d.iridescenceMap.value = h.iridescenceMap, t(h.iridescenceMap, d.iridescenceMapTransform)), h.iridescenceThicknessMap && (d.iridescenceThicknessMap.value = h.iridescenceThicknessMap, t(h.iridescenceThicknessMap, d.iridescenceThicknessMapTransform))), h.transmission > 0 && (d.transmission.value = h.transmission, d.transmissionSamplerMap.value = w.texture, d.transmissionSamplerSize.value.set(w.width, w.height), h.transmissionMap && (d.transmissionMap.value = h.transmissionMap, t(h.transmissionMap, d.transmissionMapTransform)), d.thickness.value = h.thickness, h.thicknessMap && (d.thicknessMap.value = h.thicknessMap, t(h.thicknessMap, d.thicknessMapTransform)), d.attenuationDistance.value = h.attenuationDistance, d.attenuationColor.value.copy(h.attenuationColor)), h.anisotropy > 0 && (d.anisotropyVector.value.set(h.anisotropy * Math.cos(h.anisotropyRotation), h.anisotropy * Math.sin(h.anisotropyRotation)), h.anisotropyMap && (d.anisotropyMap.value = h.anisotropyMap, t(h.anisotropyMap, d.anisotropyMapTransform))), d.specularIntensity.value = h.specularIntensity, d.specularColor.value.copy(h.specularColor), h.specularColorMap && (d.specularColorMap.value = h.specularColorMap, t(h.specularColorMap, d.specularColorMapTransform)), h.specularIntensityMap && (d.specularIntensityMap.value = h.specularIntensityMap, t(h.specularIntensityMap, d.specularIntensityMapTransform))
+    function m(d, u, T) {
+        d.ior.value = u.ior, u.sheen > 0 && (d.sheenColor.value.copy(u.sheenColor).multiplyScalar(u.sheen), d.sheenRoughness.value = u.sheenRoughness, u.sheenColorMap && (d.sheenColorMap.value = u.sheenColorMap, t(u.sheenColorMap, d.sheenColorMapTransform)), u.sheenRoughnessMap && (d.sheenRoughnessMap.value = u.sheenRoughnessMap, t(u.sheenRoughnessMap, d.sheenRoughnessMapTransform))), u.clearcoat > 0 && (d.clearcoat.value = u.clearcoat, d.clearcoatRoughness.value = u.clearcoatRoughness, u.clearcoatMap && (d.clearcoatMap.value = u.clearcoatMap, t(u.clearcoatMap, d.clearcoatMapTransform)), u.clearcoatRoughnessMap && (d.clearcoatRoughnessMap.value = u.clearcoatRoughnessMap, t(u.clearcoatRoughnessMap, d.clearcoatRoughnessMapTransform)), u.clearcoatNormalMap && (d.clearcoatNormalMap.value = u.clearcoatNormalMap, t(u.clearcoatNormalMap, d.clearcoatNormalMapTransform), d.clearcoatNormalScale.value.copy(u.clearcoatNormalScale), u.side === yt && d.clearcoatNormalScale.value.negate())), u.iridescence > 0 && (d.iridescence.value = u.iridescence, d.iridescenceIOR.value = u.iridescenceIOR, d.iridescenceThicknessMinimum.value = u.iridescenceThicknessRange[0], d.iridescenceThicknessMaximum.value = u.iridescenceThicknessRange[1], u.iridescenceMap && (d.iridescenceMap.value = u.iridescenceMap, t(u.iridescenceMap, d.iridescenceMapTransform)), u.iridescenceThicknessMap && (d.iridescenceThicknessMap.value = u.iridescenceThicknessMap, t(u.iridescenceThicknessMap, d.iridescenceThicknessMapTransform))), u.transmission > 0 && (d.transmission.value = u.transmission, d.transmissionSamplerMap.value = T.texture, d.transmissionSamplerSize.value.set(T.width, T.height), u.transmissionMap && (d.transmissionMap.value = u.transmissionMap, t(u.transmissionMap, d.transmissionMapTransform)), d.thickness.value = u.thickness, u.thicknessMap && (d.thicknessMap.value = u.thicknessMap, t(u.thicknessMap, d.thicknessMapTransform)), d.attenuationDistance.value = u.attenuationDistance, d.attenuationColor.value.copy(u.attenuationColor)), u.anisotropy > 0 && (d.anisotropyVector.value.set(u.anisotropy * Math.cos(u.anisotropyRotation), u.anisotropy * Math.sin(u.anisotropyRotation)), u.anisotropyMap && (d.anisotropyMap.value = u.anisotropyMap, t(u.anisotropyMap, d.anisotropyMapTransform))), d.specularIntensity.value = u.specularIntensity, d.specularColor.value.copy(u.specularColor), u.specularColorMap && (d.specularColorMap.value = u.specularColorMap, t(u.specularColorMap, d.specularColorMapTransform)), u.specularIntensityMap && (d.specularIntensityMap.value = u.specularIntensityMap, t(u.specularIntensityMap, d.specularIntensityMapTransform))
     }
 
-    function _(d, h) {
-        h.matcap && (d.matcap.value = h.matcap)
+    function _(d, u) {
+        u.matcap && (d.matcap.value = u.matcap)
     }
 
-    function M(d, h) {
-        let w = e.get(h).light;
-        d.referencePosition.value.setFromMatrixPosition(w.matrixWorld), d.nearDistance.value = w.shadow.camera.near, d.farDistance.value = w.shadow.camera.far
+    function M(d, u) {
+        let T = e.get(u).light;
+        d.referencePosition.value.setFromMatrixPosition(T.matrixWorld), d.nearDistance.value = T.shadow.camera.near, d.farDistance.value = T.shadow.camera.far
     }
     return {
         refreshFogUniforms: i,
         refreshMaterialUniforms: n
     }
 }
 
 function mf(r, e, t, i) {
     let n = {},
         a = {},
         o = [],
         s = t.isWebGL2 ? r.getParameter(r.MAX_UNIFORM_BUFFER_BINDINGS) : 0;
 
-    function l(w, x) {
-        let R = x.program;
-        i.uniformBlockBinding(w, R)
+    function l(T, x) {
+        let A = x.program;
+        i.uniformBlockBinding(T, A)
     }
 
-    function c(w, x) {
-        let R = n[w.id];
-        R === void 0 && (_(w), R = u(w), n[w.id] = R, w.addEventListener("dispose", d));
-        let U = x.program;
-        i.updateUBOMapping(w, U);
-        let A = e.render.frame;
-        a[w.id] !== A && (f(w), a[w.id] = A)
+    function c(T, x) {
+        let A = n[T.id];
+        A === void 0 && (_(T), A = h(T), n[T.id] = A, T.addEventListener("dispose", d));
+        let D = x.program;
+        i.updateUBOMapping(T, D);
+        let R = e.render.frame;
+        a[T.id] !== R && (f(T), a[T.id] = R)
     }
 
-    function u(w) {
+    function h(T) {
         let x = p();
-        w.__bindingPointIndex = x;
-        let R = r.createBuffer(),
-            U = w.__size,
-            A = w.usage;
-        return r.bindBuffer(r.UNIFORM_BUFFER, R), r.bufferData(r.UNIFORM_BUFFER, U, A), r.bindBuffer(r.UNIFORM_BUFFER, null), r.bindBufferBase(r.UNIFORM_BUFFER, x, R), R
+        T.__bindingPointIndex = x;
+        let A = r.createBuffer(),
+            D = T.__size,
+            R = T.usage;
+        return r.bindBuffer(r.UNIFORM_BUFFER, A), r.bufferData(r.UNIFORM_BUFFER, D, R), r.bindBuffer(r.UNIFORM_BUFFER, null), r.bindBufferBase(r.UNIFORM_BUFFER, x, A), A
     }
 
     function p() {
-        for (let w = 0; w < s; w++)
-            if (o.indexOf(w) === -1) return o.push(w), w;
+        for (let T = 0; T < s; T++)
+            if (o.indexOf(T) === -1) return o.push(T), T;
         return console.error("THREE.WebGLRenderer: Maximum number of simultaneously usable uniforms groups reached."), 0
     }
 
-    function f(w) {
-        let x = n[w.id],
-            R = w.uniforms,
-            U = w.__cache;
+    function f(T) {
+        let x = n[T.id],
+            A = T.uniforms,
+            D = T.__cache;
         r.bindBuffer(r.UNIFORM_BUFFER, x);
-        for (let A = 0, y = R.length; A < y; A++) {
-            let C = Array.isArray(R[A]) ? R[A] : [R[A]];
-            for (let Z = 0, v = C.length; Z < v; Z++) {
-                let T = C[Z];
-                if (m(T, A, Z, U) === !0) {
-                    let V = T.__offset,
-                        K = Array.isArray(T.value) ? T.value : [T.value],
-                        P = 0;
-                    for (let X = 0; X < K.length; X++) {
-                        let k = K[X],
-                            j = M(k);
-                        typeof k == "number" || typeof k == "boolean" ? (T.__data[0] = k, r.bufferSubData(r.UNIFORM_BUFFER, V + P, T.__data)) : k.isMatrix3 ? (T.__data[0] = k.elements[0], T.__data[1] = k.elements[1], T.__data[2] = k.elements[2], T.__data[3] = 0, T.__data[4] = k.elements[3], T.__data[5] = k.elements[4], T.__data[6] = k.elements[5], T.__data[7] = 0, T.__data[8] = k.elements[6], T.__data[9] = k.elements[7], T.__data[10] = k.elements[8], T.__data[11] = 0) : (k.toArray(T.__data, P), P += j.storage / Float32Array.BYTES_PER_ELEMENT)
+        for (let R = 0, b = A.length; R < b; R++) {
+            let P = Array.isArray(A[R]) ? A[R] : [A[R]];
+            for (let I = 0, v = P.length; I < v; I++) {
+                let w = P[I];
+                if (m(w, R, I, D) === !0) {
+                    let W = w.__offset,
+                        K = Array.isArray(w.value) ? w.value : [w.value],
+                        L = 0;
+                    for (let j = 0; j < K.length; j++) {
+                        let k = K[j],
+                            Y = M(k);
+                        typeof k == "number" || typeof k == "boolean" ? (w.__data[0] = k, r.bufferSubData(r.UNIFORM_BUFFER, W + L, w.__data)) : k.isMatrix3 ? (w.__data[0] = k.elements[0], w.__data[1] = k.elements[1], w.__data[2] = k.elements[2], w.__data[3] = 0, w.__data[4] = k.elements[3], w.__data[5] = k.elements[4], w.__data[6] = k.elements[5], w.__data[7] = 0, w.__data[8] = k.elements[6], w.__data[9] = k.elements[7], w.__data[10] = k.elements[8], w.__data[11] = 0) : (k.toArray(w.__data, L), L += Y.storage / Float32Array.BYTES_PER_ELEMENT)
                     }
-                    r.bufferSubData(r.UNIFORM_BUFFER, V, T.__data)
+                    r.bufferSubData(r.UNIFORM_BUFFER, W, w.__data)
                 }
             }
         }
         r.bindBuffer(r.UNIFORM_BUFFER, null)
     }
 
-    function m(w, x, R, U) {
-        let A = w.value,
-            y = x + "_" + R;
-        if (U[y] === void 0) return typeof A == "number" || typeof A == "boolean" ? U[y] = A : U[y] = A.clone(), !0;
+    function m(T, x, A, D) {
+        let R = T.value,
+            b = x + "_" + A;
+        if (D[b] === void 0) return typeof R == "number" || typeof R == "boolean" ? D[b] = R : D[b] = R.clone(), !0;
         {
-            let C = U[y];
-            if (typeof A == "number" || typeof A == "boolean") {
-                if (C !== A) return U[y] = A, !0
-            } else if (C.equals(A) === !1) return C.copy(A), !0
+            let P = D[b];
+            if (typeof R == "number" || typeof R == "boolean") {
+                if (P !== R) return D[b] = R, !0
+            } else if (P.equals(R) === !1) return P.copy(R), !0
         }
         return !1
     }
 
-    function _(w) {
-        let x = w.uniforms,
-            R = 0,
-            U = 16;
-        for (let y = 0, C = x.length; y < C; y++) {
-            let Z = Array.isArray(x[y]) ? x[y] : [x[y]];
-            for (let v = 0, T = Z.length; v < T; v++) {
-                let V = Z[v],
-                    K = Array.isArray(V.value) ? V.value : [V.value];
-                for (let P = 0, X = K.length; P < X; P++) {
-                    let k = K[P],
-                        j = M(k),
-                        q = R % U;
-                    q !== 0 && U - q < j.boundary && (R += U - q), V.__data = new Float32Array(j.storage / Float32Array.BYTES_PER_ELEMENT), V.__offset = R, R += j.storage
+    function _(T) {
+        let x = T.uniforms,
+            A = 0,
+            D = 16;
+        for (let b = 0, P = x.length; b < P; b++) {
+            let I = Array.isArray(x[b]) ? x[b] : [x[b]];
+            for (let v = 0, w = I.length; v < w; v++) {
+                let W = I[v],
+                    K = Array.isArray(W.value) ? W.value : [W.value];
+                for (let L = 0, j = K.length; L < j; L++) {
+                    let k = K[L],
+                        Y = M(k),
+                        q = A % D;
+                    q !== 0 && D - q < Y.boundary && (A += D - q), W.__data = new Float32Array(Y.storage / Float32Array.BYTES_PER_ELEMENT), W.__offset = A, A += Y.storage
                 }
             }
         }
-        let A = R % U;
-        return A > 0 && (R += U - A), w.__size = R, w.__cache = {}, this
+        let R = A % D;
+        return R > 0 && (A += D - R), T.__size = A, T.__cache = {}, this
     }
 
-    function M(w) {
+    function M(T) {
         let x = {
             boundary: 0,
             storage: 0
         };
-        return typeof w == "number" || typeof w == "boolean" ? (x.boundary = 4, x.storage = 4) : w.isVector2 ? (x.boundary = 8, x.storage = 8) : w.isVector3 || w.isColor ? (x.boundary = 16, x.storage = 12) : w.isVector4 ? (x.boundary = 16, x.storage = 16) : w.isMatrix3 ? (x.boundary = 48, x.storage = 48) : w.isMatrix4 ? (x.boundary = 64, x.storage = 64) : w.isTexture ? console.warn("THREE.WebGLRenderer: Texture samplers can not be part of an uniforms group.") : console.warn("THREE.WebGLRenderer: Unsupported uniform value type.", w), x
+        return typeof T == "number" || typeof T == "boolean" ? (x.boundary = 4, x.storage = 4) : T.isVector2 ? (x.boundary = 8, x.storage = 8) : T.isVector3 || T.isColor ? (x.boundary = 16, x.storage = 12) : T.isVector4 ? (x.boundary = 16, x.storage = 16) : T.isMatrix3 ? (x.boundary = 48, x.storage = 48) : T.isMatrix4 ? (x.boundary = 64, x.storage = 64) : T.isTexture ? console.warn("THREE.WebGLRenderer: Texture samplers can not be part of an uniforms group.") : console.warn("THREE.WebGLRenderer: Unsupported uniform value type.", T), x
     }
 
-    function d(w) {
-        let x = w.target;
+    function d(T) {
+        let x = T.target;
         x.removeEventListener("dispose", d);
-        let R = o.indexOf(x.__bindingPointIndex);
-        o.splice(R, 1), r.deleteBuffer(n[x.id]), delete n[x.id], delete a[x.id]
+        let A = o.indexOf(x.__bindingPointIndex);
+        o.splice(A, 1), r.deleteBuffer(n[x.id]), delete n[x.id], delete a[x.id]
     }
 
-    function h() {
-        for (let w in n) r.deleteBuffer(n[w]);
+    function u() {
+        for (let T in n) r.deleteBuffer(n[T]);
         o = [], n = {}, a = {}
     }
     return {
         bind: l,
         update: c,
-        dispose: h
+        dispose: u
     }
 }
 var Mn = class {
         constructor(e = {}) {
             let {
                 canvas: t = _c(),
                 context: i = null,
                 depth: n = !0,
                 stencil: a = !0,
                 alpha: o = !1,
                 antialias: s = !1,
                 premultipliedAlpha: l = !0,
                 preserveDrawingBuffer: c = !1,
-                powerPreference: u = "default",
+                powerPreference: h = "default",
                 failIfMajorPerformanceCaveat: p = !1
             } = e;
             this.isWebGLRenderer = !0;
             let f;
             i !== null ? f = i.getContextAttributes().alpha : f = o;
             let m = new Uint32Array(4),
                 _ = new Int32Array(4),
                 M = null,
                 d = null,
-                h = [],
-                w = [];
+                u = [],
+                T = [];
             this.domElement = t, this.debug = {
                 checkShaderErrors: !0,
                 onShaderError: null
             }, this.autoClear = !0, this.autoClearColor = !0, this.autoClearDepth = !0, this.autoClearStencil = !0, this.sortObjects = !0, this.clippingPlanes = [], this.localClippingEnabled = !1, this._outputColorSpace = Ft, this._useLegacyLights = !1, this.toneMapping = hi, this.toneMappingExposure = 1;
             let x = this,
-                R = !1,
-                U = 0,
-                A = 0,
-                y = null,
-                C = -1,
-                Z = null,
+                A = !1,
+                D = 0,
+                R = 0,
+                b = null,
+                P = -1,
+                I = null,
                 v = new ct,
-                T = new ct,
-                V = null,
+                w = new ct,
+                W = null,
                 K = new Ye(0),
-                P = 0,
-                X = t.width,
+                L = 0,
+                j = t.width,
                 k = t.height,
-                j = 1,
+                Y = 1,
                 q = null,
-                W = null,
-                te = new ct(0, 0, X, k),
-                ee = new ct(0, 0, X, k),
-                pe = !1,
-                xe = new gn,
-                H = !1,
-                ie = !1,
-                fe = null,
-                Te = new at,
-                _e = new De,
-                me = new D,
+                Z = null,
+                ee = new ct(0, 0, j, k),
+                ie = new ct(0, 0, j, k),
+                de = !1,
+                ge = new gn,
+                V = !1,
+                te = !1,
+                pe = null,
+                we = new at,
+                _e = new Ue,
+                fe = new U,
                 Xe = {
                     background: null,
                     fog: null,
                     environment: null,
                     overrideMaterial: null,
                     isScene: !0
                 };
 
-            function we() {
-                return y === null ? j : 1
+            function Ae() {
+                return b === null ? Y : 1
             }
-            let I = i;
+            let O = i;
 
-            function Qe(E, N) {
-                for (let z = 0; z < E.length; z++) {
-                    let G = E[z],
-                        F = t.getContext(G, N);
-                    if (F !== null) return F
+            function Je(y, N) {
+                for (let H = 0; H < y.length; H++) {
+                    let G = y[H],
+                        z = t.getContext(G, N);
+                    if (z !== null) return z
                 }
                 return null
             }
             try {
-                let E = {
+                let y = {
                     alpha: !0,
                     depth: n,
                     stencil: a,
                     antialias: s,
                     premultipliedAlpha: l,
                     preserveDrawingBuffer: c,
-                    powerPreference: u,
+                    powerPreference: h,
                     failIfMajorPerformanceCaveat: p
                 };
-                if ("setAttribute" in t && t.setAttribute("data-engine", `three.js r${ka}`), t.addEventListener("webglcontextlost", Ae, !1), t.addEventListener("webglcontextrestored", L, !1), t.addEventListener("webglcontextcreationerror", re, !1), I === null) {
+                if ("setAttribute" in t && t.setAttribute("data-engine", `three.js r${ka}`), t.addEventListener("webglcontextlost", Ce, !1), t.addEventListener("webglcontextrestored", C, !1), t.addEventListener("webglcontextcreationerror", re, !1), O === null) {
                     let N = ["webgl2", "webgl", "experimental-webgl"];
-                    if (x.isWebGL1Renderer === !0 && N.shift(), I = Qe(N, E), I === null) throw Qe(N) ? new Error("Error creating WebGL context with your selected attributes.") : new Error("Error creating WebGL context.")
+                    if (x.isWebGL1Renderer === !0 && N.shift(), O = Je(N, y), O === null) throw Je(N) ? new Error("Error creating WebGL context with your selected attributes.") : new Error("Error creating WebGL context.")
                 }
-                typeof WebGLRenderingContext < "u" && I instanceof WebGLRenderingContext && console.warn("THREE.WebGLRenderer: WebGL 1 support was deprecated in r153 and will be removed in r163."), I.getShaderPrecisionFormat === void 0 && (I.getShaderPrecisionFormat = function() {
+                typeof WebGLRenderingContext < "u" && O instanceof WebGLRenderingContext && console.warn("THREE.WebGLRenderer: WebGL 1 support was deprecated in r153 and will be removed in r163."), O.getShaderPrecisionFormat === void 0 && (O.getShaderPrecisionFormat = function() {
                     return {
                         rangeMin: 1,
                         rangeMax: 1,
                         precision: 1
                     }
                 })
-            } catch (E) {
-                throw console.error("THREE.WebGLRenderer: " + E.message), E
+            } catch (y) {
+                throw console.error("THREE.WebGLRenderer: " + y.message), y
             }
-            let ve, Ue, Me, Le, be, de, Ne, S, g, B, Y, Q, J, Ce, ye, ae, he, Ie, ne, Je, ze, Ee, ge, b;
+            let ve, Pe, Se, Ne, be, Re, xe, E, g, B, X, Q, J, Ee, Me, ae, he, Ie, ne, $e, Be, ye, me, S;
 
             function $() {
-                ve = new Ld(I), Ue = new bd(I, ve, e), ve.init(Ue), Ee = new cf(I, ve, Ue), Me = new of(I, ve, Ue), Le = new Dd(I), be = new qp, de = new lf(I, ve, Me, be, Ue, Ee, Le), Ne = new wd(x), S = new Cd(x), g = new zc(I, Ue), ge = new Sd(I, ve, g, Ue), B = new Pd(I, g, Le, ge), Y = new Fd(I, B, g, Le), ne = new Od(I, Ue, de), ae = new Td(be), Q = new Yp(x, Ne, S, ve, Ue, ge, ae), J = new ff(x, be), Ce = new Kp, ye = new rf(ve, Ue), Ie = new Ed(x, Ne, S, Me, Y, f, l), he = new sf(x, Y, Ue), b = new mf(I, Le, Ue, Me), Je = new yd(I, ve, Le, Ue), ze = new Ud(I, ve, Le, Ue), Le.programs = Q.programs, x.capabilities = Ue, x.extensions = ve, x.properties = be, x.renderLists = Ce, x.shadowMap = he, x.state = Me, x.info = Le
+                ve = new Ld(O), Pe = new Td(O, ve, e), ve.init(Pe), ye = new cf(O, ve, Pe), Se = new of(O, ve, Pe), Ne = new Ud(O), be = new qp, Re = new lf(O, ve, Se, be, Pe, ye, Ne), xe = new wd(x), E = new Cd(x), g = new Bc(O, Pe), me = new Ed(O, ve, g, Pe), B = new Pd(O, g, Ne, me), X = new Fd(O, B, g, Ne), ne = new Od(O, Pe, Re), ae = new bd(be), Q = new Yp(x, xe, E, ve, Pe, me, ae), J = new ff(x, be), Ee = new Kp, Me = new rf(ve, Pe), Ie = new yd(x, xe, E, Se, X, f, l), he = new sf(x, X, Pe), S = new mf(O, Ne, Pe, Se), $e = new Sd(O, ve, Ne, Pe), Be = new Dd(O, ve, Ne, Pe), Ne.programs = Q.programs, x.capabilities = Pe, x.extensions = ve, x.properties = be, x.renderLists = Ee, x.shadowMap = he, x.state = Se, x.info = Ne
             }
             $();
-            let oe = new Ia(x, I);
+            let oe = new Na(x, O);
             this.xr = oe, this.getContext = function() {
-                return I
+                return O
             }, this.getContextAttributes = function() {
-                return I.getContextAttributes()
+                return O.getContextAttributes()
             }, this.forceContextLoss = function() {
-                let E = ve.get("WEBGL_lose_context");
-                E && E.loseContext()
+                let y = ve.get("WEBGL_lose_context");
+                y && y.loseContext()
             }, this.forceContextRestore = function() {
-                let E = ve.get("WEBGL_lose_context");
-                E && E.restoreContext()
+                let y = ve.get("WEBGL_lose_context");
+                y && y.restoreContext()
             }, this.getPixelRatio = function() {
-                return j
-            }, this.setPixelRatio = function(E) {
-                E !== void 0 && (j = E, this.setSize(X, k, !1))
-            }, this.getSize = function(E) {
-                return E.set(X, k)
-            }, this.setSize = function(E, N, z = !0) {
+                return Y
+            }, this.setPixelRatio = function(y) {
+                y !== void 0 && (Y = y, this.setSize(j, k, !1))
+            }, this.getSize = function(y) {
+                return y.set(j, k)
+            }, this.setSize = function(y, N, H = !0) {
                 if (oe.isPresenting) {
                     console.warn("THREE.WebGLRenderer: Can't change size while VR device is presenting.");
                     return
                 }
-                X = E, k = N, t.width = Math.floor(E * j), t.height = Math.floor(N * j), z === !0 && (t.style.width = E + "px", t.style.height = N + "px"), this.setViewport(0, 0, E, N)
-            }, this.getDrawingBufferSize = function(E) {
-                return E.set(X * j, k * j).floor()
-            }, this.setDrawingBufferSize = function(E, N, z) {
-                X = E, k = N, j = z, t.width = Math.floor(E * z), t.height = Math.floor(N * z), this.setViewport(0, 0, E, N)
-            }, this.getCurrentViewport = function(E) {
-                return E.copy(v)
-            }, this.getViewport = function(E) {
-                return E.copy(te)
-            }, this.setViewport = function(E, N, z, G) {
-                E.isVector4 ? te.set(E.x, E.y, E.z, E.w) : te.set(E, N, z, G), Me.viewport(v.copy(te).multiplyScalar(j).round())
-            }, this.getScissor = function(E) {
-                return E.copy(ee)
-            }, this.setScissor = function(E, N, z, G) {
-                E.isVector4 ? ee.set(E.x, E.y, E.z, E.w) : ee.set(E, N, z, G), Me.scissor(T.copy(ee).multiplyScalar(j).round())
+                j = y, k = N, t.width = Math.floor(y * Y), t.height = Math.floor(N * Y), H === !0 && (t.style.width = y + "px", t.style.height = N + "px"), this.setViewport(0, 0, y, N)
+            }, this.getDrawingBufferSize = function(y) {
+                return y.set(j * Y, k * Y).floor()
+            }, this.setDrawingBufferSize = function(y, N, H) {
+                j = y, k = N, Y = H, t.width = Math.floor(y * H), t.height = Math.floor(N * H), this.setViewport(0, 0, y, N)
+            }, this.getCurrentViewport = function(y) {
+                return y.copy(v)
+            }, this.getViewport = function(y) {
+                return y.copy(ee)
+            }, this.setViewport = function(y, N, H, G) {
+                y.isVector4 ? ee.set(y.x, y.y, y.z, y.w) : ee.set(y, N, H, G), Se.viewport(v.copy(ee).multiplyScalar(Y).round())
+            }, this.getScissor = function(y) {
+                return y.copy(ie)
+            }, this.setScissor = function(y, N, H, G) {
+                y.isVector4 ? ie.set(y.x, y.y, y.z, y.w) : ie.set(y, N, H, G), Se.scissor(w.copy(ie).multiplyScalar(Y).round())
             }, this.getScissorTest = function() {
-                return pe
-            }, this.setScissorTest = function(E) {
-                Me.setScissorTest(pe = E)
-            }, this.setOpaqueSort = function(E) {
-                q = E
-            }, this.setTransparentSort = function(E) {
-                W = E
-            }, this.getClearColor = function(E) {
-                return E.copy(Ie.getClearColor())
+                return de
+            }, this.setScissorTest = function(y) {
+                Se.setScissorTest(de = y)
+            }, this.setOpaqueSort = function(y) {
+                q = y
+            }, this.setTransparentSort = function(y) {
+                Z = y
+            }, this.getClearColor = function(y) {
+                return y.copy(Ie.getClearColor())
             }, this.setClearColor = function() {
                 Ie.setClearColor.apply(Ie, arguments)
             }, this.getClearAlpha = function() {
                 return Ie.getClearAlpha()
             }, this.setClearAlpha = function() {
                 Ie.setClearAlpha.apply(Ie, arguments)
-            }, this.clear = function(E = !0, N = !0, z = !0) {
+            }, this.clear = function(y = !0, N = !0, H = !0) {
                 let G = 0;
-                if (E) {
-                    let F = !1;
-                    if (y !== null) {
-                        let ue = y.texture.format;
-                        F = ue === Bo || ue === Fo || ue === Oo
+                if (y) {
+                    let z = !1;
+                    if (b !== null) {
+                        let ue = b.texture.format;
+                        z = ue === zo || ue === Fo || ue === Oo
                     }
-                    if (F) {
-                        let ue = y.texture.type,
-                            Se = ue === ui || ue === li || ue === Va || ue === Ri || ue === No || ue === Io,
-                            Re = Ie.getClearColor(),
-                            Pe = Ie.getClearAlpha(),
-                            We = Re.r,
-                            He = Re.g,
-                            ke = Re.b;
-                        Se ? (m[0] = We, m[1] = He, m[2] = ke, m[3] = Pe, I.clearBufferuiv(I.COLOR, 0, m)) : (_[0] = We, _[1] = He, _[2] = ke, _[3] = Pe, I.clearBufferiv(I.COLOR, 0, _))
-                    } else G |= I.COLOR_BUFFER_BIT
+                    if (z) {
+                        let ue = b.texture.type,
+                            Te = ue === ui || ue === li || ue === Va || ue === Ri || ue === Io || ue === No,
+                            Le = Ie.getClearColor(),
+                            De = Ie.getClearAlpha(),
+                            We = Le.r,
+                            Ge = Le.g,
+                            ke = Le.b;
+                        Te ? (m[0] = We, m[1] = Ge, m[2] = ke, m[3] = De, O.clearBufferuiv(O.COLOR, 0, m)) : (_[0] = We, _[1] = Ge, _[2] = ke, _[3] = De, O.clearBufferiv(O.COLOR, 0, _))
+                    } else G |= O.COLOR_BUFFER_BIT
                 }
-                N && (G |= I.DEPTH_BUFFER_BIT), z && (G |= I.STENCIL_BUFFER_BIT, this.state.buffers.stencil.setMask(4294967295)), I.clear(G)
+                N && (G |= O.DEPTH_BUFFER_BIT), H && (G |= O.STENCIL_BUFFER_BIT, this.state.buffers.stencil.setMask(4294967295)), O.clear(G)
             }, this.clearColor = function() {
                 this.clear(!0, !1, !1)
             }, this.clearDepth = function() {
                 this.clear(!1, !0, !1)
             }, this.clearStencil = function() {
                 this.clear(!1, !1, !0)
             }, this.dispose = function() {
-                t.removeEventListener("webglcontextlost", Ae, !1), t.removeEventListener("webglcontextrestored", L, !1), t.removeEventListener("webglcontextcreationerror", re, !1), Ce.dispose(), ye.dispose(), be.dispose(), Ne.dispose(), S.dispose(), Y.dispose(), ge.dispose(), b.dispose(), Q.dispose(), oe.dispose(), oe.removeEventListener("sessionstart", $e), oe.removeEventListener("sessionend", je), fe && (fe.dispose(), fe = null), tt.stop()
+                t.removeEventListener("webglcontextlost", Ce, !1), t.removeEventListener("webglcontextrestored", C, !1), t.removeEventListener("webglcontextcreationerror", re, !1), Ee.dispose(), Me.dispose(), be.dispose(), xe.dispose(), E.dispose(), X.dispose(), me.dispose(), S.dispose(), Q.dispose(), oe.dispose(), oe.removeEventListener("sessionstart", Qe), oe.removeEventListener("sessionend", je), pe && (pe.dispose(), pe = null), tt.stop()
             };
 
-            function Ae(E) {
-                E.preventDefault(), console.log("THREE.WebGLRenderer: Context Lost."), R = !0
+            function Ce(y) {
+                y.preventDefault(), console.log("THREE.WebGLRenderer: Context Lost."), A = !0
             }
 
-            function L() {
-                console.log("THREE.WebGLRenderer: Context Restored."), R = !1;
-                let E = Le.autoReset,
+            function C() {
+                console.log("THREE.WebGLRenderer: Context Restored."), A = !1;
+                let y = Ne.autoReset,
                     N = he.enabled,
-                    z = he.autoUpdate,
+                    H = he.autoUpdate,
                     G = he.needsUpdate,
-                    F = he.type;
-                $(), Le.autoReset = E, he.enabled = N, he.autoUpdate = z, he.needsUpdate = G, he.type = F
+                    z = he.type;
+                $(), Ne.autoReset = y, he.enabled = N, he.autoUpdate = H, he.needsUpdate = G, he.type = z
             }
 
-            function re(E) {
-                console.error("THREE.WebGLRenderer: A WebGL context could not be created. Reason: ", E.statusMessage)
+            function re(y) {
+                console.error("THREE.WebGLRenderer: A WebGL context could not be created. Reason: ", y.statusMessage)
             }
 
-            function O(E) {
-                let N = E.target;
-                N.removeEventListener("dispose", O), le(N)
+            function F(y) {
+                let N = y.target;
+                N.removeEventListener("dispose", F), le(N)
             }
 
-            function le(E) {
-                se(E), be.remove(E)
+            function le(y) {
+                se(y), be.remove(y)
             }
 
-            function se(E) {
-                let N = be.get(E).programs;
-                N !== void 0 && (N.forEach(function(z) {
-                    Q.releaseProgram(z)
-                }), E.isShaderMaterial && Q.releaseShaderCache(E))
+            function se(y) {
+                let N = be.get(y).programs;
+                N !== void 0 && (N.forEach(function(H) {
+                    Q.releaseProgram(H)
+                }), y.isShaderMaterial && Q.releaseShaderCache(y))
             }
-            this.renderBufferDirect = function(E, N, z, G, F, ue) {
+            this.renderBufferDirect = function(y, N, H, G, z, ue) {
                 N === null && (N = Xe);
-                let Se = F.isMesh && F.matrixWorld.determinant() < 0,
-                    Re = $o(E, N, z, G, F);
-                Me.setMaterial(G, Se);
-                let Pe = z.index,
+                let Te = z.isMesh && z.matrixWorld.determinant() < 0,
+                    Le = $o(y, N, H, G, z);
+                Se.setMaterial(G, Te);
+                let De = H.index,
                     We = 1;
                 if (G.wireframe === !0) {
-                    if (Pe = B.getWireframeAttribute(z), Pe === void 0) return;
+                    if (De = B.getWireframeAttribute(H), De === void 0) return;
                     We = 2
                 }
-                let He = z.drawRange,
-                    ke = z.attributes.position,
-                    ht = He.start * We,
-                    nt = (He.start + He.count) * We;
-                ue !== null && (ht = Math.max(ht, ue.start * We), nt = Math.min(nt, (ue.start + ue.count) * We)), Pe !== null ? (ht = Math.max(ht, 0), nt = Math.min(nt, Pe.count)) : ke != null && (ht = Math.max(ht, 0), nt = Math.min(nt, ke.count));
+                let Ge = H.drawRange,
+                    ke = H.attributes.position,
+                    ht = Ge.start * We,
+                    nt = (Ge.start + Ge.count) * We;
+                ue !== null && (ht = Math.max(ht, ue.start * We), nt = Math.min(nt, (ue.start + ue.count) * We)), De !== null ? (ht = Math.max(ht, 0), nt = Math.min(nt, De.count)) : ke != null && (ht = Math.max(ht, 0), nt = Math.min(nt, ke.count));
                 let At = nt - ht;
                 if (At < 0 || At === 1 / 0) return;
-                ge.setup(F, G, Re, z, Pe);
-                let Ht, et = Je;
-                if (Pe !== null && (Ht = g.get(Pe), et = ze, et.setIndex(Ht)), F.isMesh) G.wireframe === !0 ? (Me.setLineWidth(G.wireframeLinewidth * we()), et.setMode(I.LINES)) : et.setMode(I.TRIANGLES);
-                else if (F.isLine) {
+                me.setup(z, G, Le, H, De);
+                let Gt, et = $e;
+                if (De !== null && (Gt = g.get(De), et = Be, et.setIndex(Gt)), z.isMesh) G.wireframe === !0 ? (Se.setLineWidth(G.wireframeLinewidth * Ae()), et.setMode(O.LINES)) : et.setMode(O.TRIANGLES);
+                else if (z.isLine) {
                     let Oe = G.linewidth;
-                    Oe === void 0 && (Oe = 1), Me.setLineWidth(Oe * we()), F.isLineSegments ? et.setMode(I.LINES) : F.isLineLoop ? et.setMode(I.LINE_LOOP) : et.setMode(I.LINE_STRIP)
-                } else F.isPoints ? et.setMode(I.POINTS) : F.isSprite && et.setMode(I.TRIANGLES);
-                if (F.isBatchedMesh) et.renderMultiDraw(F._multiDrawStarts, F._multiDrawCounts, F._multiDrawCount);
-                else if (F.isInstancedMesh) et.renderInstances(ht, At, F.count);
-                else if (z.isInstancedBufferGeometry) {
-                    let Oe = z._maxInstanceCount !== void 0 ? z._maxInstanceCount : 1 / 0,
-                        An = Math.min(z.instanceCount, Oe);
+                    Oe === void 0 && (Oe = 1), Se.setLineWidth(Oe * Ae()), z.isLineSegments ? et.setMode(O.LINES) : z.isLineLoop ? et.setMode(O.LINE_LOOP) : et.setMode(O.LINE_STRIP)
+                } else z.isPoints ? et.setMode(O.POINTS) : z.isSprite && et.setMode(O.TRIANGLES);
+                if (z.isBatchedMesh) et.renderMultiDraw(z._multiDrawStarts, z._multiDrawCounts, z._multiDrawCount);
+                else if (z.isInstancedMesh) et.renderInstances(ht, At, z.count);
+                else if (H.isInstancedBufferGeometry) {
+                    let Oe = H._maxInstanceCount !== void 0 ? H._maxInstanceCount : 1 / 0,
+                        An = Math.min(H.instanceCount, Oe);
                     et.renderInstances(ht, At, An)
                 } else et.render(ht, At)
             };
 
-            function Ge(E, N, z) {
-                E.transparent === !0 && E.side === qt && E.forceSinglePass === !1 ? (E.side = Et, E.needsUpdate = !0, wr(E, N, z), E.side = pi, E.needsUpdate = !0, wr(E, N, z), E.side = qt) : wr(E, N, z)
+            function He(y, N, H) {
+                y.transparent === !0 && y.side === qt && y.forceSinglePass === !1 ? (y.side = yt, y.needsUpdate = !0, wr(y, N, H), y.side = pi, y.needsUpdate = !0, wr(y, N, H), y.side = qt) : wr(y, N, H)
             }
-            this.compile = function(E, N, z = null) {
-                z === null && (z = E), d = ye.get(z), d.init(), w.push(d), z.traverseVisible(function(F) {
-                    F.isLight && F.layers.test(N.layers) && (d.pushLight(F), F.castShadow && d.pushShadow(F))
-                }), E !== z && E.traverseVisible(function(F) {
-                    F.isLight && F.layers.test(N.layers) && (d.pushLight(F), F.castShadow && d.pushShadow(F))
+            this.compile = function(y, N, H = null) {
+                H === null && (H = y), d = Me.get(H), d.init(), T.push(d), H.traverseVisible(function(z) {
+                    z.isLight && z.layers.test(N.layers) && (d.pushLight(z), z.castShadow && d.pushShadow(z))
+                }), y !== H && y.traverseVisible(function(z) {
+                    z.isLight && z.layers.test(N.layers) && (d.pushLight(z), z.castShadow && d.pushShadow(z))
                 }), d.setupLights(x._useLegacyLights);
                 let G = new Set;
-                return E.traverse(function(F) {
-                    let ue = F.material;
+                return y.traverse(function(z) {
+                    let ue = z.material;
                     if (ue)
                         if (Array.isArray(ue))
-                            for (let Se = 0; Se < ue.length; Se++) {
-                                let Re = ue[Se];
-                                Ge(Re, z, F), G.add(Re)
-                            } else Ge(ue, z, F), G.add(ue)
-                }), w.pop(), d = null, G
-            }, this.compileAsync = function(E, N, z = null) {
-                let G = this.compile(E, N, z);
-                return new Promise(F => {
+                            for (let Te = 0; Te < ue.length; Te++) {
+                                let Le = ue[Te];
+                                He(Le, H, z), G.add(Le)
+                            } else He(ue, H, z), G.add(ue)
+                }), T.pop(), d = null, G
+            }, this.compileAsync = function(y, N, H = null) {
+                let G = this.compile(y, N, H);
+                return new Promise(z => {
                     function ue() {
-                        if (G.forEach(function(Se) {
-                                be.get(Se).currentProgram.isReady() && G.delete(Se)
+                        if (G.forEach(function(Te) {
+                                be.get(Te).currentProgram.isReady() && G.delete(Te)
                             }), G.size === 0) {
-                            F(E);
+                            z(y);
                             return
                         }
                         setTimeout(ue, 10)
                     }
                     ve.get("KHR_parallel_shader_compile") !== null ? ue() : setTimeout(ue, 10)
                 })
             };
             let Ve = null;
 
-            function Ke(E) {
-                Ve && Ve(E)
+            function Ke(y) {
+                Ve && Ve(y)
             }
 
-            function $e() {
+            function Qe() {
                 tt.stop()
             }
 
             function je() {
                 tt.start()
             }
             let tt = new Wo;
-            tt.setAnimationLoop(Ke), typeof self < "u" && tt.setContext(self), this.setAnimationLoop = function(E) {
-                Ve = E, oe.setAnimationLoop(E), E === null ? tt.stop() : tt.start()
-            }, oe.addEventListener("sessionstart", $e), oe.addEventListener("sessionend", je), this.render = function(E, N) {
+            tt.setAnimationLoop(Ke), typeof self < "u" && tt.setContext(self), this.setAnimationLoop = function(y) {
+                Ve = y, oe.setAnimationLoop(y), y === null ? tt.stop() : tt.start()
+            }, oe.addEventListener("sessionstart", Qe), oe.addEventListener("sessionend", je), this.render = function(y, N) {
                 if (N !== void 0 && N.isCamera !== !0) {
                     console.error("THREE.WebGLRenderer.render: camera is not an instance of THREE.Camera.");
                     return
                 }
-                if (R === !0) return;
-                E.matrixWorldAutoUpdate === !0 && E.updateMatrixWorld(), N.parent === null && N.matrixWorldAutoUpdate === !0 && N.updateMatrixWorld(), oe.enabled === !0 && oe.isPresenting === !0 && (oe.cameraAutoUpdate === !0 && oe.updateCamera(N), N = oe.getCamera()), E.isScene === !0 && E.onBeforeRender(x, E, N, y), d = ye.get(E, w.length), d.init(), w.push(d), Te.multiplyMatrices(N.projectionMatrix, N.matrixWorldInverse), xe.setFromProjectionMatrix(Te), ie = this.localClippingEnabled, H = ae.init(this.clippingPlanes, ie), M = Ce.get(E, h.length), M.init(), h.push(M), yt(E, N, 0, x.sortObjects), M.finish(), x.sortObjects === !0 && M.sort(q, W), this.info.render.frame++, H === !0 && ae.beginShadows();
-                let z = d.state.shadowsArray;
-                if (he.render(z, E, N), H === !0 && ae.endShadows(), this.info.autoReset === !0 && this.info.reset(), (oe.enabled === !1 || oe.isPresenting === !1 || oe.hasDepthSensing() === !1) && Ie.render(M, E), d.setupLights(x._useLegacyLights), N.isArrayCamera) {
+                if (A === !0) return;
+                y.matrixWorldAutoUpdate === !0 && y.updateMatrixWorld(), N.parent === null && N.matrixWorldAutoUpdate === !0 && N.updateMatrixWorld(), oe.enabled === !0 && oe.isPresenting === !0 && (oe.cameraAutoUpdate === !0 && oe.updateCamera(N), N = oe.getCamera()), y.isScene === !0 && y.onBeforeRender(x, y, N, b), d = Me.get(y, T.length), d.init(), T.push(d), we.multiplyMatrices(N.projectionMatrix, N.matrixWorldInverse), ge.setFromProjectionMatrix(we), te = this.localClippingEnabled, V = ae.init(this.clippingPlanes, te), M = Ee.get(y, u.length), M.init(), u.push(M), St(y, N, 0, x.sortObjects), M.finish(), x.sortObjects === !0 && M.sort(q, Z), this.info.render.frame++, V === !0 && ae.beginShadows();
+                let H = d.state.shadowsArray;
+                if (he.render(H, y, N), V === !0 && ae.endShadows(), this.info.autoReset === !0 && this.info.reset(), (oe.enabled === !1 || oe.isPresenting === !1 || oe.hasDepthSensing() === !1) && Ie.render(M, y), d.setupLights(x._useLegacyLights), N.isArrayCamera) {
                     let G = N.cameras;
-                    for (let F = 0, ue = G.length; F < ue; F++) {
-                        let Se = G[F];
-                        Ya(M, E, Se, Se.viewport)
+                    for (let z = 0, ue = G.length; z < ue; z++) {
+                        let Te = G[z];
+                        Ya(M, y, Te, Te.viewport)
                     }
-                } else Ya(M, E, N);
-                y !== null && (de.updateMultisampleRenderTarget(y), de.updateRenderTargetMipmap(y)), E.isScene === !0 && E.onAfterRender(x, E, N), ge.resetDefaultState(), C = -1, Z = null, w.pop(), w.length > 0 ? d = w[w.length - 1] : d = null, h.pop(), h.length > 0 ? M = h[h.length - 1] : M = null
+                } else Ya(M, y, N);
+                b !== null && (Re.updateMultisampleRenderTarget(b), Re.updateRenderTargetMipmap(b)), y.isScene === !0 && y.onAfterRender(x, y, N), me.resetDefaultState(), P = -1, I = null, T.pop(), T.length > 0 ? d = T[T.length - 1] : d = null, u.pop(), u.length > 0 ? M = u[u.length - 1] : M = null
             };
 
-            function yt(E, N, z, G) {
-                if (E.visible === !1) return;
-                if (E.layers.test(N.layers)) {
-                    if (E.isGroup) z = E.renderOrder;
-                    else if (E.isLOD) E.autoUpdate === !0 && E.update(N);
-                    else if (E.isLight) d.pushLight(E), E.castShadow && d.pushShadow(E);
-                    else if (E.isSprite) {
-                        if (!E.frustumCulled || xe.intersectsSprite(E)) {
-                            G && me.setFromMatrixPosition(E.matrixWorld).applyMatrix4(Te);
-                            let ue = Y.update(E),
-                                Se = E.material;
-                            Se.visible && M.push(E, ue, Se, z, me.z, null)
+            function St(y, N, H, G) {
+                if (y.visible === !1) return;
+                if (y.layers.test(N.layers)) {
+                    if (y.isGroup) H = y.renderOrder;
+                    else if (y.isLOD) y.autoUpdate === !0 && y.update(N);
+                    else if (y.isLight) d.pushLight(y), y.castShadow && d.pushShadow(y);
+                    else if (y.isSprite) {
+                        if (!y.frustumCulled || ge.intersectsSprite(y)) {
+                            G && fe.setFromMatrixPosition(y.matrixWorld).applyMatrix4(we);
+                            let ue = X.update(y),
+                                Te = y.material;
+                            Te.visible && M.push(y, ue, Te, H, fe.z, null)
                         }
-                    } else if ((E.isMesh || E.isLine || E.isPoints) && (!E.frustumCulled || xe.intersectsObject(E))) {
-                        let ue = Y.update(E),
-                            Se = E.material;
-                        if (G && (E.boundingSphere !== void 0 ? (E.boundingSphere === null && E.computeBoundingSphere(), me.copy(E.boundingSphere.center)) : (ue.boundingSphere === null && ue.computeBoundingSphere(), me.copy(ue.boundingSphere.center)), me.applyMatrix4(E.matrixWorld).applyMatrix4(Te)), Array.isArray(Se)) {
-                            let Re = ue.groups;
-                            for (let Pe = 0, We = Re.length; Pe < We; Pe++) {
-                                let He = Re[Pe],
-                                    ke = Se[He.materialIndex];
-                                ke && ke.visible && M.push(E, ue, ke, z, me.z, He)
+                    } else if ((y.isMesh || y.isLine || y.isPoints) && (!y.frustumCulled || ge.intersectsObject(y))) {
+                        let ue = X.update(y),
+                            Te = y.material;
+                        if (G && (y.boundingSphere !== void 0 ? (y.boundingSphere === null && y.computeBoundingSphere(), fe.copy(y.boundingSphere.center)) : (ue.boundingSphere === null && ue.computeBoundingSphere(), fe.copy(ue.boundingSphere.center)), fe.applyMatrix4(y.matrixWorld).applyMatrix4(we)), Array.isArray(Te)) {
+                            let Le = ue.groups;
+                            for (let De = 0, We = Le.length; De < We; De++) {
+                                let Ge = Le[De],
+                                    ke = Te[Ge.materialIndex];
+                                ke && ke.visible && M.push(y, ue, ke, H, fe.z, Ge)
                             }
-                        } else Se.visible && M.push(E, ue, Se, z, me.z, null)
+                        } else Te.visible && M.push(y, ue, Te, H, fe.z, null)
                     }
                 }
-                let F = E.children;
-                for (let ue = 0, Se = F.length; ue < Se; ue++) yt(F[ue], N, z, G)
+                let z = y.children;
+                for (let ue = 0, Te = z.length; ue < Te; ue++) St(z[ue], N, H, G)
             }
 
-            function Ya(E, N, z, G) {
-                let F = E.opaque,
-                    ue = E.transmissive,
-                    Se = E.transparent;
-                d.setupLightsView(z), H === !0 && ae.setGlobalState(x.clippingPlanes, z), ue.length > 0 && Jo(F, ue, N, z), G && Me.viewport(v.copy(G)), F.length > 0 && Tr(F, N, z), ue.length > 0 && Tr(ue, N, z), Se.length > 0 && Tr(Se, N, z), Me.buffers.depth.setTest(!0), Me.buffers.depth.setMask(!0), Me.buffers.color.setMask(!0), Me.setPolygonOffset(!1)
+            function Ya(y, N, H, G) {
+                let z = y.opaque,
+                    ue = y.transmissive,
+                    Te = y.transparent;
+                d.setupLightsView(H), V === !0 && ae.setGlobalState(x.clippingPlanes, H), ue.length > 0 && Jo(z, ue, N, H), G && Se.viewport(v.copy(G)), z.length > 0 && br(z, N, H), ue.length > 0 && br(ue, N, H), Te.length > 0 && br(Te, N, H), Se.buffers.depth.setTest(!0), Se.buffers.depth.setMask(!0), Se.buffers.color.setMask(!0), Se.setPolygonOffset(!1)
             }
 
-            function Jo(E, N, z, G) {
-                if ((z.isScene === !0 ? z.overrideMaterial : null) !== null) return;
-                let F = Ue.isWebGL2;
-                fe === null && (fe = new $t(1, 1, {
+            function Jo(y, N, H, G) {
+                if ((H.isScene === !0 ? H.overrideMaterial : null) !== null) return;
+                let z = Pe.isWebGL2;
+                pe === null && (pe = new $t(1, 1, {
                     generateMipmaps: !0,
                     type: ve.has("EXT_color_buffer_half_float") ? Mr : ui,
                     minFilter: wi,
-                    samples: F ? 4 : 0
-                })), x.getDrawingBufferSize(_e), F ? fe.setSize(_e.x, _e.y) : fe.setSize(sn(_e.x), sn(_e.y));
+                    samples: z ? 4 : 0
+                })), x.getDrawingBufferSize(_e), z ? pe.setSize(_e.x, _e.y) : pe.setSize(sn(_e.x), sn(_e.y));
                 let ue = x.getRenderTarget();
-                x.setRenderTarget(fe), x.getClearColor(K), P = x.getClearAlpha(), P < 1 && x.setClearColor(16777215, .5), x.clear();
-                let Se = x.toneMapping;
-                x.toneMapping = hi, Tr(E, z, G), de.updateMultisampleRenderTarget(fe), de.updateRenderTargetMipmap(fe);
-                let Re = !1;
-                for (let Pe = 0, We = N.length; Pe < We; Pe++) {
-                    let He = N[Pe],
-                        ke = He.object,
-                        ht = He.geometry,
-                        nt = He.material,
-                        At = He.group;
+                x.setRenderTarget(pe), x.getClearColor(K), L = x.getClearAlpha(), L < 1 && x.setClearColor(16777215, .5), x.clear();
+                let Te = x.toneMapping;
+                x.toneMapping = hi, br(y, H, G), Re.updateMultisampleRenderTarget(pe), Re.updateRenderTargetMipmap(pe);
+                let Le = !1;
+                for (let De = 0, We = N.length; De < We; De++) {
+                    let Ge = N[De],
+                        ke = Ge.object,
+                        ht = Ge.geometry,
+                        nt = Ge.material,
+                        At = Ge.group;
                     if (nt.side === qt && ke.layers.test(G.layers)) {
-                        let Ht = nt.side;
-                        nt.side = Et, nt.needsUpdate = !0, qa(ke, z, G, ht, nt, At), nt.side = Ht, nt.needsUpdate = !0, Re = !0
+                        let Gt = nt.side;
+                        nt.side = yt, nt.needsUpdate = !0, qa(ke, H, G, ht, nt, At), nt.side = Gt, nt.needsUpdate = !0, Le = !0
                     }
                 }
-                Re === !0 && (de.updateMultisampleRenderTarget(fe), de.updateRenderTargetMipmap(fe)), x.setRenderTarget(ue), x.setClearColor(K, P), x.toneMapping = Se
+                Le === !0 && (Re.updateMultisampleRenderTarget(pe), Re.updateRenderTargetMipmap(pe)), x.setRenderTarget(ue), x.setClearColor(K, L), x.toneMapping = Te
             }
 
-            function Tr(E, N, z) {
+            function br(y, N, H) {
                 let G = N.isScene === !0 ? N.overrideMaterial : null;
-                for (let F = 0, ue = E.length; F < ue; F++) {
-                    let Se = E[F],
-                        Re = Se.object,
-                        Pe = Se.geometry,
-                        We = G === null ? Se.material : G,
-                        He = Se.group;
-                    Re.layers.test(z.layers) && qa(Re, N, z, Pe, We, He)
+                for (let z = 0, ue = y.length; z < ue; z++) {
+                    let Te = y[z],
+                        Le = Te.object,
+                        De = Te.geometry,
+                        We = G === null ? Te.material : G,
+                        Ge = Te.group;
+                    Le.layers.test(H.layers) && qa(Le, N, H, De, We, Ge)
                 }
             }
 
-            function qa(E, N, z, G, F, ue) {
-                E.onBeforeRender(x, N, z, G, F, ue), E.modelViewMatrix.multiplyMatrices(z.matrixWorldInverse, E.matrixWorld), E.normalMatrix.getNormalMatrix(E.modelViewMatrix), F.onBeforeRender(x, N, z, G, E, ue), F.transparent === !0 && F.side === qt && F.forceSinglePass === !1 ? (F.side = Et, F.needsUpdate = !0, x.renderBufferDirect(z, N, G, F, E, ue), F.side = pi, F.needsUpdate = !0, x.renderBufferDirect(z, N, G, F, E, ue), F.side = qt) : x.renderBufferDirect(z, N, G, F, E, ue), E.onAfterRender(x, N, z, G, F, ue)
+            function qa(y, N, H, G, z, ue) {
+                y.onBeforeRender(x, N, H, G, z, ue), y.modelViewMatrix.multiplyMatrices(H.matrixWorldInverse, y.matrixWorld), y.normalMatrix.getNormalMatrix(y.modelViewMatrix), z.onBeforeRender(x, N, H, G, y, ue), z.transparent === !0 && z.side === qt && z.forceSinglePass === !1 ? (z.side = yt, z.needsUpdate = !0, x.renderBufferDirect(H, N, G, z, y, ue), z.side = pi, z.needsUpdate = !0, x.renderBufferDirect(H, N, G, z, y, ue), z.side = qt) : x.renderBufferDirect(H, N, G, z, y, ue), y.onAfterRender(x, N, H, G, z, ue)
             }
 
-            function wr(E, N, z) {
+            function wr(y, N, H) {
                 N.isScene !== !0 && (N = Xe);
-                let G = be.get(E),
-                    F = d.state.lights,
+                let G = be.get(y),
+                    z = d.state.lights,
                     ue = d.state.shadowsArray,
-                    Se = F.state.version,
-                    Re = Q.getParameters(E, F.state, ue, N, z),
-                    Pe = Q.getProgramCacheKey(Re),
+                    Te = z.state.version,
+                    Le = Q.getParameters(y, z.state, ue, N, H),
+                    De = Q.getProgramCacheKey(Le),
                     We = G.programs;
-                G.environment = E.isMeshStandardMaterial ? N.environment : null, G.fog = N.fog, G.envMap = (E.isMeshStandardMaterial ? S : Ne).get(E.envMap || G.environment), G.envMapRotation = G.environment !== null && E.envMap === null ? N.environmentRotation : E.envMapRotation, We === void 0 && (E.addEventListener("dispose", O), We = new Map, G.programs = We);
-                let He = We.get(Pe);
-                if (He !== void 0) {
-                    if (G.currentProgram === He && G.lightsStateVersion === Se) return Ka(E, Re), He
-                } else Re.uniforms = Q.getUniforms(E), E.onBuild(z, Re, x), E.onBeforeCompile(Re, x), He = Q.acquireProgram(Re, Pe), We.set(Pe, He), G.uniforms = Re.uniforms;
+                G.environment = y.isMeshStandardMaterial ? N.environment : null, G.fog = N.fog, G.envMap = (y.isMeshStandardMaterial ? E : xe).get(y.envMap || G.environment), G.envMapRotation = G.environment !== null && y.envMap === null ? N.environmentRotation : y.envMapRotation, We === void 0 && (y.addEventListener("dispose", F), We = new Map, G.programs = We);
+                let Ge = We.get(De);
+                if (Ge !== void 0) {
+                    if (G.currentProgram === Ge && G.lightsStateVersion === Te) return Ka(y, Le), Ge
+                } else Le.uniforms = Q.getUniforms(y), y.onBuild(H, Le, x), y.onBeforeCompile(Le, x), Ge = Q.acquireProgram(Le, De), We.set(De, Ge), G.uniforms = Le.uniforms;
                 let ke = G.uniforms;
-                return (!E.isShaderMaterial && !E.isRawShaderMaterial || E.clipping === !0) && (ke.clippingPlanes = ae.uniform), Ka(E, Re), G.needsLights = el(E), G.lightsStateVersion = Se, G.needsLights && (ke.ambientLightColor.value = F.state.ambient, ke.lightProbe.value = F.state.probe, ke.directionalLights.value = F.state.directional, ke.directionalLightShadows.value = F.state.directionalShadow, ke.spotLights.value = F.state.spot, ke.spotLightShadows.value = F.state.spotShadow, ke.rectAreaLights.value = F.state.rectArea, ke.ltc_1.value = F.state.rectAreaLTC1, ke.ltc_2.value = F.state.rectAreaLTC2, ke.pointLights.value = F.state.point, ke.pointLightShadows.value = F.state.pointShadow, ke.hemisphereLights.value = F.state.hemi, ke.directionalShadowMap.value = F.state.directionalShadowMap, ke.directionalShadowMatrix.value = F.state.directionalShadowMatrix, ke.spotShadowMap.value = F.state.spotShadowMap, ke.spotLightMatrix.value = F.state.spotLightMatrix, ke.spotLightMap.value = F.state.spotLightMap, ke.pointShadowMap.value = F.state.pointShadowMap, ke.pointShadowMatrix.value = F.state.pointShadowMatrix), G.currentProgram = He, G.uniformsList = null, He
+                return (!y.isShaderMaterial && !y.isRawShaderMaterial || y.clipping === !0) && (ke.clippingPlanes = ae.uniform), Ka(y, Le), G.needsLights = el(y), G.lightsStateVersion = Te, G.needsLights && (ke.ambientLightColor.value = z.state.ambient, ke.lightProbe.value = z.state.probe, ke.directionalLights.value = z.state.directional, ke.directionalLightShadows.value = z.state.directionalShadow, ke.spotLights.value = z.state.spot, ke.spotLightShadows.value = z.state.spotShadow, ke.rectAreaLights.value = z.state.rectArea, ke.ltc_1.value = z.state.rectAreaLTC1, ke.ltc_2.value = z.state.rectAreaLTC2, ke.pointLights.value = z.state.point, ke.pointLightShadows.value = z.state.pointShadow, ke.hemisphereLights.value = z.state.hemi, ke.directionalShadowMap.value = z.state.directionalShadowMap, ke.directionalShadowMatrix.value = z.state.directionalShadowMatrix, ke.spotShadowMap.value = z.state.spotShadowMap, ke.spotLightMatrix.value = z.state.spotLightMatrix, ke.spotLightMap.value = z.state.spotLightMap, ke.pointShadowMap.value = z.state.pointShadowMap, ke.pointShadowMatrix.value = z.state.pointShadowMatrix), G.currentProgram = Ge, G.uniformsList = null, Ge
             }
 
-            function Za(E) {
-                if (E.uniformsList === null) {
-                    let N = E.currentProgram.getUniforms();
-                    E.uniformsList = rr.seqWithValue(N.seq, E.uniforms)
+            function Za(y) {
+                if (y.uniformsList === null) {
+                    let N = y.currentProgram.getUniforms();
+                    y.uniformsList = rr.seqWithValue(N.seq, y.uniforms)
                 }
-                return E.uniformsList
+                return y.uniformsList
             }
 
-            function Ka(E, N) {
-                let z = be.get(E);
-                z.outputColorSpace = N.outputColorSpace, z.batching = N.batching, z.instancing = N.instancing, z.instancingColor = N.instancingColor, z.instancingMorph = N.instancingMorph, z.skinning = N.skinning, z.morphTargets = N.morphTargets, z.morphNormals = N.morphNormals, z.morphColors = N.morphColors, z.morphTargetsCount = N.morphTargetsCount, z.numClippingPlanes = N.numClippingPlanes, z.numIntersection = N.numClipIntersection, z.vertexAlphas = N.vertexAlphas, z.vertexTangents = N.vertexTangents, z.toneMapping = N.toneMapping
+            function Ka(y, N) {
+                let H = be.get(y);
+                H.outputColorSpace = N.outputColorSpace, H.batching = N.batching, H.instancing = N.instancing, H.instancingColor = N.instancingColor, H.instancingMorph = N.instancingMorph, H.skinning = N.skinning, H.morphTargets = N.morphTargets, H.morphNormals = N.morphNormals, H.morphColors = N.morphColors, H.morphTargetsCount = N.morphTargetsCount, H.numClippingPlanes = N.numClippingPlanes, H.numIntersection = N.numClipIntersection, H.vertexAlphas = N.vertexAlphas, H.vertexTangents = N.vertexTangents, H.toneMapping = N.toneMapping
             }
 
-            function $o(E, N, z, G, F) {
-                N.isScene !== !0 && (N = Xe), de.resetTextureUnits();
+            function $o(y, N, H, G, z) {
+                N.isScene !== !0 && (N = Xe), Re.resetTextureUnits();
                 let ue = N.fog,
-                    Se = G.isMeshStandardMaterial ? N.environment : null,
-                    Re = y === null ? x.outputColorSpace : y.isXRRenderTarget === !0 ? y.texture.colorSpace : fi,
-                    Pe = (G.isMeshStandardMaterial ? S : Ne).get(G.envMap || Se),
-                    We = G.vertexColors === !0 && !!z.attributes.color && z.attributes.color.itemSize === 4,
-                    He = !!z.attributes.tangent && (!!G.normalMap || G.anisotropy > 0),
-                    ke = !!z.morphAttributes.position,
-                    ht = !!z.morphAttributes.normal,
-                    nt = !!z.morphAttributes.color,
+                    Te = G.isMeshStandardMaterial ? N.environment : null,
+                    Le = b === null ? x.outputColorSpace : b.isXRRenderTarget === !0 ? b.texture.colorSpace : fi,
+                    De = (G.isMeshStandardMaterial ? E : xe).get(G.envMap || Te),
+                    We = G.vertexColors === !0 && !!H.attributes.color && H.attributes.color.itemSize === 4,
+                    Ge = !!H.attributes.tangent && (!!G.normalMap || G.anisotropy > 0),
+                    ke = !!H.morphAttributes.position,
+                    ht = !!H.morphAttributes.normal,
+                    nt = !!H.morphAttributes.color,
                     At = hi;
-                G.toneMapped && (y === null || y.isXRRenderTarget === !0) && (At = x.toneMapping);
-                let Ht = z.morphAttributes.position || z.morphAttributes.normal || z.morphAttributes.color,
-                    et = Ht !== void 0 ? Ht.length : 0,
+                G.toneMapped && (b === null || b.isXRRenderTarget === !0) && (At = x.toneMapping);
+                let Gt = H.morphAttributes.position || H.morphAttributes.normal || H.morphAttributes.color,
+                    et = Gt !== void 0 ? Gt.length : 0,
                     Oe = be.get(G),
                     An = d.state.lights;
-                if (H === !0 && (ie === !0 || E !== Z)) {
-                    let Rt = E === Z && G.id === C;
-                    ae.setState(G, E, Rt)
+                if (V === !0 && (te === !0 || y !== I)) {
+                    let Rt = y === I && G.id === P;
+                    ae.setState(G, y, Rt)
                 }
                 let Rn = !1;
-                G.version === Oe.__version ? (Oe.needsLights && Oe.lightsStateVersion !== An.state.version || Oe.outputColorSpace !== Re || F.isBatchedMesh && Oe.batching === !1 || !F.isBatchedMesh && Oe.batching === !0 || F.isInstancedMesh && Oe.instancing === !1 || !F.isInstancedMesh && Oe.instancing === !0 || F.isSkinnedMesh && Oe.skinning === !1 || !F.isSkinnedMesh && Oe.skinning === !0 || F.isInstancedMesh && Oe.instancingColor === !0 && F.instanceColor === null || F.isInstancedMesh && Oe.instancingColor === !1 && F.instanceColor !== null || F.isInstancedMesh && Oe.instancingMorph === !0 && F.morphTexture === null || F.isInstancedMesh && Oe.instancingMorph === !1 && F.morphTexture !== null || Oe.envMap !== Pe || G.fog === !0 && Oe.fog !== ue || Oe.numClippingPlanes !== void 0 && (Oe.numClippingPlanes !== ae.numPlanes || Oe.numIntersection !== ae.numIntersection) || Oe.vertexAlphas !== We || Oe.vertexTangents !== He || Oe.morphTargets !== ke || Oe.morphNormals !== ht || Oe.morphColors !== nt || Oe.toneMapping !== At || Ue.isWebGL2 === !0 && Oe.morphTargetsCount !== et) && (Rn = !0) : (Rn = !0, Oe.__version = G.version);
+                G.version === Oe.__version ? (Oe.needsLights && Oe.lightsStateVersion !== An.state.version || Oe.outputColorSpace !== Le || z.isBatchedMesh && Oe.batching === !1 || !z.isBatchedMesh && Oe.batching === !0 || z.isInstancedMesh && Oe.instancing === !1 || !z.isInstancedMesh && Oe.instancing === !0 || z.isSkinnedMesh && Oe.skinning === !1 || !z.isSkinnedMesh && Oe.skinning === !0 || z.isInstancedMesh && Oe.instancingColor === !0 && z.instanceColor === null || z.isInstancedMesh && Oe.instancingColor === !1 && z.instanceColor !== null || z.isInstancedMesh && Oe.instancingMorph === !0 && z.morphTexture === null || z.isInstancedMesh && Oe.instancingMorph === !1 && z.morphTexture !== null || Oe.envMap !== De || G.fog === !0 && Oe.fog !== ue || Oe.numClippingPlanes !== void 0 && (Oe.numClippingPlanes !== ae.numPlanes || Oe.numIntersection !== ae.numIntersection) || Oe.vertexAlphas !== We || Oe.vertexTangents !== Ge || Oe.morphTargets !== ke || Oe.morphNormals !== ht || Oe.morphColors !== nt || Oe.toneMapping !== At || Pe.isWebGL2 === !0 && Oe.morphTargetsCount !== et) && (Rn = !0) : (Rn = !0, Oe.__version = G.version);
                 let mi = Oe.currentProgram;
-                Rn === !0 && (mi = wr(G, N, F));
+                Rn === !0 && (mi = wr(G, N, z));
                 let Ja = !1,
                     dr = !1,
                     Cn = !1,
                     ut = mi.getUniforms(),
                     gi = Oe.uniforms;
-                if (Me.useProgram(mi.program) && (Ja = !0, dr = !0, Cn = !0), G.id !== C && (C = G.id, dr = !0), Ja || Z !== E) {
-                    ut.setValue(I, "projectionMatrix", E.projectionMatrix), ut.setValue(I, "viewMatrix", E.matrixWorldInverse);
+                if (Se.useProgram(mi.program) && (Ja = !0, dr = !0, Cn = !0), G.id !== P && (P = G.id, dr = !0), Ja || I !== y) {
+                    ut.setValue(O, "projectionMatrix", y.projectionMatrix), ut.setValue(O, "viewMatrix", y.matrixWorldInverse);
                     let Rt = ut.map.cameraPosition;
-                    Rt !== void 0 && Rt.setValue(I, me.setFromMatrixPosition(E.matrixWorld)), Ue.logarithmicDepthBuffer && ut.setValue(I, "logDepthBufFC", 2 / (Math.log(E.far + 1) / Math.LN2)), (G.isMeshPhongMaterial || G.isMeshToonMaterial || G.isMeshLambertMaterial || G.isMeshBasicMaterial || G.isMeshStandardMaterial || G.isShaderMaterial) && ut.setValue(I, "isOrthographic", E.isOrthographicCamera === !0), Z !== E && (Z = E, dr = !0, Cn = !0)
+                    Rt !== void 0 && Rt.setValue(O, fe.setFromMatrixPosition(y.matrixWorld)), Pe.logarithmicDepthBuffer && ut.setValue(O, "logDepthBufFC", 2 / (Math.log(y.far + 1) / Math.LN2)), (G.isMeshPhongMaterial || G.isMeshToonMaterial || G.isMeshLambertMaterial || G.isMeshBasicMaterial || G.isMeshStandardMaterial || G.isShaderMaterial) && ut.setValue(O, "isOrthographic", y.isOrthographicCamera === !0), I !== y && (I = y, dr = !0, Cn = !0)
                 }
-                if (F.isSkinnedMesh) {
-                    ut.setOptional(I, F, "bindMatrix"), ut.setOptional(I, F, "bindMatrixInverse");
-                    let Rt = F.skeleton;
-                    Rt && (Ue.floatVertexTextures ? (Rt.boneTexture === null && Rt.computeBoneTexture(), ut.setValue(I, "boneTexture", Rt.boneTexture, de)) : console.warn("THREE.WebGLRenderer: SkinnedMesh can only be used with WebGL 2. With WebGL 1 OES_texture_float and vertex textures support is required."))
-                }
-                F.isBatchedMesh && (ut.setOptional(I, F, "batchingTexture"), ut.setValue(I, "batchingTexture", F._matricesTexture, de));
-                let Ln = z.morphAttributes;
-                if ((Ln.position !== void 0 || Ln.normal !== void 0 || Ln.color !== void 0 && Ue.isWebGL2 === !0) && ne.update(F, z, mi), (dr || Oe.receiveShadow !== F.receiveShadow) && (Oe.receiveShadow = F.receiveShadow, ut.setValue(I, "receiveShadow", F.receiveShadow)), G.isMeshGouraudMaterial && G.envMap !== null && (gi.envMap.value = Pe, gi.flipEnvMap.value = Pe.isCubeTexture && Pe.isRenderTargetTexture === !1 ? -1 : 1), dr && (ut.setValue(I, "toneMappingExposure", x.toneMappingExposure), Oe.needsLights && Qo(gi, Cn), ue && G.fog === !0 && J.refreshFogUniforms(gi, ue), J.refreshMaterialUniforms(gi, G, j, k, fe), rr.upload(I, Za(Oe), gi, de)), G.isShaderMaterial && G.uniformsNeedUpdate === !0 && (rr.upload(I, Za(Oe), gi, de), G.uniformsNeedUpdate = !1), G.isSpriteMaterial && ut.setValue(I, "center", F.center), ut.setValue(I, "modelViewMatrix", F.modelViewMatrix), ut.setValue(I, "normalMatrix", F.normalMatrix), ut.setValue(I, "modelMatrix", F.matrixWorld), G.isShaderMaterial || G.isRawShaderMaterial) {
+                if (z.isSkinnedMesh) {
+                    ut.setOptional(O, z, "bindMatrix"), ut.setOptional(O, z, "bindMatrixInverse");
+                    let Rt = z.skeleton;
+                    Rt && (Pe.floatVertexTextures ? (Rt.boneTexture === null && Rt.computeBoneTexture(), ut.setValue(O, "boneTexture", Rt.boneTexture, Re)) : console.warn("THREE.WebGLRenderer: SkinnedMesh can only be used with WebGL 2. With WebGL 1 OES_texture_float and vertex textures support is required."))
+                }
+                z.isBatchedMesh && (ut.setOptional(O, z, "batchingTexture"), ut.setValue(O, "batchingTexture", z._matricesTexture, Re));
+                let Ln = H.morphAttributes;
+                if ((Ln.position !== void 0 || Ln.normal !== void 0 || Ln.color !== void 0 && Pe.isWebGL2 === !0) && ne.update(z, H, mi), (dr || Oe.receiveShadow !== z.receiveShadow) && (Oe.receiveShadow = z.receiveShadow, ut.setValue(O, "receiveShadow", z.receiveShadow)), G.isMeshGouraudMaterial && G.envMap !== null && (gi.envMap.value = De, gi.flipEnvMap.value = De.isCubeTexture && De.isRenderTargetTexture === !1 ? -1 : 1), dr && (ut.setValue(O, "toneMappingExposure", x.toneMappingExposure), Oe.needsLights && Qo(gi, Cn), ue && G.fog === !0 && J.refreshFogUniforms(gi, ue), J.refreshMaterialUniforms(gi, G, Y, k, pe), rr.upload(O, Za(Oe), gi, Re)), G.isShaderMaterial && G.uniformsNeedUpdate === !0 && (rr.upload(O, Za(Oe), gi, Re), G.uniformsNeedUpdate = !1), G.isSpriteMaterial && ut.setValue(O, "center", z.center), ut.setValue(O, "modelViewMatrix", z.modelViewMatrix), ut.setValue(O, "normalMatrix", z.normalMatrix), ut.setValue(O, "modelMatrix", z.matrixWorld), G.isShaderMaterial || G.isRawShaderMaterial) {
                     let Rt = G.uniformsGroups;
                     for (let Pn = 0, tl = Rt.length; Pn < tl; Pn++)
-                        if (Ue.isWebGL2) {
+                        if (Pe.isWebGL2) {
                             let $a = Rt[Pn];
-                            b.update($a, mi), b.bind($a, mi)
+                            S.update($a, mi), S.bind($a, mi)
                         } else console.warn("THREE.WebGLRenderer: Uniform Buffer Objects can only be used with WebGL 2.")
                 }
                 return mi
             }
 
-            function Qo(E, N) {
-                E.ambientLightColor.needsUpdate = N, E.lightProbe.needsUpdate = N, E.directionalLights.needsUpdate = N, E.directionalLightShadows.needsUpdate = N, E.pointLights.needsUpdate = N, E.pointLightShadows.needsUpdate = N, E.spotLights.needsUpdate = N, E.spotLightShadows.needsUpdate = N, E.rectAreaLights.needsUpdate = N, E.hemisphereLights.needsUpdate = N
+            function Qo(y, N) {
+                y.ambientLightColor.needsUpdate = N, y.lightProbe.needsUpdate = N, y.directionalLights.needsUpdate = N, y.directionalLightShadows.needsUpdate = N, y.pointLights.needsUpdate = N, y.pointLightShadows.needsUpdate = N, y.spotLights.needsUpdate = N, y.spotLightShadows.needsUpdate = N, y.rectAreaLights.needsUpdate = N, y.hemisphereLights.needsUpdate = N
             }
 
-            function el(E) {
-                return E.isMeshLambertMaterial || E.isMeshToonMaterial || E.isMeshPhongMaterial || E.isMeshStandardMaterial || E.isShadowMaterial || E.isShaderMaterial && E.lights === !0
+            function el(y) {
+                return y.isMeshLambertMaterial || y.isMeshToonMaterial || y.isMeshPhongMaterial || y.isMeshStandardMaterial || y.isShadowMaterial || y.isShaderMaterial && y.lights === !0
             }
             this.getActiveCubeFace = function() {
-                return U
+                return D
             }, this.getActiveMipmapLevel = function() {
-                return A
+                return R
             }, this.getRenderTarget = function() {
-                return y
-            }, this.setRenderTargetTextures = function(E, N, z) {
-                be.get(E.texture).__webglTexture = N, be.get(E.depthTexture).__webglTexture = z;
-                let G = be.get(E);
-                G.__hasExternalTextures = !0, G.__autoAllocateDepthBuffer = z === void 0, G.__autoAllocateDepthBuffer || ve.has("WEBGL_multisampled_render_to_texture") === !0 && (console.warn("THREE.WebGLRenderer: Render-to-texture extension was disabled because an external texture was provided"), G.__useRenderToTexture = !1)
-            }, this.setRenderTargetFramebuffer = function(E, N) {
-                let z = be.get(E);
-                z.__webglFramebuffer = N, z.__useDefaultFramebuffer = N === void 0
-            }, this.setRenderTarget = function(E, N = 0, z = 0) {
-                y = E, U = N, A = z;
+                return b
+            }, this.setRenderTargetTextures = function(y, N, H) {
+                be.get(y.texture).__webglTexture = N, be.get(y.depthTexture).__webglTexture = H;
+                let G = be.get(y);
+                G.__hasExternalTextures = !0, G.__autoAllocateDepthBuffer = H === void 0, G.__autoAllocateDepthBuffer || ve.has("WEBGL_multisampled_render_to_texture") === !0 && (console.warn("THREE.WebGLRenderer: Render-to-texture extension was disabled because an external texture was provided"), G.__useRenderToTexture = !1)
+            }, this.setRenderTargetFramebuffer = function(y, N) {
+                let H = be.get(y);
+                H.__webglFramebuffer = N, H.__useDefaultFramebuffer = N === void 0
+            }, this.setRenderTarget = function(y, N = 0, H = 0) {
+                b = y, D = N, R = H;
                 let G = !0,
-                    F = null,
+                    z = null,
                     ue = !1,
-                    Se = !1;
-                if (E) {
-                    let Re = be.get(E);
-                    Re.__useDefaultFramebuffer !== void 0 ? (Me.bindFramebuffer(I.FRAMEBUFFER, null), G = !1) : Re.__webglFramebuffer === void 0 ? de.setupRenderTarget(E) : Re.__hasExternalTextures && de.rebindTextures(E, be.get(E.texture).__webglTexture, be.get(E.depthTexture).__webglTexture);
-                    let Pe = E.texture;
-                    (Pe.isData3DTexture || Pe.isDataArrayTexture || Pe.isCompressedArrayTexture) && (Se = !0);
-                    let We = be.get(E).__webglFramebuffer;
-                    E.isWebGLCubeRenderTarget ? (Array.isArray(We[N]) ? F = We[N][z] : F = We[N], ue = !0) : Ue.isWebGL2 && E.samples > 0 && de.useMultisampledRTT(E) === !1 ? F = be.get(E).__webglMultisampledFramebuffer : Array.isArray(We) ? F = We[z] : F = We, v.copy(E.viewport), T.copy(E.scissor), V = E.scissorTest
-                } else v.copy(te).multiplyScalar(j).floor(), T.copy(ee).multiplyScalar(j).floor(), V = pe;
-                if (Me.bindFramebuffer(I.FRAMEBUFFER, F) && Ue.drawBuffers && G && Me.drawBuffers(E, F), Me.viewport(v), Me.scissor(T), Me.setScissorTest(V), ue) {
-                    let Re = be.get(E.texture);
-                    I.framebufferTexture2D(I.FRAMEBUFFER, I.COLOR_ATTACHMENT0, I.TEXTURE_CUBE_MAP_POSITIVE_X + N, Re.__webglTexture, z)
-                } else if (Se) {
-                    let Re = be.get(E.texture),
-                        Pe = N || 0;
-                    I.framebufferTextureLayer(I.FRAMEBUFFER, I.COLOR_ATTACHMENT0, Re.__webglTexture, z || 0, Pe)
-                }
-                C = -1
-            }, this.readRenderTargetPixels = function(E, N, z, G, F, ue, Se) {
-                if (!(E && E.isWebGLRenderTarget)) {
+                    Te = !1;
+                if (y) {
+                    let Le = be.get(y);
+                    Le.__useDefaultFramebuffer !== void 0 ? (Se.bindFramebuffer(O.FRAMEBUFFER, null), G = !1) : Le.__webglFramebuffer === void 0 ? Re.setupRenderTarget(y) : Le.__hasExternalTextures && Re.rebindTextures(y, be.get(y.texture).__webglTexture, be.get(y.depthTexture).__webglTexture);
+                    let De = y.texture;
+                    (De.isData3DTexture || De.isDataArrayTexture || De.isCompressedArrayTexture) && (Te = !0);
+                    let We = be.get(y).__webglFramebuffer;
+                    y.isWebGLCubeRenderTarget ? (Array.isArray(We[N]) ? z = We[N][H] : z = We[N], ue = !0) : Pe.isWebGL2 && y.samples > 0 && Re.useMultisampledRTT(y) === !1 ? z = be.get(y).__webglMultisampledFramebuffer : Array.isArray(We) ? z = We[H] : z = We, v.copy(y.viewport), w.copy(y.scissor), W = y.scissorTest
+                } else v.copy(ee).multiplyScalar(Y).floor(), w.copy(ie).multiplyScalar(Y).floor(), W = de;
+                if (Se.bindFramebuffer(O.FRAMEBUFFER, z) && Pe.drawBuffers && G && Se.drawBuffers(y, z), Se.viewport(v), Se.scissor(w), Se.setScissorTest(W), ue) {
+                    let Le = be.get(y.texture);
+                    O.framebufferTexture2D(O.FRAMEBUFFER, O.COLOR_ATTACHMENT0, O.TEXTURE_CUBE_MAP_POSITIVE_X + N, Le.__webglTexture, H)
+                } else if (Te) {
+                    let Le = be.get(y.texture),
+                        De = N || 0;
+                    O.framebufferTextureLayer(O.FRAMEBUFFER, O.COLOR_ATTACHMENT0, Le.__webglTexture, H || 0, De)
+                }
+                P = -1
+            }, this.readRenderTargetPixels = function(y, N, H, G, z, ue, Te) {
+                if (!(y && y.isWebGLRenderTarget)) {
                     console.error("THREE.WebGLRenderer.readRenderTargetPixels: renderTarget is not THREE.WebGLRenderTarget.");
                     return
                 }
-                let Re = be.get(E).__webglFramebuffer;
-                if (E.isWebGLCubeRenderTarget && Se !== void 0 && (Re = Re[Se]), Re) {
-                    Me.bindFramebuffer(I.FRAMEBUFFER, Re);
+                let Le = be.get(y).__webglFramebuffer;
+                if (y.isWebGLCubeRenderTarget && Te !== void 0 && (Le = Le[Te]), Le) {
+                    Se.bindFramebuffer(O.FRAMEBUFFER, Le);
                     try {
-                        let Pe = E.texture,
-                            We = Pe.format,
-                            He = Pe.type;
-                        if (We !== Ot && Ee.convert(We) !== I.getParameter(I.IMPLEMENTATION_COLOR_READ_FORMAT)) {
+                        let De = y.texture,
+                            We = De.format,
+                            Ge = De.type;
+                        if (We !== Ot && ye.convert(We) !== O.getParameter(O.IMPLEMENTATION_COLOR_READ_FORMAT)) {
                             console.error("THREE.WebGLRenderer.readRenderTargetPixels: renderTarget is not in RGBA or implementation defined format.");
                             return
                         }
-                        let ke = He === Mr && (ve.has("EXT_color_buffer_half_float") || Ue.isWebGL2 && ve.has("EXT_color_buffer_float"));
-                        if (He !== ui && Ee.convert(He) !== I.getParameter(I.IMPLEMENTATION_COLOR_READ_TYPE) && !(He === Zt && (Ue.isWebGL2 || ve.has("OES_texture_float") || ve.has("WEBGL_color_buffer_float"))) && !ke) {
+                        let ke = Ge === Mr && (ve.has("EXT_color_buffer_half_float") || Pe.isWebGL2 && ve.has("EXT_color_buffer_float"));
+                        if (Ge !== ui && ye.convert(Ge) !== O.getParameter(O.IMPLEMENTATION_COLOR_READ_TYPE) && !(Ge === Zt && (Pe.isWebGL2 || ve.has("OES_texture_float") || ve.has("WEBGL_color_buffer_float"))) && !ke) {
                             console.error("THREE.WebGLRenderer.readRenderTargetPixels: renderTarget is not in UnsignedByteType or implementation defined type.");
                             return
                         }
-                        N >= 0 && N <= E.width - G && z >= 0 && z <= E.height - F && I.readPixels(N, z, G, F, Ee.convert(We), Ee.convert(He), ue)
+                        N >= 0 && N <= y.width - G && H >= 0 && H <= y.height - z && O.readPixels(N, H, G, z, ye.convert(We), ye.convert(Ge), ue)
                     } finally {
-                        let Pe = y !== null ? be.get(y).__webglFramebuffer : null;
-                        Me.bindFramebuffer(I.FRAMEBUFFER, Pe)
+                        let De = b !== null ? be.get(b).__webglFramebuffer : null;
+                        Se.bindFramebuffer(O.FRAMEBUFFER, De)
                     }
                 }
-            }, this.copyFramebufferToTexture = function(E, N, z = 0) {
-                let G = Math.pow(2, -z),
-                    F = Math.floor(N.image.width * G),
+            }, this.copyFramebufferToTexture = function(y, N, H = 0) {
+                let G = Math.pow(2, -H),
+                    z = Math.floor(N.image.width * G),
                     ue = Math.floor(N.image.height * G);
-                de.setTexture2D(N, 0), I.copyTexSubImage2D(I.TEXTURE_2D, z, 0, 0, E.x, E.y, F, ue), Me.unbindTexture()
-            }, this.copyTextureToTexture = function(E, N, z, G = 0) {
-                let F = N.image.width,
+                Re.setTexture2D(N, 0), O.copyTexSubImage2D(O.TEXTURE_2D, H, 0, 0, y.x, y.y, z, ue), Se.unbindTexture()
+            }, this.copyTextureToTexture = function(y, N, H, G = 0) {
+                let z = N.image.width,
                     ue = N.image.height,
-                    Se = Ee.convert(z.format),
-                    Re = Ee.convert(z.type);
-                de.setTexture2D(z, 0), I.pixelStorei(I.UNPACK_FLIP_Y_WEBGL, z.flipY), I.pixelStorei(I.UNPACK_PREMULTIPLY_ALPHA_WEBGL, z.premultiplyAlpha), I.pixelStorei(I.UNPACK_ALIGNMENT, z.unpackAlignment), N.isDataTexture ? I.texSubImage2D(I.TEXTURE_2D, G, E.x, E.y, F, ue, Se, Re, N.image.data) : N.isCompressedTexture ? I.compressedTexSubImage2D(I.TEXTURE_2D, G, E.x, E.y, N.mipmaps[0].width, N.mipmaps[0].height, Se, N.mipmaps[0].data) : I.texSubImage2D(I.TEXTURE_2D, G, E.x, E.y, Se, Re, N.image), G === 0 && z.generateMipmaps && I.generateMipmap(I.TEXTURE_2D), Me.unbindTexture()
-            }, this.copyTextureToTexture3D = function(E, N, z, G, F = 0) {
+                    Te = ye.convert(H.format),
+                    Le = ye.convert(H.type);
+                Re.setTexture2D(H, 0), O.pixelStorei(O.UNPACK_FLIP_Y_WEBGL, H.flipY), O.pixelStorei(O.UNPACK_PREMULTIPLY_ALPHA_WEBGL, H.premultiplyAlpha), O.pixelStorei(O.UNPACK_ALIGNMENT, H.unpackAlignment), N.isDataTexture ? O.texSubImage2D(O.TEXTURE_2D, G, y.x, y.y, z, ue, Te, Le, N.image.data) : N.isCompressedTexture ? O.compressedTexSubImage2D(O.TEXTURE_2D, G, y.x, y.y, N.mipmaps[0].width, N.mipmaps[0].height, Te, N.mipmaps[0].data) : O.texSubImage2D(O.TEXTURE_2D, G, y.x, y.y, Te, Le, N.image), G === 0 && H.generateMipmaps && O.generateMipmap(O.TEXTURE_2D), Se.unbindTexture()
+            }, this.copyTextureToTexture3D = function(y, N, H, G, z = 0) {
                 if (x.isWebGL1Renderer) {
                     console.warn("THREE.WebGLRenderer.copyTextureToTexture3D: can only be used with WebGL2.");
                     return
                 }
-                let ue = Math.round(E.max.x - E.min.x),
-                    Se = Math.round(E.max.y - E.min.y),
-                    Re = E.max.z - E.min.z + 1,
-                    Pe = Ee.convert(G.format),
-                    We = Ee.convert(G.type),
-                    He;
-                if (G.isData3DTexture) de.setTexture3D(G, 0), He = I.TEXTURE_3D;
-                else if (G.isDataArrayTexture || G.isCompressedArrayTexture) de.setTexture2DArray(G, 0), He = I.TEXTURE_2D_ARRAY;
+                let ue = Math.round(y.max.x - y.min.x),
+                    Te = Math.round(y.max.y - y.min.y),
+                    Le = y.max.z - y.min.z + 1,
+                    De = ye.convert(G.format),
+                    We = ye.convert(G.type),
+                    Ge;
+                if (G.isData3DTexture) Re.setTexture3D(G, 0), Ge = O.TEXTURE_3D;
+                else if (G.isDataArrayTexture || G.isCompressedArrayTexture) Re.setTexture2DArray(G, 0), Ge = O.TEXTURE_2D_ARRAY;
                 else {
                     console.warn("THREE.WebGLRenderer.copyTextureToTexture3D: only supports THREE.DataTexture3D and THREE.DataTexture2DArray.");
                     return
                 }
-                I.pixelStorei(I.UNPACK_FLIP_Y_WEBGL, G.flipY), I.pixelStorei(I.UNPACK_PREMULTIPLY_ALPHA_WEBGL, G.premultiplyAlpha), I.pixelStorei(I.UNPACK_ALIGNMENT, G.unpackAlignment);
-                let ke = I.getParameter(I.UNPACK_ROW_LENGTH),
-                    ht = I.getParameter(I.UNPACK_IMAGE_HEIGHT),
-                    nt = I.getParameter(I.UNPACK_SKIP_PIXELS),
-                    At = I.getParameter(I.UNPACK_SKIP_ROWS),
-                    Ht = I.getParameter(I.UNPACK_SKIP_IMAGES),
-                    et = z.isCompressedTexture ? z.mipmaps[F] : z.image;
-                I.pixelStorei(I.UNPACK_ROW_LENGTH, et.width), I.pixelStorei(I.UNPACK_IMAGE_HEIGHT, et.height), I.pixelStorei(I.UNPACK_SKIP_PIXELS, E.min.x), I.pixelStorei(I.UNPACK_SKIP_ROWS, E.min.y), I.pixelStorei(I.UNPACK_SKIP_IMAGES, E.min.z), z.isDataTexture || z.isData3DTexture ? I.texSubImage3D(He, F, N.x, N.y, N.z, ue, Se, Re, Pe, We, et.data) : G.isCompressedArrayTexture ? I.compressedTexSubImage3D(He, F, N.x, N.y, N.z, ue, Se, Re, Pe, et.data) : I.texSubImage3D(He, F, N.x, N.y, N.z, ue, Se, Re, Pe, We, et), I.pixelStorei(I.UNPACK_ROW_LENGTH, ke), I.pixelStorei(I.UNPACK_IMAGE_HEIGHT, ht), I.pixelStorei(I.UNPACK_SKIP_PIXELS, nt), I.pixelStorei(I.UNPACK_SKIP_ROWS, At), I.pixelStorei(I.UNPACK_SKIP_IMAGES, Ht), F === 0 && G.generateMipmaps && I.generateMipmap(He), Me.unbindTexture()
-            }, this.initTexture = function(E) {
-                E.isCubeTexture ? de.setTextureCube(E, 0) : E.isData3DTexture ? de.setTexture3D(E, 0) : E.isDataArrayTexture || E.isCompressedArrayTexture ? de.setTexture2DArray(E, 0) : de.setTexture2D(E, 0), Me.unbindTexture()
+                O.pixelStorei(O.UNPACK_FLIP_Y_WEBGL, G.flipY), O.pixelStorei(O.UNPACK_PREMULTIPLY_ALPHA_WEBGL, G.premultiplyAlpha), O.pixelStorei(O.UNPACK_ALIGNMENT, G.unpackAlignment);
+                let ke = O.getParameter(O.UNPACK_ROW_LENGTH),
+                    ht = O.getParameter(O.UNPACK_IMAGE_HEIGHT),
+                    nt = O.getParameter(O.UNPACK_SKIP_PIXELS),
+                    At = O.getParameter(O.UNPACK_SKIP_ROWS),
+                    Gt = O.getParameter(O.UNPACK_SKIP_IMAGES),
+                    et = H.isCompressedTexture ? H.mipmaps[z] : H.image;
+                O.pixelStorei(O.UNPACK_ROW_LENGTH, et.width), O.pixelStorei(O.UNPACK_IMAGE_HEIGHT, et.height), O.pixelStorei(O.UNPACK_SKIP_PIXELS, y.min.x), O.pixelStorei(O.UNPACK_SKIP_ROWS, y.min.y), O.pixelStorei(O.UNPACK_SKIP_IMAGES, y.min.z), H.isDataTexture || H.isData3DTexture ? O.texSubImage3D(Ge, z, N.x, N.y, N.z, ue, Te, Le, De, We, et.data) : G.isCompressedArrayTexture ? O.compressedTexSubImage3D(Ge, z, N.x, N.y, N.z, ue, Te, Le, De, et.data) : O.texSubImage3D(Ge, z, N.x, N.y, N.z, ue, Te, Le, De, We, et), O.pixelStorei(O.UNPACK_ROW_LENGTH, ke), O.pixelStorei(O.UNPACK_IMAGE_HEIGHT, ht), O.pixelStorei(O.UNPACK_SKIP_PIXELS, nt), O.pixelStorei(O.UNPACK_SKIP_ROWS, At), O.pixelStorei(O.UNPACK_SKIP_IMAGES, Gt), z === 0 && G.generateMipmaps && O.generateMipmap(Ge), Se.unbindTexture()
+            }, this.initTexture = function(y) {
+                y.isCubeTexture ? Re.setTextureCube(y, 0) : y.isData3DTexture ? Re.setTexture3D(y, 0) : y.isDataArrayTexture || y.isCompressedArrayTexture ? Re.setTexture2DArray(y, 0) : Re.setTexture2D(y, 0), Se.unbindTexture()
             }, this.resetState = function() {
-                U = 0, A = 0, y = null, Me.reset(), ge.reset()
+                D = 0, R = 0, b = null, Se.reset(), me.reset()
             }, typeof __THREE_DEVTOOLS__ < "u" && __THREE_DEVTOOLS__.dispatchEvent(new CustomEvent("observe", {
                 detail: this
             }))
         }
         get coordinateSystem() {
             return Kt
         }
         get outputColorSpace() {
             return this._outputColorSpace
         }
         set outputColorSpace(e) {
             this._outputColorSpace = e;
             let t = this.getContext();
-            t.drawingBufferColorSpace = e === Wa ? "display-p3" : "srgb", t.unpackColorSpace = qe.workingColorSpace === Tn ? "display-p3" : "srgb"
+            t.drawingBufferColorSpace = e === Wa ? "display-p3" : "srgb", t.unpackColorSpace = qe.workingColorSpace === bn ? "display-p3" : "srgb"
         }
         get useLegacyLights() {
             return console.warn("THREE.WebGLRenderer: The property .useLegacyLights has been deprecated. Migrate your lighting according to the following guide: https://discourse.threejs.org/t/updates-to-lighting-in-three-js-r155/53733."), this._useLegacyLights
         }
         set useLegacyLights(e) {
             console.warn("THREE.WebGLRenderer: The property .useLegacyLights has been deprecated. Migrate your lighting according to the following guide: https://discourse.threejs.org/t/updates-to-lighting-in-three-js-r155/53733."), this._useLegacyLights = e
         }
@@ -14765,81 +14765,81 @@
         constructor(e) {
             super(), this.isLineBasicMaterial = !0, this.type = "LineBasicMaterial", this.color = new Ye(16777215), this.map = null, this.linewidth = 1, this.linecap = "round", this.linejoin = "round", this.fog = !0, this.setValues(e)
         }
         copy(e) {
             return super.copy(e), this.color.copy(e.color), this.map = e.map, this.linewidth = e.linewidth, this.linecap = e.linecap, this.linejoin = e.linejoin, this.fog = e.fog, this
         }
     },
-    Eo = new D,
-    So = new D,
-    yo = new at,
-    la = new Sr,
+    yo = new U,
+    Eo = new U,
+    So = new at,
+    la = new Er,
     qr = new or,
-    br = class extends wt {
-        constructor(e = new St, t = new cr) {
+    Tr = class extends wt {
+        constructor(e = new Et, t = new cr) {
             super(), this.isLine = !0, this.type = "Line", this.geometry = e, this.material = t, this.updateMorphTargets()
         }
         copy(e, t) {
             return super.copy(e, t), this.material = Array.isArray(e.material) ? e.material.slice() : e.material, this.geometry = e.geometry, this
         }
         computeLineDistances() {
             let e = this.geometry;
             if (e.index === null) {
                 let t = e.attributes.position,
                     i = [0];
-                for (let n = 1, a = t.count; n < a; n++) Eo.fromBufferAttribute(t, n - 1), So.fromBufferAttribute(t, n), i[n] = i[n - 1], i[n] += Eo.distanceTo(So);
+                for (let n = 1, a = t.count; n < a; n++) yo.fromBufferAttribute(t, n - 1), Eo.fromBufferAttribute(t, n), i[n] = i[n - 1], i[n] += yo.distanceTo(Eo);
                 e.setAttribute("lineDistance", new rt(i, 1))
             } else console.warn("THREE.Line.computeLineDistances(): Computation only possible with non-indexed BufferGeometry.");
             return this
         }
         raycast(e, t) {
             let i = this.geometry,
                 n = this.matrixWorld,
                 a = e.params.Line.threshold,
                 o = i.drawRange;
             if (i.boundingSphere === null && i.computeBoundingSphere(), qr.copy(i.boundingSphere), qr.applyMatrix4(n), qr.radius += a, e.ray.intersectsSphere(qr) === !1) return;
-            yo.copy(n).invert(), la.copy(e.ray).applyMatrix4(yo);
+            So.copy(n).invert(), la.copy(e.ray).applyMatrix4(So);
             let s = a / ((this.scale.x + this.scale.y + this.scale.z) / 3),
                 l = s * s,
-                c = new D,
-                u = new D,
-                p = new D,
-                f = new D,
+                c = new U,
+                h = new U,
+                p = new U,
+                f = new U,
                 m = this.isLineSegments ? 2 : 1,
                 _ = i.index,
                 M = i.attributes.position;
             if (_ !== null) {
                 let d = Math.max(0, o.start),
-                    h = Math.min(_.count, o.start + o.count);
-                for (let w = d, x = h - 1; w < x; w += m) {
-                    let R = _.getX(w),
-                        U = _.getX(w + 1);
-                    if (c.fromBufferAttribute(M, R), u.fromBufferAttribute(M, U), la.distanceSqToSegment(c, u, f, p) > l) continue;
+                    u = Math.min(_.count, o.start + o.count);
+                for (let T = d, x = u - 1; T < x; T += m) {
+                    let A = _.getX(T),
+                        D = _.getX(T + 1);
+                    if (c.fromBufferAttribute(M, A), h.fromBufferAttribute(M, D), la.distanceSqToSegment(c, h, f, p) > l) continue;
                     f.applyMatrix4(this.matrixWorld);
-                    let A = e.ray.origin.distanceTo(f);
-                    A < e.near || A > e.far || t.push({
-                        distance: A,
+                    let R = e.ray.origin.distanceTo(f);
+                    R < e.near || R > e.far || t.push({
+                        distance: R,
                         point: p.clone().applyMatrix4(this.matrixWorld),
-                        index: w,
+                        index: T,
                         face: null,
                         faceIndex: null,
                         object: this
                     })
                 }
             } else {
                 let d = Math.max(0, o.start),
-                    h = Math.min(M.count, o.start + o.count);
-                for (let w = d, x = h - 1; w < x; w += m) {
-                    if (c.fromBufferAttribute(M, w), u.fromBufferAttribute(M, w + 1), la.distanceSqToSegment(c, u, f, p) > l) continue;
+                    u = Math.min(M.count, o.start + o.count);
+                for (let T = d, x = u - 1; T < x; T += m) {
+                    if (c.fromBufferAttribute(M, T), h.fromBufferAttribute(M, T + 1), la.distanceSqToSegment(c, h, f, p) > l) continue;
                     f.applyMatrix4(this.matrixWorld);
-                    let R = e.ray.origin.distanceTo(f);
-                    R < e.near || R > e.far || t.push({
-                        distance: R,
+                    let A = e.ray.origin.distanceTo(f);
+                    A < e.near || A > e.far || t.push({
+                        distance: A,
                         point: p.clone().applyMatrix4(this.matrixWorld),
-                        index: w,
+                        index: T,
                         face: null,
                         faceIndex: null,
                         object: this
                     })
                 }
             }
         }
@@ -14854,153 +14854,153 @@
                         let o = i[n].name || String(n);
                         this.morphTargetInfluences.push(0), this.morphTargetDictionary[o] = n
                     }
                 }
             }
         }
     },
-    bo = new D,
-    To = new D,
-    Ba = class extends br {
+    To = new U,
+    bo = new U,
+    za = class extends Tr {
         constructor(e, t) {
             super(e, t), this.isLineSegments = !0, this.type = "LineSegments"
         }
         computeLineDistances() {
             let e = this.geometry;
             if (e.index === null) {
                 let t = e.attributes.position,
                     i = [];
-                for (let n = 0, a = t.count; n < a; n += 2) bo.fromBufferAttribute(t, n), To.fromBufferAttribute(t, n + 1), i[n] = n === 0 ? 0 : i[n - 1], i[n + 1] = i[n] + bo.distanceTo(To);
+                for (let n = 0, a = t.count; n < a; n += 2) To.fromBufferAttribute(t, n), bo.fromBufferAttribute(t, n + 1), i[n] = n === 0 ? 0 : i[n - 1], i[n + 1] = i[n] + To.distanceTo(bo);
                 e.setAttribute("lineDistance", new rt(i, 1))
             } else console.warn("THREE.LineSegments.computeLineDistances(): Computation only possible with non-indexed BufferGeometry.");
             return this
         }
     },
-    za = class r extends St {
+    Ba = class r extends Et {
         constructor(e = 1, t = 1, i = 1, n = 32, a = 1, o = !1, s = 0, l = Math.PI * 2) {
             super(), this.type = "CylinderGeometry", this.parameters = {
                 radiusTop: e,
                 radiusBottom: t,
                 height: i,
                 radialSegments: n,
                 heightSegments: a,
                 openEnded: o,
                 thetaStart: s,
                 thetaLength: l
             };
             let c = this;
             n = Math.floor(n), a = Math.floor(a);
-            let u = [],
+            let h = [],
                 p = [],
                 f = [],
                 m = [],
                 _ = 0,
                 M = [],
                 d = i / 2,
-                h = 0;
-            w(), o === !1 && (e > 0 && x(!0), t > 0 && x(!1)), this.setIndex(u), this.setAttribute("position", new rt(p, 3)), this.setAttribute("normal", new rt(f, 3)), this.setAttribute("uv", new rt(m, 2));
+                u = 0;
+            T(), o === !1 && (e > 0 && x(!0), t > 0 && x(!1)), this.setIndex(h), this.setAttribute("position", new rt(p, 3)), this.setAttribute("normal", new rt(f, 3)), this.setAttribute("uv", new rt(m, 2));
 
-            function w() {
-                let R = new D,
-                    U = new D,
-                    A = 0,
-                    y = (t - e) / i;
-                for (let C = 0; C <= a; C++) {
-                    let Z = [],
-                        v = C / a,
-                        T = v * (t - e) + e;
-                    for (let V = 0; V <= n; V++) {
-                        let K = V / n,
-                            P = K * l + s,
-                            X = Math.sin(P),
-                            k = Math.cos(P);
-                        U.x = T * X, U.y = -v * i + d, U.z = T * k, p.push(U.x, U.y, U.z), R.set(X, y, k).normalize(), f.push(R.x, R.y, R.z), m.push(K, 1 - v), Z.push(_++)
+            function T() {
+                let A = new U,
+                    D = new U,
+                    R = 0,
+                    b = (t - e) / i;
+                for (let P = 0; P <= a; P++) {
+                    let I = [],
+                        v = P / a,
+                        w = v * (t - e) + e;
+                    for (let W = 0; W <= n; W++) {
+                        let K = W / n,
+                            L = K * l + s,
+                            j = Math.sin(L),
+                            k = Math.cos(L);
+                        D.x = w * j, D.y = -v * i + d, D.z = w * k, p.push(D.x, D.y, D.z), A.set(j, b, k).normalize(), f.push(A.x, A.y, A.z), m.push(K, 1 - v), I.push(_++)
                     }
-                    M.push(Z)
+                    M.push(I)
                 }
-                for (let C = 0; C < n; C++)
-                    for (let Z = 0; Z < a; Z++) {
-                        let v = M[Z][C],
-                            T = M[Z + 1][C],
-                            V = M[Z + 1][C + 1],
-                            K = M[Z][C + 1];
-                        u.push(v, T, K), u.push(T, V, K), A += 6
+                for (let P = 0; P < n; P++)
+                    for (let I = 0; I < a; I++) {
+                        let v = M[I][P],
+                            w = M[I + 1][P],
+                            W = M[I + 1][P + 1],
+                            K = M[I][P + 1];
+                        h.push(v, w, K), h.push(w, W, K), R += 6
                     }
-                c.addGroup(h, A, 0), h += A
+                c.addGroup(u, R, 0), u += R
             }
 
-            function x(R) {
-                let U = _,
-                    A = new De,
-                    y = new D,
-                    C = 0,
-                    Z = R === !0 ? e : t,
-                    v = R === !0 ? 1 : -1;
-                for (let V = 1; V <= n; V++) p.push(0, d * v, 0), f.push(0, v, 0), m.push(.5, .5), _++;
-                let T = _;
-                for (let V = 0; V <= n; V++) {
-                    let K = V / n * l + s,
-                        P = Math.cos(K),
-                        X = Math.sin(K);
-                    y.x = Z * X, y.y = d * v, y.z = Z * P, p.push(y.x, y.y, y.z), f.push(0, v, 0), A.x = P * .5 + .5, A.y = X * .5 * v + .5, m.push(A.x, A.y), _++
-                }
-                for (let V = 0; V < n; V++) {
-                    let K = U + V,
-                        P = T + V;
-                    R === !0 ? u.push(P, P + 1, K) : u.push(P + 1, P, K), C += 3
+            function x(A) {
+                let D = _,
+                    R = new Ue,
+                    b = new U,
+                    P = 0,
+                    I = A === !0 ? e : t,
+                    v = A === !0 ? 1 : -1;
+                for (let W = 1; W <= n; W++) p.push(0, d * v, 0), f.push(0, v, 0), m.push(.5, .5), _++;
+                let w = _;
+                for (let W = 0; W <= n; W++) {
+                    let K = W / n * l + s,
+                        L = Math.cos(K),
+                        j = Math.sin(K);
+                    b.x = I * j, b.y = d * v, b.z = I * L, p.push(b.x, b.y, b.z), f.push(0, v, 0), R.x = L * .5 + .5, R.y = j * .5 * v + .5, m.push(R.x, R.y), _++
+                }
+                for (let W = 0; W < n; W++) {
+                    let K = D + W,
+                        L = w + W;
+                    A === !0 ? h.push(L, L + 1, K) : h.push(L + 1, L, K), P += 3
                 }
-                c.addGroup(h, C, R === !0 ? 1 : 2), h += C
+                c.addGroup(u, P, A === !0 ? 1 : 2), u += P
             }
         }
         copy(e) {
             return super.copy(e), this.parameters = Object.assign({}, e.parameters), this
         }
         static fromJSON(e) {
             return new r(e.radiusTop, e.radiusBottom, e.height, e.radialSegments, e.heightSegments, e.openEnded, e.thetaStart, e.thetaLength)
         }
     },
-    Zr = new D,
-    Kr = new D,
-    ca = new D,
+    Zr = new U,
+    Kr = new U,
+    ca = new U,
     Jr = new Ai,
-    Ga = class extends St {
+    Ha = class extends Et {
         constructor(e = null, t = 1) {
             if (super(), this.type = "EdgesGeometry", this.parameters = {
                     geometry: e,
                     thresholdAngle: t
                 }, e !== null) {
                 let i = Math.pow(10, 4),
                     n = Math.cos(tr * t),
                     a = e.getIndex(),
                     o = e.getAttribute("position"),
                     s = a ? a.count : o.count,
                     l = [0, 0, 0],
                     c = ["a", "b", "c"],
-                    u = new Array(3),
+                    h = new Array(3),
                     p = {},
                     f = [];
                 for (let m = 0; m < s; m += 3) {
                     a ? (l[0] = a.getX(m), l[1] = a.getX(m + 1), l[2] = a.getX(m + 2)) : (l[0] = m, l[1] = m + 1, l[2] = m + 2);
                     let {
                         a: _,
                         b: M,
                         c: d
                     } = Jr;
-                    if (_.fromBufferAttribute(o, l[0]), M.fromBufferAttribute(o, l[1]), d.fromBufferAttribute(o, l[2]), Jr.getNormal(ca), u[0] = `${Math.round(_.x*i)},${Math.round(_.y*i)},${Math.round(_.z*i)}`, u[1] = `${Math.round(M.x*i)},${Math.round(M.y*i)},${Math.round(M.z*i)}`, u[2] = `${Math.round(d.x*i)},${Math.round(d.y*i)},${Math.round(d.z*i)}`, !(u[0] === u[1] || u[1] === u[2] || u[2] === u[0]))
-                        for (let h = 0; h < 3; h++) {
-                            let w = (h + 1) % 3,
-                                x = u[h],
-                                R = u[w],
-                                U = Jr[c[h]],
-                                A = Jr[c[w]],
-                                y = `${x}_${R}`,
-                                C = `${R}_${x}`;
-                            C in p && p[C] ? (ca.dot(p[C].normal) <= n && (f.push(U.x, U.y, U.z), f.push(A.x, A.y, A.z)), p[C] = null) : y in p || (p[y] = {
-                                index0: l[h],
-                                index1: l[w],
+                    if (_.fromBufferAttribute(o, l[0]), M.fromBufferAttribute(o, l[1]), d.fromBufferAttribute(o, l[2]), Jr.getNormal(ca), h[0] = `${Math.round(_.x*i)},${Math.round(_.y*i)},${Math.round(_.z*i)}`, h[1] = `${Math.round(M.x*i)},${Math.round(M.y*i)},${Math.round(M.z*i)}`, h[2] = `${Math.round(d.x*i)},${Math.round(d.y*i)},${Math.round(d.z*i)}`, !(h[0] === h[1] || h[1] === h[2] || h[2] === h[0]))
+                        for (let u = 0; u < 3; u++) {
+                            let T = (u + 1) % 3,
+                                x = h[u],
+                                A = h[T],
+                                D = Jr[c[u]],
+                                R = Jr[c[T]],
+                                b = `${x}_${A}`,
+                                P = `${A}_${x}`;
+                            P in p && p[P] ? (ca.dot(p[P].normal) <= n && (f.push(D.x, D.y, D.z), f.push(R.x, R.y, R.z)), p[P] = null) : b in p || (p[b] = {
+                                index0: l[u],
+                                index1: l[T],
                                 normal: ca.clone()
                             })
                         }
                 }
                 for (let m in p)
                     if (p[m]) {
                         let {
@@ -15011,63 +15011,63 @@
                     } this.setAttribute("position", new rt(f, 3))
             }
         }
         copy(e) {
             return super.copy(e), this.parameters = Object.assign({}, e.parameters), this
         }
     },
-    En = class r extends St {
+    yn = class r extends Et {
         constructor(e = 1, t = 32, i = 16, n = 0, a = Math.PI * 2, o = 0, s = Math.PI) {
             super(), this.type = "SphereGeometry", this.parameters = {
                 radius: e,
                 widthSegments: t,
                 heightSegments: i,
                 phiStart: n,
                 phiLength: a,
                 thetaStart: o,
                 thetaLength: s
             }, t = Math.max(3, Math.floor(t)), i = Math.max(2, Math.floor(i));
             let l = Math.min(o + s, Math.PI),
                 c = 0,
-                u = [],
-                p = new D,
-                f = new D,
+                h = [],
+                p = new U,
+                f = new U,
                 m = [],
                 _ = [],
                 M = [],
                 d = [];
-            for (let h = 0; h <= i; h++) {
-                let w = [],
-                    x = h / i,
-                    R = 0;
-                h === 0 && o === 0 ? R = .5 / t : h === i && l === Math.PI && (R = -.5 / t);
-                for (let U = 0; U <= t; U++) {
-                    let A = U / t;
-                    p.x = -e * Math.cos(n + A * a) * Math.sin(o + x * s), p.y = e * Math.cos(o + x * s), p.z = e * Math.sin(n + A * a) * Math.sin(o + x * s), _.push(p.x, p.y, p.z), f.copy(p).normalize(), M.push(f.x, f.y, f.z), d.push(A + R, 1 - x), w.push(c++)
-                }
-                u.push(w)
-            }
-            for (let h = 0; h < i; h++)
-                for (let w = 0; w < t; w++) {
-                    let x = u[h][w + 1],
-                        R = u[h][w],
-                        U = u[h + 1][w],
-                        A = u[h + 1][w + 1];
-                    (h !== 0 || o > 0) && m.push(x, R, A), (h !== i - 1 || l < Math.PI) && m.push(R, U, A)
+            for (let u = 0; u <= i; u++) {
+                let T = [],
+                    x = u / i,
+                    A = 0;
+                u === 0 && o === 0 ? A = .5 / t : u === i && l === Math.PI && (A = -.5 / t);
+                for (let D = 0; D <= t; D++) {
+                    let R = D / t;
+                    p.x = -e * Math.cos(n + R * a) * Math.sin(o + x * s), p.y = e * Math.cos(o + x * s), p.z = e * Math.sin(n + R * a) * Math.sin(o + x * s), _.push(p.x, p.y, p.z), f.copy(p).normalize(), M.push(f.x, f.y, f.z), d.push(R + A, 1 - x), T.push(c++)
+                }
+                h.push(T)
+            }
+            for (let u = 0; u < i; u++)
+                for (let T = 0; T < t; T++) {
+                    let x = h[u][T + 1],
+                        A = h[u][T],
+                        D = h[u + 1][T],
+                        R = h[u + 1][T + 1];
+                    (u !== 0 || o > 0) && m.push(x, A, R), (u !== i - 1 || l < Math.PI) && m.push(A, D, R)
                 }
             this.setIndex(m), this.setAttribute("position", new rt(_, 3)), this.setAttribute("normal", new rt(M, 3)), this.setAttribute("uv", new rt(d, 2))
         }
         copy(e) {
             return super.copy(e), this.parameters = Object.assign({}, e.parameters), this
         }
         static fromJSON(e) {
             return new r(e.radius, e.widthSegments, e.heightSegments, e.phiStart, e.phiLength, e.thetaStart, e.thetaLength)
         }
     },
-    Sn = class {
+    En = class {
         constructor(e = 1, t = 0, i = 0) {
             return this.radius = e, this.phi = t, this.theta = i, this
         }
         set(e, t, i) {
             return this.radius = e, this.phi = t, this.theta = i, this
         }
         copy(e) {
@@ -15082,18 +15082,18 @@
         setFromCartesianCoords(e, t, i) {
             return this.radius = Math.sqrt(e * e + t * t + i * i), this.radius === 0 ? (this.theta = 0, this.phi = 0) : (this.theta = Math.atan2(e, i), this.phi = Math.acos(ft(t / this.radius, -1, 1))), this
         }
         clone() {
             return new this.constructor().copy(this)
         }
     },
-    wo = new D,
-    $r, ha, yn = class extends wt {
-        constructor(e = new D(0, 0, 1), t = new D(0, 0, 0), i = 1, n = 16776960, a = i * .2, o = a * .2) {
-            super(), this.type = "ArrowHelper", $r === void 0 && ($r = new St, $r.setAttribute("position", new rt([0, 0, 0, 0, 1, 0], 3)), ha = new za(0, .5, 1, 5, 1), ha.translate(0, -.5, 0)), this.position.copy(t), this.line = new br($r, new cr({
+    wo = new U,
+    $r, ha, Sn = class extends wt {
+        constructor(e = new U(0, 0, 1), t = new U(0, 0, 0), i = 1, n = 16776960, a = i * .2, o = a * .2) {
+            super(), this.type = "ArrowHelper", $r === void 0 && ($r = new Et, $r.setAttribute("position", new rt([0, 0, 0, 0, 1, 0], 3)), ha = new Ba(0, .5, 1, 5, 1), ha.translate(0, -.5, 0)), this.position.copy(t), this.line = new Tr($r, new cr({
                 color: n,
                 toneMapped: !1
             })), this.line.matrixAutoUpdate = !1, this.add(this.line), this.cone = new vt(ha, new di({
                 color: n,
                 toneMapped: !1
             })), this.cone.matrixAutoUpdate = !1, this.add(this.cone), this.setDirection(e), this.setLength(i, a, o)
         }
@@ -15130,535 +15130,535 @@
     },
     ua = {
         type: "start"
     },
     Ro = {
         type: "end"
     },
-    Qr = new Sr,
-    Co = new Bt,
+    Qr = new Er,
+    Co = new zt,
     gf = Math.cos(70 * gc.DEG2RAD),
-    Ha = class extends Jt {
+    Ga = class extends Jt {
         constructor(e, t) {
-            super(), this.object = e, this.domElement = t, this.domElement.style.touchAction = "none", this.enabled = !0, this.target = new D, this.cursor = new D, this.minDistance = 0, this.maxDistance = 1 / 0, this.minZoom = 0, this.maxZoom = 1 / 0, this.minTargetRadius = 0, this.maxTargetRadius = 1 / 0, this.minPolarAngle = 0, this.maxPolarAngle = Math.PI, this.minAzimuthAngle = -1 / 0, this.maxAzimuthAngle = 1 / 0, this.enableDamping = !1, this.dampingFactor = .05, this.enableZoom = !0, this.zoomSpeed = 1, this.enableRotate = !0, this.rotateSpeed = 1, this.enablePan = !0, this.panSpeed = 1, this.screenSpacePanning = !0, this.keyPanSpeed = 7, this.zoomToCursor = !1, this.autoRotate = !1, this.autoRotateSpeed = 2, this.keys = {
+            super(), this.object = e, this.domElement = t, this.domElement.style.touchAction = "none", this.enabled = !0, this.target = new U, this.cursor = new U, this.minDistance = 0, this.maxDistance = 1 / 0, this.minZoom = 0, this.maxZoom = 1 / 0, this.minTargetRadius = 0, this.maxTargetRadius = 1 / 0, this.minPolarAngle = 0, this.maxPolarAngle = Math.PI, this.minAzimuthAngle = -1 / 0, this.maxAzimuthAngle = 1 / 0, this.enableDamping = !1, this.dampingFactor = .05, this.enableZoom = !0, this.zoomSpeed = 1, this.enableRotate = !0, this.rotateSpeed = 1, this.enablePan = !0, this.panSpeed = 1, this.screenSpacePanning = !0, this.keyPanSpeed = 7, this.zoomToCursor = !1, this.autoRotate = !1, this.autoRotateSpeed = 2, this.keys = {
                 LEFT: "ArrowLeft",
                 UP: "ArrowUp",
                 RIGHT: "ArrowRight",
                 BOTTOM: "ArrowDown"
             }, this.mouseButtons = {
-                LEFT: Ui.ROTATE,
-                MIDDLE: Ui.DOLLY,
-                RIGHT: Ui.PAN
+                LEFT: Di.ROTATE,
+                MIDDLE: Di.DOLLY,
+                RIGHT: Di.PAN
             }, this.touches = {
-                ONE: Di.ROTATE,
-                TWO: Di.DOLLY_PAN
+                ONE: Ui.ROTATE,
+                TWO: Ui.DOLLY_PAN
             }, this.target0 = this.target.clone(), this.position0 = this.object.position.clone(), this.zoom0 = this.object.zoom, this._domElementKeyEvents = null, this.getPolarAngle = function() {
                 return s.phi
             }, this.getAzimuthalAngle = function() {
                 return s.theta
             }, this.getDistance = function() {
                 return this.object.position.distanceTo(this.target)
-            }, this.listenToKeyEvents = function(b) {
-                b.addEventListener("keydown", ye), this._domElementKeyEvents = b
+            }, this.listenToKeyEvents = function(S) {
+                S.addEventListener("keydown", Me), this._domElementKeyEvents = S
             }, this.stopListenToKeyEvents = function() {
-                this._domElementKeyEvents.removeEventListener("keydown", ye), this._domElementKeyEvents = null
+                this._domElementKeyEvents.removeEventListener("keydown", Me), this._domElementKeyEvents = null
             }, this.saveState = function() {
                 i.target0.copy(i.target), i.position0.copy(i.object.position), i.zoom0 = i.object.zoom
             }, this.reset = function() {
                 i.target.copy(i.target0), i.object.position.copy(i.position0), i.object.zoom = i.zoom0, i.object.updateProjectionMatrix(), i.dispatchEvent(Ao), i.update(), a = n.NONE
             }, this.update = function() {
-                let b = new D,
-                    $ = new Qt().setFromUnitVectors(e.up, new D(0, 1, 0)),
+                let S = new U,
+                    $ = new Qt().setFromUnitVectors(e.up, new U(0, 1, 0)),
                     oe = $.clone().invert(),
-                    Ae = new D,
-                    L = new Qt,
-                    re = new D,
-                    O = 2 * Math.PI;
+                    Ce = new U,
+                    C = new Qt,
+                    re = new U,
+                    F = 2 * Math.PI;
                 return function(le = null) {
                     let se = i.object.position;
-                    b.copy(se).sub(i.target), b.applyQuaternion($), s.setFromVector3(b), i.autoRotate && a === n.NONE && V(v(le)), i.enableDamping ? (s.theta += l.theta * i.dampingFactor, s.phi += l.phi * i.dampingFactor) : (s.theta += l.theta, s.phi += l.phi);
-                    let Ge = i.minAzimuthAngle,
+                    S.copy(se).sub(i.target), S.applyQuaternion($), s.setFromVector3(S), i.autoRotate && a === n.NONE && W(v(le)), i.enableDamping ? (s.theta += l.theta * i.dampingFactor, s.phi += l.phi * i.dampingFactor) : (s.theta += l.theta, s.phi += l.phi);
+                    let He = i.minAzimuthAngle,
                         Ve = i.maxAzimuthAngle;
-                    isFinite(Ge) && isFinite(Ve) && (Ge < -Math.PI ? Ge += O : Ge > Math.PI && (Ge -= O), Ve < -Math.PI ? Ve += O : Ve > Math.PI && (Ve -= O), Ge <= Ve ? s.theta = Math.max(Ge, Math.min(Ve, s.theta)) : s.theta = s.theta > (Ge + Ve) / 2 ? Math.max(Ge, s.theta) : Math.min(Ve, s.theta)), s.phi = Math.max(i.minPolarAngle, Math.min(i.maxPolarAngle, s.phi)), s.makeSafe(), i.enableDamping === !0 ? i.target.addScaledVector(u, i.dampingFactor) : i.target.add(u), i.target.sub(i.cursor), i.target.clampLength(i.minTargetRadius, i.maxTargetRadius), i.target.add(i.cursor);
+                    isFinite(He) && isFinite(Ve) && (He < -Math.PI ? He += F : He > Math.PI && (He -= F), Ve < -Math.PI ? Ve += F : Ve > Math.PI && (Ve -= F), He <= Ve ? s.theta = Math.max(He, Math.min(Ve, s.theta)) : s.theta = s.theta > (He + Ve) / 2 ? Math.max(He, s.theta) : Math.min(Ve, s.theta)), s.phi = Math.max(i.minPolarAngle, Math.min(i.maxPolarAngle, s.phi)), s.makeSafe(), i.enableDamping === !0 ? i.target.addScaledVector(h, i.dampingFactor) : i.target.add(h), i.target.sub(i.cursor), i.target.clampLength(i.minTargetRadius, i.maxTargetRadius), i.target.add(i.cursor);
                     let Ke = !1;
-                    if (i.zoomToCursor && A || i.object.isOrthographicCamera) s.radius = te(s.radius);
+                    if (i.zoomToCursor && R || i.object.isOrthographicCamera) s.radius = ee(s.radius);
                     else {
-                        let $e = s.radius;
-                        s.radius = te(s.radius * c), Ke = $e != s.radius
+                        let Qe = s.radius;
+                        s.radius = ee(s.radius * c), Ke = Qe != s.radius
                     }
-                    if (b.setFromSpherical(s), b.applyQuaternion(oe), se.copy(i.target).add(b), i.object.lookAt(i.target), i.enableDamping === !0 ? (l.theta *= 1 - i.dampingFactor, l.phi *= 1 - i.dampingFactor, u.multiplyScalar(1 - i.dampingFactor)) : (l.set(0, 0, 0), u.set(0, 0, 0)), i.zoomToCursor && A) {
-                        let $e = null;
+                    if (S.setFromSpherical(s), S.applyQuaternion(oe), se.copy(i.target).add(S), i.object.lookAt(i.target), i.enableDamping === !0 ? (l.theta *= 1 - i.dampingFactor, l.phi *= 1 - i.dampingFactor, h.multiplyScalar(1 - i.dampingFactor)) : (l.set(0, 0, 0), h.set(0, 0, 0)), i.zoomToCursor && R) {
+                        let Qe = null;
                         if (i.object.isPerspectiveCamera) {
-                            let je = b.length();
-                            $e = te(je * c);
-                            let tt = je - $e;
-                            i.object.position.addScaledVector(R, tt), i.object.updateMatrixWorld(), Ke = !!tt
+                            let je = S.length();
+                            Qe = ee(je * c);
+                            let tt = je - Qe;
+                            i.object.position.addScaledVector(A, tt), i.object.updateMatrixWorld(), Ke = !!tt
                         } else if (i.object.isOrthographicCamera) {
-                            let je = new D(U.x, U.y, 0);
+                            let je = new U(D.x, D.y, 0);
                             je.unproject(i.object);
                             let tt = i.object.zoom;
                             i.object.zoom = Math.max(i.minZoom, Math.min(i.maxZoom, i.object.zoom / c)), i.object.updateProjectionMatrix(), Ke = tt !== i.object.zoom;
-                            let yt = new D(U.x, U.y, 0);
-                            yt.unproject(i.object), i.object.position.sub(yt).add(je), i.object.updateMatrixWorld(), $e = b.length()
+                            let St = new U(D.x, D.y, 0);
+                            St.unproject(i.object), i.object.position.sub(St).add(je), i.object.updateMatrixWorld(), Qe = S.length()
                         } else console.warn("WARNING: OrbitControls.js encountered an unknown camera type - zoom to cursor disabled."), i.zoomToCursor = !1;
-                        $e !== null && (this.screenSpacePanning ? i.target.set(0, 0, -1).transformDirection(i.object.matrix).multiplyScalar($e).add(i.object.position) : (Qr.origin.copy(i.object.position), Qr.direction.set(0, 0, -1).transformDirection(i.object.matrix), Math.abs(i.object.up.dot(Qr.direction)) < gf ? e.lookAt(i.target) : (Co.setFromNormalAndCoplanarPoint(i.object.up, i.target), Qr.intersectPlane(Co, i.target))))
+                        Qe !== null && (this.screenSpacePanning ? i.target.set(0, 0, -1).transformDirection(i.object.matrix).multiplyScalar(Qe).add(i.object.position) : (Qr.origin.copy(i.object.position), Qr.direction.set(0, 0, -1).transformDirection(i.object.matrix), Math.abs(i.object.up.dot(Qr.direction)) < gf ? e.lookAt(i.target) : (Co.setFromNormalAndCoplanarPoint(i.object.up, i.target), Qr.intersectPlane(Co, i.target))))
                     } else if (i.object.isOrthographicCamera) {
-                        let $e = i.object.zoom;
-                        i.object.zoom = Math.max(i.minZoom, Math.min(i.maxZoom, i.object.zoom / c)), $e !== i.object.zoom && (i.object.updateProjectionMatrix(), Ke = !0)
+                        let Qe = i.object.zoom;
+                        i.object.zoom = Math.max(i.minZoom, Math.min(i.maxZoom, i.object.zoom / c)), Qe !== i.object.zoom && (i.object.updateProjectionMatrix(), Ke = !0)
                     }
-                    return c = 1, A = !1, Ke || Ae.distanceToSquared(i.object.position) > o || 8 * (1 - L.dot(i.object.quaternion)) > o || re.distanceToSquared(i.target) > o ? (i.dispatchEvent(Ao), Ae.copy(i.object.position), L.copy(i.object.quaternion), re.copy(i.target), !0) : !1
+                    return c = 1, R = !1, Ke || Ce.distanceToSquared(i.object.position) > o || 8 * (1 - C.dot(i.object.quaternion)) > o || re.distanceToSquared(i.target) > o ? (i.dispatchEvent(Ao), Ce.copy(i.object.position), C.copy(i.object.quaternion), re.copy(i.target), !0) : !1
                 }
             }(), this.dispose = function() {
-                i.domElement.removeEventListener("contextmenu", Ie), i.domElement.removeEventListener("pointerdown", de), i.domElement.removeEventListener("pointercancel", S), i.domElement.removeEventListener("wheel", Y), i.domElement.removeEventListener("pointermove", Ne), i.domElement.removeEventListener("pointerup", S), i.domElement.getRootNode().removeEventListener("keydown", J, {
+                i.domElement.removeEventListener("contextmenu", Ie), i.domElement.removeEventListener("pointerdown", Re), i.domElement.removeEventListener("pointercancel", E), i.domElement.removeEventListener("wheel", X), i.domElement.removeEventListener("pointermove", xe), i.domElement.removeEventListener("pointerup", E), i.domElement.getRootNode().removeEventListener("keydown", J, {
                     capture: !0
-                }), i._domElementKeyEvents !== null && (i._domElementKeyEvents.removeEventListener("keydown", ye), i._domElementKeyEvents = null)
+                }), i._domElementKeyEvents !== null && (i._domElementKeyEvents.removeEventListener("keydown", Me), i._domElementKeyEvents = null)
             };
             let i = this,
                 n = {
                     NONE: -1,
                     ROTATE: 0,
                     DOLLY: 1,
                     PAN: 2,
                     TOUCH_ROTATE: 3,
                     TOUCH_PAN: 4,
                     TOUCH_DOLLY_PAN: 5,
                     TOUCH_DOLLY_ROTATE: 6
                 },
                 a = n.NONE,
                 o = 1e-6,
-                s = new Sn,
-                l = new Sn,
+                s = new En,
+                l = new En,
                 c = 1,
-                u = new D,
-                p = new De,
-                f = new De,
-                m = new De,
-                _ = new De,
-                M = new De,
-                d = new De,
-                h = new De,
-                w = new De,
-                x = new De,
-                R = new D,
-                U = new De,
-                A = !1,
-                y = [],
-                C = {},
-                Z = !1;
+                h = new U,
+                p = new Ue,
+                f = new Ue,
+                m = new Ue,
+                _ = new Ue,
+                M = new Ue,
+                d = new Ue,
+                u = new Ue,
+                T = new Ue,
+                x = new Ue,
+                A = new U,
+                D = new Ue,
+                R = !1,
+                b = [],
+                P = {},
+                I = !1;
 
-            function v(b) {
-                return b !== null ? 2 * Math.PI / 60 * i.autoRotateSpeed * b : 2 * Math.PI / 60 / 60 * i.autoRotateSpeed
+            function v(S) {
+                return S !== null ? 2 * Math.PI / 60 * i.autoRotateSpeed * S : 2 * Math.PI / 60 / 60 * i.autoRotateSpeed
             }
 
-            function T(b) {
-                let $ = Math.abs(b * .01);
+            function w(S) {
+                let $ = Math.abs(S * .01);
                 return Math.pow(.95, i.zoomSpeed * $)
             }
 
-            function V(b) {
-                l.theta -= b
+            function W(S) {
+                l.theta -= S
             }
 
-            function K(b) {
-                l.phi -= b
+            function K(S) {
+                l.phi -= S
             }
-            let P = function() {
-                    let b = new D;
+            let L = function() {
+                    let S = new U;
                     return function($, oe) {
-                        b.setFromMatrixColumn(oe, 0), b.multiplyScalar(-$), u.add(b)
+                        S.setFromMatrixColumn(oe, 0), S.multiplyScalar(-$), h.add(S)
                     }
                 }(),
-                X = function() {
-                    let b = new D;
+                j = function() {
+                    let S = new U;
                     return function($, oe) {
-                        i.screenSpacePanning === !0 ? b.setFromMatrixColumn(oe, 1) : (b.setFromMatrixColumn(oe, 0), b.crossVectors(i.object.up, b)), b.multiplyScalar($), u.add(b)
+                        i.screenSpacePanning === !0 ? S.setFromMatrixColumn(oe, 1) : (S.setFromMatrixColumn(oe, 0), S.crossVectors(i.object.up, S)), S.multiplyScalar($), h.add(S)
                     }
                 }(),
                 k = function() {
-                    let b = new D;
+                    let S = new U;
                     return function($, oe) {
-                        let Ae = i.domElement;
+                        let Ce = i.domElement;
                         if (i.object.isPerspectiveCamera) {
-                            let L = i.object.position;
-                            b.copy(L).sub(i.target);
-                            let re = b.length();
-                            re *= Math.tan(i.object.fov / 2 * Math.PI / 180), P(2 * $ * re / Ae.clientHeight, i.object.matrix), X(2 * oe * re / Ae.clientHeight, i.object.matrix)
-                        } else i.object.isOrthographicCamera ? (P($ * (i.object.right - i.object.left) / i.object.zoom / Ae.clientWidth, i.object.matrix), X(oe * (i.object.top - i.object.bottom) / i.object.zoom / Ae.clientHeight, i.object.matrix)) : (console.warn("WARNING: OrbitControls.js encountered an unknown camera type - pan disabled."), i.enablePan = !1)
+                            let C = i.object.position;
+                            S.copy(C).sub(i.target);
+                            let re = S.length();
+                            re *= Math.tan(i.object.fov / 2 * Math.PI / 180), L(2 * $ * re / Ce.clientHeight, i.object.matrix), j(2 * oe * re / Ce.clientHeight, i.object.matrix)
+                        } else i.object.isOrthographicCamera ? (L($ * (i.object.right - i.object.left) / i.object.zoom / Ce.clientWidth, i.object.matrix), j(oe * (i.object.top - i.object.bottom) / i.object.zoom / Ce.clientHeight, i.object.matrix)) : (console.warn("WARNING: OrbitControls.js encountered an unknown camera type - pan disabled."), i.enablePan = !1)
                     }
                 }();
 
-            function j(b) {
-                i.object.isPerspectiveCamera || i.object.isOrthographicCamera ? c /= b : (console.warn("WARNING: OrbitControls.js encountered an unknown camera type - dolly/zoom disabled."), i.enableZoom = !1)
+            function Y(S) {
+                i.object.isPerspectiveCamera || i.object.isOrthographicCamera ? c /= S : (console.warn("WARNING: OrbitControls.js encountered an unknown camera type - dolly/zoom disabled."), i.enableZoom = !1)
             }
 
-            function q(b) {
-                i.object.isPerspectiveCamera || i.object.isOrthographicCamera ? c *= b : (console.warn("WARNING: OrbitControls.js encountered an unknown camera type - dolly/zoom disabled."), i.enableZoom = !1)
+            function q(S) {
+                i.object.isPerspectiveCamera || i.object.isOrthographicCamera ? c *= S : (console.warn("WARNING: OrbitControls.js encountered an unknown camera type - dolly/zoom disabled."), i.enableZoom = !1)
             }
 
-            function W(b, $) {
+            function Z(S, $) {
                 if (!i.zoomToCursor) return;
-                A = !0;
+                R = !0;
                 let oe = i.domElement.getBoundingClientRect(),
-                    Ae = b - oe.left,
-                    L = $ - oe.top,
+                    Ce = S - oe.left,
+                    C = $ - oe.top,
                     re = oe.width,
-                    O = oe.height;
-                U.x = Ae / re * 2 - 1, U.y = -(L / O) * 2 + 1, R.set(U.x, U.y, 1).unproject(i.object).sub(i.object.position).normalize()
+                    F = oe.height;
+                D.x = Ce / re * 2 - 1, D.y = -(C / F) * 2 + 1, A.set(D.x, D.y, 1).unproject(i.object).sub(i.object.position).normalize()
             }
 
-            function te(b) {
-                return Math.max(i.minDistance, Math.min(i.maxDistance, b))
+            function ee(S) {
+                return Math.max(i.minDistance, Math.min(i.maxDistance, S))
             }
 
-            function ee(b) {
-                p.set(b.clientX, b.clientY)
+            function ie(S) {
+                p.set(S.clientX, S.clientY)
             }
 
-            function pe(b) {
-                W(b.clientX, b.clientX), h.set(b.clientX, b.clientY)
+            function de(S) {
+                Z(S.clientX, S.clientX), u.set(S.clientX, S.clientY)
             }
 
-            function xe(b) {
-                _.set(b.clientX, b.clientY)
+            function ge(S) {
+                _.set(S.clientX, S.clientY)
             }
 
-            function H(b) {
-                f.set(b.clientX, b.clientY), m.subVectors(f, p).multiplyScalar(i.rotateSpeed);
+            function V(S) {
+                f.set(S.clientX, S.clientY), m.subVectors(f, p).multiplyScalar(i.rotateSpeed);
                 let $ = i.domElement;
-                V(2 * Math.PI * m.x / $.clientHeight), K(2 * Math.PI * m.y / $.clientHeight), p.copy(f), i.update()
+                W(2 * Math.PI * m.x / $.clientHeight), K(2 * Math.PI * m.y / $.clientHeight), p.copy(f), i.update()
             }
 
-            function ie(b) {
-                w.set(b.clientX, b.clientY), x.subVectors(w, h), x.y > 0 ? j(T(x.y)) : x.y < 0 && q(T(x.y)), h.copy(w), i.update()
+            function te(S) {
+                T.set(S.clientX, S.clientY), x.subVectors(T, u), x.y > 0 ? Y(w(x.y)) : x.y < 0 && q(w(x.y)), u.copy(T), i.update()
             }
 
-            function fe(b) {
-                M.set(b.clientX, b.clientY), d.subVectors(M, _).multiplyScalar(i.panSpeed), k(d.x, d.y), _.copy(M), i.update()
+            function pe(S) {
+                M.set(S.clientX, S.clientY), d.subVectors(M, _).multiplyScalar(i.panSpeed), k(d.x, d.y), _.copy(M), i.update()
             }
 
-            function Te(b) {
-                W(b.clientX, b.clientY), b.deltaY < 0 ? q(T(b.deltaY)) : b.deltaY > 0 && j(T(b.deltaY)), i.update()
+            function we(S) {
+                Z(S.clientX, S.clientY), S.deltaY < 0 ? q(w(S.deltaY)) : S.deltaY > 0 && Y(w(S.deltaY)), i.update()
             }
 
-            function _e(b) {
+            function _e(S) {
                 let $ = !1;
-                switch (b.code) {
+                switch (S.code) {
                     case i.keys.UP:
-                        b.ctrlKey || b.metaKey || b.shiftKey ? K(2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(0, i.keyPanSpeed), $ = !0;
+                        S.ctrlKey || S.metaKey || S.shiftKey ? K(2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(0, i.keyPanSpeed), $ = !0;
                         break;
                     case i.keys.BOTTOM:
-                        b.ctrlKey || b.metaKey || b.shiftKey ? K(-2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(0, -i.keyPanSpeed), $ = !0;
+                        S.ctrlKey || S.metaKey || S.shiftKey ? K(-2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(0, -i.keyPanSpeed), $ = !0;
                         break;
                     case i.keys.LEFT:
-                        b.ctrlKey || b.metaKey || b.shiftKey ? V(2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(i.keyPanSpeed, 0), $ = !0;
+                        S.ctrlKey || S.metaKey || S.shiftKey ? W(2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(i.keyPanSpeed, 0), $ = !0;
                         break;
                     case i.keys.RIGHT:
-                        b.ctrlKey || b.metaKey || b.shiftKey ? V(-2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(-i.keyPanSpeed, 0), $ = !0;
+                        S.ctrlKey || S.metaKey || S.shiftKey ? W(-2 * Math.PI * i.rotateSpeed / i.domElement.clientHeight) : k(-i.keyPanSpeed, 0), $ = !0;
                         break
                 }
-                $ && (b.preventDefault(), i.update())
+                $ && (S.preventDefault(), i.update())
             }
 
-            function me(b) {
-                if (y.length === 1) p.set(b.pageX, b.pageY);
+            function fe(S) {
+                if (b.length === 1) p.set(S.pageX, S.pageY);
                 else {
-                    let $ = ge(b),
-                        oe = .5 * (b.pageX + $.x),
-                        Ae = .5 * (b.pageY + $.y);
-                    p.set(oe, Ae)
+                    let $ = me(S),
+                        oe = .5 * (S.pageX + $.x),
+                        Ce = .5 * (S.pageY + $.y);
+                    p.set(oe, Ce)
                 }
             }
 
-            function Xe(b) {
-                if (y.length === 1) _.set(b.pageX, b.pageY);
+            function Xe(S) {
+                if (b.length === 1) _.set(S.pageX, S.pageY);
                 else {
-                    let $ = ge(b),
-                        oe = .5 * (b.pageX + $.x),
-                        Ae = .5 * (b.pageY + $.y);
-                    _.set(oe, Ae)
+                    let $ = me(S),
+                        oe = .5 * (S.pageX + $.x),
+                        Ce = .5 * (S.pageY + $.y);
+                    _.set(oe, Ce)
                 }
             }
 
-            function we(b) {
-                let $ = ge(b),
-                    oe = b.pageX - $.x,
-                    Ae = b.pageY - $.y,
-                    L = Math.sqrt(oe * oe + Ae * Ae);
-                h.set(0, L)
+            function Ae(S) {
+                let $ = me(S),
+                    oe = S.pageX - $.x,
+                    Ce = S.pageY - $.y,
+                    C = Math.sqrt(oe * oe + Ce * Ce);
+                u.set(0, C)
             }
 
-            function I(b) {
-                i.enableZoom && we(b), i.enablePan && Xe(b)
+            function O(S) {
+                i.enableZoom && Ae(S), i.enablePan && Xe(S)
             }
 
-            function Qe(b) {
-                i.enableZoom && we(b), i.enableRotate && me(b)
+            function Je(S) {
+                i.enableZoom && Ae(S), i.enableRotate && fe(S)
             }
 
-            function ve(b) {
-                if (y.length == 1) f.set(b.pageX, b.pageY);
+            function ve(S) {
+                if (b.length == 1) f.set(S.pageX, S.pageY);
                 else {
-                    let oe = ge(b),
-                        Ae = .5 * (b.pageX + oe.x),
-                        L = .5 * (b.pageY + oe.y);
-                    f.set(Ae, L)
+                    let oe = me(S),
+                        Ce = .5 * (S.pageX + oe.x),
+                        C = .5 * (S.pageY + oe.y);
+                    f.set(Ce, C)
                 }
                 m.subVectors(f, p).multiplyScalar(i.rotateSpeed);
                 let $ = i.domElement;
-                V(2 * Math.PI * m.x / $.clientHeight), K(2 * Math.PI * m.y / $.clientHeight), p.copy(f)
+                W(2 * Math.PI * m.x / $.clientHeight), K(2 * Math.PI * m.y / $.clientHeight), p.copy(f)
             }
 
-            function Ue(b) {
-                if (y.length === 1) M.set(b.pageX, b.pageY);
+            function Pe(S) {
+                if (b.length === 1) M.set(S.pageX, S.pageY);
                 else {
-                    let $ = ge(b),
-                        oe = .5 * (b.pageX + $.x),
-                        Ae = .5 * (b.pageY + $.y);
-                    M.set(oe, Ae)
+                    let $ = me(S),
+                        oe = .5 * (S.pageX + $.x),
+                        Ce = .5 * (S.pageY + $.y);
+                    M.set(oe, Ce)
                 }
                 d.subVectors(M, _).multiplyScalar(i.panSpeed), k(d.x, d.y), _.copy(M)
             }
 
-            function Me(b) {
-                let $ = ge(b),
-                    oe = b.pageX - $.x,
-                    Ae = b.pageY - $.y,
-                    L = Math.sqrt(oe * oe + Ae * Ae);
-                w.set(0, L), x.set(0, Math.pow(w.y / h.y, i.zoomSpeed)), j(x.y), h.copy(w);
-                let re = (b.pageX + $.x) * .5,
-                    O = (b.pageY + $.y) * .5;
-                W(re, O)
+            function Se(S) {
+                let $ = me(S),
+                    oe = S.pageX - $.x,
+                    Ce = S.pageY - $.y,
+                    C = Math.sqrt(oe * oe + Ce * Ce);
+                T.set(0, C), x.set(0, Math.pow(T.y / u.y, i.zoomSpeed)), Y(x.y), u.copy(T);
+                let re = (S.pageX + $.x) * .5,
+                    F = (S.pageY + $.y) * .5;
+                Z(re, F)
             }
 
-            function Le(b) {
-                i.enableZoom && Me(b), i.enablePan && Ue(b)
+            function Ne(S) {
+                i.enableZoom && Se(S), i.enablePan && Pe(S)
             }
 
-            function be(b) {
-                i.enableZoom && Me(b), i.enableRotate && ve(b)
+            function be(S) {
+                i.enableZoom && Se(S), i.enableRotate && ve(S)
             }
 
-            function de(b) {
-                i.enabled !== !1 && (y.length === 0 && (i.domElement.setPointerCapture(b.pointerId), i.domElement.addEventListener("pointermove", Ne), i.domElement.addEventListener("pointerup", S)), !ze(b) && (ne(b), b.pointerType === "touch" ? ae(b) : g(b)))
+            function Re(S) {
+                i.enabled !== !1 && (b.length === 0 && (i.domElement.setPointerCapture(S.pointerId), i.domElement.addEventListener("pointermove", xe), i.domElement.addEventListener("pointerup", E)), !Be(S) && (ne(S), S.pointerType === "touch" ? ae(S) : g(S)))
             }
 
-            function Ne(b) {
-                i.enabled !== !1 && (b.pointerType === "touch" ? he(b) : B(b))
+            function xe(S) {
+                i.enabled !== !1 && (S.pointerType === "touch" ? he(S) : B(S))
             }
 
-            function S(b) {
-                switch (Je(b), y.length) {
+            function E(S) {
+                switch ($e(S), b.length) {
                     case 0:
-                        i.domElement.releasePointerCapture(b.pointerId), i.domElement.removeEventListener("pointermove", Ne), i.domElement.removeEventListener("pointerup", S), i.dispatchEvent(Ro), a = n.NONE;
+                        i.domElement.releasePointerCapture(S.pointerId), i.domElement.removeEventListener("pointermove", xe), i.domElement.removeEventListener("pointerup", E), i.dispatchEvent(Ro), a = n.NONE;
                         break;
                     case 1:
-                        let $ = y[0],
-                            oe = C[$];
+                        let $ = b[0],
+                            oe = P[$];
                         ae({
                             pointerId: $,
                             pageX: oe.x,
                             pageY: oe.y
                         });
                         break
                 }
             }
 
-            function g(b) {
+            function g(S) {
                 let $;
-                switch (b.button) {
+                switch (S.button) {
                     case 0:
                         $ = i.mouseButtons.LEFT;
                         break;
                     case 1:
                         $ = i.mouseButtons.MIDDLE;
                         break;
                     case 2:
                         $ = i.mouseButtons.RIGHT;
                         break;
                     default:
                         $ = -1
                 }
                 switch ($) {
-                    case Ui.DOLLY:
+                    case Di.DOLLY:
                         if (i.enableZoom === !1) return;
-                        pe(b), a = n.DOLLY;
+                        de(S), a = n.DOLLY;
                         break;
-                    case Ui.ROTATE:
-                        if (b.ctrlKey || b.metaKey || b.shiftKey) {
+                    case Di.ROTATE:
+                        if (S.ctrlKey || S.metaKey || S.shiftKey) {
                             if (i.enablePan === !1) return;
-                            xe(b), a = n.PAN
+                            ge(S), a = n.PAN
                         } else {
                             if (i.enableRotate === !1) return;
-                            ee(b), a = n.ROTATE
+                            ie(S), a = n.ROTATE
                         }
                         break;
-                    case Ui.PAN:
-                        if (b.ctrlKey || b.metaKey || b.shiftKey) {
+                    case Di.PAN:
+                        if (S.ctrlKey || S.metaKey || S.shiftKey) {
                             if (i.enableRotate === !1) return;
-                            ee(b), a = n.ROTATE
+                            ie(S), a = n.ROTATE
                         } else {
                             if (i.enablePan === !1) return;
-                            xe(b), a = n.PAN
+                            ge(S), a = n.PAN
                         }
                         break;
                     default:
                         a = n.NONE
                 }
                 a !== n.NONE && i.dispatchEvent(ua)
             }
 
-            function B(b) {
+            function B(S) {
                 switch (a) {
                     case n.ROTATE:
                         if (i.enableRotate === !1) return;
-                        H(b);
+                        V(S);
                         break;
                     case n.DOLLY:
                         if (i.enableZoom === !1) return;
-                        ie(b);
+                        te(S);
                         break;
                     case n.PAN:
                         if (i.enablePan === !1) return;
-                        fe(b);
+                        pe(S);
                         break
                 }
             }
 
-            function Y(b) {
-                i.enabled === !1 || i.enableZoom === !1 || a !== n.NONE || (b.preventDefault(), i.dispatchEvent(ua), Te(Q(b)), i.dispatchEvent(Ro))
+            function X(S) {
+                i.enabled === !1 || i.enableZoom === !1 || a !== n.NONE || (S.preventDefault(), i.dispatchEvent(ua), we(Q(S)), i.dispatchEvent(Ro))
             }
 
-            function Q(b) {
-                let $ = b.deltaMode,
+            function Q(S) {
+                let $ = S.deltaMode,
                     oe = {
-                        clientX: b.clientX,
-                        clientY: b.clientY,
-                        deltaY: b.deltaY
+                        clientX: S.clientX,
+                        clientY: S.clientY,
+                        deltaY: S.deltaY
                     };
                 switch ($) {
                     case 1:
                         oe.deltaY *= 16;
                         break;
                     case 2:
                         oe.deltaY *= 100;
                         break
                 }
-                return b.ctrlKey && !Z && (oe.deltaY *= 10), oe
+                return S.ctrlKey && !I && (oe.deltaY *= 10), oe
             }
 
-            function J(b) {
-                b.key === "Control" && (Z = !0, i.domElement.getRootNode().addEventListener("keyup", Ce, {
+            function J(S) {
+                S.key === "Control" && (I = !0, i.domElement.getRootNode().addEventListener("keyup", Ee, {
                     passive: !0,
                     capture: !0
                 }))
             }
 
-            function Ce(b) {
-                b.key === "Control" && (Z = !1, i.domElement.getRootNode().removeEventListener("keyup", Ce, {
+            function Ee(S) {
+                S.key === "Control" && (I = !1, i.domElement.getRootNode().removeEventListener("keyup", Ee, {
                     passive: !0,
                     capture: !0
                 }))
             }
 
-            function ye(b) {
-                i.enabled === !1 || i.enablePan === !1 || _e(b)
+            function Me(S) {
+                i.enabled === !1 || i.enablePan === !1 || _e(S)
             }
 
-            function ae(b) {
-                switch (Ee(b), y.length) {
+            function ae(S) {
+                switch (ye(S), b.length) {
                     case 1:
                         switch (i.touches.ONE) {
-                            case Di.ROTATE:
+                            case Ui.ROTATE:
                                 if (i.enableRotate === !1) return;
-                                me(b), a = n.TOUCH_ROTATE;
+                                fe(S), a = n.TOUCH_ROTATE;
                                 break;
-                            case Di.PAN:
+                            case Ui.PAN:
                                 if (i.enablePan === !1) return;
-                                Xe(b), a = n.TOUCH_PAN;
+                                Xe(S), a = n.TOUCH_PAN;
                                 break;
                             default:
                                 a = n.NONE
                         }
                         break;
                     case 2:
                         switch (i.touches.TWO) {
-                            case Di.DOLLY_PAN:
+                            case Ui.DOLLY_PAN:
                                 if (i.enableZoom === !1 && i.enablePan === !1) return;
-                                I(b), a = n.TOUCH_DOLLY_PAN;
+                                O(S), a = n.TOUCH_DOLLY_PAN;
                                 break;
-                            case Di.DOLLY_ROTATE:
+                            case Ui.DOLLY_ROTATE:
                                 if (i.enableZoom === !1 && i.enableRotate === !1) return;
-                                Qe(b), a = n.TOUCH_DOLLY_ROTATE;
+                                Je(S), a = n.TOUCH_DOLLY_ROTATE;
                                 break;
                             default:
                                 a = n.NONE
                         }
                         break;
                     default:
                         a = n.NONE
                 }
                 a !== n.NONE && i.dispatchEvent(ua)
             }
 
-            function he(b) {
-                switch (Ee(b), a) {
+            function he(S) {
+                switch (ye(S), a) {
                     case n.TOUCH_ROTATE:
                         if (i.enableRotate === !1) return;
-                        ve(b), i.update();
+                        ve(S), i.update();
                         break;
                     case n.TOUCH_PAN:
                         if (i.enablePan === !1) return;
-                        Ue(b), i.update();
+                        Pe(S), i.update();
                         break;
                     case n.TOUCH_DOLLY_PAN:
                         if (i.enableZoom === !1 && i.enablePan === !1) return;
-                        Le(b), i.update();
+                        Ne(S), i.update();
                         break;
                     case n.TOUCH_DOLLY_ROTATE:
                         if (i.enableZoom === !1 && i.enableRotate === !1) return;
-                        be(b), i.update();
+                        be(S), i.update();
                         break;
                     default:
                         a = n.NONE
                 }
             }
 
-            function Ie(b) {
-                i.enabled !== !1 && b.preventDefault()
+            function Ie(S) {
+                i.enabled !== !1 && S.preventDefault()
             }
 
-            function ne(b) {
-                y.push(b.pointerId)
+            function ne(S) {
+                b.push(S.pointerId)
             }
 
-            function Je(b) {
-                delete C[b.pointerId];
-                for (let $ = 0; $ < y.length; $++)
-                    if (y[$] == b.pointerId) {
-                        y.splice($, 1);
+            function $e(S) {
+                delete P[S.pointerId];
+                for (let $ = 0; $ < b.length; $++)
+                    if (b[$] == S.pointerId) {
+                        b.splice($, 1);
                         return
                     }
             }
 
-            function ze(b) {
-                for (let $ = 0; $ < y.length; $++)
-                    if (y[$] == b.pointerId) return !0;
+            function Be(S) {
+                for (let $ = 0; $ < b.length; $++)
+                    if (b[$] == S.pointerId) return !0;
                 return !1
             }
 
-            function Ee(b) {
-                let $ = C[b.pointerId];
-                $ === void 0 && ($ = new De, C[b.pointerId] = $), $.set(b.pageX, b.pageY)
+            function ye(S) {
+                let $ = P[S.pointerId];
+                $ === void 0 && ($ = new Ue, P[S.pointerId] = $), $.set(S.pageX, S.pageY)
             }
 
-            function ge(b) {
-                let $ = b.pointerId === y[0] ? y[1] : y[0];
-                return C[$]
+            function me(S) {
+                let $ = S.pointerId === b[0] ? b[1] : b[0];
+                return P[$]
             }
-            i.domElement.addEventListener("contextmenu", Ie), i.domElement.addEventListener("pointerdown", de), i.domElement.addEventListener("pointercancel", S), i.domElement.addEventListener("wheel", Y, {
+            i.domElement.addEventListener("contextmenu", Ie), i.domElement.addEventListener("pointerdown", Re), i.domElement.addEventListener("pointercancel", E), i.domElement.addEventListener("wheel", X, {
                 passive: !1
             }), i.domElement.getRootNode().addEventListener("keydown", J, {
                 passive: !0,
                 capture: !0
             }), this.update()
         }
     },
@@ -15672,224 +15672,225 @@
     vf = function(i, n, t) {
         var i = i,
             n = n;
         t == null && (t = {});
         var a = t.showAxes ?? !0,
             o = t.showBVectors ?? !0,
             s = t.showPathpoints ?? !1,
-            l = !1,
-            c = [],
-            u = new di({
+            l = t.disableInteractOverlay ?? !1,
+            c = !1,
+            h = [],
+            p = new di({
                 color: 13975119,
                 opacity: .5,
                 transparent: !0
             }),
-            p = new cr({
+            f = new cr({
                 color: 3355443,
                 opacity: 1,
                 transparent: !1,
                 linewidth: 1
             }),
-            f = new cr({
+            m = new cr({
                 color: 285405,
                 opacity: 1,
                 transparent: !1
             }),
-            m = new di({
+            _ = new di({
                 color: 3311805,
                 opacity: 1,
                 transparent: !1
             }),
-            _ = new di({
+            M = new di({
                 color: 8925746,
                 opacity: 1,
                 transparent: !1
             }),
-            M = null,
             d = null,
-            h = null;
+            u = null,
+            T = null;
         this.resizeRenderer = function() {
             if (i) {
-                var A = window.devicePixelRatio || 1,
-                    y = i.offsetWidth,
-                    C = i.offsetHeight;
-                h && (d.aspect = y / C, d.updateProjectionMatrix(), h.setSize(y * A, C * A), h.domElement.style.width = y + "px", h.domElement.style.height = C + "px", h.domElement.width = y * A, h.domElement.height = C * A, U())
+                var b = window.devicePixelRatio || 1,
+                    P = i.offsetWidth,
+                    I = i.offsetHeight;
+                T && (u.aspect = P / I, u.updateProjectionMatrix(), T.setSize(P * b, I * b), T.domElement.style.width = P + "px", T.domElement.style.height = I + "px", T.domElement.width = P * b, T.domElement.height = I * b, R())
             }
         };
-        var w = function(A, y) {
-                y = typeof y < "u" ? y : "#000000";
-                var C;
+        var x = function(b, P) {
+                P = typeof P < "u" ? P : "#000000";
+                var I;
                 {
-                    var C = document.createElement("div");
-                    C.style.position = "absolute", C.style.fontFamily = "'Helvetica Neue', Helvetica, Arial, sans-serif", C.style.color = y, C.style.width = 100, C.style.height = 100, C.style.fontSize = "12px", C.innerHTML = A, C.style.top = "-100px", C.style.left = "-100px", C.style.userSelect = "none", C.style.userSelect = "none", C.style.webkitUserSelect = "none", C.style.MozUserSelect = "none", C.setAttribute("unselectable", "on"), C.style.pointerEvents = "none"
+                    var I = document.createElement("div");
+                    I.style.position = "absolute", I.style.fontFamily = "'Helvetica Neue', Helvetica, Arial, sans-serif", I.style.color = P, I.style.width = 100, I.style.height = 100, I.style.fontSize = "12px", I.innerHTML = b, I.style.top = "-100px", I.style.left = "-100px", I.style.userSelect = "none", I.style.userSelect = "none", I.style.webkitUserSelect = "none", I.style.MozUserSelect = "none", I.setAttribute("unselectable", "on"), I.style.pointerEvents = "none"
                 }
-                return C
+                return I
             },
-            x = function(A) {
-                var y = document.createElement("div");
-                y.classList.add(A), y.style.position = "absolute", y.style.fontFamily = "'Helvetica Neue', Helvetica, Arial, sans-serif", y.style.zIndex = 1, y.style.width = "100%", y.style.height = "100%", y.style.display = "table", y.style.top = "0px", y.style.left = "0px", y.style.textAlign = "center", y.style.verticalAlign = "middle", y.style.userSelect = "none", y.style.userSelect = "none", y.style.webkitUserSelect = "none", y.style.MozUserSelect = "none", y.setAttribute("unselectable", "on");
-                var C = document.createElement("span");
-                return C.innerHTML = "Double click to toggle interaction", C.style.color = "rgb(80, 80, 80)", C.style.fontSize = "24px", C.style.fontWeight = "bold", C.style.backgroundColor = "rgba(230,230,230,0.5)", C.style.display = "table-cell", C.style.verticalAlign = "middle", C.style.lineHeight = "normal", C.style.userSelect = "none", C.style.userSelect = "none", C.style.webkitUserSelect = "none", C.style.MozUserSelect = "none", C.setAttribute("unselectable", "on"), C.onmouseover = function() {
+            A = function(b) {
+                var P = document.createElement("div");
+                P.classList.add(b), P.style.position = "absolute", P.style.fontFamily = "'Helvetica Neue', Helvetica, Arial, sans-serif", P.style.zIndex = 1, P.style.width = "100%", P.style.height = "100%", P.style.display = "table", P.style.top = "0px", P.style.left = "0px", P.style.textAlign = "center", P.style.verticalAlign = "middle", P.style.userSelect = "none", P.style.userSelect = "none", P.style.webkitUserSelect = "none", P.style.MozUserSelect = "none", P.setAttribute("unselectable", "on");
+                var I = document.createElement("span");
+                return I.innerHTML = "Double click to toggle interaction", I.style.color = "rgb(80, 80, 80)", I.style.fontSize = "24px", I.style.fontWeight = "bold", I.style.backgroundColor = "rgba(230,230,230,0.5)", I.style.display = "table-cell", I.style.verticalAlign = "middle", I.style.lineHeight = "normal", I.style.userSelect = "none", I.style.userSelect = "none", I.style.webkitUserSelect = "none", I.style.MozUserSelect = "none", I.setAttribute("unselectable", "on"), I.onmouseover = function() {
                     this.style.backgroundColor = "rgba(230,230,230,0.5)", this.innerHTML = "Double click to toggle interaction"
-                }, C.onmouseleave = function() {
+                }, I.onmouseleave = function() {
                     this.style.backgroundColor = "rgba(255,255,255,0.01)", this.innerHTML = ""
-                }, y.appendChild(C), y
+                }, P.appendChild(I), P
             };
-        this.loadBZ = function(A) {
-            if (A == null || Object.keys(A).length === 0 || i == null || i.id == "" || n == null) return;
-            var y = window.devicePixelRatio || 1;
+        this.loadBZ = function(b) {
+            if (b == null || Object.keys(b).length === 0 || i == null || i.id == "" || n == null) return;
+            var P = window.devicePixelRatio || 1;
             n.innerHTML = "";
-            for (var C = i; C.firstChild;) C.removeChild(C.firstChild);
-            c = [], M = new Fa;
-            let Z = C.offsetWidth,
-                v = C.offsetHeight;
-            d = new Mt(45, Z / v, .01, 1e3), d.position.z = 3, h = new Mn({
+            for (var I = i; I.firstChild;) I.removeChild(I.firstChild);
+            h = [], d = new Fa;
+            let v = I.offsetWidth,
+                w = I.offsetHeight;
+            u = new Mt(45, v / w, .01, 1e3), u.position.z = 3, T = new Mn({
                 alpha: !0,
                 preserveDrawingBuffer: !0
-            }), h.setClearColor(16777215, 0), h.setSize(Z * y, v * y), h.domElement.style.width = Z + "px", h.domElement.style.height = v + "px", h.domElement.width = Z * y, h.domElement.height = v * y, C.appendChild(h.domElement);
-            let T = new Ha(d, h.domElement);
-            T.addEventListener("change", U), T.enableDamping = !0, T.dampingFactor = .25, T.enableZoom = !0;
-            let V = A.kpoints,
-                K = A.b1,
-                P = A.b2,
-                X = A.b3,
-                k = Math.sqrt(Math.max(Math.pow(K[0], 2) + Math.pow(K[1], 2) + Math.pow(K[2], 2), Math.pow(P[0], 2) + Math.pow(P[1], 2) + Math.pow(P[2], 2), Math.pow(X[0], 2) + Math.pow(X[1], 2) + Math.pow(X[2], 2)));
-            var j = k * 1.5;
-            d.position.z = k * 3;
-            let q = A.faces_data;
-            for (var W in V) {
-                let de = V[W],
-                    Ne = .02 * k;
-                var te = new En(Ne, 16, 16),
-                    ee = new vt(te, m);
-                ee.translateX(de[0]), ee.translateY(de[1]), ee.translateZ(de[2]), M.add(ee), W = _f(W, l);
-                var pe = w(W);
-                C.appendChild(pe), c.push([new D(de[0], de[1], de[2]), pe])
+            }), T.setClearColor(16777215, 0), T.setSize(v * P, w * P), T.domElement.style.width = v + "px", T.domElement.style.height = w + "px", T.domElement.width = v * P, T.domElement.height = w * P, I.appendChild(T.domElement);
+            let W = new Ga(u, T.domElement);
+            W.addEventListener("change", R), W.enableDamping = !0, W.dampingFactor = .25, W.enableZoom = !0;
+            let K = b.kpoints,
+                L = b.b1,
+                j = b.b2,
+                k = b.b3,
+                Y = Math.sqrt(Math.max(Math.pow(L[0], 2) + Math.pow(L[1], 2) + Math.pow(L[2], 2), Math.pow(j[0], 2) + Math.pow(j[1], 2) + Math.pow(j[2], 2), Math.pow(k[0], 2) + Math.pow(k[1], 2) + Math.pow(k[2], 2)));
+            var q = Y * 1.5;
+            u.position.z = Y * 3;
+            let Z = b.faces_data;
+            for (var ee in K) {
+                let xe = K[ee],
+                    E = .02 * Y;
+                var ie = new yn(E, 16, 16),
+                    de = new vt(ie, _);
+                de.translateX(xe[0]), de.translateY(xe[1]), de.translateZ(xe[2]), d.add(de), ee = _f(ee, c);
+                var ge = x(ee);
+                I.appendChild(ge), h.push([new U(xe[0], xe[1], xe[2]), ge])
             }
             if (a) {
-                var xe = [
-                    [new D(1, 0, 0), '<span style="font-style: italic">x</span>'],
-                    [new D(0, 1, 0), '<span style="font-style: italic">y</span>'],
-                    [new D(0, 0, 1), '<span style="font-style: italic">z</span>']
+                var V = [
+                    [new U(1, 0, 0), '<span style="font-style: italic">x</span>'],
+                    [new U(0, 1, 0), '<span style="font-style: italic">y</span>'],
+                    [new U(0, 0, 1), '<span style="font-style: italic">z</span>']
                 ];
-                xe.forEach(function(de) {
-                    var Ne = de[0],
-                        S = de[1],
-                        g = new D(0, 0, 0),
-                        B = 5592405,
-                        Y = new yn(Ne, g, j, B, j / 10, j / 20);
-                    M.add(Y);
-                    var Q = "#555555";
-                    pe = w(S, Q);
-                    var J = Ne.clone();
-                    J.sub(g), J.multiplyScalar(j), C.appendChild(pe), c.push([J, pe])
+                V.forEach(function(xe) {
+                    var E = xe[0],
+                        g = xe[1],
+                        B = new U(0, 0, 0),
+                        X = 5592405,
+                        Q = new Sn(E, B, q, X, q / 10, q / 20);
+                    d.add(Q);
+                    var J = "#555555";
+                    ge = x(g, J);
+                    var Ee = E.clone();
+                    Ee.sub(B), Ee.multiplyScalar(q), I.appendChild(ge), h.push([Ee, ge])
                 })
             }
-            var H = [
-                    [K, '<span style="font-weight: bold">b</span><sub>1</sub>'],
-                    [P, '<span style="font-weight: bold">b</span><sub>2</sub>'],
-                    [X, '<span style="font-weight: bold">b</span><sub>3</sub>']
+            var te = [
+                    [L, '<span style="font-weight: bold">b</span><sub>1</sub>'],
+                    [j, '<span style="font-weight: bold">b</span><sub>2</sub>'],
+                    [k, '<span style="font-weight: bold">b</span><sub>3</sub>']
                 ],
-                H;
-            o || (H = []), H.forEach(function(de) {
-                var Ne = de[0];
-                W = de[1];
-                var S = Math.sqrt(Math.pow(Ne[0], 2) + Math.pow(Ne[1], 2) + Math.pow(Ne[2], 2)),
-                    g = new D(Ne[0] / S, Ne[1] / S, Ne[2] / S),
-                    B = new D(0, 0, 0),
-                    Y = 0,
-                    Q = new yn(g, B, length = S, Y = Y, S / 10, S / 20);
-                M.add(Q);
-                var J = w(W = W),
-                    Ce = g.clone();
-                Ce.sub(B), Ce.multiplyScalar(S), C.appendChild(J), c.push([Ce, J])
+                te;
+            o || (te = []), te.forEach(function(xe) {
+                var E = xe[0];
+                ee = xe[1];
+                var g = Math.sqrt(Math.pow(E[0], 2) + Math.pow(E[1], 2) + Math.pow(E[2], 2)),
+                    B = new U(E[0] / g, E[1] / g, E[2] / g),
+                    X = new U(0, 0, 0),
+                    Q = 0,
+                    J = new Sn(B, X, length = g, Q = Q, g / 10, g / 20);
+                d.add(J);
+                var Ee = x(ee = ee),
+                    Me = B.clone();
+                Me.sub(X), Me.multiplyScalar(g), I.appendChild(Ee), h.push([Me, Ee])
             });
-            var ie = new St,
-                fe = [];
-            q.triangles_vertices.forEach(function(de) {
-                fe.push(de[0], de[1], de[2])
-            }), ie.setAttribute("position", new rt(fe, 3));
-            var Te = [];
-            q.triangles.forEach(function(de) {
-                Te.push(de[0], de[1], de[2])
-            }), ie.setIndex(Te);
-            var _e = new vt(ie, u),
-                me = new Ga(_e.geometry),
-                Xe = new Ba(me, p);
-            M.add(_e), M.add(Xe);
-            var we = A.path;
-            if (we.forEach(function(de) {
-                    var Ne = de[0],
-                        S = de[1],
-                        g = V[Ne],
-                        B = V[S],
-                        Y = [];
-                    Y.push(new D(g[0], g[1], g[2])), Y.push(new D(B[0], B[1], B[2]));
-                    var Q = new St().setFromPoints(Y),
-                        J = new br(Q, f);
-                    J.material.linewidth = 4, M.add(J)
+            var pe = new Et,
+                we = [];
+            Z.triangles_vertices.forEach(function(xe) {
+                we.push(xe[0], xe[1], xe[2])
+            }), pe.setAttribute("position", new rt(we, 3));
+            var _e = [];
+            Z.triangles.forEach(function(xe) {
+                _e.push(xe[0], xe[1], xe[2])
+            }), pe.setIndex(_e);
+            var fe = new vt(pe, p),
+                Xe = new Ha(fe.geometry),
+                Ae = new za(Xe, f);
+            d.add(fe), d.add(Ae);
+            var O = b.path;
+            if (O.forEach(function(xe) {
+                    var E = xe[0],
+                        g = xe[1],
+                        B = K[E],
+                        X = K[g],
+                        Q = [];
+                    Q.push(new U(B[0], B[1], B[2])), Q.push(new U(X[0], X[1], X[2]));
+                    var J = new Et().setFromPoints(Q),
+                        Ee = new Tr(J, m);
+                    Ee.material.linewidth = 4, d.add(Ee)
                 }), s) {
-                var I = A.explicit_kpoints_abs;
-                for (var Qe in I) {
-                    var ve = I[Qe],
-                        Ue = .005 * k,
-                        te = new En(Ue, 16, 16),
-                        ee = new vt(te, _);
-                    ee.translateX(ve[0]), ee.translateY(ve[1]), ee.translateZ(ve[2]), M.add(ee)
-                }
-            }
-            U();
-            var Me = function(de, Ne) {
-                if (typeof Ne > "u") var S = !T.enabled;
-                else var S = Ne;
-                T.enabled = S;
-                for (var g = C.getElementsByClassName("BZDoubleClickText"), B = 0; B < g.length; B++) C.removeChild(g[B]);
-                S || C.appendChild(x("BZDoubleClickText"))
+                var Je = b.explicit_kpoints_abs;
+                for (var ve in Je) {
+                    var Pe = Je[ve],
+                        Se = .005 * Y,
+                        ie = new yn(Se, 16, 16),
+                        de = new vt(ie, M);
+                    de.translateX(Pe[0]), de.translateY(Pe[1]), de.translateZ(Pe[2]), d.add(de)
+                }
+            }
+            R();
+            var Ne = function(xe, E) {
+                if (typeof E > "u") var g = !W.enabled;
+                else var g = E;
+                W.enabled = g;
+                for (var B = I.getElementsByClassName("BZDoubleClickText"), X = 0; X < B.length; X++) I.removeChild(B[X]);
+                g || I.appendChild(A("BZDoubleClickText"))
             };
-            Me(), C.addEventListener("dblclick", Me);
-            var Le, be = !1;
-            C.addEventListener("touchend", function(de) {
-                if (typeof Le < "u" && clearTimeout(Le), be) be = !1, de.preventDefault(), Me();
+            l || (Ne(), I.addEventListener("dblclick", Ne));
+            var be, Re = !1;
+            I.addEventListener("touchend", function(xe) {
+                if (typeof be < "u" && clearTimeout(be), Re) Re = !1, xe.preventDefault(), Ne();
                 else {
-                    if (de.targetTouches.length != 0) {
-                        typeof Le < "u" && (clearTimeout(Le), be = !1);
+                    if (xe.targetTouches.length != 0) {
+                        typeof be < "u" && (clearTimeout(be), Re = !1);
                         return
                     }
-                    be = !0, Le = setTimeout(function() {
-                        be = !1
+                    Re = !0, be = setTimeout(function() {
+                        Re = !1
                     }, 500)
                 }
-            }), C.addEventListener("touchcancel", function(de) {
-                typeof Le < "u" && (clearTimeout(Le), be = !1)
-            }), C.addEventListener("touchmove", function(de) {
-                typeof Le < "u" && (clearTimeout(Le), be = !1)
+            }), I.addEventListener("touchcancel", function(xe) {
+                typeof be < "u" && (clearTimeout(be), Re = !1)
+            }), I.addEventListener("touchmove", function(xe) {
+                typeof be < "u" && (clearTimeout(be), Re = !1)
             })
         };
 
-        function R(A, y) {
-            var C = A.clone().project(y),
-                Z = window.devicePixelRatio || 1,
-                v, T;
+        function D(b, P) {
+            var I = b.clone().project(P),
+                v = window.devicePixelRatio || 1,
+                w, W;
             {
-                var v = .5 * h.domElement.width / Z,
-                    T = .5 * h.domElement.height / Z;
-                C.x = C.x * v + v, C.y = -(C.y * T) + T
+                var w = .5 * T.domElement.width / v,
+                    W = .5 * T.domElement.height / v;
+                I.x = I.x * w + w, I.y = -(I.y * W) + W
             }
             return {
-                left: C.x,
-                top: C.y
+                left: I.x,
+                top: I.y
             }
         }
 
-        function U() {
-            h.render(M, d), c.forEach(function(A) {
-                var y = A[0],
-                    C = A[1],
-                    Z = R(y, d);
-                C.style.top = Z.top + "px", C.style.left = Z.left + "px"
+        function R() {
+            T.render(d, u), h.forEach(function(b) {
+                var P = b[0],
+                    I = b[1],
+                    v = D(P, u);
+                I.style.top = v.top + "px", I.style.left = v.left + "px"
             })
         }
     };
 
 function xf(r) {
     let e = "";
     for (; e.length < r;) e += Math.random().toString(36).substring(2);
@@ -15911,20 +15912,29 @@
 }
 
 function Mf({
     model: r,
     el: e
 }) {
     let t = () => r.get("seekpath_data"),
-        i = document.createElement("div");
-    i.style.width = r.get("width"), i.style.height = r.get("height"), i.style.margin = "0 auto";
-    let n = Ko(i, t());
+        i = () => r.get("show_axes"),
+        n = () => r.get("show_bvectors"),
+        a = () => r.get("show_pathpoints"),
+        o = () => r.get("disable_interact_overlay"),
+        s = document.createElement("div");
+    s.style.width = r.get("width"), s.style.height = r.get("height"), s.style.margin = "0 auto";
+    let l = Ko(s, t(), {
+        showAxes: i(),
+        showBVectors: n(),
+        showPathpoints: a(),
+        disableInteractOverlay: o()
+    });
     r.on("change:seekpath_data", () => {
-        n.loadBZ(t())
-    }), e.appendChild(i)
+        l.loadBZ(t())
+    }), e.appendChild(s)
 }
 var wf = {
     render: Mf
 };
 export {
     wf as
     default
```

### Comparing `widget_bzvisualizer-0.2.2/README.md` & `widget_bzvisualizer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.2/pyproject.toml` & `widget_bzvisualizer-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "widget-bzvisualizer"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
   "anywidget~=0.9.3",
   "numpy~=1.21",
   "scipy~=1.10",
   "seekpath~=2.1",
 ]
 readme = "README.md"
@@ -37,15 +37,15 @@
 dependencies = ["hatch-jupyter-builder>=0.5.0"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 npm = "npm"
 build_cmd = "build"
 
 [tool.bumpver]
-current_version = "v0.2.2"
+current_version = "v0.2.3"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `widget_bzvisualizer-0.2.2/PKG-INFO` & `widget_bzvisualizer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: widget-bzvisualizer
-Version: 0.2.2
+Version: 0.2.3
 Requires-Dist: anywidget~=0.9.3
 Requires-Dist: numpy~=1.21
 Requires-Dist: scipy~=1.10
 Requires-Dist: seekpath~=2.1
 Provides-Extra: dev
 Requires-Dist: ase; extra == 'dev'
 Requires-Dist: bumpver==2023.1129; extra == 'dev'
```

