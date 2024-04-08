# Comparing `tmp/simsimd-4.2.2-cp39-cp39-win_arm64.whl.zip` & `tmp/simsimd-4.3.0-cp312-cp312-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 26104 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    32768 b- defN 24-Mar-31 21:54 simsimd.cp39-win_arm64.pyd
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Mar-31 21:54 simsimd-4.2.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    30025 b- defN 24-Mar-31 21:54 simsimd-4.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-31 21:54 simsimd-4.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-31 21:54 simsimd-4.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      472 b- defN 24-Mar-31 21:54 simsimd-4.2.2.dist-info/RECORD
-6 files, 74931 bytes uncompressed, 25256 bytes compressed:  66.3%
+Zip file size: 382621 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-08 18:13 simsimd-4.3.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-08 18:13 simsimd./
+-rwxr-xr-x  2.0 unx   592825 b- defN 24-Apr-08 18:13 simsimd.cpython-312-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-08 18:13 simsimd-4.3.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    30214 b- defN 24-Apr-08 18:13 simsimd-4.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 24-Apr-08 18:13 simsimd-4.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      679 b- defN 24-Apr-08 18:13 simsimd-4.3.0.dist-info/RECORD
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-08 18:13 simsimd-4.3.0.dist-info/LICENSE
+-rwxr-xr-x  2.0 unx   253289 b- defN 24-Apr-08 18:13 simsimd./libgomp-a97153a2.so.1.0.0
+-rwxr-xr-x  2.0 unx   181969 b- defN 24-Apr-08 18:13 simsimd./libmvec-2-1d7272ed.28.so
+10 files, 1070455 bytes uncompressed, 381243 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: simsimd.cp39-win_arm64.pyd
+Filename: simsimd-4.3.0.dist-info/
 Comment: 
 
-Filename: simsimd-4.2.2.dist-info/LICENSE
+Filename: simsimd./
 Comment: 
 
-Filename: simsimd-4.2.2.dist-info/METADATA
+Filename: simsimd.cpython-312-x86_64-linux-gnu.so
 Comment: 
 
-Filename: simsimd-4.2.2.dist-info/WHEEL
+Filename: simsimd-4.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: simsimd-4.2.2.dist-info/top_level.txt
+Filename: simsimd-4.3.0.dist-info/METADATA
 Comment: 
 
-Filename: simsimd-4.2.2.dist-info/RECORD
+Filename: simsimd-4.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: simsimd-4.3.0.dist-info/RECORD
+Comment: 
+
+Filename: simsimd-4.3.0.dist-info/LICENSE
+Comment: 
+
+Filename: simsimd./libgomp-a97153a2.so.1.0.0
+Comment: 
+
+Filename: simsimd./libmvec-2-1d7272ed.28.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `simsimd-4.2.2.dist-info/LICENSE` & `simsimd-4.3.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `simsimd-4.2.2.dist-info/METADATA` & `simsimd-4.3.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,742 +1,763 @@
-Metadata-Version: 2.1
-Name: simsimd
-Version: 4.2.2
-Summary: Fastest SIMD-Accelerated Vector Similarity Functions for x86 and Arm
-Home-page: https://github.com/ashvardanian/simsimd
-Author: Ash Vardanian
-Author-email: 1983160+ashvardanian@users.noreply.github.com
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# SimSIMD 📏
-
-_Computing dot-products, similarity measures, and distances between low- and high-dimensional vectors is ubiquitous in Machine Learning, Scientific Computing, Geo-Spatial Analysis, and Information Retrieval.
-These algorithms generally have linear complexity in time, constant complexity in space, and are data-parallel.
-In other words, it is easily parallelizable and vectorizable and often available in packages like BLAS and LAPACK, as well as higher-level `numpy` and `scipy` Python libraries.
-Ironically, even with decades of evolution in compilers and numerical computing, [most libraries can be 3-200x slower than hardware potential][benchmarks] even on the most popular hardware, like 64-bit x86 and Arm CPUs.
-SimSIMD attempts to fill that gap.
-1️⃣ SimSIMD functions are practically as fast as `memcpy`.
-2️⃣ SimSIMD [compiles to more platforms than NumPy (105 vs 35)][compatibility] and has more backends than most BLAS implementations._
-
-[benchmarks]: https://ashvardanian.com/posts/simsimd-faster-scipy
-[compatibility]: https://pypi.org/project/simsimd/#files
-
-<div>
-<a href="https://pepy.tech/project/simsimd">
-    <img alt="PyPI" src="https://static.pepy.tech/personalized-badge/simsimd?period=total&units=abbreviation&left_color=black&right_color=blue&left_text=SimSIMD%20Python%20installs" />
-</a>
-<a href="https://www.npmjs.com/package/simsimd">
-    <img alt="npm" src="https://img.shields.io/npm/dy/simsimd?label=JavaScript%20NPM%20installs" />
-</a>
-<a href="https://crates.io/crates/simsimd">
-    <img alt="rust" src="https://img.shields.io/crates/d/simsimd?label=Rust%20Crate%20installs" />
-</a>
-<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ashvardanian/simsimd">
-<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
-    <img alt="GitHub Actions Ubuntu" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=Ubuntu&logo=github&color=blue">
-</a>
-<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
-    <img alt="GitHub Actions Windows" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=Windows&logo=windows&color=blue">
-</a>
-<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
-    <img alt="GitHub Actions MacOS" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=MacOS&logo=apple&color=blue">
-</a>
-<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
-    <img alt="GitHub Actions CentOS Linux" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=CentOS&logo=centos&color=blue">
-</a>
-
-</div>
-
-## Features
-
-SimSIMD provides over 100 SIMD-optimized kernels for various distance and similarity measures, accelerating search in [USearch](https://github.com/unum-cloud/usearch) and several DBMS products.
-Implemented distance functions include:
-
-- Euclidean (L2) and Cosine (Angular) spatial distances for Vector Search.
-- Dot-Products for real & complex vectors for DSP & Quantum computing.
-- Hamming (~ Manhattan) and Jaccard (~ Tanimoto) bit-level distances.
-- Kullback-Leibler and Jensen–Shannon divergences for probability distributions.
-- Haversine and Vincenty's formulae for Geospatial Analysis.
-- For Levenshtein, Needleman–Wunsch and other text metrics, check [StringZilla][stringzilla].
-
-[scipy]: https://docs.scipy.org/doc/scipy/reference/spatial.distance.html#module-scipy.spatial.distance
-[numpy]: https://numpy.org/doc/stable/reference/generated/numpy.inner.html
-[stringzilla]: https://github.com/ashvardanian/stringzilla
-
-Moreover, SimSIMD...
-
-- handles `f64`, `f32`, and `f16` real & complex vectors.
-- handles `i8` integral and `b8` binary vectors.
-- is a zero-dependency [header-only C 99](#using-simsimd-in-c) library.
-- has bindings for [Python](#using-simsimd-in-python), [Rust](#using-simsimd-in-rust) and [JavaScript](#using-simsimd-in-javascript).
-- has Arm backends for NEON and Scalable Vector Extensions (SVE).
-- has x86 backends for Haswell, Skylake, Ice Lake, and Sapphire Rapids.
-
-Due to the high-level of fragmentation of SIMD support in different x86 CPUs, SimSIMD uses the names of select Intel CPU generations for its backends.
-They, however, also work on AMD CPUs.
-Inel Haswell is compatible with AMD Zen 1/2/3, while AMD Genoa Zen 4 covers AVX-512 instructions added to Intel Skylake and Ice Lake.
-You can learn more about the technical implementation details in the following blogposts:
-
-- [Uses Horner's method for polynomial approximations, beating GCC 12 by 119x](https://ashvardanian.com/posts/gcc-12-vs-avx512fp16/).
-- [Uses Arm SVE and x86 AVX-512's masked loads to eliminate tail `for`-loops](https://ashvardanian.com/posts/simsimd-faster-scipy/#tails-of-the-past-the-significance-of-masked-loads).
-- [Uses AVX-512 FP16 for half-precision operations, that few compilers vectorize](https://ashvardanian.com/posts/simsimd-faster-scipy/#the-challenge-of-f16).
-- [Substitutes LibC's `sqrt` calls with bit-hacks using Jan Kadlec's constant](https://ashvardanian.com/posts/simsimd-faster-scipy/#bonus-section-bypassing-sqrt-and-libc-dependencies).
-- [For Python avoids slow PyBind11, SWIG, and even `PyArg_ParseTuple` for speed](https://ashvardanian.com/posts/pybind11-cpython-tutorial/).
-- [For JavaScript uses typed arrays and NAPI for zero-copy calls](https://ashvardanian.com/posts/javascript-ai-vector-search/).
-
-## Benchmarks
-
-### Against NumPy and SciPy
-
-Given 1000 embeddings from OpenAI Ada API with 1536 dimensions, running on the Apple M2 Pro Arm CPU with NEON support, here's how SimSIMD performs against conventional methods:
-
-| Kind                      | `f32` improvement | `f16` improvement | `i8` improvement | Conventional method                    | SimSIMD         |
-| :------------------------ | ----------------: | ----------------: | ---------------: | :------------------------------------- | :-------------- |
-| Inner Product             |           __2 x__ |           __9 x__ |         __18 x__ | `numpy.inner`                          | `inner`         |
-| Cosine Distance           |          __32 x__ |          __79 x__ |        __133 x__ | `scipy.spatial.distance.cosine`        | `cosine`        |
-| Euclidean Distance ²      |           __5 x__ |          __26 x__ |         __17 x__ | `scipy.spatial.distance.sqeuclidean`   | `sqeuclidean`   |
-| Jensen-Shannon Divergence |          __31 x__ |          __53 x__ |                  | `scipy.spatial.distance.jensenshannon` | `jensenshannon` |
-
-### Against GCC Auto-Vectorization
-
-On the Intel Sapphire Rapids platform, SimSIMD was benchmarked against auto-vectorized code using GCC 12.
-GCC handles single-precision `float` but might not be the best choice for `int8` and `_Float16` arrays, which have been part of the C language since 2011.
-
-| Kind                      | GCC 12 `f32` | GCC 12 `f16` | SimSIMD `f16` | `f16` improvement |
-| :------------------------ | -----------: | -----------: | ------------: | ----------------: |
-| Inner Product             |    3,810 K/s |      192 K/s |     5,990 K/s |          __31 x__ |
-| Cosine Distance           |    3,280 K/s |      336 K/s |     6,880 K/s |          __20 x__ |
-| Euclidean Distance ²      |    4,620 K/s |      147 K/s |     5,320 K/s |          __36 x__ |
-| Jensen-Shannon Divergence |    1,180 K/s |       18 K/s |     2,140 K/s |         __118 x__ |
-
-__Broader Benchmarking Results__:
-
-- [Apple M2 Pro](https://ashvardanian.com/posts/simsimd-faster-scipy/#appendix-1-performance-on-apple-m2-pro).
-- [4th Gen Intel Xeon Platinum](https://ashvardanian.com/posts/simsimd-faster-scipy/#appendix-2-performance-on-4th-gen-intel-xeon-platinum-8480).
-- [AWS Graviton 3](https://ashvardanian.com/posts/simsimd-faster-scipy/#appendix-3-performance-on-aws-graviton-3).
-
-## Using SimSIMD in Python
-
-The package is intended to replace the usage of `numpy.inner`, `numpy.dot`, and `scipy.spatial.distance`.
-Aside from drastic performance improvements, SimSIMD significantly improves accuracy in mixed precision setups.
-NumPy and SciPy, processing `i8` or `f16` vectors, will use the same types for accumulators, while SimSIMD can combine `i8` enumeration, `i16` multiplication, and `i32` accumulation to avoid overflows entirely.
-The same applies to processing `f16` values with `f32` precision.
-
-### Installation
-
-Use the following snippet to install SimSIMD and list available hardware acceleration options available on your machine:
-
-```sh
-pip install simsimd
-python -c "import simsimd; print(simsimd.get_capabilities())"
-```
-
-### One-to-One Distance
-
-```py
-import simsimd
-import numpy as np
-
-vec1 = np.random.randn(1536).astype(np.float32)
-vec2 = np.random.randn(1536).astype(np.float32)
-dist = simsimd.cosine(vec1, vec2)
-```
-
-Supported functions include `cosine`, `inner`, `sqeuclidean`, `hamming`, and `jaccard`.
-Dot products are supported for both real and complex numbers:
-
-```py
-vec1 = np.random.randn(768).astype(np.float64) + 1j * np.random.randn(768).astype(np.float64)
-vec2 = np.random.randn(768).astype(np.float64) + 1j * np.random.randn(768).astype(np.float64)
-
-dist = simsimd.dot(vec1.astype(np.complex128), vec2.astype(np.complex128))
-dist = simsimd.dot(vec1.astype(np.complex64), vec2.astype(np.complex64))
-dist = simsimd.vdot(vec1.astype(np.complex64), vec2.astype(np.complex64)) # conjugate, same as `np.vdot`
-```
-
-Unlike SciPy, SimSIMD allows explicitly stating the precision of the input vectors, which is especially useful for mixed-precision setups.
-
-```py
-dist = simsimd.cosine(vec1, vec2, "i8")
-dist = simsimd.cosine(vec1, vec2, "f16")
-dist = simsimd.cosine(vec1, vec2, "f32")
-dist = simsimd.cosine(vec1, vec2, "f64")
-```
-
-It also allows using SimSIMD for half-precision complex numbers, which NumPy does not support.
-For that, view data as continuous even-length `np.float16` vectors and override type-resolution with `complex32` string.
-
-```py
-vec1 = np.random.randn(1536).astype(np.float16)
-vec2 = np.random.randn(1536).astype(np.float16)
-simd.dot(vec1, vec2, "complex32")
-simd.vdot(vec1, vec2, "complex32")
-```
-
-### One-to-Many Distances
-
-Every distance function can be used not only for one-to-one but also one-to-many and many-to-many distance calculations.
-For one-to-many:
-
-```py
-vec1 = np.random.randn(1536).astype(np.float32) # rank 1 tensor
-batch1 = np.random.randn(1, 1536).astype(np.float32) # rank 2 tensor
-batch2 = np.random.randn(100, 1536).astype(np.float32)
-
-dist_rank1 = simsimd.cosine(vec1, batch2)
-dist_rank2 = simsimd.cosine(batch1, batch2)
-```
-
-### Many-to-Many Distances
-
-All distance functions in SimSIMD can be used to compute many-to-many distances.
-For two batches of 100 vectors to compute 100 distances, one would call it like this:
-
-```py
-batch1 = np.random.randn(100, 1536).astype(np.float32)
-batch2 = np.random.randn(100, 1536).astype(np.float32)
-dist = simsimd.cosine(batch1, batch2)
-```
-
-Input matrices must have identical shapes.
-This functionality isn't natively present in NumPy or SciPy, and generally requires creating intermediate arrays, which is inefficient and memory-consuming.
-
-### Many-to-Many All-Pairs Distances
-
-One can use SimSIMD to compute distances between all possible pairs of rows across two matrices (akin to [`scipy.spatial.distance.cdist`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.cdist.html)).
-The resulting object will have a type `DistancesTensor`, zero-copy compatible with NumPy and other libraries.
-For two arrays of 10 and 1,000 entries, the resulting tensor will have 10,000 cells:
-
-```py
-import numpy as np
-from simsimd import cdist, DistancesTensor
-
-matrix1 = np.random.randn(1000, 1536).astype(np.float32)
-matrix2 = np.random.randn(10, 1536).astype(np.float32)
-distances: DistancesTensor = simsimd.cdist(matrix1, matrix2, metric="cosine") # zero-copy
-distances_array: np.ndarray = np.array(distances, copy=True) # now managed by NumPy
-```
-
-### Multithreading
-
-By default, computations use a single CPU core.
-To optimize and utilize all CPU cores on Linux systems, add the `threads=0` argument.
-Alternatively, specify a custom number of threads:
-
-```py
-distances = simsimd.cdist(matrix1, matrix2, metric="cosine", threads=0)
-```
-
-### Using Python API with USearch
-
-Want to use it in Python with [USearch](https://github.com/unum-cloud/usearch)?
-You can wrap the raw C function pointers SimSIMD backends into a `CompiledMetric` and pass it to USearch, similar to how it handles Numba's JIT-compiled code.
-
-```py
-from usearch.index import Index, CompiledMetric, MetricKind, MetricSignature
-from simsimd import pointer_to_sqeuclidean, pointer_to_cosine, pointer_to_inner
-
-metric = CompiledMetric(
-    pointer=pointer_to_cosine("f16"),
-    kind=MetricKind.Cos,
-    signature=MetricSignature.ArrayArraySize,
-)
-
-index = Index(256, metric=metric)
-```
-
-## Using SimSIMD in Rust
-
-To install, add the following to your `Cargo.toml`:
-
-```toml
-[dependencies]
-simsimd = "..."
-```
-
-Before using the SimSIMD library, ensure you have imported the necessary traits and types into your Rust source file.
-The library provides several traits for different distance/similarity kinds - `SpatialSimilarity`, `BinarySimilarity`, and `ProbabilitySimilarity`.
-
-### Spatial Similarity: Cosine and Euclidean Distances
-
-```rust
-use simsimd::SpatialSimilarity;
-
-fn main() {
-    let vector_a: Vec<f32> = vec![1.0, 2.0, 3.0];
-    let vector_b: Vec<f32> = vec![4.0, 5.0, 6.0];
-
-    // Compute the cosine similarity between vector_a and vector_b
-    let cosine_similarity = f32::cosine(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Cosine Similarity: {}", cosine_similarity);
-
-    // Compute the squared Euclidean distance between vector_a and vector_b
-    let sq_euclidean_distance = f32::sqeuclidean(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Squared Euclidean Distance: {}", sq_euclidean_distance);
-}
-```
-
-Spatial similarity functions are available for `f64`, `f32`, `f16`, and `i8` types.
-
-### Dot-Products: Inner and Complex Inner Products
-
-```rust
-use simsimd::SpatialSimilarity;
-use simsimd::ComplexProducts;
-
-fn main() {
-    let vector_a: Vec<f32> = vec![1.0, 2.0, 3.0, 4.0];
-    let vector_b: Vec<f32> = vec![5.0, 6.0, 7.0, 8.0];
-
-    // Compute the inner product between vector_a and vector_b
-    let inner_product = SpatialSimilarity::dot(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Inner Product: {}", inner_product);
-
-    // Compute the complex inner product between complex_vector_a and complex_vector_b
-    let complex_inner_product = ComplexProducts::dot(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    let complex_conjugate_inner_product = ComplexProducts::vdot(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Complex Inner Product: {:?}", complex_inner_product); // -18, 69
-    println!("Complex C. Inner Product: {:?}", complex_conjugate_inner_product); // 70, -8
-}
-```
-
-Complex inner products are available for `f64`, `f32`, and `f16` types.
-
-### Probability Distributions: Jensen-Shannon and Kullback-Leibler Divergences
-
-```rust
-use simsimd::SpatialSimilarity;
-
-fn main() {
-    let vector_a: Vec<f32> = vec![1.0, 2.0, 3.0];
-    let vector_b: Vec<f32> = vec![4.0, 5.0, 6.0];
-
-    let cosine_similarity = f32::jensenshannon(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Cosine Similarity: {}", cosine_similarity);
-
-    let sq_euclidean_distance = f32::kullbackleibler(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Squared Euclidean Distance: {}", sq_euclidean_distance);
-}
-```
-
-Probability similarity functions are available for `f64`, `f32`, and `f16` types.
-
-### Binary Similarity: Hamming and Jaccard Distances
-
-Similar to spatial distances, one can compute bit-level distance functions between slices of unsigned integers:
-
-```rust
-use simsimd::BinarySimilarity;
-
-fn main() {
-    let vector_a = &[0b11110000, 0b00001111, 0b10101010];
-    let vector_b = &[0b11110000, 0b00001111, 0b01010101];
-
-    // Compute the Hamming distance between vector_a and vector_b
-    let hamming_distance = u8::hamming(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Hamming Distance: {}", hamming_distance);
-
-    // Compute the Jaccard distance between vector_a and vector_b
-    let jaccard_distance = u8::jaccard(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Jaccard Distance: {}", jaccard_distance);
-}
-```
-
-Binary similarity functions are available only for `u8` types.
-
-### Half-Precision Floating-Point Numbers
-
-Rust has no native support for half-precision floating-point numbers, but SimSIMD provides a `f16` type.
-It has no functionality - it is a `transparent` wrapper around `u16` and can be used with `half` or any other half-precision library.
-
-```rust
-use simsimd::SpatialSimilarity;
-use simsimd::f16 as SimF16;
-use half::f16 as HalfF16;
-
-fn main() {
-    let vector_a: Vec<HalfF16> = ...
-    let vector_b: Vec<HalfF16> = ...
-
-    let buffer_a: &[SimF16] = unsafe { std::slice::from_raw_parts(a_half.as_ptr() as *const SimF16, a_half.len()) };
-    let buffer_b: &[SimF16] = unsafe { std::slice::from_raw_parts(b_half.as_ptr() as *const SimF16, b_half.len()) };
-
-    // Compute the cosine similarity between vector_a and vector_b
-    let cosine_similarity = SimF16::cosine(&vector_a, &vector_b)
-        .expect("Vectors must be of the same length");
-
-    println!("Cosine Similarity: {}", cosine_similarity);
-}
-```
-
-### Dynamic Dispatch
-
-SimSIMD provides a dynamic dispatch mechanism to select the most advanced micro-kernel for the current CPU.
-You can query supported backends and use the `SimSIMD::capabilities` function to select the best one.
-
-```rust
-println!("uses neon: {}", capabilties::uses_neon());
-println!("uses sve: {}", capabilties::uses_sve());
-println!("uses haswell: {}", capabilties::uses_haswell());
-println!("uses skylake: {}", capabilties::uses_skylake());
-println!("uses ice: {}", capabilties::uses_ice());
-println!("uses sapphire: {}", capabilties::uses_sapphire());
-```
-
-## Using SimSIMD in JavaScript
-
-To install, choose one of the following options depending on your environment:
-
-- `npm install --save simsimd`
-- `yarn add simsimd`
-- `pnpm add simsimd`
-- `bun install simsimd`
-
-The package is distributed with prebuilt binaries for Node.js v10 and above for Linux (x86_64, arm64), macOS (x86_64, arm64), and Windows (i386, x86_64).
-If your platform is not supported, you can build the package from the source via `npm run build`.
-This will automatically happen unless you install the package with the `--ignore-scripts` flag or use Bun.
-After you install it, you will be able to call the SimSIMD functions on various `TypedArray` variants:
-
-```js
-const { sqeuclidean, cosine, inner, hamming, jaccard } = require('simsimd');
-
-const vectorA = new Float32Array([1.0, 2.0, 3.0]);
-const vectorB = new Float32Array([4.0, 5.0, 6.0]);
-
-const distance = sqeuclidean(vectorA, vectorB);
-console.log('Squared Euclidean Distance:', distance);
-```
-
-Other numeric types and precision levels are supported as well:
-
-```js
-const vectorA = new Float64Array([1.0, 2.0, 3.0]);
-const vectorB = new Float64Array([4.0, 5.0, 6.0]);
-
-const distance = cosine(vectorA, vectorB);
-console.log('Cosine Similarity:', distance);
-```
-
-## Using SimSIMD in C
-
-For integration within a CMake-based project, add the following segment to your `CMakeLists.txt`:
-
-```cmake
-FetchContent_Declare(
-    simsimd
-    GIT_REPOSITORY https://github.com/ashvardanian/simsimd.git
-    GIT_SHALLOW TRUE
-)
-FetchContent_MakeAvailable(simsimd)
-```
-
-After that, you can use the SimSIMD library in your C code in several ways.
-Simplest of all, you can include the headers, and the compiler will automatically select the most recent CPU extensions that SimSIMD will use.
-
-```c
-#include <simsimd/simsimd.h>
-
-int main() {
-    simsimd_f32_t vector_a[1536];
-    simsimd_f32_t vector_b[1536];
-    simsimd_metric_punned_t distance_function = simsimd_metric_punned(
-        simsimd_metric_cos_k, // Metric kind, like the angular cosine distance
-        simsimd_datatype_f32_k, // Data type, like: f16, f32, f64, i8, b8, and complex variants
-        simsimd_cap_any_k); // Which CPU capabilities are we allowed to use
-    simsimd_distance_t distance;
-    distance_function(vector_a, vector_b, 1536, &distance);
-    return 0;
-}
-```
-
-### Dynamic Dispatch
-
-To avoid hard-coding the backend, you can rely on `c/lib.c` to prepackage all possible backends in one binary, and select the most recent CPU features at runtime.
-That feature of the C library is called dynamic dispatch and is extensively used in the Python, JavaScript, and Rust bindings.
-To test which CPU features are available on the machine at runtime, use the following APIs:
-
-```c
-int uses_neon = simsimd_uses_neon();
-int uses_sve = simsimd_uses_sve();
-int uses_haswell = simsimd_uses_haswell();
-int uses_skylake = simsimd_uses_skylake();
-int uses_ice = simsimd_uses_ice();
-int uses_sapphire = simsimd_uses_sapphire();
-
-simsimd_capability_t capabilities = simsimd_capabilities();
-```
-
-To differentiate between runtime and compile-time dispatch, define the following macro:
-
-```c
-#define SIMSIMD_DYNAMIC_DISPATCH 1 // or 0
-```
-
-### Spatial Distances: Cosine and Euclidean Distances
-
-```c
-#include <simsimd/simsimd.h>
-
-int main() {
-    simsimd_f64_t f64s[1536];
-    simsimd_f32_t f32s[1536];
-    simsimd_f16_t f16s[1536];
-    simsimd_i8_t i8[1536];
-    simsimd_distance_t distance;
-
-    // Cosine distance between two vectors
-    simsimd_cos_i8(i8s, i8s, 1536, &distance);
-    simsimd_cos_f16(f16s, f16s, 1536, &distance);
-    simsimd_cos_f32(f32s, f32s, 1536, &distance);
-    simsimd_cos_f64(f64s, f64s, 1536, &distance);
-    
-    // Euclidean distance between two vectors
-    simsimd_l2sq_i8(i8s, i8s, 1536, &distance);
-    simsimd_l2sq_f16(f16s, f16s, 1536, &distance);
-    simsimd_l2sq_f32(f32s, f32s, 1536, &distance);
-    simsimd_l2sq_f64(f64s, f64s, 1536, &distance);
-
-    return 0;
-}
-```
-
-### Dot-Products: Inner and Complex Inner Products
-
-```c
-#include <simsimd/simsimd.h>
-
-int main() {
-    simsimd_f64_t f64s[1536];
-    simsimd_f32_t f32s[1536];
-    simsimd_f16_t f16s[1536];
-    simsimd_distance_t distance;
-
-    // Inner product between two vectors
-    simsimd_dot_f16(f16s, f16s, 1536, &distance);
-    simsimd_dot_f32(f32s, f32s, 1536, &distance);
-    simsimd_dot_f64(f64s, f64s, 1536, &distance);
-
-    // Complex inner product between two vectors
-    simsimd_dot_f16c(f16s, f16s, 1536, &distance);
-    simsimd_dot_f32c(f32s, f32s, 1536, &distance);
-    simsimd_dot_f64c(f64s, f64s, 1536, &distance);
-
-    // Complex conjugate inner product between two vectors
-    simsimd_vdot_f16c(f16s, f16s, 1536, &distance);
-    simsimd_vdot_f32c(f32s, f32s, 1536, &distance);
-    simsimd_vdot_f64c(f64s, f64s, 1536, &distance);
-
-    return 0;
-}
-```
-
-### Binary Distances: Hamming and Jaccard Distances
-
-```c
-#include <simsimd/simsimd.h>
-
-int main() {
-    simsimd_b8_t b8s[1536 / 8]; // 8 bits per word
-    simsimd_distance_t distance;
-
-    // Hamming distance between two vectors
-    simsimd_hamming_b8(b8s, b8s, 1536 / 8, &distance);
-
-    // Jaccard distance between two vectors
-    simsimd_jaccard_b8(b8s, b8s, 1536 / 8, &distance);
-
-    return 0;
-}
-```
-
-### Probability Distributions: Jensen-Shannon and Kullback-Leibler Divergences
-
-```c
-#include <simsimd/simsimd.h>
-
-int main() {
-    simsimd_f64_t f64s[1536];
-    simsimd_f32_t f32s[1536];
-    simsimd_f16_t f16s[1536];
-    simsimd_distance_t distance;
-
-    // Jensen-Shannon divergence between two vectors
-    simsimd_js_f16(f16s, f16s, 1536, &distance);
-    simsimd_js_f32(f32s, f32s, 1536, &distance);
-    simsimd_js_f64(f64s, f64s, 1536, &distance);
-
-    // Kullback-Leibler divergence between two vectors
-    simsimd_kl_f16(f16s, f16s, 1536, &distance);
-    simsimd_kl_f32(f32s, f32s, 1536, &distance);
-    simsimd_kl_f64(f64s, f64s, 1536, &distance);
-
-    return 0;
-}
-```
-
-### Half-Precision Floating-Point Numbers
-
-If you aim to utilize the `_Float16` functionality with SimSIMD, ensure your development environment is compatible with C 11.
-For other SimSIMD functionalities, C 99 compatibility will suffice.
-To explicitly disable half-precision support, define the following macro before imports:
-
-```c
-#define SIMSIMD_NATIVE_F16 0 // or 1
-#include <simsimd/simsimd.h>
-```
-
-### Target Specific Backends
-
-SimSIMD exposes all kernels for all backends, and you can select the most advanced one for the current CPU without relying on built-in dispatch mechanisms.
-All of the function names follow the same pattern: `simsimd_{function}_{type}_{backend}`.
-
-- The backend can be `serial`, `haswell`, `skylake`, `ice`, `sapphire`, `neon`, or `sve`.
-- The type can be `f64`, `f32`, `f16`, `f64c`, `f32c`, `f16c`, `i8`, or `b8`.
-- The function can be `dot`, `vdot`, `cos`, `l2sq`, `hamming`, `jaccard`, `kl`, or `js`.
-
-To avoid hard-coding the backend, you can use the `simsimd_metric_punned_t` to pun the function pointer and the `simsimd_capabilities` function to get the available backends at runtime.
-
-```c
-simsimd_dot_f64_sve
-simsimd_cos_f64_sve
-simsimd_l2sq_f64_sve
-simsimd_dot_f64_skylake
-simsimd_cos_f64_skylake
-simsimd_l2sq_f64_skylake
-simsimd_dot_f64_serial
-simsimd_cos_f64_serial
-simsimd_l2sq_f64_serial
-simsimd_js_f64_serial
-simsimd_kl_f64_serial
-simsimd_dot_f32_sve
-simsimd_cos_f32_sve
-simsimd_l2sq_f32_sve
-simsimd_dot_f32_neon
-simsimd_cos_f32_neon
-simsimd_l2sq_f32_neon
-simsimd_js_f32_neon
-simsimd_kl_f32_neon
-simsimd_dot_f32_skylake
-simsimd_cos_f32_skylake
-simsimd_l2sq_f32_skylake
-simsimd_js_f32_skylake
-simsimd_kl_f32_skylake
-simsimd_dot_f32_serial
-simsimd_cos_f32_serial
-simsimd_l2sq_f32_serial
-simsimd_js_f32_serial
-simsimd_kl_f32_serial
-simsimd_dot_f16_sve
-simsimd_cos_f16_sve
-simsimd_l2sq_f16_sve
-simsimd_dot_f16_neon
-simsimd_cos_f16_neon
-simsimd_l2sq_f16_neon
-simsimd_js_f16_neon
-simsimd_kl_f16_neon
-simsimd_dot_f16_sapphire
-simsimd_cos_f16_sapphire
-simsimd_l2sq_f16_sapphire
-simsimd_js_f16_sapphire
-simsimd_kl_f16_sapphire
-simsimd_dot_f16_haswell
-simsimd_cos_f16_haswell
-simsimd_l2sq_f16_haswell
-simsimd_js_f16_haswell
-simsimd_kl_f16_haswell
-simsimd_dot_f16_serial
-simsimd_cos_f16_serial
-simsimd_l2sq_f16_serial
-simsimd_js_f16_serial
-simsimd_kl_f16_serial
-simsimd_cos_i8_neon
-simsimd_cos_i8_neon
-simsimd_l2sq_i8_neon
-simsimd_cos_i8_ice
-simsimd_cos_i8_ice
-simsimd_l2sq_i8_ice
-simsimd_cos_i8_haswell
-simsimd_cos_i8_haswell
-simsimd_l2sq_i8_haswell
-simsimd_cos_i8_serial
-simsimd_cos_i8_serial
-simsimd_l2sq_i8_serial
-simsimd_hamming_b8_sve
-simsimd_jaccard_b8_sve
-simsimd_hamming_b8_neon
-simsimd_jaccard_b8_neon
-simsimd_hamming_b8_ice
-simsimd_jaccard_b8_ice
-simsimd_hamming_b8_haswell
-simsimd_jaccard_b8_haswell
-simsimd_hamming_b8_serial
-simsimd_jaccard_b8_serial
-simsimd_dot_f32c_sve
-simsimd_vdot_f32c_sve
-simsimd_dot_f32c_neon
-simsimd_vdot_f32c_neon
-simsimd_dot_f32c_haswell
-simsimd_vdot_f32c_haswell
-simsimd_dot_f32c_skylake
-simsimd_vdot_f32c_skylake
-simsimd_dot_f32c_serial
-simsimd_vdot_f32c_serial
-simsimd_dot_f64c_sve
-simsimd_vdot_f64c_sve
-simsimd_dot_f64c_skylake
-simsimd_vdot_f64c_skylake
-simsimd_dot_f64c_serial
-simsimd_vdot_f64c_serial
-simsimd_dot_f16c_sve
-simsimd_vdot_f16c_sve
-simsimd_dot_f16c_neon
-simsimd_vdot_f16c_neon
-simsimd_dot_f16c_haswell
-simsimd_vdot_f16c_haswell
-simsimd_dot_f16c_sapphire
-simsimd_vdot_f16c_sapphire
-simsimd_dot_f16c_serial
-simsimd_vdot_f16c_serial
-```
+Metadata-Version: 2.1
+Name: simsimd
+Version: 4.3.0
+Summary: Fastest SIMD-Accelerated Vector Similarity Functions for x86 and Arm
+Home-page: https://github.com/ashvardanian/simsimd
+Author: Ash Vardanian
+Author-email: 1983160+ashvardanian@users.noreply.github.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SimSIMD 📏
+
+![SimSIMD banner](https://github.com/ashvardanian/ashvardanian/blob/master/repositories/SimSIMD.png?raw=true)
+
+Computing dot-products, similarity measures, and distances between low- and high-dimensional vectors is ubiquitous in Machine Learning, Scientific Computing, Geo-Spatial Analysis, and Information Retrieval.
+These algorithms generally have linear complexity in time, constant complexity in space, and are data-parallel.
+In other words, it is easily parallelizable and vectorizable and often available in packages like BLAS and LAPACK, as well as higher-level `numpy` and `scipy` Python libraries.
+Ironically, even with decades of evolution in compilers and numerical computing, [most libraries can be 3-200x slower than hardware potential][benchmarks] even on the most popular hardware, like 64-bit x86 and Arm CPUs.
+SimSIMD attempts to fill that gap.
+1️⃣ SimSIMD functions are practically as fast as `memcpy`.
+2️⃣ SimSIMD [compiles to more platforms than NumPy (105 vs 35)][compatibility] and has more backends than most BLAS implementations.
+
+[benchmarks]: https://ashvardanian.com/posts/simsimd-faster-scipy
+[compatibility]: https://pypi.org/project/simsimd/#files
+
+<div>
+<a href="https://pepy.tech/project/simsimd">
+    <img alt="PyPI" src="https://static.pepy.tech/personalized-badge/simsimd?period=total&units=abbreviation&left_color=black&right_color=blue&left_text=SimSIMD%20Python%20installs" />
+</a>
+<a href="https://www.npmjs.com/package/simsimd">
+    <img alt="npm" src="https://img.shields.io/npm/dy/simsimd?label=JavaScript%20NPM%20installs" />
+</a>
+<a href="https://crates.io/crates/simsimd">
+    <img alt="rust" src="https://img.shields.io/crates/d/simsimd?label=Rust%20Crate%20installs" />
+</a>
+<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ashvardanian/simsimd">
+<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
+    <img alt="GitHub Actions Ubuntu" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=Ubuntu&logo=github&color=blue">
+</a>
+<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
+    <img alt="GitHub Actions Windows" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=Windows&logo=windows&color=blue">
+</a>
+<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
+    <img alt="GitHub Actions MacOS" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=MacOS&logo=apple&color=blue">
+</a>
+<a href="https://github.com/ashvardanian/SimSIMD/actions/workflows/release.yml">
+    <img alt="GitHub Actions CentOS Linux" src="https://img.shields.io/github/actions/workflow/status/ashvardanian/SimSIMD/release.yml?branch=main&label=CentOS&logo=centos&color=blue">
+</a>
+
+</div>
+
+## Features
+
+SimSIMD provides over 100 SIMD-optimized kernels for various distance and similarity measures, accelerating search in [USearch](https://github.com/unum-cloud/usearch) and several DBMS products.
+Implemented distance functions include:
+
+- Euclidean (L2) and Cosine (Angular) spatial distances for Vector Search.
+- Dot-Products for real & complex vectors for DSP & Quantum computing.
+- Hamming (~ Manhattan) and Jaccard (~ Tanimoto) bit-level distances.
+- Kullback-Leibler and Jensen–Shannon divergences for probability distributions.
+- Haversine and Vincenty's formulae for Geospatial Analysis.
+- For Levenshtein, Needleman–Wunsch and other text metrics, check [StringZilla][stringzilla].
+
+[scipy]: https://docs.scipy.org/doc/scipy/reference/spatial.distance.html#module-scipy.spatial.distance
+[numpy]: https://numpy.org/doc/stable/reference/generated/numpy.inner.html
+[stringzilla]: https://github.com/ashvardanian/stringzilla
+
+Moreover, SimSIMD...
+
+- handles `f64`, `f32`, and `f16` real & complex vectors.
+- handles `i8` integral and `b8` binary vectors.
+- is a zero-dependency [header-only C 99](#using-simsimd-in-c) library.
+- has bindings for [Python](#using-simsimd-in-python), [Rust](#using-simsimd-in-rust) and [JavaScript](#using-simsimd-in-javascript).
+- has Arm backends for NEON and Scalable Vector Extensions (SVE).
+- has x86 backends for Haswell, Skylake, Ice Lake, and Sapphire Rapids.
+
+Due to the high-level of fragmentation of SIMD support in different x86 CPUs, SimSIMD uses the names of select Intel CPU generations for its backends.
+They, however, also work on AMD CPUs.
+Inel Haswell is compatible with AMD Zen 1/2/3, while AMD Genoa Zen 4 covers AVX-512 instructions added to Intel Skylake and Ice Lake.
+You can learn more about the technical implementation details in the following blogposts:
+
+- [Uses Horner's method for polynomial approximations, beating GCC 12 by 119x](https://ashvardanian.com/posts/gcc-12-vs-avx512fp16/).
+- [Uses Arm SVE and x86 AVX-512's masked loads to eliminate tail `for`-loops](https://ashvardanian.com/posts/simsimd-faster-scipy/#tails-of-the-past-the-significance-of-masked-loads).
+- [Uses AVX-512 FP16 for half-precision operations, that few compilers vectorize](https://ashvardanian.com/posts/simsimd-faster-scipy/#the-challenge-of-f16).
+- [Substitutes LibC's `sqrt` calls with bit-hacks using Jan Kadlec's constant](https://ashvardanian.com/posts/simsimd-faster-scipy/#bonus-section-bypassing-sqrt-and-libc-dependencies).
+- [For Python avoids slow PyBind11, SWIG, and even `PyArg_ParseTuple` for speed](https://ashvardanian.com/posts/pybind11-cpython-tutorial/).
+- [For JavaScript uses typed arrays and NAPI for zero-copy calls](https://ashvardanian.com/posts/javascript-ai-vector-search/).
+
+## Benchmarks
+
+### Against NumPy and SciPy
+
+Given 1000 embeddings from OpenAI Ada API with 1536 dimensions, running on the Apple M2 Pro Arm CPU with NEON support, here's how SimSIMD performs against conventional methods:
+
+| Kind                      | `f32` improvement | `f16` improvement | `i8` improvement | Conventional method                    | SimSIMD         |
+| :------------------------ | ----------------: | ----------------: | ---------------: | :------------------------------------- | :-------------- |
+| Inner Product             |           __2 x__ |           __9 x__ |         __18 x__ | `numpy.inner`                          | `inner`         |
+| Cosine Distance           |          __32 x__ |          __79 x__ |        __133 x__ | `scipy.spatial.distance.cosine`        | `cosine`        |
+| Euclidean Distance ²      |           __5 x__ |          __26 x__ |         __17 x__ | `scipy.spatial.distance.sqeuclidean`   | `sqeuclidean`   |
+| Jensen-Shannon Divergence |          __31 x__ |          __53 x__ |                  | `scipy.spatial.distance.jensenshannon` | `jensenshannon` |
+
+### Against GCC Auto-Vectorization
+
+On the Intel Sapphire Rapids platform, SimSIMD was benchmarked against auto-vectorized code using GCC 12.
+GCC handles single-precision `float` but might not be the best choice for `int8` and `_Float16` arrays, which have been part of the C language since 2011.
+
+| Kind                      | GCC 12 `f32` | GCC 12 `f16` | SimSIMD `f16` | `f16` improvement |
+| :------------------------ | -----------: | -----------: | ------------: | ----------------: |
+| Inner Product             |    3,810 K/s |      192 K/s |     5,990 K/s |          __31 x__ |
+| Cosine Distance           |    3,280 K/s |      336 K/s |     6,880 K/s |          __20 x__ |
+| Euclidean Distance ²      |    4,620 K/s |      147 K/s |     5,320 K/s |          __36 x__ |
+| Jensen-Shannon Divergence |    1,180 K/s |       18 K/s |     2,140 K/s |         __118 x__ |
+
+__Broader Benchmarking Results__:
+
+- [Apple M2 Pro](https://ashvardanian.com/posts/simsimd-faster-scipy/#appendix-1-performance-on-apple-m2-pro).
+- [4th Gen Intel Xeon Platinum](https://ashvardanian.com/posts/simsimd-faster-scipy/#appendix-2-performance-on-4th-gen-intel-xeon-platinum-8480).
+- [AWS Graviton 3](https://ashvardanian.com/posts/simsimd-faster-scipy/#appendix-3-performance-on-aws-graviton-3).
+
+## Using SimSIMD in Python
+
+The package is intended to replace the usage of `numpy.inner`, `numpy.dot`, and `scipy.spatial.distance`.
+Aside from drastic performance improvements, SimSIMD significantly improves accuracy in mixed precision setups.
+NumPy and SciPy, processing `i8` or `f16` vectors, will use the same types for accumulators, while SimSIMD can combine `i8` enumeration, `i16` multiplication, and `i32` accumulation to avoid overflows entirely.
+The same applies to processing `f16` values with `f32` precision.
+
+### Installation
+
+Use the following snippet to install SimSIMD and list available hardware acceleration options available on your machine:
+
+```sh
+pip install simsimd
+python -c "import simsimd; print(simsimd.get_capabilities())"
+```
+
+### One-to-One Distance
+
+```py
+import simsimd
+import numpy as np
+
+vec1 = np.random.randn(1536).astype(np.float32)
+vec2 = np.random.randn(1536).astype(np.float32)
+dist = simsimd.cosine(vec1, vec2)
+```
+
+Supported functions include `cosine`, `inner`, `sqeuclidean`, `hamming`, and `jaccard`.
+Dot products are supported for both real and complex numbers:
+
+```py
+vec1 = np.random.randn(768).astype(np.float64) + 1j * np.random.randn(768).astype(np.float64)
+vec2 = np.random.randn(768).astype(np.float64) + 1j * np.random.randn(768).astype(np.float64)
+
+dist = simsimd.dot(vec1.astype(np.complex128), vec2.astype(np.complex128))
+dist = simsimd.dot(vec1.astype(np.complex64), vec2.astype(np.complex64))
+dist = simsimd.vdot(vec1.astype(np.complex64), vec2.astype(np.complex64)) # conjugate, same as `np.vdot`
+```
+
+Unlike SciPy, SimSIMD allows explicitly stating the precision of the input vectors, which is especially useful for mixed-precision setups.
+
+```py
+dist = simsimd.cosine(vec1, vec2, "i8")
+dist = simsimd.cosine(vec1, vec2, "f16")
+dist = simsimd.cosine(vec1, vec2, "f32")
+dist = simsimd.cosine(vec1, vec2, "f64")
+```
+
+It also allows using SimSIMD for half-precision complex numbers, which NumPy does not support.
+For that, view data as continuous even-length `np.float16` vectors and override type-resolution with `complex32` string.
+
+```py
+vec1 = np.random.randn(1536).astype(np.float16)
+vec2 = np.random.randn(1536).astype(np.float16)
+simd.dot(vec1, vec2, "complex32")
+simd.vdot(vec1, vec2, "complex32")
+```
+
+### One-to-Many Distances
+
+Every distance function can be used not only for one-to-one but also one-to-many and many-to-many distance calculations.
+For one-to-many:
+
+```py
+vec1 = np.random.randn(1536).astype(np.float32) # rank 1 tensor
+batch1 = np.random.randn(1, 1536).astype(np.float32) # rank 2 tensor
+batch2 = np.random.randn(100, 1536).astype(np.float32)
+
+dist_rank1 = simsimd.cosine(vec1, batch2)
+dist_rank2 = simsimd.cosine(batch1, batch2)
+```
+
+### Many-to-Many Distances
+
+All distance functions in SimSIMD can be used to compute many-to-many distances.
+For two batches of 100 vectors to compute 100 distances, one would call it like this:
+
+```py
+batch1 = np.random.randn(100, 1536).astype(np.float32)
+batch2 = np.random.randn(100, 1536).astype(np.float32)
+dist = simsimd.cosine(batch1, batch2)
+```
+
+Input matrices must have identical shapes.
+This functionality isn't natively present in NumPy or SciPy, and generally requires creating intermediate arrays, which is inefficient and memory-consuming.
+
+### Many-to-Many All-Pairs Distances
+
+One can use SimSIMD to compute distances between all possible pairs of rows across two matrices (akin to [`scipy.spatial.distance.cdist`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.cdist.html)).
+The resulting object will have a type `DistancesTensor`, zero-copy compatible with NumPy and other libraries.
+For two arrays of 10 and 1,000 entries, the resulting tensor will have 10,000 cells:
+
+```py
+import numpy as np
+from simsimd import cdist, DistancesTensor
+
+matrix1 = np.random.randn(1000, 1536).astype(np.float32)
+matrix2 = np.random.randn(10, 1536).astype(np.float32)
+distances: DistancesTensor = simsimd.cdist(matrix1, matrix2, metric="cosine") # zero-copy
+distances_array: np.ndarray = np.array(distances, copy=True) # now managed by NumPy
+```
+
+### Multithreading
+
+By default, computations use a single CPU core.
+To optimize and utilize all CPU cores on Linux systems, add the `threads=0` argument.
+Alternatively, specify a custom number of threads:
+
+```py
+distances = simsimd.cdist(matrix1, matrix2, metric="cosine", threads=0)
+```
+
+### Using Python API with USearch
+
+Want to use it in Python with [USearch](https://github.com/unum-cloud/usearch)?
+You can wrap the raw C function pointers SimSIMD backends into a `CompiledMetric` and pass it to USearch, similar to how it handles Numba's JIT-compiled code.
+
+```py
+from usearch.index import Index, CompiledMetric, MetricKind, MetricSignature
+from simsimd import pointer_to_sqeuclidean, pointer_to_cosine, pointer_to_inner
+
+metric = CompiledMetric(
+    pointer=pointer_to_cosine("f16"),
+    kind=MetricKind.Cos,
+    signature=MetricSignature.ArrayArraySize,
+)
+
+index = Index(256, metric=metric)
+```
+
+## Using SimSIMD in Rust
+
+To install, add the following to your `Cargo.toml`:
+
+```toml
+[dependencies]
+simsimd = "..."
+```
+
+Before using the SimSIMD library, ensure you have imported the necessary traits and types into your Rust source file.
+The library provides several traits for different distance/similarity kinds - `SpatialSimilarity`, `BinarySimilarity`, and `ProbabilitySimilarity`.
+
+### Spatial Similarity: Cosine and Euclidean Distances
+
+```rust
+use simsimd::SpatialSimilarity;
+
+fn main() {
+    let vector_a: Vec<f32> = vec![1.0, 2.0, 3.0];
+    let vector_b: Vec<f32> = vec![4.0, 5.0, 6.0];
+
+    // Compute the cosine similarity between vector_a and vector_b
+    let cosine_similarity = f32::cosine(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Cosine Similarity: {}", cosine_similarity);
+
+    // Compute the squared Euclidean distance between vector_a and vector_b
+    let sq_euclidean_distance = f32::sqeuclidean(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Squared Euclidean Distance: {}", sq_euclidean_distance);
+}
+```
+
+Spatial similarity functions are available for `f64`, `f32`, `f16`, and `i8` types.
+
+### Dot-Products: Inner and Complex Inner Products
+
+```rust
+use simsimd::SpatialSimilarity;
+use simsimd::ComplexProducts;
+
+fn main() {
+    let vector_a: Vec<f32> = vec![1.0, 2.0, 3.0, 4.0];
+    let vector_b: Vec<f32> = vec![5.0, 6.0, 7.0, 8.0];
+
+    // Compute the inner product between vector_a and vector_b
+    let inner_product = SpatialSimilarity::dot(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Inner Product: {}", inner_product);
+
+    // Compute the complex inner product between complex_vector_a and complex_vector_b
+    let complex_inner_product = ComplexProducts::dot(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    let complex_conjugate_inner_product = ComplexProducts::vdot(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Complex Inner Product: {:?}", complex_inner_product); // -18, 69
+    println!("Complex C. Inner Product: {:?}", complex_conjugate_inner_product); // 70, -8
+}
+```
+
+Complex inner products are available for `f64`, `f32`, and `f16` types.
+
+### Probability Distributions: Jensen-Shannon and Kullback-Leibler Divergences
+
+```rust
+use simsimd::SpatialSimilarity;
+
+fn main() {
+    let vector_a: Vec<f32> = vec![1.0, 2.0, 3.0];
+    let vector_b: Vec<f32> = vec![4.0, 5.0, 6.0];
+
+    let cosine_similarity = f32::jensenshannon(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Cosine Similarity: {}", cosine_similarity);
+
+    let sq_euclidean_distance = f32::kullbackleibler(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Squared Euclidean Distance: {}", sq_euclidean_distance);
+}
+```
+
+Probability similarity functions are available for `f64`, `f32`, and `f16` types.
+
+### Binary Similarity: Hamming and Jaccard Distances
+
+Similar to spatial distances, one can compute bit-level distance functions between slices of unsigned integers:
+
+```rust
+use simsimd::BinarySimilarity;
+
+fn main() {
+    let vector_a = &[0b11110000, 0b00001111, 0b10101010];
+    let vector_b = &[0b11110000, 0b00001111, 0b01010101];
+
+    // Compute the Hamming distance between vector_a and vector_b
+    let hamming_distance = u8::hamming(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Hamming Distance: {}", hamming_distance);
+
+    // Compute the Jaccard distance between vector_a and vector_b
+    let jaccard_distance = u8::jaccard(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Jaccard Distance: {}", jaccard_distance);
+}
+```
+
+Binary similarity functions are available only for `u8` types.
+
+### Half-Precision Floating-Point Numbers
+
+Rust has no native support for half-precision floating-point numbers, but SimSIMD provides a `f16` type.
+It has no functionality - it is a `transparent` wrapper around `u16` and can be used with `half` or any other half-precision library.
+
+```rust
+use simsimd::SpatialSimilarity;
+use simsimd::f16 as SimF16;
+use half::f16 as HalfF16;
+
+fn main() {
+    let vector_a: Vec<HalfF16> = ...
+    let vector_b: Vec<HalfF16> = ...
+
+    let buffer_a: &[SimF16] = unsafe { std::slice::from_raw_parts(a_half.as_ptr() as *const SimF16, a_half.len()) };
+    let buffer_b: &[SimF16] = unsafe { std::slice::from_raw_parts(b_half.as_ptr() as *const SimF16, b_half.len()) };
+
+    // Compute the cosine similarity between vector_a and vector_b
+    let cosine_similarity = SimF16::cosine(&vector_a, &vector_b)
+        .expect("Vectors must be of the same length");
+
+    println!("Cosine Similarity: {}", cosine_similarity);
+}
+```
+
+### Dynamic Dispatch
+
+SimSIMD provides a dynamic dispatch mechanism to select the most advanced micro-kernel for the current CPU.
+You can query supported backends and use the `SimSIMD::capabilities` function to select the best one.
+
+```rust
+println!("uses neon: {}", capabilties::uses_neon());
+println!("uses sve: {}", capabilties::uses_sve());
+println!("uses haswell: {}", capabilties::uses_haswell());
+println!("uses skylake: {}", capabilties::uses_skylake());
+println!("uses ice: {}", capabilties::uses_ice());
+println!("uses sapphire: {}", capabilties::uses_sapphire());
+```
+
+## Using SimSIMD in JavaScript
+
+To install, choose one of the following options depending on your environment:
+
+- `npm install --save simsimd`
+- `yarn add simsimd`
+- `pnpm add simsimd`
+- `bun install simsimd`
+
+The package is distributed with prebuilt binaries, but if your platform is not supported, you can build the package from the source via `npm run build`.
+This will automatically happen unless you install the package with the `--ignore-scripts` flag or use Bun.
+After you install it, you will be able to call the SimSIMD functions on various `TypedArray` variants:
+
+```js
+const { sqeuclidean, cosine, inner, hamming, jaccard } = require('simsimd');
+
+const vectorA = new Float32Array([1.0, 2.0, 3.0]);
+const vectorB = new Float32Array([4.0, 5.0, 6.0]);
+
+const distance = sqeuclidean(vectorA, vectorB);
+console.log('Squared Euclidean Distance:', distance);
+```
+
+Other numeric types and precision levels are supported as well.
+For double-precsion floating-point numbers, use `Float64Array`:
+
+```js
+const vectorA = new Float64Array([1.0, 2.0, 3.0]);
+const vectorB = new Float64Array([4.0, 5.0, 6.0]);
+const distance = cosine(vectorA, vectorB);
+```
+
+When doing machine learning and vector search with high-dimensional vectors you may want to quantize them to 8-bit integers.
+You may want to project values from the $[-1, 1]$ range to the $[-100, 100]$ range and then cast them to `Uint8Array`:
+
+```js
+const quantizedVectorA = new Uint8Array(vectorA.map(v => (v * 100)));
+const quantizedVectorB = new Uint8Array(vectorB.map(v => (v * 100)));
+const distance = cosine(quantizedVectorA, quantizedVectorB);
+```
+
+A more extreme quantization case would be to use binary vectors.
+You can map all positive values to `1` and all negative values and zero to `0`, packing eight values into a single byte.
+After that, Hamming and Jaccard distances can be computed.
+
+```js
+const { toBinary, hamming } = require('simsimd');
+
+const binaryVectorA = toBinary(vectorA);
+const binaryVectorB = toBinary(vectorB);
+const distance = hamming(binaryVectorA, binaryVectorB);
+```
+
+## Using SimSIMD in C
+
+For integration within a CMake-based project, add the following segment to your `CMakeLists.txt`:
+
+```cmake
+FetchContent_Declare(
+    simsimd
+    GIT_REPOSITORY https://github.com/ashvardanian/simsimd.git
+    GIT_SHALLOW TRUE
+)
+FetchContent_MakeAvailable(simsimd)
+```
+
+After that, you can use the SimSIMD library in your C code in several ways.
+Simplest of all, you can include the headers, and the compiler will automatically select the most recent CPU extensions that SimSIMD will use.
+
+```c
+#include <simsimd/simsimd.h>
+
+int main() {
+    simsimd_f32_t vector_a[1536];
+    simsimd_f32_t vector_b[1536];
+    simsimd_metric_punned_t distance_function = simsimd_metric_punned(
+        simsimd_metric_cos_k, // Metric kind, like the angular cosine distance
+        simsimd_datatype_f32_k, // Data type, like: f16, f32, f64, i8, b8, and complex variants
+        simsimd_cap_any_k); // Which CPU capabilities are we allowed to use
+    simsimd_distance_t distance;
+    distance_function(vector_a, vector_b, 1536, &distance);
+    return 0;
+}
+```
+
+### Dynamic Dispatch
+
+To avoid hard-coding the backend, you can rely on `c/lib.c` to prepackage all possible backends in one binary, and select the most recent CPU features at runtime.
+That feature of the C library is called dynamic dispatch and is extensively used in the Python, JavaScript, and Rust bindings.
+To test which CPU features are available on the machine at runtime, use the following APIs:
+
+```c
+int uses_neon = simsimd_uses_neon();
+int uses_sve = simsimd_uses_sve();
+int uses_haswell = simsimd_uses_haswell();
+int uses_skylake = simsimd_uses_skylake();
+int uses_ice = simsimd_uses_ice();
+int uses_sapphire = simsimd_uses_sapphire();
+
+simsimd_capability_t capabilities = simsimd_capabilities();
+```
+
+To differentiate between runtime and compile-time dispatch, define the following macro:
+
+```c
+#define SIMSIMD_DYNAMIC_DISPATCH 1 // or 0
+```
+
+### Spatial Distances: Cosine and Euclidean Distances
+
+```c
+#include <simsimd/simsimd.h>
+
+int main() {
+    simsimd_f64_t f64s[1536];
+    simsimd_f32_t f32s[1536];
+    simsimd_f16_t f16s[1536];
+    simsimd_i8_t i8[1536];
+    simsimd_distance_t distance;
+
+    // Cosine distance between two vectors
+    simsimd_cos_i8(i8s, i8s, 1536, &distance);
+    simsimd_cos_f16(f16s, f16s, 1536, &distance);
+    simsimd_cos_f32(f32s, f32s, 1536, &distance);
+    simsimd_cos_f64(f64s, f64s, 1536, &distance);
+    
+    // Euclidean distance between two vectors
+    simsimd_l2sq_i8(i8s, i8s, 1536, &distance);
+    simsimd_l2sq_f16(f16s, f16s, 1536, &distance);
+    simsimd_l2sq_f32(f32s, f32s, 1536, &distance);
+    simsimd_l2sq_f64(f64s, f64s, 1536, &distance);
+
+    return 0;
+}
+```
+
+### Dot-Products: Inner and Complex Inner Products
+
+```c
+#include <simsimd/simsimd.h>
+
+int main() {
+    simsimd_f64_t f64s[1536];
+    simsimd_f32_t f32s[1536];
+    simsimd_f16_t f16s[1536];
+    simsimd_distance_t distance;
+
+    // Inner product between two vectors
+    simsimd_dot_f16(f16s, f16s, 1536, &distance);
+    simsimd_dot_f32(f32s, f32s, 1536, &distance);
+    simsimd_dot_f64(f64s, f64s, 1536, &distance);
+
+    // Complex inner product between two vectors
+    simsimd_dot_f16c(f16s, f16s, 1536, &distance);
+    simsimd_dot_f32c(f32s, f32s, 1536, &distance);
+    simsimd_dot_f64c(f64s, f64s, 1536, &distance);
+
+    // Complex conjugate inner product between two vectors
+    simsimd_vdot_f16c(f16s, f16s, 1536, &distance);
+    simsimd_vdot_f32c(f32s, f32s, 1536, &distance);
+    simsimd_vdot_f64c(f64s, f64s, 1536, &distance);
+
+    return 0;
+}
+```
+
+### Binary Distances: Hamming and Jaccard Distances
+
+```c
+#include <simsimd/simsimd.h>
+
+int main() {
+    simsimd_b8_t b8s[1536 / 8]; // 8 bits per word
+    simsimd_distance_t distance;
+
+    // Hamming distance between two vectors
+    simsimd_hamming_b8(b8s, b8s, 1536 / 8, &distance);
+
+    // Jaccard distance between two vectors
+    simsimd_jaccard_b8(b8s, b8s, 1536 / 8, &distance);
+
+    return 0;
+}
+```
+
+### Probability Distributions: Jensen-Shannon and Kullback-Leibler Divergences
+
+```c
+#include <simsimd/simsimd.h>
+
+int main() {
+    simsimd_f64_t f64s[1536];
+    simsimd_f32_t f32s[1536];
+    simsimd_f16_t f16s[1536];
+    simsimd_distance_t distance;
+
+    // Jensen-Shannon divergence between two vectors
+    simsimd_js_f16(f16s, f16s, 1536, &distance);
+    simsimd_js_f32(f32s, f32s, 1536, &distance);
+    simsimd_js_f64(f64s, f64s, 1536, &distance);
+
+    // Kullback-Leibler divergence between two vectors
+    simsimd_kl_f16(f16s, f16s, 1536, &distance);
+    simsimd_kl_f32(f32s, f32s, 1536, &distance);
+    simsimd_kl_f64(f64s, f64s, 1536, &distance);
+
+    return 0;
+}
+```
+
+### Half-Precision Floating-Point Numbers
+
+If you aim to utilize the `_Float16` functionality with SimSIMD, ensure your development environment is compatible with C 11.
+For other SimSIMD functionalities, C 99 compatibility will suffice.
+To explicitly disable half-precision support, define the following macro before imports:
+
+```c
+#define SIMSIMD_NATIVE_F16 0 // or 1
+#include <simsimd/simsimd.h>
+```
+
+### Target Specific Backends
+
+SimSIMD exposes all kernels for all backends, and you can select the most advanced one for the current CPU without relying on built-in dispatch mechanisms.
+All of the function names follow the same pattern: `simsimd_{function}_{type}_{backend}`.
+
+- The backend can be `serial`, `haswell`, `skylake`, `ice`, `sapphire`, `neon`, or `sve`.
+- The type can be `f64`, `f32`, `f16`, `f64c`, `f32c`, `f16c`, `i8`, or `b8`.
+- The function can be `dot`, `vdot`, `cos`, `l2sq`, `hamming`, `jaccard`, `kl`, or `js`.
+
+To avoid hard-coding the backend, you can use the `simsimd_metric_punned_t` to pun the function pointer and the `simsimd_capabilities` function to get the available backends at runtime.
+
+```c
+simsimd_dot_f64_sve
+simsimd_cos_f64_sve
+simsimd_l2sq_f64_sve
+simsimd_dot_f64_skylake
+simsimd_cos_f64_skylake
+simsimd_l2sq_f64_skylake
+simsimd_dot_f64_serial
+simsimd_cos_f64_serial
+simsimd_l2sq_f64_serial
+simsimd_js_f64_serial
+simsimd_kl_f64_serial
+simsimd_dot_f32_sve
+simsimd_cos_f32_sve
+simsimd_l2sq_f32_sve
+simsimd_dot_f32_neon
+simsimd_cos_f32_neon
+simsimd_l2sq_f32_neon
+simsimd_js_f32_neon
+simsimd_kl_f32_neon
+simsimd_dot_f32_skylake
+simsimd_cos_f32_skylake
+simsimd_l2sq_f32_skylake
+simsimd_js_f32_skylake
+simsimd_kl_f32_skylake
+simsimd_dot_f32_serial
+simsimd_cos_f32_serial
+simsimd_l2sq_f32_serial
+simsimd_js_f32_serial
+simsimd_kl_f32_serial
+simsimd_dot_f16_sve
+simsimd_cos_f16_sve
+simsimd_l2sq_f16_sve
+simsimd_dot_f16_neon
+simsimd_cos_f16_neon
+simsimd_l2sq_f16_neon
+simsimd_js_f16_neon
+simsimd_kl_f16_neon
+simsimd_dot_f16_sapphire
+simsimd_cos_f16_sapphire
+simsimd_l2sq_f16_sapphire
+simsimd_js_f16_sapphire
+simsimd_kl_f16_sapphire
+simsimd_dot_f16_haswell
+simsimd_cos_f16_haswell
+simsimd_l2sq_f16_haswell
+simsimd_js_f16_haswell
+simsimd_kl_f16_haswell
+simsimd_dot_f16_serial
+simsimd_cos_f16_serial
+simsimd_l2sq_f16_serial
+simsimd_js_f16_serial
+simsimd_kl_f16_serial
+simsimd_cos_i8_neon
+simsimd_cos_i8_neon
+simsimd_l2sq_i8_neon
+simsimd_cos_i8_ice
+simsimd_cos_i8_ice
+simsimd_l2sq_i8_ice
+simsimd_cos_i8_haswell
+simsimd_cos_i8_haswell
+simsimd_l2sq_i8_haswell
+simsimd_cos_i8_serial
+simsimd_cos_i8_serial
+simsimd_l2sq_i8_serial
+simsimd_hamming_b8_sve
+simsimd_jaccard_b8_sve
+simsimd_hamming_b8_neon
+simsimd_jaccard_b8_neon
+simsimd_hamming_b8_ice
+simsimd_jaccard_b8_ice
+simsimd_hamming_b8_haswell
+simsimd_jaccard_b8_haswell
+simsimd_hamming_b8_serial
+simsimd_jaccard_b8_serial
+simsimd_dot_f32c_sve
+simsimd_vdot_f32c_sve
+simsimd_dot_f32c_neon
+simsimd_vdot_f32c_neon
+simsimd_dot_f32c_haswell
+simsimd_vdot_f32c_haswell
+simsimd_dot_f32c_skylake
+simsimd_vdot_f32c_skylake
+simsimd_dot_f32c_serial
+simsimd_vdot_f32c_serial
+simsimd_dot_f64c_sve
+simsimd_vdot_f64c_sve
+simsimd_dot_f64c_skylake
+simsimd_vdot_f64c_skylake
+simsimd_dot_f64c_serial
+simsimd_vdot_f64c_serial
+simsimd_dot_f16c_sve
+simsimd_vdot_f16c_sve
+simsimd_dot_f16c_neon
+simsimd_vdot_f16c_neon
+simsimd_dot_f16c_haswell
+simsimd_vdot_f16c_haswell
+simsimd_dot_f16c_sapphire
+simsimd_vdot_f16c_sapphire
+simsimd_dot_f16c_serial
+simsimd_vdot_f16c_serial
+```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simsimd Version: 4.2.2 Summary: Fastest SIMD-
+Metadata-Version: 2.1 Name: simsimd Version: 4.3.0 Summary: Fastest SIMD-
 Accelerated Vector Similarity Functions for x86 and Arm Home-page: https://
 github.com/ashvardanian/simsimd Author: Ash Vardanian Author-email:
 1983160+ashvardanian@users.noreply.github.com License: Apache-2.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS Classifier: Development Status :: 5 -
 Production/Stable Classifier: Natural Language :: English Classifier: Intended
@@ -14,30 +14,31 @@
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Information Analysis Classifier: Topic :: Scientific/Engineering
 :: Bio-Informatics Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown License-File: LICENSE # SimSIMD ð
-_Computing dot-products, similarity measures, and distances between low- and
-high-dimensional vectors is ubiquitous in Machine Learning, Scientific
-Computing, Geo-Spatial Analysis, and Information Retrieval. These algorithms
-generally have linear complexity in time, constant complexity in space, and are
-data-parallel. In other words, it is easily parallelizable and vectorizable and
-often available in packages like BLAS and LAPACK, as well as higher-level
-`numpy` and `scipy` Python libraries. Ironically, even with decades of
-evolution in compilers and numerical computing, [most libraries can be 3-200x
-slower than hardware potential][benchmarks] even on the most popular hardware,
-like 64-bit x86 and Arm CPUs. SimSIMD attempts to fill that gap. 1ï¸â£
-SimSIMD functions are practically as fast as `memcpy`. 2ï¸â£ SimSIMD
-[compiles to more platforms than NumPy (105 vs 35)][compatibility] and has more
-backends than most BLAS implementations._ [benchmarks]: https://
-ashvardanian.com/posts/simsimd-faster-scipy [compatibility]: https://pypi.org/
-project/simsimd/#files
+Description-Content-Type: text/markdown License-File: LICENSE # SimSIMD ð !
+[SimSIMD banner](https://github.com/ashvardanian/ashvardanian/blob/master/
+repositories/SimSIMD.png?raw=true) Computing dot-products, similarity measures,
+and distances between low- and high-dimensional vectors is ubiquitous in
+Machine Learning, Scientific Computing, Geo-Spatial Analysis, and Information
+Retrieval. These algorithms generally have linear complexity in time, constant
+complexity in space, and are data-parallel. In other words, it is easily
+parallelizable and vectorizable and often available in packages like BLAS and
+LAPACK, as well as higher-level `numpy` and `scipy` Python libraries.
+Ironically, even with decades of evolution in compilers and numerical
+computing, [most libraries can be 3-200x slower than hardware potential]
+[benchmarks] even on the most popular hardware, like 64-bit x86 and Arm CPUs.
+SimSIMD attempts to fill that gap. 1ï¸â£ SimSIMD functions are practically as
+fast as `memcpy`. 2ï¸â£ SimSIMD [compiles to more platforms than NumPy (105
+vs 35)][compatibility] and has more backends than most BLAS implementations.
+[benchmarks]: https://ashvardanian.com/posts/simsimd-faster-scipy
+[compatibility]: https://pypi.org/project/simsimd/#files
 _[_P_y_P_I_]_[_n_p_m_]_[_r_u_s_t_][GitHub code size in bytes]_[_G_i_t_H_u_b_ _A_c_t_i_o_n_s_ _U_b_u_n_t_u_]_[_G_i_t_H_u_b
 _A_c_t_i_o_n_s_ _W_i_n_d_o_w_s_]_[_G_i_t_H_u_b_ _A_c_t_i_o_n_s_ _M_a_c_O_S_]_[_G_i_t_H_u_b_ _A_c_t_i_o_n_s_ _C_e_n_t_O_S_ _L_i_n_u_x_]
 ## Features SimSIMD provides over 100 SIMD-optimized kernels for various
 distance and similarity measures, accelerating search in [USearch](https://
 github.com/unum-cloud/usearch) and several DBMS products. Implemented distance
 functions include: - Euclidean (L2) and Cosine (Angular) spatial distances for
 Vector Search. - Dot-Products for real & complex vectors for DSP & Quantum
@@ -231,35 +232,45 @@
 ```rust println!("uses neon: {}", capabilties::uses_neon()); println!("uses
 sve: {}", capabilties::uses_sve()); println!("uses haswell: {}", capabilties::
 uses_haswell()); println!("uses skylake: {}", capabilties::uses_skylake());
 println!("uses ice: {}", capabilties::uses_ice()); println!("uses sapphire:
 {}", capabilties::uses_sapphire()); ``` ## Using SimSIMD in JavaScript To
 install, choose one of the following options depending on your environment: -
 `npm install --save simsimd` - `yarn add simsimd` - `pnpm add simsimd` - `bun
-install simsimd` The package is distributed with prebuilt binaries for Node.js
-v10 and above for Linux (x86_64, arm64), macOS (x86_64, arm64), and Windows
-(i386, x86_64). If your platform is not supported, you can build the package
-from the source via `npm run build`. This will automatically happen unless you
-install the package with the `--ignore-scripts` flag or use Bun. After you
-install it, you will be able to call the SimSIMD functions on various
-`TypedArray` variants: ```js const { sqeuclidean, cosine, inner, hamming,
-jaccard } = require('simsimd'); const vectorA = new Float32Array([1.0, 2.0,
-3.0]); const vectorB = new Float32Array([4.0, 5.0, 6.0]); const distance =
-sqeuclidean(vectorA, vectorB); console.log('Squared Euclidean Distance:',
-distance); ``` Other numeric types and precision levels are supported as well:
-```js const vectorA = new Float64Array([1.0, 2.0, 3.0]); const vectorB = new
-Float64Array([4.0, 5.0, 6.0]); const distance = cosine(vectorA, vectorB);
-console.log('Cosine Similarity:', distance); ``` ## Using SimSIMD in C For
-integration within a CMake-based project, add the following segment to your
-`CMakeLists.txt`: ```cmake FetchContent_Declare( simsimd GIT_REPOSITORY https:/
-/github.com/ashvardanian/simsimd.git GIT_SHALLOW TRUE )
-FetchContent_MakeAvailable(simsimd) ``` After that, you can use the SimSIMD
-library in your C code in several ways. Simplest of all, you can include the
-headers, and the compiler will automatically select the most recent CPU
-extensions that SimSIMD will use. ```c #include
+install simsimd` The package is distributed with prebuilt binaries, but if your
+platform is not supported, you can build the package from the source via `npm
+run build`. This will automatically happen unless you install the package with
+the `--ignore-scripts` flag or use Bun. After you install it, you will be able
+to call the SimSIMD functions on various `TypedArray` variants: ```js const
+{ sqeuclidean, cosine, inner, hamming, jaccard } = require('simsimd'); const
+vectorA = new Float32Array([1.0, 2.0, 3.0]); const vectorB = new Float32Array(
+[4.0, 5.0, 6.0]); const distance = sqeuclidean(vectorA, vectorB); console.log
+('Squared Euclidean Distance:', distance); ``` Other numeric types and
+precision levels are supported as well. For double-precsion floating-point
+numbers, use `Float64Array`: ```js const vectorA = new Float64Array([1.0, 2.0,
+3.0]); const vectorB = new Float64Array([4.0, 5.0, 6.0]); const distance =
+cosine(vectorA, vectorB); ``` When doing machine learning and vector search
+with high-dimensional vectors you may want to quantize them to 8-bit integers.
+You may want to project values from the $[-1, 1]$ range to the $[-100, 100]$
+range and then cast them to `Uint8Array`: ```js const quantizedVectorA = new
+Uint8Array(vectorA.map(v => (v * 100))); const quantizedVectorB = new
+Uint8Array(vectorB.map(v => (v * 100))); const distance = cosine
+(quantizedVectorA, quantizedVectorB); ``` A more extreme quantization case
+would be to use binary vectors. You can map all positive values to `1` and all
+negative values and zero to `0`, packing eight values into a single byte. After
+that, Hamming and Jaccard distances can be computed. ```js const { toBinary,
+hamming } = require('simsimd'); const binaryVectorA = toBinary(vectorA); const
+binaryVectorB = toBinary(vectorB); const distance = hamming(binaryVectorA,
+binaryVectorB); ``` ## Using SimSIMD in C For integration within a CMake-based
+project, add the following segment to your `CMakeLists.txt`: ```cmake
+FetchContent_Declare( simsimd GIT_REPOSITORY https://github.com/ashvardanian/
+simsimd.git GIT_SHALLOW TRUE ) FetchContent_MakeAvailable(simsimd) ``` After
+that, you can use the SimSIMD library in your C code in several ways. Simplest
+of all, you can include the headers, and the compiler will automatically select
+the most recent CPU extensions that SimSIMD will use. ```c #include
 imsimd.h> int main() { simsimd_f32_t vector_a[1536]; simsimd_f32_t vector_b
 [1536]; simsimd_metric_punned_t distance_function = simsimd_metric_punned
 ( simsimd_metric_cos_k, // Metric kind, like the angular cosine distance
 simsimd_datatype_f32_k, // Data type, like: f16, f32, f64, i8, b8, and complex
 variants simsimd_cap_any_k); // Which CPU capabilities are we allowed to use
 simsimd_distance_t distance; distance_function(vector_a, vector_b, 1536,
 &distance); return 0; } ``` ### Dynamic Dispatch To avoid hard-coding the
```

