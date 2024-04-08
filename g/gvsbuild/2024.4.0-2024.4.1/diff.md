# Comparing `tmp/gvsbuild-2024.4.0.tar.gz` & `tmp/gvsbuild-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvsbuild-2024.4.0.tar", max compression
+gzip compressed data, was "gvsbuild-2024.4.1.tar", max compression
```

## Comparing `gvsbuild-2024.4.0.tar` & `gvsbuild-2024.4.1.tar`

### file list

```diff
@@ -1,932 +1,931 @@
--rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/AUTHORS.md
--rw-r--r--   0        0        0    18433 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/COPYING
--rw-r--r--   0        0        0       37 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/__init__.py
--rw-r--r--   0        0        0    16410 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/build.py
--rw-r--r--   0        0        0     7322 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/deps.py
--rw-r--r--   0        0        0     2121 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/groups.py
--rw-r--r--   0        0        0      244 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/info.py
--rw-r--r--   0        0        0     5581 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/list.py
--rw-r--r--   0        0        0     1977 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/main.py
--rw-r--r--   0        0        0     2609 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/outdated.py
--rw-r--r--   0        0        0      634 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch
--rw-r--r--   0        0        0      213 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/check_utils.c
--rw-r--r--   0        0        0      537 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/check_utils.h
--rw-r--r--   0        0        0    18437 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/COPYING
--rw-r--r--   0        0        0     9831 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/meson.build
--rw-r--r--   0        0        0      175 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_atk.c
--rw-r--r--   0        0        0      167 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_cairo.c
--rw-r--r--   0        0        0      224 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_freetype2.c
--rw-r--r--   0        0        0      205 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
--rw-r--r--   0        0        0      170 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_glib.c
--rw-r--r--   0        0        0      183 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_jasper.c
--rw-r--r--   0        0        0      204 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_json_glib.c
--rw-r--r--   0        0        0      201 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libarchive.c
--rw-r--r--   0        0        0      191 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libcurl.c
--rw-r--r--   0        0        0      125 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libffi.c
--rw-r--r--   0        0        0      193 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
--rw-r--r--   0        0        0      194 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libjpeg.c
--rw-r--r--   0        0        0      188 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libpng.c
--rw-r--r--   0        0        0      187 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libtiff-4.c
--rw-r--r--   0        0        0      179 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libxml2.c
--rw-r--r--   0        0        0      187 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libyuv.c
--rw-r--r--   0        0        0      173 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_pango.c
--rw-r--r--   0        0        0      180 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_wing.c
--rw-r--r--   0        0        0      127 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_zlib.c
--rw-r--r--   0        0        0     9047 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
--rw-r--r--   0        0        0    10665 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
--rw-r--r--   0        0        0    29220 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
--rw-r--r--   0        0        0    50071 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19138 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4749 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt
--rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0    13484 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
--rw-r--r--   0        0        0     5987 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
--rw-r--r--   0        0        0      464 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
--rw-r--r--   0        0        0     9685 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
--rw-r--r--   0        0        0     8719 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9047 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
--rw-r--r--   0        0        0    10665 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27777 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
--rw-r--r--   0        0        0    50071 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19138 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4749 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt
--rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8719 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9126 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9180 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9636 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9164 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9112 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
--rw-r--r--   0        0        0    10744 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27909 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
--rw-r--r--   0        0        0    50150 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19138 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4749 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8798 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8976 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8901 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8807 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8817 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8794 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8801 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8888 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
--rw-r--r--   0        0        0      316 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
--rw-r--r--   0        0        0      339 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
--rw-r--r--   0        0        0     3533 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
--rw-r--r--   0        0        0    14290 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
--rw-r--r--   0        0        0    48250 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19171 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4783 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt
--rw-r--r--   0        0        0    13862 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
--rw-r--r--   0        0        0    14290 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
--rw-r--r--   0        0        0    48250 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19171 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4783 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt
--rw-r--r--   0        0        0    13862 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
--rw-r--r--   0        0        0    10284 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8997 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9318 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
--rw-r--r--   0        0        0    14369 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12930 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16426 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
--rw-r--r--   0        0        0    12161 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
--rw-r--r--   0        0        0    48329 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19171 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4783 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt
--rw-r--r--   0        0        0    13941 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0   244356 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glcorearb.h
--rw-r--r--   0        0        0   810011 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glext.h
--rw-r--r--   0        0        0    48113 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glxext.h
--rw-r--r--   0        0        0    44095 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/wglext.h
--rw-r--r--   0        0        0     1121 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
--rw-r--r--   0        0        0     1060 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
--rw-r--r--   0        0        0      740 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
--rw-r--r--   0        0        0     1135 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
--rw-r--r--   0        0        0     1045 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/include/md5global.h
--rw-r--r--   0        0        0      312 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
--rw-r--r--   0        0        0      418 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/config.h
--rw-r--r--   0        0        0      660 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/libenchant.rc
--rw-r--r--   0        0        0    17426 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/makefile.mak
--rw-r--r--   0        0        0      754 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch
--rw-r--r--   0        0        0     2152 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/ffmpeg/build/build.sh
--rw-r--r--   0        0        0      787 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
--rw-r--r--   0        0        0     3296 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch
--rw-r--r--   0        0        0    33686 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-tools-c99.patch
--rw-r--r--   0        0        0      367 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
--rw-r--r--   0        0        0     9543 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/libtextstyle-c99.patch
--rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     7623 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33617 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0     2128 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43681 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27515 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4377 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32044 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
--rw-r--r--   0        0        0    37498 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
--rw-r--r--   0        0        0     4322 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63279 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63715 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
--rw-r--r--   0        0        0    44998 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0     3250 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    35655 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
--rw-r--r--   0        0        0    81450 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    62421 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38906 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    20126 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
--rw-r--r--   0        0        0    19299 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
--rw-r--r--   0        0        0     3088 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
--rw-r--r--   0        0        0     2708 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
--rw-r--r--   0        0        0     7648 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
--rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     2093 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
--rw-r--r--   0        0        0    22716 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
--rw-r--r--   0        0        0    30933 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
--rw-r--r--   0        0        0     7623 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33701 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0    25904 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
--rw-r--r--   0        0        0     2128 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43508 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27538 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4658 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4377 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32067 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
--rw-r--r--   0        0        0     1209 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
--rw-r--r--   0        0        0    23409 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
--rw-r--r--   0        0        0    37554 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
--rw-r--r--   0        0        0    61302 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
--rw-r--r--   0        0        0     4298 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63335 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63743 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
--rw-r--r--   0        0        0    24900 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
--rw-r--r--   0        0        0    32949 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
--rw-r--r--   0        0        0    44998 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0    29890 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
--rw-r--r--   0        0        0     3250 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    24835 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
--rw-r--r--   0        0        0    35681 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
--rw-r--r--   0        0        0     7748 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
--rw-r--r--   0        0        0    42529 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
--rw-r--r--   0        0        0     4287 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
--rw-r--r--   0        0        0     1625 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
--rw-r--r--   0        0        0    81730 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    24592 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
--rw-r--r--   0        0        0    62584 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38904 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    27214 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
--rw-r--r--   0        0        0     1287 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
--rw-r--r--   0        0        0    91289 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
--rw-r--r--   0        0        0     4873 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
--rw-r--r--   0        0        0    23344 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
--rw-r--r--   0        0        0    46391 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
--rw-r--r--   0        0        0     1629 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
--rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
--rw-r--r--   0        0        0     7648 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
--rw-r--r--   0        0        0    33726 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
--rw-r--r--   0        0        0    17539 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
--rw-r--r--   0        0        0    26333 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
--rw-r--r--   0        0        0    43508 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
--rw-r--r--   0        0        0     4402 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
--rw-r--r--   0        0        0    32092 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
--rw-r--r--   0        0        0    37579 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
--rw-r--r--   0        0        0     4333 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
--rw-r--r--   0        0        0    63360 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
--rw-r--r--   0        0        0    63768 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
--rw-r--r--   0        0        0    45023 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
--rw-r--r--   0        0        0     3275 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
--rw-r--r--   0        0        0    13023 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
--rw-r--r--   0        0        0    35677 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
--rw-r--r--   0        0        0     7748 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
--rw-r--r--   0        0        0    42529 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
--rw-r--r--   0        0        0     4287 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
--rw-r--r--   0        0        0    81764 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
--rw-r--r--   0        0        0     2239 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
--rw-r--r--   0        0        0    62609 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
--rw-r--r--   0        0        0    38929 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
--rw-r--r--   0        0        0    27563 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
--rw-r--r--   0        0        0     4432 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
--rw-r--r--   0        0        0     1230 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
--rw-r--r--   0        0        0    23446 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
--rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
--rw-r--r--   0        0        0     7643 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
--rw-r--r--   0        0        0    33637 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
--rw-r--r--   0        0        0     4938 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
--rw-r--r--   0        0        0     5545 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
--rw-r--r--   0        0        0     9729 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
--rw-r--r--   0        0        0     2028 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
--rw-r--r--   0        0        0     2257 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
--rw-r--r--   0        0        0    10124 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
--rw-r--r--   0        0        0     6212 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
--rw-r--r--   0        0        0    16052 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
--rw-r--r--   0        0        0     2765 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
--rw-r--r--   0        0        0     6279 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
--rw-r--r--   0        0        0    43677 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
--rw-r--r--   0        0        0     4658 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4396 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
--rw-r--r--   0        0        0    37518 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
--rw-r--r--   0        0        0     4873 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
--rw-r--r--   0        0        0     4326 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
--rw-r--r--   0        0        0    23157 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
--rw-r--r--   0        0        0    63299 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
--rw-r--r--   0        0        0    63735 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
--rw-r--r--   0        0        0    46251 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
--rw-r--r--   0        0        0    45018 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
--rw-r--r--   0        0        0    29922 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
--rw-r--r--   0        0        0     3272 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
--rw-r--r--   0        0        0     1649 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
--rw-r--r--   0        0        0     4432 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
--rw-r--r--   0        0        0     1230 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
--rw-r--r--   0        0        0    35661 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
--rw-r--r--   0        0        0    81477 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
--rw-r--r--   0        0        0    62439 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
--rw-r--r--   0        0        0    54409 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75068 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97908 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75124 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75149 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54408 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75065 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97907 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75121 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75146 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54410 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97906 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    21997 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49879 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54407 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74958 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97900 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75014 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75039 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54406 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97945 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    22956 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
--rw-r--r--   0        0        0     6490 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/config-msvc.mak
--rw-r--r--   0        0        0    16869 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
--rwxr-xr-x   0        0        0      846 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists.bat
--rw-r--r--   0        0        0     5708 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
--rw-r--r--   0        0        0      772 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak
--rw-r--r--   0        0        0     4576 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
--rw-r--r--   0        0        0     8982 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
--rw-r--r--   0        0        0     2466 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextlib.def
--rw-r--r--   0        0        0     2852 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def
--rw-r--r--   0        0        0     3788 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
--rw-r--r--   0        0        0     2635 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle.def
--rw-r--r--   0        0        0     1051 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/Makefile.vc
--rw-r--r--   0        0        0     1582 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib/001-glib-package-installation-directory.patch
--rw-r--r--   0        0        0     3238 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch
--rw-r--r--   0        0        0     1582 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch
--rw-r--r--   0        0        0     3238 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch
--rw-r--r--   0        0        0       30 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
--rw-r--r--   0        0        0       27 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
--rw-r--r--   0        0        0     1123 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
--rw-r--r--   0        0        0      394 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/meson.build
--rw-r--r--   0        0        0      611 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch
--rw-r--r--   0        0        0     1468 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
--rw-r--r--   0        0        0      759 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
--rw-r--r--   0        0        0     2083 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
--rw-r--r--   0        0        0     1668 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch
--rw-r--r--   0        0        0     1958 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
--rw-r--r--   0        0        0     1186 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
--rw-r--r--   0        0        0     1920 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
--rw-r--r--   0        0        0     1956 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
--rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
--rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
--rw-r--r--   0        0        0    10679 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
--rw-r--r--   0        0        0     1080 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
--rw-r--r--   0        0        0    11397 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
--rw-r--r--   0        0        0     3760 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
--rw-r--r--   0        0        0    13364 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
--rw-r--r--   0        0        0     4222 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
--rw-r--r--   0        0        0     6519 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
--rw-r--r--   0        0        0     3640 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
--rw-r--r--   0        0        0    12279 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
--rw-r--r--   0        0        0     4640 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
--rw-r--r--   0        0        0     1962 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
--rw-r--r--   0        0        0    23804 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
--rw-r--r--   0        0        0     7938 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
--rw-r--r--   0        0        0     9247 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
--rw-r--r--   0        0        0      706 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
--rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
--rw-r--r--   0        0        0    26897 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
--rw-r--r--   0        0        0    26470 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
--rw-r--r--   0        0        0     9451 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
--rw-r--r--   0        0        0     1756 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
--rw-r--r--   0        0        0     3586 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
--rw-r--r--   0        0        0      803 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-accel.patch
--rw-r--r--   0        0        0      599 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-bgimg.patch
--rw-r--r--   0        0        0      682 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch
--rw-r--r--   0        0        0     2154 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
--rw-r--r--   0        0        0     1104 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/mod.md
--rw-r--r--   0        0        0     6104 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
--rw-r--r--   0        0        0    11322 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
--rw-r--r--   0        0        0     1630 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
--rw-r--r--   0        0        0     1261 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk4/001-fix-pangoft2-file-not-found.patch
--rw-r--r--   0        0        0     1088 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch
--rw-r--r--   0        0        0      102 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/hello-world/hello-world.c
--rw-r--r--   0        0        0       66 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/hello-world/meson.build
--rw-r--r--   0        0        0      359 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/icu/pc-files/icu-uc.pc
--rw-r--r--   0        0        0      360 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
--rw-r--r--   0        0        0    39523 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch
--rw-r--r--   0        0        0      652 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/mod.md
--rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
--rw-r--r--   0        0        0     4827 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/fficonfig.h.meson
--rw-r--r--   0        0        0      475 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/include/meson.build
--rw-r--r--   0        0        0      248 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson-scripts/extract-libtool-version.py
--rw-r--r--   0        0        0    13940 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson.build
--rw-r--r--   0        0        0     1154 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson_options.txt
--rw-r--r--   0        0        0     3334 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/src/meson.build
--rw-r--r--   0        0        0      936 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch
--rw-r--r--   0        0        0     1243 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch
--rw-r--r--   0        0        0     9777 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch
--rw-r--r--   0        0        0       44 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libpng/mod.md
--rw-r--r--   0        0        0      318 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libpng/pc-files/libpng.pc
--rw-r--r--   0        0        0      318 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libpng/pc-files/libpng16.pc
--rw-r--r--   0        0        0     2998 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
--rw-r--r--   0        0        0     2326 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
--rw-r--r--   0        0        0     2998 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
--rw-r--r--   0        0        0     2326 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
--rw-r--r--   0        0        0     9178 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
--rw-r--r--   0        0        0      937 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
--rw-r--r--   0        0        0     4286 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
--rw-r--r--   0        0        0      572 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    17549 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     3085 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     2998 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
--rw-r--r--   0        0        0     8574 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
--rw-r--r--   0        0        0     1026 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
--rw-r--r--   0        0        0      931 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
--rw-r--r--   0        0        0     2133 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
--rw-r--r--   0        0        0     6578 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
--rw-r--r--   0        0        0     2326 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
--rw-r--r--   0        0        0     8979 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
--rw-r--r--   0        0        0      925 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
--rw-r--r--   0        0        0    14576 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
--rw-r--r--   0        0        0     3427 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
--rw-r--r--   0        0        0      866 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
--rw-r--r--   0        0        0     5490 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/config.h
--rw-r--r--   0        0        0     8059 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj
--rw-r--r--   0        0        0      834 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
--rw-r--r--   0        0        0     3769 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/property.props
--rw-r--r--   0        0        0    40095 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/config.h
--rw-r--r--   0        0        0     8059 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj
--rw-r--r--   0        0        0      834 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
--rw-r--r--   0        0        0     3767 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/property.props
--rw-r--r--   0        0        0    40095 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/config.h
--rw-r--r--   0        0        0     8138 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj
--rw-r--r--   0        0        0      834 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
--rw-r--r--   0        0        0     3899 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/property.props
--rw-r--r--   0        0        0    40174 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     1079 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/mod.md
--rw-r--r--   0        0        0      809 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
--rw-r--r--   0        0        0     2586 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
--rw-r--r--   0        0        0     1251 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
--rw-r--r--   0        0        0     1025 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/include/libxml/meson.build
--rw-r--r--   0        0        0     1089 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/LICENSE.build
--rw-r--r--   0        0        0     7284 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/meson.build
--rw-r--r--   0        0        0      323 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
--rw-r--r--   0        0        0      943 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libyuv/001-win-build.patch
--rw-r--r--   0        0        0      392 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libyuv/pc-files/libyuv.pc
--rw-r--r--   0        0        0      352 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/luajit/pc-files/luajit.pc
--rw-r--r--   0        0        0      971 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/luajit/set-paths.patch
--rw-r--r--   0        0        0      319 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/pc-files/liblz4.pc
--rw-r--r--   0        0        0     8964 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
--rw-r--r--   0        0        0     8964 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
--rw-r--r--   0        0        0     8966 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9317 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9317 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10138 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9145 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9206 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9309 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
--rw-r--r--   0        0        0     8964 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
--rw-r--r--   0        0        0     9976 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
--rw-r--r--   0        0        0       93 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/mod.md
--rw-r--r--   0        0        0      733 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
--rw-r--r--   0        0        0     2184 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch
--rw-r--r--   0        0        0  1290625 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/certdata.txt
--rw-r--r--   0        0        0    19616 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/mk-ca-bundle.pl
--rw-r--r--   0        0        0      412 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/mod.md
--rw-r--r--   0        0        0      275 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/pc-files/libcrypto.pc
--rw-r--r--   0        0        0      285 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/pc-files/libssl.pc
--rw-r--r--   0        0        0      236 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/pc-files/openssl.pc
--rw-r--r--   0        0        0      383 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/opus/pc-files/opus.pc
--rw-r--r--   0        0        0    11464 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch
--rw-r--r--   0        0        0     1027 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch
--rw-r--r--   0        0        0     1089 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pcre2/LICENSE.build
--rw-r--r--   0        0        0     7523 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pcre2/meson.build
--rw-r--r--   0        0        0      473 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pcre2/meson_options.txt
--rw-r--r--   0        0        0     1241 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
--rw-r--r--   0        0        0     1036 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
--rw-r--r--   0        0        0     2647 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
--rw-r--r--   0        0        0      319 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
--rw-r--r--   0        0        0     1912 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch
--rw-r--r--   0        0        0      633 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/stack.props
--rw-r--r--   0        0        0     1565 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/win-iconv/COPYING
--rw-r--r--   0        0        0       92 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/win-iconv/mod.md
--rw-r--r--   0        0        0      671 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/x264/build/build.sh
--rw-r--r--   0        0        0     1385 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch
--rw-r--r--   0        0        0      343 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/zlib/pc-files/zlib.pc
--rw-r--r--   0        0        0     4259 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/__init__.py
--rw-r--r--   0        0        0     2040 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/adwaita_icon_theme.py
--rw-r--r--   0        0        0     1808 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/atk.py
--rw-r--r--   0        0        0     1774 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/boringssl.py
--rw-r--r--   0        0        0     1598 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cairo.py
--rw-r--r--   0        0        0     1509 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cairomm.py
--rw-r--r--   0        0        0     1912 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/check_libs.py
--rw-r--r--   0        0        0     1620 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/clutter.py
--rw-r--r--   0        0        0     1758 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cogl.py
--rw-r--r--   0        0        0     2872 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cyrus_sasl.py
--rw-r--r--   0        0        0     2844 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/dev_shell.py
--rw-r--r--   0        0        0     1648 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/emeus.py
--rw-r--r--   0        0        0     2807 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/enchant.py
--rw-r--r--   0        0        0     1572 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/expat.py
--rw-r--r--   0        0        0     3388 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/ffmpeg.py
--rw-r--r--   0        0        0     1725 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/freerdp.py
--rw-r--r--   0        0        0     1638 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/freetype.py
--rw-r--r--   0        0        0     2093 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/fribidi.py
--rw-r--r--   0        0        0     2204 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gdk_pixbuf.py
--rw-r--r--   0        0        0     4032 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gettext.py
--rw-r--r--   0        0        0     4682 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/glib.py
--rw-r--r--   0        0        0     1704 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/glibmm.py
--rw-r--r--   0        0        0     2684 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gobject_introspection.py
--rw-r--r--   0        0        0     1312 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gperf.py
--rw-r--r--   0        0        0     1752 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/graphene.py
--rw-r--r--   0        0        0     1813 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gsettings_desktop_schemas.py
--rw-r--r--   0        0        0     8797 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gstreamer.py
--rw-r--r--   0        0        0     5945 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gtk.py
--rw-r--r--   0        0        0     1806 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gtkmm.py
--rw-r--r--   0        0        0     2846 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gtksourceview.py
--rw-r--r--   0        0        0     1672 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/harfbuzz.py
--rw-r--r--   0        0        0     1184 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/hello_world.py
--rw-r--r--   0        0        0     1382 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/hicolor_icon_theme.py
--rw-r--r--   0        0        0     2276 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/icu.py
--rw-r--r--   0        0        0     1832 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/json_glib.py
--rw-r--r--   0        0        0     1392 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/jsonc.py
--rw-r--r--   0        0        0     1624 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/leveldb.py
--rw-r--r--   0        0        0     1417 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/lgi.py
--rw-r--r--   0        0        0     2063 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libadwaita.py
--rw-r--r--   0        0        0     2075 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libarchive.py
--rw-r--r--   0        0        0     1781 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libcbor.py
--rw-r--r--   0        0        0     1496 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libcroco.py
--rw-r--r--   0        0        0     1903 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libcurl.py
--rw-r--r--   0        0        0     1447 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libepoxy.py
--rw-r--r--   0        0        0     1341 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libffi.py
--rw-r--r--   0        0        0     2597 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libfido2.py
--rw-r--r--   0        0        0     1989 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libgxps.py
--rw-r--r--   0        0        0     1741 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libjpeg_turbo.py
--rw-r--r--   0        0        0     2331 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libmicrohttpd.py
--rw-r--r--   0        0        0     1704 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libpng.py
--rw-r--r--   0        0        0     1595 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libpsl.py
--rw-r--r--   0        0        0     2405 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/librsvg.py
--rw-r--r--   0        0        0     1737 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libsigcplusplus.py
--rw-r--r--   0        0        0     3368 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libsoup.py
--rw-r--r--   0        0        0     2181 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libssh.py
--rw-r--r--   0        0        0     1586 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libtiff.py
--rw-r--r--   0        0        0     1514 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libuv.py
--rw-r--r--   0        0        0     1511 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libvorbis.py
--rw-r--r--   0        0        0     3265 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libvpx.py
--rw-r--r--   0        0        0     1574 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libxml2.py
--rw-r--r--   0        0        0     1576 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libyuv.py
--rw-r--r--   0        0        0     1411 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libzip.py
--rw-r--r--   0        0        0     1426 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/lmdb.py
--rw-r--r--   0        0        0     1761 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/luajit.py
--rw-r--r--   0        0        0     1778 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/lz4.py
--rw-r--r--   0        0        0     2279 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/mit_kerberos.py
--rw-r--r--   0        0        0     1587 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/nghttp2.py
--rw-r--r--   0        0        0     1477 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/ogg.py
--rw-r--r--   0        0        0     1521 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/openh264.py
--rw-r--r--   0        0        0     3381 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/openssl.py
--rw-r--r--   0        0        0     2056 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/opus.py
--rw-r--r--   0        0        0     2046 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pango.py
--rw-r--r--   0        0        0     1768 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pangomm.py
--rw-r--r--   0        0        0      712 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pcre2.py
--rw-r--r--   0        0        0     1672 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pixman.py
--rw-r--r--   0        0        0     1692 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pkgconf.py
--rw-r--r--   0        0        0     2711 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/protobuf.py
--rw-r--r--   0        0        0     2102 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pycairo.py
--rw-r--r--   0        0        0     2591 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pygobject.py
--rw-r--r--   0        0        0     1618 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/sqlite.py
--rw-r--r--   0        0        0     1607 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/win_iconv.py
--rw-r--r--   0        0        0     1470 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/wing.py
--rw-r--r--   0        0        0     2341 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/x264.py
--rw-r--r--   0        0        0     2444 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/zlib.py
--rw-r--r--   0        0        0     7545 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/tools.py
--rw-r--r--   0        0        0       30 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/__init__.py
--rw-r--r--   0        0        0     8512 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_builders.py
--rw-r--r--   0        0        0    15193 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_expanders.py
--rw-r--r--   0        0        0     1339 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_group.py
--rw-r--r--   0        0        0    20353 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_project.py
--rw-r--r--   0        0        0     2749 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_tool.py
--rw-r--r--   0        0        0    38283 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/builder.py
--rw-r--r--   0        0        0     9899 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/simple_ui.py
--rw-r--r--   0        0        0     3899 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/utils.py
--rw-r--r--   0        0        0     1653 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0    12300 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/README.md
--rw-r--r--   0        0        0    13026 1970-01-01 00:00:00.000000 gvsbuild-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.040712 gvsbuild-2024.4.1/AUTHORS.md
+-rw-r--r--   0        0        0    18433 2024-04-08 18:08:22.040712 gvsbuild-2024.4.1/COPYING
+-rw-r--r--   0        0        0       37 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/__init__.py
+-rw-r--r--   0        0        0    16410 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/build.py
+-rw-r--r--   0        0        0     7322 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/deps.py
+-rw-r--r--   0        0        0     2121 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/groups.py
+-rw-r--r--   0        0        0      244 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/info.py
+-rw-r--r--   0        0        0     5581 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/list.py
+-rw-r--r--   0        0        0     1977 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/main.py
+-rw-r--r--   0        0        0     2609 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/outdated.py
+-rw-r--r--   0        0        0      634 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch
+-rw-r--r--   0        0        0      213 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/check_utils.c
+-rw-r--r--   0        0        0      537 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/check_utils.h
+-rw-r--r--   0        0        0    18437 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/COPYING
+-rw-r--r--   0        0        0     9831 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/meson.build
+-rw-r--r--   0        0        0      175 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_atk.c
+-rw-r--r--   0        0        0      167 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_cairo.c
+-rw-r--r--   0        0        0      224 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_freetype2.c
+-rw-r--r--   0        0        0      205 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
+-rw-r--r--   0        0        0      170 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_glib.c
+-rw-r--r--   0        0        0      183 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_jasper.c
+-rw-r--r--   0        0        0      204 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_json_glib.c
+-rw-r--r--   0        0        0      201 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libarchive.c
+-rw-r--r--   0        0        0      191 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libcurl.c
+-rw-r--r--   0        0        0      125 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libffi.c
+-rw-r--r--   0        0        0      193 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
+-rw-r--r--   0        0        0      194 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libjpeg.c
+-rw-r--r--   0        0        0      188 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libpng.c
+-rw-r--r--   0        0        0      187 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libtiff-4.c
+-rw-r--r--   0        0        0      179 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libxml2.c
+-rw-r--r--   0        0        0      187 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libyuv.c
+-rw-r--r--   0        0        0      173 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_pango.c
+-rw-r--r--   0        0        0      180 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_wing.c
+-rw-r--r--   0        0        0      127 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_zlib.c
+-rw-r--r--   0        0        0     9047 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
+-rw-r--r--   0        0        0    10665 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    29220 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
+-rw-r--r--   0        0        0    50071 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0    13484 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
+-rw-r--r--   0        0        0     5987 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
+-rw-r--r--   0        0        0      464 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0     9685 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
+-rw-r--r--   0        0        0     8719 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9047 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
+-rw-r--r--   0        0        0    10665 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27777 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
+-rw-r--r--   0        0        0    50071 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8719 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9126 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9180 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9636 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9164 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9112 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
+-rw-r--r--   0        0        0    10744 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27909 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
+-rw-r--r--   0        0        0    50150 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8798 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8976 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8901 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8807 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8817 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8794 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8801 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8888 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
+-rw-r--r--   0        0        0      316 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
+-rw-r--r--   0        0        0      339 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
+-rw-r--r--   0        0        0     3533 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
+-rw-r--r--   0        0        0    14290 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
+-rw-r--r--   0        0        0    48250 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0    13862 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
+-rw-r--r--   0        0        0    14290 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
+-rw-r--r--   0        0        0    48250 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0    13862 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
+-rw-r--r--   0        0        0    10284 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8997 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9318 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
+-rw-r--r--   0        0        0    14369 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12930 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16426 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
+-rw-r--r--   0        0        0    12161 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
+-rw-r--r--   0        0        0    48329 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0    13941 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0   244356 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glcorearb.h
+-rw-r--r--   0        0        0   810011 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glext.h
+-rw-r--r--   0        0        0    48113 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glxext.h
+-rw-r--r--   0        0        0    44095 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/wglext.h
+-rw-r--r--   0        0        0     1121 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
+-rw-r--r--   0        0        0     1060 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
+-rw-r--r--   0        0        0      740 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
+-rw-r--r--   0        0        0     1135 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
+-rw-r--r--   0        0        0     1045 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/include/md5global.h
+-rw-r--r--   0        0        0      312 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
+-rw-r--r--   0        0        0      418 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/config.h
+-rw-r--r--   0        0        0      660 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/libenchant.rc
+-rw-r--r--   0        0        0    17426 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/makefile.mak
+-rw-r--r--   0        0        0      754 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch
+-rw-r--r--   0        0        0     2152 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/ffmpeg/build/build.sh
+-rw-r--r--   0        0        0      787 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
+-rw-r--r--   0        0        0     3296 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-runtime-c99.patch
+-rw-r--r--   0        0        0    33686 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-tools-c99.patch
+-rw-r--r--   0        0        0      367 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
+-rw-r--r--   0        0        0     9543 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/libtextstyle-c99.patch
+-rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     7623 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33617 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0     2128 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43681 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27515 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4377 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32044 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
+-rw-r--r--   0        0        0    37498 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
+-rw-r--r--   0        0        0     4322 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63279 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63715 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
+-rw-r--r--   0        0        0    44998 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0     3250 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    35655 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
+-rw-r--r--   0        0        0    81450 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    62421 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38906 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    20126 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
+-rw-r--r--   0        0        0    19299 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
+-rw-r--r--   0        0        0     3088 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
+-rw-r--r--   0        0        0     2708 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
+-rw-r--r--   0        0        0     7648 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
+-rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     2093 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
+-rw-r--r--   0        0        0    22716 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
+-rw-r--r--   0        0        0    30933 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
+-rw-r--r--   0        0        0     7623 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33701 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0    25904 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
+-rw-r--r--   0        0        0     2128 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43508 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27538 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4658 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4377 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32067 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
+-rw-r--r--   0        0        0     1209 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
+-rw-r--r--   0        0        0    23409 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
+-rw-r--r--   0        0        0    37554 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
+-rw-r--r--   0        0        0    61302 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
+-rw-r--r--   0        0        0     4298 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63335 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63743 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
+-rw-r--r--   0        0        0    24900 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
+-rw-r--r--   0        0        0    32949 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
+-rw-r--r--   0        0        0    44998 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0    29890 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
+-rw-r--r--   0        0        0     3250 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    24835 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
+-rw-r--r--   0        0        0    35681 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
+-rw-r--r--   0        0        0     7748 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
+-rw-r--r--   0        0        0    42529 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
+-rw-r--r--   0        0        0     4287 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
+-rw-r--r--   0        0        0     1625 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
+-rw-r--r--   0        0        0    81730 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    24592 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
+-rw-r--r--   0        0        0    62584 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38904 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    27214 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
+-rw-r--r--   0        0        0     1287 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
+-rw-r--r--   0        0        0    91289 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
+-rw-r--r--   0        0        0     4873 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
+-rw-r--r--   0        0        0    23344 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
+-rw-r--r--   0        0        0    46391 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
+-rw-r--r--   0        0        0     1629 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
+-rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
+-rw-r--r--   0        0        0     7648 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
+-rw-r--r--   0        0        0    33726 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
+-rw-r--r--   0        0        0    17539 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
+-rw-r--r--   0        0        0    26333 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
+-rw-r--r--   0        0        0    43508 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
+-rw-r--r--   0        0        0     4402 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
+-rw-r--r--   0        0        0    32092 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
+-rw-r--r--   0        0        0    37579 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
+-rw-r--r--   0        0        0     4333 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
+-rw-r--r--   0        0        0    63360 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
+-rw-r--r--   0        0        0    63768 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
+-rw-r--r--   0        0        0    45023 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
+-rw-r--r--   0        0        0     3275 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
+-rw-r--r--   0        0        0    13023 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
+-rw-r--r--   0        0        0    35677 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
+-rw-r--r--   0        0        0     7748 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
+-rw-r--r--   0        0        0    42529 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
+-rw-r--r--   0        0        0     4287 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
+-rw-r--r--   0        0        0    81764 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
+-rw-r--r--   0        0        0    62609 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
+-rw-r--r--   0        0        0    38929 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
+-rw-r--r--   0        0        0    27563 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
+-rw-r--r--   0        0        0     4432 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    23446 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
+-rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
+-rw-r--r--   0        0        0     7643 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
+-rw-r--r--   0        0        0    33637 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
+-rw-r--r--   0        0        0     4938 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
+-rw-r--r--   0        0        0     5545 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
+-rw-r--r--   0        0        0     9729 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
+-rw-r--r--   0        0        0     2028 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
+-rw-r--r--   0        0        0     2257 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
+-rw-r--r--   0        0        0    10124 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
+-rw-r--r--   0        0        0     6212 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
+-rw-r--r--   0        0        0    16052 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
+-rw-r--r--   0        0        0     2765 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
+-rw-r--r--   0        0        0     6279 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
+-rw-r--r--   0        0        0    43677 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
+-rw-r--r--   0        0        0     4658 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4396 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
+-rw-r--r--   0        0        0    37518 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
+-rw-r--r--   0        0        0     4873 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
+-rw-r--r--   0        0        0     4326 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
+-rw-r--r--   0        0        0    23157 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
+-rw-r--r--   0        0        0    63299 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
+-rw-r--r--   0        0        0    63735 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
+-rw-r--r--   0        0        0    46251 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
+-rw-r--r--   0        0        0    45018 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
+-rw-r--r--   0        0        0    29922 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
+-rw-r--r--   0        0        0     3272 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
+-rw-r--r--   0        0        0     1649 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
+-rw-r--r--   0        0        0     4432 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    35661 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
+-rw-r--r--   0        0        0    81477 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
+-rw-r--r--   0        0        0    62439 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
+-rw-r--r--   0        0        0    54409 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75068 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97908 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75124 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75149 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54408 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75065 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97907 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75121 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75146 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54410 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97906 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    21997 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49879 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54407 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74958 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97900 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75014 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75039 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54406 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97945 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    22956 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
+-rw-r--r--   0        0        0     6490 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/config-msvc.mak
+-rw-r--r--   0        0        0    16869 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
+-rwxr-xr-x   0        0        0      846 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists.bat
+-rw-r--r--   0        0        0     5708 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
+-rw-r--r--   0        0        0      772 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/generate-msvc.mak
+-rw-r--r--   0        0        0     4576 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
+-rw-r--r--   0        0        0     8982 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
+-rw-r--r--   0        0        0     2466 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextlib.def
+-rw-r--r--   0        0        0     2852 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextsrc.def
+-rw-r--r--   0        0        0     3788 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
+-rw-r--r--   0        0        0     2635 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle.def
+-rw-r--r--   0        0        0     1051 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/Makefile.vc
+-rw-r--r--   0        0        0     1582 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib/001-glib-package-installation-directory.patch
+-rw-r--r--   0        0        0     3238 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch
+-rw-r--r--   0        0        0     1582 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch
+-rw-r--r--   0        0        0     3238 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch
+-rw-r--r--   0        0        0       30 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
+-rw-r--r--   0        0        0       27 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
+-rw-r--r--   0        0        0     1123 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
+-rw-r--r--   0        0        0      394 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/meson.build
+-rw-r--r--   0        0        0      611 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch
+-rw-r--r--   0        0        0     1468 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
+-rw-r--r--   0        0        0      759 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
+-rw-r--r--   0        0        0     2083 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
+-rw-r--r--   0        0        0     1668 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch
+-rw-r--r--   0        0        0     1958 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
+-rw-r--r--   0        0        0     1186 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
+-rw-r--r--   0        0        0     1920 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
+-rw-r--r--   0        0        0     1956 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
+-rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
+-rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
+-rw-r--r--   0        0        0    10679 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
+-rw-r--r--   0        0        0     1080 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
+-rw-r--r--   0        0        0    11397 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
+-rw-r--r--   0        0        0     3760 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
+-rw-r--r--   0        0        0    13364 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
+-rw-r--r--   0        0        0     4222 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
+-rw-r--r--   0        0        0     6519 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
+-rw-r--r--   0        0        0     3640 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
+-rw-r--r--   0        0        0    12279 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
+-rw-r--r--   0        0        0     4640 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
+-rw-r--r--   0        0        0     1962 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
+-rw-r--r--   0        0        0    23804 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
+-rw-r--r--   0        0        0     7938 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
+-rw-r--r--   0        0        0     9247 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
+-rw-r--r--   0        0        0      706 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
+-rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
+-rw-r--r--   0        0        0    26897 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
+-rw-r--r--   0        0        0    26470 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
+-rw-r--r--   0        0        0     9451 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
+-rw-r--r--   0        0        0     1756 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
+-rw-r--r--   0        0        0     3586 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0      803 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-accel.patch
+-rw-r--r--   0        0        0      599 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-bgimg.patch
+-rw-r--r--   0        0        0      682 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-multimonitor.patch
+-rw-r--r--   0        0        0     2154 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
+-rw-r--r--   0        0        0     1104 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/mod.md
+-rw-r--r--   0        0        0     6104 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
+-rw-r--r--   0        0        0    11322 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
+-rw-r--r--   0        0        0     1630 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
+-rw-r--r--   0        0        0     1088 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch
+-rw-r--r--   0        0        0      102 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/hello-world/hello-world.c
+-rw-r--r--   0        0        0       66 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/hello-world/meson.build
+-rw-r--r--   0        0        0      359 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/icu/pc-files/icu-uc.pc
+-rw-r--r--   0        0        0      360 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
+-rw-r--r--   0        0        0    39523 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch
+-rw-r--r--   0        0        0      652 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/mod.md
+-rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
+-rw-r--r--   0        0        0     4827 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/fficonfig.h.meson
+-rw-r--r--   0        0        0      475 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/include/meson.build
+-rw-r--r--   0        0        0      248 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson-scripts/extract-libtool-version.py
+-rw-r--r--   0        0        0    13940 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson.build
+-rw-r--r--   0        0        0     1154 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson_options.txt
+-rw-r--r--   0        0        0     3334 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/src/meson.build
+-rw-r--r--   0        0        0      936 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch
+-rw-r--r--   0        0        0     1243 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch
+-rw-r--r--   0        0        0     9777 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch
+-rw-r--r--   0        0        0       44 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libpng/mod.md
+-rw-r--r--   0        0        0      318 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libpng/pc-files/libpng.pc
+-rw-r--r--   0        0        0      318 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libpng/pc-files/libpng16.pc
+-rw-r--r--   0        0        0     2998 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
+-rw-r--r--   0        0        0     2133 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
+-rw-r--r--   0        0        0     2326 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
+-rw-r--r--   0        0        0     2998 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
+-rw-r--r--   0        0        0     2133 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
+-rw-r--r--   0        0        0     2326 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
+-rw-r--r--   0        0        0     9178 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
+-rw-r--r--   0        0        0      937 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
+-rw-r--r--   0        0        0     4286 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
+-rw-r--r--   0        0        0      572 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    17549 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     3085 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     2998 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
+-rw-r--r--   0        0        0     8574 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
+-rw-r--r--   0        0        0     1026 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
+-rw-r--r--   0        0        0      931 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
+-rw-r--r--   0        0        0     2133 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
+-rw-r--r--   0        0        0     6578 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
+-rw-r--r--   0        0        0     2326 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
+-rw-r--r--   0        0        0     8979 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
+-rw-r--r--   0        0        0      925 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
+-rw-r--r--   0        0        0    14576 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
+-rw-r--r--   0        0        0     3427 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
+-rw-r--r--   0        0        0      866 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
+-rw-r--r--   0        0        0     5490 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/config.h
+-rw-r--r--   0        0        0     8059 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
+-rw-r--r--   0        0        0     3769 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/property.props
+-rw-r--r--   0        0        0    40095 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/config.h
+-rw-r--r--   0        0        0     8059 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
+-rw-r--r--   0        0        0     3767 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/property.props
+-rw-r--r--   0        0        0    40095 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/config.h
+-rw-r--r--   0        0        0     8138 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
+-rw-r--r--   0        0        0     3899 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/property.props
+-rw-r--r--   0        0        0    40174 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     1079 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/mod.md
+-rw-r--r--   0        0        0      809 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
+-rw-r--r--   0        0        0     2586 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
+-rw-r--r--   0        0        0     1251 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
+-rw-r--r--   0        0        0     1025 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/include/libxml/meson.build
+-rw-r--r--   0        0        0     1089 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/LICENSE.build
+-rw-r--r--   0        0        0     7284 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/meson.build
+-rw-r--r--   0        0        0      323 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
+-rw-r--r--   0        0        0      943 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libyuv/001-win-build.patch
+-rw-r--r--   0        0        0      392 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libyuv/pc-files/libyuv.pc
+-rw-r--r--   0        0        0      352 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/luajit/pc-files/luajit.pc
+-rw-r--r--   0        0        0      971 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/luajit/set-paths.patch
+-rw-r--r--   0        0        0      319 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/pc-files/liblz4.pc
+-rw-r--r--   0        0        0     8964 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
+-rw-r--r--   0        0        0     8964 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
+-rw-r--r--   0        0        0     8966 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9317 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9317 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10138 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9145 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9206 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9309 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
+-rw-r--r--   0        0        0     8964 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
+-rw-r--r--   0        0        0     9976 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
+-rw-r--r--   0        0        0       93 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/mod.md
+-rw-r--r--   0        0        0      733 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
+-rw-r--r--   0        0        0     2184 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch
+-rw-r--r--   0        0        0  1290625 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/certdata.txt
+-rw-r--r--   0        0        0    19616 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/mk-ca-bundle.pl
+-rw-r--r--   0        0        0      412 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/mod.md
+-rw-r--r--   0        0        0      275 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/pc-files/libcrypto.pc
+-rw-r--r--   0        0        0      285 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/pc-files/libssl.pc
+-rw-r--r--   0        0        0      236 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/pc-files/openssl.pc
+-rw-r--r--   0        0        0      383 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/opus/pc-files/opus.pc
+-rw-r--r--   0        0        0    11464 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch
+-rw-r--r--   0        0        0     1027 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch
+-rw-r--r--   0        0        0     1089 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pcre2/LICENSE.build
+-rw-r--r--   0        0        0     7523 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pcre2/meson.build
+-rw-r--r--   0        0        0      473 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pcre2/meson_options.txt
+-rw-r--r--   0        0        0     1241 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
+-rw-r--r--   0        0        0     1036 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
+-rw-r--r--   0        0        0     2647 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
+-rw-r--r--   0        0        0      319 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
+-rw-r--r--   0        0        0     1912 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch
+-rw-r--r--   0        0        0      633 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/stack.props
+-rw-r--r--   0        0        0     1565 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/win-iconv/COPYING
+-rw-r--r--   0        0        0       92 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/win-iconv/mod.md
+-rw-r--r--   0        0        0      671 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/x264/build/build.sh
+-rw-r--r--   0        0        0     1385 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch
+-rw-r--r--   0        0        0      343 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/zlib/pc-files/zlib.pc
+-rw-r--r--   0        0        0     4259 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/__init__.py
+-rw-r--r--   0        0        0     2040 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/adwaita_icon_theme.py
+-rw-r--r--   0        0        0     1808 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/atk.py
+-rw-r--r--   0        0        0     1774 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/boringssl.py
+-rw-r--r--   0        0        0     1598 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cairo.py
+-rw-r--r--   0        0        0     1509 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cairomm.py
+-rw-r--r--   0        0        0     1912 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/check_libs.py
+-rw-r--r--   0        0        0     1620 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/clutter.py
+-rw-r--r--   0        0        0     1758 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cogl.py
+-rw-r--r--   0        0        0     2872 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cyrus_sasl.py
+-rw-r--r--   0        0        0     2844 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/dev_shell.py
+-rw-r--r--   0        0        0     1648 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/emeus.py
+-rw-r--r--   0        0        0     2807 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/enchant.py
+-rw-r--r--   0        0        0     1572 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/expat.py
+-rw-r--r--   0        0        0     3386 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/ffmpeg.py
+-rw-r--r--   0        0        0     1725 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/freerdp.py
+-rw-r--r--   0        0        0     1638 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/freetype.py
+-rw-r--r--   0        0        0     2093 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/fribidi.py
+-rw-r--r--   0        0        0     2204 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gdk_pixbuf.py
+-rw-r--r--   0        0        0     4032 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gettext.py
+-rw-r--r--   0        0        0     4682 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/glib.py
+-rw-r--r--   0        0        0     1704 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/glibmm.py
+-rw-r--r--   0        0        0     2684 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gobject_introspection.py
+-rw-r--r--   0        0        0     1312 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gperf.py
+-rw-r--r--   0        0        0     1752 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/graphene.py
+-rw-r--r--   0        0        0     1813 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gsettings_desktop_schemas.py
+-rw-r--r--   0        0        0     8797 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gstreamer.py
+-rw-r--r--   0        0        0     5848 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gtk.py
+-rw-r--r--   0        0        0     1806 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gtkmm.py
+-rw-r--r--   0        0        0     2846 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gtksourceview.py
+-rw-r--r--   0        0        0     1672 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/harfbuzz.py
+-rw-r--r--   0        0        0     1184 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/hello_world.py
+-rw-r--r--   0        0        0     1382 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/hicolor_icon_theme.py
+-rw-r--r--   0        0        0     2276 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/icu.py
+-rw-r--r--   0        0        0     1832 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/json_glib.py
+-rw-r--r--   0        0        0     1392 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/jsonc.py
+-rw-r--r--   0        0        0     1624 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/leveldb.py
+-rw-r--r--   0        0        0     1417 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/lgi.py
+-rw-r--r--   0        0        0     2027 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libadwaita.py
+-rw-r--r--   0        0        0     2075 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libarchive.py
+-rw-r--r--   0        0        0     1781 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libcbor.py
+-rw-r--r--   0        0        0     1496 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libcroco.py
+-rw-r--r--   0        0        0     1903 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libcurl.py
+-rw-r--r--   0        0        0     1447 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libepoxy.py
+-rw-r--r--   0        0        0     1341 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libffi.py
+-rw-r--r--   0        0        0     2597 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libfido2.py
+-rw-r--r--   0        0        0     1989 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libgxps.py
+-rw-r--r--   0        0        0     1741 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libjpeg_turbo.py
+-rw-r--r--   0        0        0     2331 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libmicrohttpd.py
+-rw-r--r--   0        0        0     1704 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libpng.py
+-rw-r--r--   0        0        0     1595 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libpsl.py
+-rw-r--r--   0        0        0     2405 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/librsvg.py
+-rw-r--r--   0        0        0     1737 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libsigcplusplus.py
+-rw-r--r--   0        0        0     3368 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libsoup.py
+-rw-r--r--   0        0        0     2181 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libssh.py
+-rw-r--r--   0        0        0     1586 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libtiff.py
+-rw-r--r--   0        0        0     1514 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libuv.py
+-rw-r--r--   0        0        0     1511 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libvorbis.py
+-rw-r--r--   0        0        0     3265 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libvpx.py
+-rw-r--r--   0        0        0     1574 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libxml2.py
+-rw-r--r--   0        0        0     1576 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libyuv.py
+-rw-r--r--   0        0        0     1411 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libzip.py
+-rw-r--r--   0        0        0     1426 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/lmdb.py
+-rw-r--r--   0        0        0     1761 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/luajit.py
+-rw-r--r--   0        0        0     1778 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/lz4.py
+-rw-r--r--   0        0        0     2279 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/mit_kerberos.py
+-rw-r--r--   0        0        0     1587 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/nghttp2.py
+-rw-r--r--   0        0        0     1477 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/ogg.py
+-rw-r--r--   0        0        0     1521 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/openh264.py
+-rw-r--r--   0        0        0     3381 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/openssl.py
+-rw-r--r--   0        0        0     2056 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/opus.py
+-rw-r--r--   0        0        0     2046 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pango.py
+-rw-r--r--   0        0        0     1768 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pangomm.py
+-rw-r--r--   0        0        0      712 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pcre2.py
+-rw-r--r--   0        0        0     1672 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pixman.py
+-rw-r--r--   0        0        0     1692 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pkgconf.py
+-rw-r--r--   0        0        0     2711 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/protobuf.py
+-rw-r--r--   0        0        0     2102 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pycairo.py
+-rw-r--r--   0        0        0     2591 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pygobject.py
+-rw-r--r--   0        0        0     1618 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/sqlite.py
+-rw-r--r--   0        0        0     1607 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/win_iconv.py
+-rw-r--r--   0        0        0     1470 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/wing.py
+-rw-r--r--   0        0        0     2341 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/x264.py
+-rw-r--r--   0        0        0     2444 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/zlib.py
+-rw-r--r--   0        0        0     7545 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/tools.py
+-rw-r--r--   0        0        0       30 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/__init__.py
+-rw-r--r--   0        0        0     8512 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_builders.py
+-rw-r--r--   0        0        0    15193 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_expanders.py
+-rw-r--r--   0        0        0     1339 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_group.py
+-rw-r--r--   0        0        0    20353 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_project.py
+-rw-r--r--   0        0        0     2749 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_tool.py
+-rw-r--r--   0        0        0    38283 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/builder.py
+-rw-r--r--   0        0        0     9899 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/simple_ui.py
+-rw-r--r--   0        0        0     3899 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/utils.py
+-rw-r--r--   0        0        0     1708 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12300 2024-04-08 18:08:22.040712 gvsbuild-2024.4.1/README.md
+-rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 gvsbuild-2024.4.1/PKG-INFO
```

### Comparing `gvsbuild-2024.4.0/AUTHORS.md` & `gvsbuild-2024.4.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/COPYING` & `gvsbuild-2024.4.1/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/build.py` & `gvsbuild-2024.4.1/gvsbuild/build.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/deps.py` & `gvsbuild-2024.4.1/gvsbuild/deps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/groups.py` & `gvsbuild-2024.4.1/gvsbuild/groups.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/list.py` & `gvsbuild-2024.4.1/gvsbuild/list.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/main.py` & `gvsbuild-2024.4.1/gvsbuild/main.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/outdated.py` & `gvsbuild-2024.4.1/gvsbuild/outdated.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/check-libs/check_utils.h` & `gvsbuild-2024.4.1/gvsbuild/patches/check-libs/check_utils.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/check-libs/COPYING` & `gvsbuild-2024.4.1/gvsbuild/patches/check-libs/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/check-libs/meson.build` & `gvsbuild-2024.4.1/gvsbuild/patches/check-libs/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glcorearb.h` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glcorearb.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glext.h` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glxext.h` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glxext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/wglext.h` & `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/wglext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/include/md5global.h` & `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/include/md5global.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/libenchant.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/libenchant.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/makefile.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/makefile.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/ffmpeg/build/build.sh` & `gvsbuild-2024.4.1/gvsbuild/patches/ffmpeg/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-runtime-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-tools-c99.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-tools-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/libtextstyle-c99.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/libtextstyle-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/config-msvc.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/config-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists.bat` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists.bat`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/generate-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextlib.def` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextlib.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextsrc.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle.def` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/Makefile.vc` & `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/Makefile.vc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/glib/001-glib-package-installation-directory.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/glib/001-glib-package-installation-directory.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c` & `gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/introspection.body.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-accel.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-accel.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-bgimg.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-bgimg.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-multimonitor.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/mod.md` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/winpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/mod.md` & `gvsbuild-2024.4.1/gvsbuild/patches/libcroco/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libffi/fficonfig.h.meson` & `gvsbuild-2024.4.1/gvsbuild/patches/libffi/fficonfig.h.meson`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson.build` & `gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson_options.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson_options.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libffi/src/meson.build` & `gvsbuild-2024.4.1/gvsbuild/patches/libffi/src/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/vs2019-support.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/property.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/property.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/config.h` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/property.props` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libssh/mod.md` & `gvsbuild-2024.4.1/gvsbuild/patches/libssh/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libxml2/include/libxml/meson.build` & `gvsbuild-2024.4.1/gvsbuild/patches/libxml2/include/libxml/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libxml2/LICENSE.build` & `gvsbuild-2024.4.1/gvsbuild/patches/libxml2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libxml2/meson.build` & `gvsbuild-2024.4.1/gvsbuild/patches/libxml2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/libyuv/001-win-build.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/libyuv/001-win-build.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/luajit/set-paths.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/luajit/set-paths.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln` & `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/certdata.txt` & `gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/certdata.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/mk-ca-bundle.pl` & `gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/mk-ca-bundle.pl`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/pcre2/LICENSE.build` & `gvsbuild-2024.4.1/gvsbuild/patches/pcre2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/pcre2/meson.build` & `gvsbuild-2024.4.1/gvsbuild/patches/pcre2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/stack.props` & `gvsbuild-2024.4.1/gvsbuild/patches/stack.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/win-iconv/COPYING` & `gvsbuild-2024.4.1/gvsbuild/patches/win-iconv/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/x264/build/build.sh` & `gvsbuild-2024.4.1/gvsbuild/patches/x264/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch` & `gvsbuild-2024.4.1/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/__init__.py` & `gvsbuild-2024.4.1/gvsbuild/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/adwaita_icon_theme.py` & `gvsbuild-2024.4.1/gvsbuild/projects/adwaita_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/atk.py` & `gvsbuild-2024.4.1/gvsbuild/projects/atk.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/boringssl.py` & `gvsbuild-2024.4.1/gvsbuild/projects/boringssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/cairo.py` & `gvsbuild-2024.4.1/gvsbuild/projects/cairo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/cairomm.py` & `gvsbuild-2024.4.1/gvsbuild/projects/cairomm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/check_libs.py` & `gvsbuild-2024.4.1/gvsbuild/projects/check_libs.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/clutter.py` & `gvsbuild-2024.4.1/gvsbuild/projects/clutter.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/cogl.py` & `gvsbuild-2024.4.1/gvsbuild/projects/cogl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/cyrus_sasl.py` & `gvsbuild-2024.4.1/gvsbuild/projects/cyrus_sasl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/dev_shell.py` & `gvsbuild-2024.4.1/gvsbuild/projects/dev_shell.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/emeus.py` & `gvsbuild-2024.4.1/gvsbuild/projects/emeus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/enchant.py` & `gvsbuild-2024.4.1/gvsbuild/projects/enchant.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/expat.py` & `gvsbuild-2024.4.1/gvsbuild/projects/expat.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/ffmpeg.py` & `gvsbuild-2024.4.1/gvsbuild/projects/ffmpeg.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 @project_add
 class Ffmpeg(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
             "ffmpeg",
-            version="6.1.1",
+            version="7.0",
             archive_url="https://ffmpeg.org/releases/ffmpeg-{version}.tar.xz",
-            hash="8684f4b00f94b85461884c3719382f1261f0d9eb3d59640a1f4ac0873616f968",
+            hash="4426a94dd2c814945456600c8adfc402bee65ec14a70e8c531ec9a2cd651da7b",
             dependencies=["nasm", "msys2", "pkgconf", "nv-codec-headers"],
             patches=[],
         )
         if self.opts.ffmpeg_enable_gpl:
             self.add_dependency("x264")
 
     def build(self):
@@ -73,16 +73,16 @@
 
 @project_add
 class NvCodecHeaders(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
             "nv-codec-headers",
-            version="12.1.14.0",
+            version="12.2.72.0",
             archive_url="https://github.com/FFmpeg/nv-codec-headers/releases/download/n{version}/nv-codec-headers-{version}.tar.gz",
-            hash="62b30ab37e4e9be0d0c5b37b8fee4b094e38e570984d56e1135a6b6c2c164c9f",
+            hash="c295a2ba8a06434d4bdc5c2208f8a825285210d71d91d572329b2c51fd0d4d03",
         )
 
     def build(self):
         add_path = os.path.join(self.builder.opts.msys_dir, "usr", "bin")
 
         self.exec_vs(r'make install PREFIX="%(gtk_dir)s"', add_path=add_path)
```

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/freerdp.py` & `gvsbuild-2024.4.1/gvsbuild/projects/freerdp.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/freetype.py` & `gvsbuild-2024.4.1/gvsbuild/projects/freetype.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/fribidi.py` & `gvsbuild-2024.4.1/gvsbuild/projects/fribidi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gdk_pixbuf.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gdk_pixbuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gettext.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gettext.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/glib.py` & `gvsbuild-2024.4.1/gvsbuild/projects/glib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/glibmm.py` & `gvsbuild-2024.4.1/gvsbuild/projects/glibmm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gobject_introspection.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gobject_introspection.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gperf.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gperf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/graphene.py` & `gvsbuild-2024.4.1/gvsbuild/projects/graphene.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gsettings_desktop_schemas.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gsettings_desktop_schemas.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gstreamer.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gstreamer.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gtk.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gtk.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,33 +118,30 @@
 @project_add
 class Gtk4(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gtk4",
             prj_dir="gtk4",
-            version="4.14.1",
+            version="4.14.2",
             lastversion_major=4,
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/gtk",
             archive_url="https://download.gnome.org/sources/gtk/{major}.{minor}/gtk-{version}.tar.xz",
-            hash="fcefb3f132f8cc4711a9efa5b353c9ae9bb5eeff0246fa74dbc2f2f839b9e308",
+            hash="22604cef2898a79e5f2143bb7aee2b7d1fa2eb946989a9d1338ecf9c8ae0e072",
             dependencies=[
                 "gdk-pixbuf",
                 "pango",
                 "libepoxy",
                 "graphene",
                 "cairo",
                 "harfbuzz",
                 "glib",
                 "fribidi",
             ],
-            patches=[
-                "001-fix-pangoft2-file-not-found.patch",
-            ],
         )
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
         else:
             enable_gi = "disabled"
```

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gtkmm.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gtkmm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/gtksourceview.py` & `gvsbuild-2024.4.1/gvsbuild/projects/gtksourceview.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/harfbuzz.py` & `gvsbuild-2024.4.1/gvsbuild/projects/harfbuzz.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/hello_world.py` & `gvsbuild-2024.4.1/gvsbuild/projects/hello_world.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/hicolor_icon_theme.py` & `gvsbuild-2024.4.1/gvsbuild/projects/hicolor_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/icu.py` & `gvsbuild-2024.4.1/gvsbuild/projects/icu.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/json_glib.py` & `gvsbuild-2024.4.1/gvsbuild/projects/json_glib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/jsonc.py` & `gvsbuild-2024.4.1/gvsbuild/projects/jsonc.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/leveldb.py` & `gvsbuild-2024.4.1/gvsbuild/projects/leveldb.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/lgi.py` & `gvsbuild-2024.4.1/gvsbuild/projects/lgi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libadwaita.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libadwaita.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 class Libadwaita(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "libadwaita",
             repository="https://gitlab.gnome.org/GNOME/libadwaita",
             version="1.5.0",
-            lastversion_even=True,
             archive_url="https://download.gnome.org/sources/libadwaita/{major}.{minor}/libadwaita-{version}.tar.xz",
             hash="fd92287df9bb95c963654fb6e70d3e082e2bcb37b147e0e3c905567167993783",
             dependencies=[
                 "ninja",
                 "meson",
                 "msys2",
                 "pkgconf",
```

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libarchive.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libarchive.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libcbor.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libcbor.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libcroco.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libcroco.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libcurl.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libcurl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libepoxy.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libepoxy.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libffi.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libffi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libfido2.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libfido2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libgxps.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libgxps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libjpeg_turbo.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libjpeg_turbo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libmicrohttpd.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libmicrohttpd.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libpng.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libpng.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libpsl.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libpsl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/librsvg.py` & `gvsbuild-2024.4.1/gvsbuild/projects/librsvg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libsigcplusplus.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libsigcplusplus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libsoup.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libsoup.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libssh.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libssh.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libtiff.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libtiff.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libuv.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libvorbis.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libvorbis.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libvpx.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libvpx.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libxml2.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libxml2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libyuv.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libyuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/libzip.py` & `gvsbuild-2024.4.1/gvsbuild/projects/libzip.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/lmdb.py` & `gvsbuild-2024.4.1/gvsbuild/projects/lmdb.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/luajit.py` & `gvsbuild-2024.4.1/gvsbuild/projects/luajit.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/lz4.py` & `gvsbuild-2024.4.1/gvsbuild/projects/lz4.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/mit_kerberos.py` & `gvsbuild-2024.4.1/gvsbuild/projects/mit_kerberos.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/nghttp2.py` & `gvsbuild-2024.4.1/gvsbuild/projects/nghttp2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/ogg.py` & `gvsbuild-2024.4.1/gvsbuild/projects/ogg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/openh264.py` & `gvsbuild-2024.4.1/gvsbuild/projects/openh264.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/openssl.py` & `gvsbuild-2024.4.1/gvsbuild/projects/openssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/opus.py` & `gvsbuild-2024.4.1/gvsbuild/projects/opus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pango.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pango.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pangomm.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pangomm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pcre2.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pcre2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pixman.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pixman.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pkgconf.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pkgconf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/protobuf.py` & `gvsbuild-2024.4.1/gvsbuild/projects/protobuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pycairo.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pycairo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/pygobject.py` & `gvsbuild-2024.4.1/gvsbuild/projects/pygobject.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/sqlite.py` & `gvsbuild-2024.4.1/gvsbuild/projects/sqlite.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/win_iconv.py` & `gvsbuild-2024.4.1/gvsbuild/projects/win_iconv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/wing.py` & `gvsbuild-2024.4.1/gvsbuild/projects/wing.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/x264.py` & `gvsbuild-2024.4.1/gvsbuild/projects/x264.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/projects/zlib.py` & `gvsbuild-2024.4.1/gvsbuild/projects/zlib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/tools.py` & `gvsbuild-2024.4.1/gvsbuild/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
 @tool_add
 class ToolCmake(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "cmake",
-            version="3.29.0",
+            version="3.29.1",
             archive_url="https://github.com/Kitware/CMake/releases/download/v{version}/cmake-{version}-windows-x86_64.zip",
-            hash="9ab28eba1ab7911a0e57ab274f5990a283fffa1d22eb711792d5562e5869f9ef",
+            hash="c8cf6ed50551d00ad8cd1f3b232810cd0a8b43b4a1d4f1393f0a575d423884dc",
             dir_part="cmake-{version}-windows-x86_64",
         )
 
     def load_defaults(self):
         Tool.load_defaults(self)
         self.tool_path = os.path.join(self.build_dir, "bin")
         self.full_exe = os.path.join(self.tool_path, "cmake.exe")
@@ -131,17 +131,17 @@
 
 @tool_add
 class ToolNasm(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "nasm",
-            version="2.16.01",
+            version="2.16.02",
             archive_url="https://www.nasm.us/pub/nasm/releasebuilds/{version}/win64/nasm-{version}-win64.zip",
-            hash="029eed31faf0d2c5f95783294432cbea6c15bf633430f254bb3c1f195c67ca3a",
+            hash="3facb987f97b9fc4a485d2f95aa64219dbfa991fc5d1867f7b0f93e416074d3c",
             dir_part="nasm-{version}",
             exe_name="nasm.exe",
         )
 
     def unpack(self):
         # We download directly the exe file so we copy it on the tool directory ...
         self.mark_deps = extract_exec(
@@ -205,17 +205,17 @@
 
 @tool_add
 class ToolGo(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "go",
-            version="1.22.1",
+            version="1.22.2",
             archive_url="https://go.dev/dl/go{version}.windows-amd64.zip",
-            hash="cf9c66a208a106402a527f5b956269ca506cfe535fc388e828d249ea88ed28ba",
+            hash="8e581cf330f49d3266e936521a2d8263679ef7e2fc2cbbceb85659122d883596",
             dir_part="go-{version}",
         )
 
     def load_defaults(self):
         Tool.load_defaults(self)
         self.tool_path = os.path.join(self.build_dir, "bin")
         self.full_exe = os.path.join(self.tool_path, "go.exe")
```

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/base_builders.py` & `gvsbuild-2024.4.1/gvsbuild/utils/base_builders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/base_expanders.py` & `gvsbuild-2024.4.1/gvsbuild/utils/base_expanders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/base_group.py` & `gvsbuild-2024.4.1/gvsbuild/utils/base_group.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/base_project.py` & `gvsbuild-2024.4.1/gvsbuild/utils/base_project.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/base_tool.py` & `gvsbuild-2024.4.1/gvsbuild/utils/base_tool.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/builder.py` & `gvsbuild-2024.4.1/gvsbuild/utils/builder.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/simple_ui.py` & `gvsbuild-2024.4.1/gvsbuild/utils/simple_ui.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/gvsbuild/utils/utils.py` & `gvsbuild-2024.4.1/gvsbuild/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/pyproject.toml` & `gvsbuild-2024.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gvsbuild"
-version = "2024.4.0"
+version = "2024.4.1"
 description = "GTK stack for Windows"
 authors = ["Ignacio Casal Quinteiro <qignacio@amazon.com>", "Dan Yeaw <dan@yeaw.me>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Build Tools",
@@ -14,14 +14,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 build = ">=0.9,<1.3"
 lastversion = { version = ">=2.4.2,<4.0.0", optional = true }
 packaging = { version = ">=21.3,<25.0", optional = true }
 typer = {extras = ["all"], version = ">=0.6.1,<0.13.0"}
+setuptools = {version = "^69.2.0", python = ">=3.12"}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.1"
 pytest = ">=7.1.3,<9.0.0"
 tox = "^4.1.2"
 
 [tool.poetry.extras]
```

### Comparing `gvsbuild-2024.4.0/README.md` & `gvsbuild-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.0/PKG-INFO` & `gvsbuild-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvsbuild
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: GTK stack for Windows
 License: GPL-2.0-only
 Author: Ignacio Casal Quinteiro
 Author-email: qignacio@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: outdated
 Requires-Dist: build (>=0.9,<1.3)
 Requires-Dist: lastversion (>=2.4.2,<4.0.0) ; extra == "outdated"
 Requires-Dist: packaging (>=21.3,<25.0) ; extra == "outdated"
+Requires-Dist: setuptools (>=69.2.0,<70.0.0) ; python_version >= "3.12"
 Requires-Dist: typer[all] (>=0.6.1,<0.13.0)
 Description-Content-Type: text/markdown
 
 # gvsbuild
 
 ![CI](https://github.com/wingtk/gvsbuild/actions/workflows/ci.yml/badge.svg)
```

