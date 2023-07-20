# Comparing `tmp/vfbLib-0.5.1.tar.gz` & `tmp/vfbLib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfbLib-0.5.1.tar", last modified: Thu Jul 20 12:07:18 2023, max compression
+gzip compressed data, was "vfbLib-0.5.2.tar", last modified: Thu Jul 20 14:59:11 2023, max compression
```

## Comparing `vfbLib-0.5.1.tar` & `vfbLib-0.5.2.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.191898 vfbLib-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-20 12:07:04.000000 vfbLib-0.5.1/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 12:07:04.000000 vfbLib-0.5.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.175898 vfbLib-0.5.1/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.179898 vfbLib-0.5.1/Lib/vfbLib/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.183898 vfbLib-0.5.1/Lib/vfbLib/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/compilers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/compilers/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/cu2qu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.183898 vfbLib-0.5.1/Lib/vfbLib/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/guides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/mm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/truetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.187898 vfbLib-0.5.1/Lib/vfbLib/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/templates/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/truetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.187898 vfbLib-0.5.1/Lib/vfbLib/ufo/
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/designspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/guides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/kerning.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/pshints.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/tth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/vfb2ufo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/value.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.191898 vfbLib-0.5.1/Lib/vfbLib/vfb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/pens.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/vfb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.179898 vfbLib-0.5.1/Lib/vfbLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:07:17.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-20 12:07:18.191898 vfbLib-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-20 12:07:04.000000 vfbLib-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 12:07:04.000000 vfbLib-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-20 12:07:18.191898 vfbLib-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-20 12:07:04.000000 vfbLib-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.861729 vfbLib-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-20 14:58:59.000000 vfbLib-0.5.2/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 14:58:59.000000 vfbLib-0.5.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.849729 vfbLib-0.5.2/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.853729 vfbLib-0.5.2/Lib/vfbLib/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.853729 vfbLib-0.5.2/Lib/vfbLib/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/compilers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/compilers/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/cu2qu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.857729 vfbLib-0.5.2/Lib/vfbLib/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/mm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/parsers/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.857729 vfbLib-0.5.2/Lib/vfbLib/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/templates/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.861729 vfbLib-0.5.2/Lib/vfbLib/ufo/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/kerning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/pshints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/tth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/ufo/vfb2ufo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.861729 vfbLib-0.5.2/Lib/vfbLib/vfb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/pens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-20 14:58:59.000000 vfbLib-0.5.2/Lib/vfbLib/vfb/vfb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:59:11.853729 vfbLib-0.5.2/Lib/vfbLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 14:59:11.000000 vfbLib-0.5.2/Lib/vfbLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-20 14:59:11.861729 vfbLib-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-20 14:58:59.000000 vfbLib-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 14:58:59.000000 vfbLib-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-20 14:59:11.861729 vfbLib-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-20 14:58:59.000000 vfbLib-0.5.2/setup.py
```

### Comparing `vfbLib-0.5.1/DESCRIPTION.md` & `vfbLib-0.5.2/DESCRIPTION.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 ```
 
 will convert the file to `MyFile.ufo` in the same directory. Existing files will
 not be overwritten unless you specify the `-fo` option.
 
 ```
 vfb3ufo -h
-usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] inputpath [outputpath]
+usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] [-u] inputpath [outputpath]
 
-VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
+VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-19
 
 positional arguments:
   inputpath             input file path (.vfb)
   outputpath            output file path (.ufo[z])
 
 options:
   -h, --help            show this help message and exit
@@ -56,14 +56,16 @@
                         force overwrite
   -64, --base64         write GLIF lib 'data' section using base64 (recommended)
   -s, --silent          no display (silent mode)
   -nops, --no-postscript-hints
                         Don't output PostScript hinting
   -z, --zip             write UFOZ (compressed UFO)
   -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
+  -u, --unicode-strings
+                        interpret name table strings as Unicode instead of Windows-1252
 
 Not yet implemented options:
 
   -ttx, --ttx           convert binary OpenType Layout data using TTX-like format
 ```
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/cmdline.py` & `vfbLib-0.5.2/Lib/vfbLib/cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import codecs
 import json
 import logging
 
 from argparse import ArgumentParser
 from pathlib import Path
-from vfbLib.ufo import VfbToUfoBuilder
+from vfbLib.ufo.builder import VfbToUfoBuilder
 from vfbLib.version import build_date
 from vfbLib.vfb.vfb import Vfb
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/compilers/__init__.py` & `vfbLib-0.5.2/Lib/vfbLib/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/compilers/glyph.py` & `vfbLib-0.5.2/Lib/vfbLib/compilers/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/compilers/value.py` & `vfbLib-0.5.2/Lib/vfbLib/compilers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/constants.py` & `vfbLib-0.5.2/Lib/vfbLib/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from vfbLib.compilers.glyph import GlyphCompiler
 
-from vfbLib.parsers import (
+from vfbLib.parsers.base import (
     BaseParser,
     # EncodedValueParser,
     EncodedValueListParser,
     EncodedValueListWithCountParser,
     EncodedKeyValuesParser,
     EncodedKeyValuesParser1742,
     GaspParser,
@@ -36,15 +36,15 @@
     AxisMappingsParser,
     MasterLocationParser,
     PrimaryInstancesParser,
 )
 from vfbLib.parsers.numeric import (
     DoubleListParser,
     DoubleParser,
-    FloatListParser,
+    # FloatListParser,
     IntParser,
     IntListParser,
     PanoseParser,
     SignedIntParser,
 )
 from vfbLib.parsers.options import ExportOptionsParser
 from vfbLib.parsers.ps import PostScriptInfoParser
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/cu2qu.py` & `vfbLib-0.5.2/Lib/vfbLib/cu2qu.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/diff.py` & `vfbLib-0.5.2/Lib/vfbLib/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,13 +52,13 @@
     vfb1_str = json.dumps(vfb1.as_dict(), ensure_ascii=False, indent=4).splitlines()
     vfb2_str = json.dumps(vfb2.as_dict(), ensure_ascii=False, indent=4).splitlines()
     if args.html:
         html_diff = HtmlDiff()
         html = html_diff.make_file(
             vfb1_str, vfb2_str, str(vfb1_path), str(vfb2_path), context=True, numlines=5
         )
-        with codecs.open(args.html[0], "wb", "utf-8") as f:
+        with codecs.open(args.html, "wb", "utf-8") as f:
             f.write(html)
     else:
         d = unified_diff(vfb1_str, vfb2_str, str(vfb1_path), str(vfb2_path))
         for line in d:
             print(line)
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/__init__.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/base.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/bitmap.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/bitmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 from fontTools.misc.textTools import num2binary
 
 # from math import log2
 # from struct import unpack
 from typing import Any, Dict, List
-from vfbLib.parsers import BaseParser, read_encoded_value
+from vfbLib.parsers.base import BaseParser, read_encoded_value
 
 
 logger = logging.getLogger(__name__)
 
 
 def pprint_bitmap(bitmap, invert=False) -> List[str]:
     print(bitmap)
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/cmap.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/cmap.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 
-from vfbLib.parsers import BaseParser
+from vfbLib.parsers.base import BaseParser
 from vfbLib.parsers.value import read_encoded_value
 
 
 logger = logging.getLogger(__name__)
 
 
 class CustomCmapParser(BaseParser):
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/glyph.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/glyph.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 from fontTools.misc.textTools import hexStr  # , num2binary
 from fontTools.ttLib.tables.ttProgram import Program
 from io import BytesIO
 from struct import unpack
 from typing import Any, Dict, List, Literal
-from vfbLib.parsers import BaseParser, read_encoded_value
+from vfbLib.parsers.base import BaseParser, read_encoded_value
 from vfbLib.parsers.guides import parse_guides
 from vfbLib.truetype import TT_COMMANDS
 from vfbLib.typing import (
     Anchor,
     Component,
     GdefDict,
     GlyphData,
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/guides.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/guides.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 
 from typing import TYPE_CHECKING, List, Literal, Sequence
 from math import atan2, degrees
-from vfbLib.parsers import BaseParser, read_encoded_value
+from vfbLib.parsers.base import BaseParser, read_encoded_value
 from vfbLib.typing import Guide, GuideDict, GuideProperty
 
 if TYPE_CHECKING:
     from io import BytesIO
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/header.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/header.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 
 from io import BufferedReader
 from typing import Any, Dict, Tuple
-from vfbLib.parsers import read_encoded_value, uint8, uint16
+from vfbLib.parsers.base import read_encoded_value, uint8, uint16
 
 
 logger = logging.getLogger(__name__)
 
 
 class VfbHeaderParser:
     stream: BufferedReader | None = None
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/mm.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/mm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 
 from typing import Any, Dict, List, Tuple
-from vfbLib.parsers import BaseParser, read_encoded_value
+from vfbLib.parsers.base import BaseParser, read_encoded_value
 
 
 logger = logging.getLogger(__name__)
 
 
 class AnisotropicInterpolationsParser(BaseParser):
     @classmethod
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/numeric.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 
-from vfbLib.parsers import BaseParser
+from vfbLib.parsers.base import BaseParser
 from struct import unpack
 
 
 logger = logging.getLogger(__name__)
 
 
 class DoubleParser(BaseParser):
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/ps.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/ps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 
-from vfbLib.parsers import BaseParser
+from vfbLib.parsers.base import BaseParser
 
 
 logger = logging.getLogger(__name__)
 
 
 class PostScriptInfoParser(BaseParser):
     """
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/text.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 
 from typing import Dict, List
-from vfbLib.parsers import BaseParser, read_encoded_value
+from vfbLib.parsers.base import BaseParser, read_encoded_value
 
 
 logger = logging.getLogger(__name__)
 
 
 class NameRecordsParser(BaseParser):
     @classmethod
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/truetype.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/truetype.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 
 from io import BytesIO
 from typing import Dict, List
 from vfbLib.helpers import binaryToIntList
-from vfbLib.parsers import BaseParser, read_encoded_value
+from vfbLib.parsers.base import BaseParser, read_encoded_value
 
 
 logger = logging.getLogger(__name__)
 
 
 class TrueTypeInfoParser(BaseParser):
     """
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/parsers/value.py` & `vfbLib-0.5.2/Lib/vfbLib/parsers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/truetype.py` & `vfbLib-0.5.2/Lib/vfbLib/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/typing.py` & `vfbLib-0.5.2/Lib/vfbLib/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/__init__.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/builder.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/designspace.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/designspace.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/glyph.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/groups.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/groups.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/guides.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/helpers.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/helpers.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/info.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/kerning.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/kerning.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/paths.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/paths.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/pshints.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/pshints.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/tth.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/tth.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/typing.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/ufo/vfb2ufo.py` & `vfbLib-0.5.2/Lib/vfbLib/ufo/vfb2ufo.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/value.py` & `vfbLib-0.5.2/Lib/vfbLib/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/vfb/entry.py` & `vfbLib-0.5.2/Lib/vfbLib/vfb/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from io import BytesIO
 from struct import pack
 from typing import TYPE_CHECKING, Any, Dict, Tuple, Type
 
 # from vfbLib.reader import FALLBACK_PARSER
 from vfbLib.compilers import BaseCompiler
 from vfbLib.constants import parser_classes
-from vfbLib.parsers import BaseParser
+from vfbLib.parsers.base import BaseParser
 
 if TYPE_CHECKING:
     from io import BufferedReader
     from vfbLib.vfb.vfb import Vfb
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib/vfb/glyph.py` & `vfbLib-0.5.2/Lib/vfbLib/vfb/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/vfb/header.py` & `vfbLib-0.5.2/Lib/vfbLib/vfb/header.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/vfb/info.py` & `vfbLib-0.5.2/Lib/vfbLib/vfb/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/vfb/pens.py` & `vfbLib-0.5.2/Lib/vfbLib/vfb/pens.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/Lib/vfbLib/vfb/vfb.py` & `vfbLib-0.5.2/Lib/vfbLib/vfb/vfb.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(
         self,
         vfb_path: Path,
         timing=True,
         minimal=False,
         drop_keys: Set[str] | None = None,
         only_header=False,
-        unicode_strings = False,
+        unicode_strings=False,
     ) -> None:
         self.vfb_path = vfb_path
         self.timing = timing
         self.minimal = minimal
         if drop_keys is None:
             self.drop_keys = set()
         else:
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib.egg-info/PKG-INFO` & `vfbLib-0.5.2/Lib/vfbLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
@@ -54,17 +54,17 @@
 ```
 
 will convert the file to `MyFile.ufo` in the same directory. Existing files will
 not be overwritten unless you specify the `-fo` option.
 
 ```
 vfb3ufo -h
-usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] inputpath [outputpath]
+usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] [-u] inputpath [outputpath]
 
-VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
+VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-19
 
 positional arguments:
   inputpath             input file path (.vfb)
   outputpath            output file path (.ufo[z])
 
 options:
   -h, --help            show this help message and exit
@@ -73,14 +73,16 @@
                         force overwrite
   -64, --base64         write GLIF lib 'data' section using base64 (recommended)
   -s, --silent          no display (silent mode)
   -nops, --no-postscript-hints
                         Don't output PostScript hinting
   -z, --zip             write UFOZ (compressed UFO)
   -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
+  -u, --unicode-strings
+                        interpret name table strings as Unicode instead of Windows-1252
 
 Not yet implemented options:
 
   -ttx, --ttx           convert binary OpenType Layout data using TTX-like format
 ```
```

### Comparing `vfbLib-0.5.1/Lib/vfbLib.egg-info/SOURCES.txt` & `vfbLib-0.5.2/Lib/vfbLib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Lib/vfbLib.egg-info/not-zip-safe
 Lib/vfbLib.egg-info/requires.txt
 Lib/vfbLib.egg-info/top_level.txt
 Lib/vfbLib/compilers/__init__.py
 Lib/vfbLib/compilers/glyph.py
 Lib/vfbLib/compilers/value.py
 Lib/vfbLib/parsers/__init__.py
+Lib/vfbLib/parsers/base.py
 Lib/vfbLib/parsers/bitmap.py
 Lib/vfbLib/parsers/cmap.py
 Lib/vfbLib/parsers/glyph.py
 Lib/vfbLib/parsers/guides.py
 Lib/vfbLib/parsers/header.py
 Lib/vfbLib/parsers/mm.py
 Lib/vfbLib/parsers/numeric.py
@@ -36,14 +37,15 @@
 Lib/vfbLib/parsers/ps.py
 Lib/vfbLib/parsers/text.py
 Lib/vfbLib/parsers/truetype.py
 Lib/vfbLib/parsers/value.py
 Lib/vfbLib/templates/__init__.py
 Lib/vfbLib/templates/glyph.py
 Lib/vfbLib/ufo/__init__.py
+Lib/vfbLib/ufo/builder.py
 Lib/vfbLib/ufo/designspace.py
 Lib/vfbLib/ufo/glyph.py
 Lib/vfbLib/ufo/groups.py
 Lib/vfbLib/ufo/guides.py
 Lib/vfbLib/ufo/helpers.py
 Lib/vfbLib/ufo/info.py
 Lib/vfbLib/ufo/kerning.py
```

### Comparing `vfbLib-0.5.1/PKG-INFO` & `vfbLib-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
@@ -54,17 +54,17 @@
 ```
 
 will convert the file to `MyFile.ufo` in the same directory. Existing files will
 not be overwritten unless you specify the `-fo` option.
 
 ```
 vfb3ufo -h
-usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] inputpath [outputpath]
+usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] [-u] inputpath [outputpath]
 
-VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
+VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-19
 
 positional arguments:
   inputpath             input file path (.vfb)
   outputpath            output file path (.ufo[z])
 
 options:
   -h, --help            show this help message and exit
@@ -73,14 +73,16 @@
                         force overwrite
   -64, --base64         write GLIF lib 'data' section using base64 (recommended)
   -s, --silent          no display (silent mode)
   -nops, --no-postscript-hints
                         Don't output PostScript hinting
   -z, --zip             write UFOZ (compressed UFO)
   -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
+  -u, --unicode-strings
+                        interpret name table strings as Unicode instead of Windows-1252
 
 Not yet implemented options:
 
   -ttx, --ttx           convert binary OpenType Layout data using TTX-like format
 ```
```

### Comparing `vfbLib-0.5.1/README.md` & `vfbLib-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.1/setup.cfg` & `vfbLib-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vfbLib
-version = 0.5.1
+version = 0.5.2
 description = Tools for converting FontLab Studio 5 (VFB) files.
 long_description = file: DESCRIPTION.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/vfblib/
 author = Jens Kutilek
 license = MIT
 license_files = LICENSE
```

