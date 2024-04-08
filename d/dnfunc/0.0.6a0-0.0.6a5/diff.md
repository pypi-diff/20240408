# Comparing `tmp/dnfunc-0.0.6a0.tar.gz` & `tmp/dnfunc-0.0.6a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnfunc-0.0.6a0.tar", max compression
+gzip compressed data, was "dnfunc-0.0.6a5.tar", max compression
```

## Comparing `dnfunc-0.0.6a0.tar` & `dnfunc-0.0.6a5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-01-10 09:20:39.044551 dnfunc-0.0.6a0/LICENSE
--rw-r--r--   0        0        0      534 2024-01-10 09:20:39.044551 dnfunc-0.0.6a0/README.md
--rw-r--r--   0        0        0     3003 2024-01-10 09:20:49.892538 dnfunc-0.0.6a0/pyproject.toml
--rw-r--r--   0        0        0      112 2024-01-10 09:20:39.048551 dnfunc-0.0.6a0/src/dnfunc/__init__.py
--rw-r--r--   0        0        0    50755 2024-01-10 09:20:39.048551 dnfunc-0.0.6a0/src/dnfunc/dnfunc.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 dnfunc-0.0.6a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 20:33:30.630529 dnfunc-0.0.6a5/LICENSE
+-rw-r--r--   0        0        0      782 2024-04-08 20:33:30.630529 dnfunc-0.0.6a5/README.md
+-rw-r--r--   0        0        0     2786 2024-04-08 20:33:42.658450 dnfunc-0.0.6a5/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-08 20:33:30.630529 dnfunc-0.0.6a5/src/dnfunc/__init__.py
+-rwxr-xr-x   0        0        0    52989 2024-04-08 20:33:30.630529 dnfunc-0.0.6a5/src/dnfunc/dnfunc.py
+-rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 dnfunc-0.0.6a5/PKG-INFO
```

### Comparing `dnfunc-0.0.6a0/LICENSE` & `dnfunc-0.0.6a5/LICENSE`

 * *Files identical despite different names*

### Comparing `dnfunc-0.0.6a0/README.md` & `dnfunc-0.0.6a5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # dnfunc
 
 > A collection of Vapoursynth functions and wrappers
 
-[![PyPI version](https://img.shields.io/pypi/v/dnfunc)](https://pypi.org/project/dnfunc)
-[![Main](https://github.com/DeadNews/dnfunc/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/dnfunc/actions/workflows/main.yml)
-[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/dnfunc/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/dnfunc/main)
+[![PyPI: Version](https://img.shields.io/pypi/v/dnfunc?logo=pypi&logoColor=white)](https://pypi.org/project/dnfunc)
+[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/dnfunc?logo=github&logoColor=white)](https://github.com/deadnews/dnfunc/releases/latest)
+[![CI: Main](https://img.shields.io/github/actions/workflow/status/deadnews/dnfunc/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/dnfunc/actions/workflows/main.yml)
+[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/dnfunc/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/dnfunc/main)
 
 ## Deps
 
 <https://github.com/DeadNews/zsh-scripts/blob/main/src/vs-plugins.zsh>
```

### Comparing `dnfunc-0.0.6a0/pyproject.toml` & `dnfunc-0.0.6a5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "dnfunc"
-version = "0.0.6-alpha.0"
+version = "0.0.6-alpha.5"
 description = "A collection of Vapoursynth functions and wrappers"
-authors = ["DeadNews <aurczpbgr@mozmail.com>"]
+authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/dnfunc"
 repository = "https://github.com/DeadNews/dnfunc"
 keywords = ["vapoursynth", "vapoursynth-functions", "video-encoding"]
 classifiers = [
   "Operating System :: OS Independent",
@@ -23,22 +23,22 @@
 havsfunc = "^33"
 lvsfunc = "^0.8.0"
 pyyaml = "^6.0.1"
 vstools = "^3.0.1"
 vsutil = "^0.8.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "^1.8.0"
-poethepoet = "^0.24.4"
-ruff = "^0.1.11"
+mypy = "^1.9.0"
+poethepoet = "^0.25.0"
+ruff = "^0.3.5"
 types-pyyaml = "^6.0.12.12"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4.4"
-pytest-cov = "^4.1.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poe.tasks]
@@ -70,51 +70,49 @@
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
+[tool.pyright]
+include = ["src"]
+ignore = ["tests"]
+typeCheckingMode = "off"
+
 [tool.ruff]
 line-length = 99
 target-version = "py311" # Until Poetry v2
 
 [tool.ruff.format]
 line-ending = "lf"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
   "COM812",  # Trailing comma missing
-  "D203",    # 1 blank line required before class docstring
-  "D212",    # Multi-line docstring summary should start at the first line
-  "E501",    # Line too long
-  "EXE001",  # Shebang is present but file is not executable
   "FBT001",  # Boolean positional arg in function definition
   "FBT002",  # Boolean default value in function definition
-  "ISC001",  # Checks for implicitly concatenated strings on a single line.
+  "ISC001",  # Checks for implicitly concatenated strings on a single line
   "PLR0913", # Too many arguments to function call
   #
   "D101",    # Missing docstring in public class
   "D102",    # Missing docstring in public method
   "D103",    # Missing docstring in public function
-  "ERA001",  # Found commented-out code
   "PLR2004", # Magic value used in comparison
 ]
 
-[tool.ruff.per-file-ignores]
-"tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
-
-[tool.ruff.flake8-comprehensions]
-allow-dict-calls-with-keyword-arguments = false
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = ["ANN", "D", "E501", "PLC1901", "PLR2004", "S"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.pydocstyle]
-convention = "google"
-
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 129
+max-line-length = 129
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
```

### Comparing `dnfunc-0.0.6a0/src/dnfunc/dnfunc.py` & `dnfunc-0.0.6a5/src/dnfunc/dnfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 #!/usr/bin/env python
 """A collection of Vapoursynth functions and wrappers."""
-from __future__ import annotations
 
-from dataclasses import dataclass, field, replace
+from collections.abc import Callable, Iterable
+from dataclasses import _DataclassT, dataclass, field, replace
 from functools import partial
 from pathlib import Path, PurePath
 from shutil import which
-from typing import TYPE_CHECKING, NamedTuple
+from typing import Any, NamedTuple, TypeAlias
 
 import havsfunc as hav
 import insane_aa as iaa
 import kagefunc as kg
 import vapoursynth as vs
-from vstools import rfs
+from vstools import FrameRange, FrameRangeN, FrameRangesN, rfs
 from vsutil import depth, get_depth, get_y, iterate, join, split
 from yaml import safe_load
 
-if TYPE_CHECKING:
-    from collections.abc import Callable, Iterable
-    from dataclasses import _DataclassT
-    from typing import Any, TypeAlias
+Maps: TypeAlias = FrameRangeN | FrameRangesN
+"""Maps type alias."""
+VideoFunc: TypeAlias = Callable[..., vs.VideoNode]
+"""VideoFunc type alias."""
 
-    from vstools import FrameRange, FrameRangeN, FrameRangesN
+PROC_DEPTH = 16
+"""The processing depth."""
 
-    Maps: TypeAlias = FrameRangeN | FrameRangesN
-    VideoFunc: TypeAlias = Callable[..., vs.VideoNode]
 
-PROC_DEPTH = 16  # processing_depth
+def load_yaml(file_path: str) -> dict | None:
+    """Load yaml settings from a file.
 
+    Args:
+        file_path: The path to the YAML file.
 
-def load_yaml(file_path: str) -> dict | None:
-    """Load yaml settings."""
+    Returns:
+        The loaded YAML settings as a dictionary, or None if the file does not exist.
+    """
     f1 = Path(file_path)
 
     return safe_load(f1.read_text()) if f1.is_file() else None
 
 
 def override_dc(
     data_class: _DataclassT,
     block: str,
     zone: str = "",
     **override: Any,
 ) -> _DataclassT:
-    """
-    Override default data_class params.
+    """Override default data_class params.
+
+    Notes:
+        Configuration preference order:
+        1. func params
+        2. yaml zone
+        3. yaml main
+        4. default
+
+    Args:
+        data_class: The original data class object.
+        block: The block name to retrieve settings from.
+        zone: The zone name to retrieve settings from.
+        **override: Any additional keyword arguments to override the data class.
 
-    Configuration preference order:
-    1. func params
-    2. yaml zone
-    3. yaml main
-    4. default
+    Returns:
+        The data class object with overridden parameters.
     """
     settings = load_yaml("./settings.yaml")
 
     if settings is not None:
         block_settings = settings.get(block)
 
         if block_settings is not None:
@@ -70,24 +82,41 @@
 
 ######
 # aa #
 ######
 
 
 class NumFramesError(Exception):
-    pass
+    """Exception raised for errors related to the number of frames.
+
+    Attributes:
+        message -- explanation of the error
+    """
 
 
 class Edi3Mode(NamedTuple):
+    """Represents the configuration for eedi3/nnedi3.
+
+    Attributes:
+        eedi3_mode: The EEDI3 mode.
+        device: The device number.
+        nnedi3_mode: The NNEDI3 mode.
+    """
+
     eedi3_mode: iaa.EEDI3Mode
     device: int
     nnedi3_mode: iaa.NNEDI3Mode
 
 
 def get_edi3_mode() -> Edi3Mode:
+    """Returns the Edi3Mode based on the availability of the `nvidia-smi` command.
+
+    Returns:
+        The Edi3Mode based on the availability of `nvidia-smi`.
+    """
     if which("nvidia-smi") is not None:
         return Edi3Mode(
             eedi3_mode=iaa.EEDI3Mode.OPENCL,
             device=0,
             nnedi3_mode=iaa.NNEDI3Mode.NNEDI3CL,
         )
 
@@ -186,15 +215,26 @@
 def aa(
     clip: vs.VideoNode,
     zone: str = "",
     epname: str = "",
     ext_mask: vs.VideoNode | None = None,
     **override: Any,
 ) -> vs.VideoNode:
-    """Anti-aliasing wrapper."""
+    """Anti-aliasing wrapper.
+
+    Args:
+        clip: Input video clip.
+        zone: Zone parameter.
+        epname: Episode name.
+        ext_mask: External mask.
+        **override: Additional override parameters.
+
+    Returns:
+        Anti-aliased video clip.
+    """
     if epname:
         f1 = Path(f"./temp/{epname}_aa_lossless.mp4")
         if f1.is_file():
             aa_lossless = source(f1)
 
             if aa_lossless.num_frames != clip.num_frames:
                 msg = f"{aa_lossless.num_frames=}, {clip.num_frames=}"
@@ -278,18 +318,17 @@
         ncoped_aa = aa(ncoped_aa_src, zone=zone)
 
     if filtr:
         if input_aa:
             ncoped = ncoped_aa
             # ↑ if you want to keep the AA-Titles
         f2 = Path(f"./temp/{name}_filt_lossless.mp4")
-        if f2.is_file():
-            ncoped_aa = source(f2).std.Trim(offset, ncoped_end)
-        else:
-            ncoped_aa = filtr(ncoped_aa, ncoped)
+        ncoped_aa = (
+            source(f2).std.Trim(offset, ncoped_end) if f2.is_file() else filtr(ncoped_aa, ncoped)
+        )
 
     if not (oped_clip.num_frames == ncoped.num_frames == ncoped_aa.num_frames):
         msg = f"{oped_clip.num_frames=}, {ncoped.num_frames=}, {ncoped_aa.num_frames=}"
         raise NumFramesError(msg)
 
     return save_titles(oped_clip=oped_clip, ncoped=ncoped, ncoped_aa=ncoped_aa)
 
@@ -500,14 +539,26 @@
 def bm3d_(
     clip: vs.VideoNode,
     bm_sigma: float = 2,
     bm_radius: float = 1,
     sm_thr: int = 48,
     sm_pref_mode: int = 1,
 ) -> vs.VideoNode:
+    """Apply BM3D denoising to the input clip.
+
+    Args:
+        clip: Input video clip.
+        bm_sigma: Sigma parameter for BM3D.
+        bm_radius: Radius parameter for BM3D.
+        sm_thr: Threshold parameter for smdegrain.
+        sm_pref_mode: Prefilter mode for smdegrain.
+
+    Returns:
+        Denoised video clip.
+    """
     from mvsfunc import BM3D
 
     planes = split(clip)
 
     planes[0] = BM3D(planes[0], sigma=bm_sigma, radius1=bm_radius)
     planes[1] = smdegrain_(planes[1], sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
     planes[2] = smdegrain_(planes[2], sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
@@ -555,14 +606,26 @@
 def filt(  # noqa: PLR0911, PLR0912, PLR0915, C901
     mrgc: vs.VideoNode,
     zone: str = "",
     out_mode: int = 0,
     prefilt_func: VideoFunc | None = None,
     **override: Any,
 ) -> vs.VideoNode:
+    """Apply various filters and denoising techniques to the input video clip.
+
+    Args:
+        mrgc: The input video clip.
+        zone: The zone to apply the filters to.
+        out_mode: The output mode.
+        prefilt_func: The pre-filter function.
+        **override: Additional parameters to override the default filter settings.
+
+    Returns:
+        The filtered video clip.
+    """
     fset = FilterSettings()
     fset = override_dc(fset, block="filt", zone=zone, **override)
 
     clip16 = depth(mrgc, PROC_DEPTH)
 
     if prefilt_func:
         clip16 = prefilt_func(mrgc, clip16)
@@ -814,18 +877,19 @@
     bits: int = 0,
     fpsnum: int = 0,
     fpsden: int = 0,
 ) -> vs.VideoNode:
     """Load video source."""
     f1 = PurePath(file)
 
-    if f1.suffix == ".mp4":
-        src = vs.core.lsmas.LibavSMASHSource(source=f1)
-    else:
-        src = vs.core.lsmas.LWLibavSource(source=f1)
+    src = (
+        vs.core.lsmas.LibavSMASHSource(source=f1)
+        if f1.suffix == ".mp4"
+        else vs.core.lsmas.LWLibavSource(source=f1)
+    )
 
     if fpsnum and fpsden:
         src = src.std.AssumeFPS(fpsnum=fpsnum, fpsden=fpsden)
 
     if not bits:
         bits = PROC_DEPTH
 
@@ -918,19 +982,14 @@
         raise NumFramesError(msg)
 
 
 def _mask_resize(
     mask: vs.VideoNode,
     format_src: vs.VideoNode | None = None,  # noqa: ARG001
 ) -> vs.VideoNode:
-    # if format_src:
-    #     mask_format = format_src.format.replace(color_family=GRAY, subsampling_w=0, subsampling_h=0)
-    # else:
-    #     mask_format = vs.GRAY16
-
     mask_format = vs.GRAY16
 
     return (
         mask.resize.Point(matrix_s="709", format=mask_format)
         if mask.format.color_family == vs.RGB
         else mask.resize.Point(format=mask_format)
     )
@@ -1000,18 +1059,22 @@
 
     replaced = masked_merge(mrgc, epis, mask=mask, yuv=yuv)
 
     return rfs(mrgc, replaced, maps) if maps else replaced
 
 
 def diff_rescale_mask(source: vs.VideoNode, dset: AASettings) -> vs.VideoNode:
-    """
-    Build mask from difference of original and re-upscales clips.
+    """Build mask from difference of original and re-upscales clips.
 
-    Based on atomchtools.
+    Args:
+        source: The original video clip.
+        dset: The settings for the anti-aliasing process.
+
+    Returns:
+        The mask representing the difference between the original and re-upscaled clips.
     """
     from descale import Descale
     from fvsfunc import Resize
 
     clip = get_y(source) if source.format.num_planes != 1 else source
 
     desc = Descale(
@@ -1137,16 +1200,15 @@
     input_type: int = 1
     preset: str = "placebo"
     match_enhance: float = 0.95
     sharp: float = 0.2
 
 
 def qtgmc(clip: vs.VideoNode, zone: str = "", **override: Any) -> vs.VideoNode:
-    """
-    QTGMC.
+    """QTGMC.
 
     InputType — 0 for interlaced input. Mode 1 is for general progressive material.
     Modes 2 & 3 are designed for badly deinterlaced material.
     Sharpness — The default 1.0 is fairly sharp. If using source-match the default is 0.2
     """
     qset = QTGMCSettings()
     qset = override_dc(qset, block="qtgmc", zone=zone, **override)
@@ -1416,15 +1478,15 @@
     radius: int | list[int] = 0
     yuv: bool = False
 
     @staticmethod
     def to_list(val: int | list[int]) -> list[int]:
         return val if isinstance(val, list) else [val, 0, 0]
 
-    def check_yuv(self: EdgeFixSettings) -> None:
+    def check_yuv(self: "EdgeFixSettings") -> None:
         self.yuv = any(
             isinstance(val, list)
             for val in (self.top, self.bottom, self.left, self.right, self.radius)
         )
 
 
 def edgefix(
@@ -1597,16 +1659,15 @@
     if mode == "svp":
         return to60fps_svp(clip)
 
     return None
 
 
 def chromashift(clip: vs.VideoNode, cx: int = 0, cy: int = 0) -> vs.VideoNode:
-    """
-    Shift hroma.
+    """Shift hroma.
 
     cx — Horizontal chroma shift. Positive value shifts chroma to left, negative value shifts chroma to right.
     cy — Vertical chroma shift. Positive value shifts chroma upwards, negative value shifts chroma downwards.
     """
     planes = split(clip)
 
     planes[1] = vs.core.resize.Spline36(planes[1], src_left=cx, src_top=cy)
@@ -1809,14 +1870,26 @@
 def pv_diff(
     tv: vs.VideoNode,
     bd: vs.VideoNode,
     thr: float = 72,
     name: str = "",
     exclude_ranges: list[FrameRange] | None = None,
 ) -> vs.VideoNode:
+    """Perform pixel value difference between two video clips.
+
+    Args:
+        tv: The first video clip.
+        bd: The second video clip.
+        thr: The threshold for considering a difference.
+        name: The name to be logged.
+        exclude_ranges: List of frame ranges to exclude from comparison.
+
+    Returns:
+        The comparison result.
+    """
     from lvsfunc import diff
 
     clips = [tv, bd]
     num_frames = [clip.num_frames for clip in clips]
     clips = [clip.std.Trim(0, min(num_frames) - 1) for clip in clips]
 
     comparison, frames = diff(clips[0], clips[1], thr=thr, return_ranges=True)
```

### Comparing `dnfunc-0.0.6a0/PKG-INFO` & `dnfunc-0.0.6a5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dnfunc
-Version: 0.0.6a0
+Version: 0.0.6a5
 Summary: A collection of Vapoursynth functions and wrappers
 Home-page: https://github.com/DeadNews/dnfunc
 License: MIT
 Keywords: vapoursynth,vapoursynth-functions,video-encoding
 Author: DeadNews
-Author-email: aurczpbgr@mozmail.com
+Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Video
@@ -23,15 +23,16 @@
 Project-URL: Repository, https://github.com/DeadNews/dnfunc
 Description-Content-Type: text/markdown
 
 # dnfunc
 
 > A collection of Vapoursynth functions and wrappers
 
-[![PyPI version](https://img.shields.io/pypi/v/dnfunc)](https://pypi.org/project/dnfunc)
-[![Main](https://github.com/DeadNews/dnfunc/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/dnfunc/actions/workflows/main.yml)
-[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/dnfunc/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/dnfunc/main)
+[![PyPI: Version](https://img.shields.io/pypi/v/dnfunc?logo=pypi&logoColor=white)](https://pypi.org/project/dnfunc)
+[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/dnfunc?logo=github&logoColor=white)](https://github.com/deadnews/dnfunc/releases/latest)
+[![CI: Main](https://img.shields.io/github/actions/workflow/status/deadnews/dnfunc/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/dnfunc/actions/workflows/main.yml)
+[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/dnfunc/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/dnfunc/main)
 
 ## Deps
 
 <https://github.com/DeadNews/zsh-scripts/blob/main/src/vs-plugins.zsh>
```

