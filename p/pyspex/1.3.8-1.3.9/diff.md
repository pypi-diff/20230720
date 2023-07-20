# Comparing `tmp/pyspex-1.3.8.tar.gz` & `tmp/pyspex-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspex-1.3.8.tar", last modified: Tue Mar 28 15:29:36 2023, max compression
+gzip compressed data, was "pyspex-1.3.9.tar", last modified: Wed Mar 29 15:22:14 2023, max compression
```

## Comparing `pyspex-1.3.8.tar` & `pyspex-1.3.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.602519 pyspex-1.3.8/
--rw-r--r--   0 richardh  (1304) earth     (3300)      188 2023-03-28 15:23:25.000000 pyspex-1.3.8/.gitignore
--rw-r--r--   0 richardh  (1304) earth     (3300)      175 2023-03-28 14:35:04.000000 pyspex-1.3.8/.readthedocs.yaml
--rw-r--r--   0 richardh  (1304) earth     (3300)      490 2023-03-28 14:35:04.000000 pyspex-1.3.8/CITATION.cff
--rw-r--r--   0 richardh  (1304) earth     (3300)      915 2023-03-28 14:35:04.000000 pyspex-1.3.8/ChangeLog.md
--rw-r--r--   0 richardh  (1304) earth     (3300)     1730 2023-03-28 14:35:04.000000 pyspex-1.3.8/INSTALL.md
--rw-r--r--   0 richardh  (1304) earth     (3300)     1550 2023-03-28 14:35:04.000000 pyspex-1.3.8/LICENSE
--rw-r--r--   0 richardh  (1304) earth     (3300)        0 2023-03-28 14:35:04.000000 pyspex-1.3.8/MANIFEST.in
--rw-r--r--   0 richardh  (1304) earth     (3300)     2683 2023-03-28 15:29:36.602519 pyspex-1.3.8/PKG-INFO
--rw-r--r--   0 richardh  (1304) earth     (3300)     1609 2023-03-28 14:35:04.000000 pyspex-1.3.8/README.md
--rw-r--r--   0 richardh  (1304) earth     (3300)      732 2023-03-28 14:35:04.000000 pyspex-1.3.8/ToDo.md
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.598519 pyspex-1.3.8/docs/
--rw-r--r--   0 richardh  (1304) earth     (3300)      634 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/Makefile
--rw-r--r--   0 richardh  (1304) earth     (3300)     1725 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/build.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     1230 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/conf.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     1427 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/index.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)      800 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/make.bat
--rw-r--r--   0 richardh  (1304) earth     (3300)       49 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/modules.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)      335 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/pyspex.gen_l1a.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     1058 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/pyspex.lib.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     2846 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/pyspex.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)      426 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/quick.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     7194 2023-03-28 14:35:04.000000 pyspex-1.3.8/docs/tools.rst
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.598519 pyspex-1.3.8/examples/
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.598519 pyspex-1.3.8/examples/l1agen_spex/
--rw-r--r--   0 richardh  (1304) earth     (3300)    14960 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl
--rw-r--r--   0 richardh  (1304) earth     (3300)    12158 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl
--rw-r--r--   0 richardh  (1304) earth     (3300)    12158 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl
--rw-r--r--   0 richardh  (1304) earth     (3300)    11929 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl
--rw-r--r--   0 richardh  (1304) earth     (3300)     3270 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/README.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)      670 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/run_393-398+hkt.yaml
--rw-r--r--   0 richardh  (1304) earth     (3300)      356 2023-03-28 14:35:04.000000 pyspex-1.3.8/examples/l1agen_spex/run_429-432.yaml
--rw-r--r--   0 richardh  (1304) earth     (3300)     1611 2023-03-28 15:23:25.000000 pyspex-1.3.8/pyproject.toml
--rw-r--r--   0 richardh  (1304) earth     (3300)      375 2023-03-28 14:35:04.000000 pyspex-1.3.8/requirement.txt
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.598519 pyspex-1.3.8/scripts/
--rwxr-xr-x   0 richardh  (1304) earth     (3300)      678 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/l1agen_spex.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)     1823 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_add_egse2l1a.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)     5382 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_add_ogse2l1a.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)     9914 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_ccsds2l1a.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)    15175 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_ckd_report.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)     3168 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_csv2bin_tbl.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)     8743 2023-03-28 15:23:25.000000 pyspex-1.3.8/scripts/spx1_dem2l1a.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     6312 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_l1a_select.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)     4958 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_quicklook_lite.py
--rwxr-xr-x   0 richardh  (1304) earth     (3300)    10216 2023-03-28 14:35:04.000000 pyspex-1.3.8/scripts/spx1_tif2l1a.py
--rw-r--r--   0 richardh  (1304) earth     (3300)      434 2023-03-28 15:29:36.602519 pyspex-1.3.8/setup.cfg
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.598519 pyspex-1.3.8/src/
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.598519 pyspex-1.3.8/src/pyspex/
--rw-r--r--   0 richardh  (1304) earth     (3300)      444 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/__init__.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     8700 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/binning_tables.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    20549 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/ccsds_io.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     8942 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/ckd_io.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.602519 pyspex-1.3.8/src/pyspex/data/
--rw-r--r--   0 richardh  (1304) earth     (3300)     3321 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/data/tai-utc.dat
--rw-r--r--   0 richardh  (1304) earth     (3300)    15467 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/dem_io.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    12901 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/egse_db.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.602519 pyspex-1.3.8/src/pyspex/gen_l1a/
--rw-r--r--   0 richardh  (1304) earth     (3300)        0 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/gen_l1a/__init__.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     2356 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/gen_l1a/cli.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     7325 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/hkt_io.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.602519 pyspex-1.3.8/src/pyspex/lib/
--rw-r--r--   0 richardh  (1304) earth     (3300)      201 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/lib/__init__.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     3507 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/lib/attrs_def.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     8413 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/lib/l1a_def.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    11384 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/lib/l1b_def.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    15027 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/lib/l1c_def.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     1617 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/lib/leap_sec.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    26986 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/lib/tmtc_def.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    24127 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/lv0_io.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    10098 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/lv1_args.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    10514 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/lv1_gse.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    35163 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/lv1_io.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    13316 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/ogse_db.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     2318 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/ogse_dolp.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     5868 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/ogse_grande.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    24872 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/ogse_helios.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     2984 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/ogse_laser.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     1459 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/spx_product.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     5373 2023-03-28 15:23:25.000000 pyspex-1.3.8/src/pyspex/tif_io.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     6786 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/tm_science.py
--rw-r--r--   0 richardh  (1304) earth     (3300)      596 2023-03-28 14:35:04.000000 pyspex-1.3.8/src/pyspex/version.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:29:36.602519 pyspex-1.3.8/src/pyspex.egg-info/
--rw-r--r--   0 richardh  (1304) earth     (3300)     2683 2023-03-28 15:29:36.000000 pyspex-1.3.8/src/pyspex.egg-info/PKG-INFO
--rw-r--r--   0 richardh  (1304) earth     (3300)     1890 2023-03-28 15:29:36.000000 pyspex-1.3.8/src/pyspex.egg-info/SOURCES.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)        1 2023-03-28 15:29:36.000000 pyspex-1.3.8/src/pyspex.egg-info/dependency_links.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)       58 2023-03-28 15:29:36.000000 pyspex-1.3.8/src/pyspex.egg-info/entry_points.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)      244 2023-03-28 15:29:36.000000 pyspex-1.3.8/src/pyspex.egg-info/requires.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)        7 2023-03-28 15:29:36.000000 pyspex-1.3.8/src/pyspex.egg-info/top_level.txt
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.695713 pyspex-1.3.9/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      188 2023-03-27 13:44:41.000000 pyspex-1.3.9/.gitignore
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      175 2023-03-27 13:44:41.000000 pyspex-1.3.9/.readthedocs.yaml
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      490 2023-03-27 13:44:41.000000 pyspex-1.3.9/CITATION.cff
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      915 2023-03-27 13:44:41.000000 pyspex-1.3.9/ChangeLog.md
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1730 2023-03-27 13:44:41.000000 pyspex-1.3.9/INSTALL.md
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1550 2023-03-27 13:44:41.000000 pyspex-1.3.9/LICENSE
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)        0 2023-03-27 13:44:41.000000 pyspex-1.3.9/MANIFEST.in
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     2683 2023-03-29 15:22:14.695713 pyspex-1.3.9/PKG-INFO
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1609 2023-03-27 13:44:41.000000 pyspex-1.3.9/README.md
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      732 2023-03-27 13:44:41.000000 pyspex-1.3.9/ToDo.md
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.683713 pyspex-1.3.9/docs/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      634 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/Makefile
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1725 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/build.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1230 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/conf.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1427 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/index.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      800 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/make.bat
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)       49 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/modules.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      335 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/pyspex.gen_l1a.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1058 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/pyspex.lib.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     2846 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/pyspex.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      426 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/quick.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     7194 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/tools.rst
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.679713 pyspex-1.3.9/examples/
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.687713 pyspex-1.3.9/examples/l1agen_spex/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    14960 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    12158 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    12158 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    11929 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     3270 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/README.rst
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      670 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/run_393-398+hkt.yaml
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      356 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/run_429-432.yaml
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1483 2023-03-29 15:20:38.000000 pyspex-1.3.9/pyproject.toml
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      375 2023-03-27 13:44:41.000000 pyspex-1.3.9/requirement.txt
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.687713 pyspex-1.3.9/scripts/
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)      678 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/l1agen_spex.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)     1823 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_add_egse2l1a.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)     5382 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_add_ogse2l1a.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)     9914 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_ccsds2l1a.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)    15175 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_ckd_report.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)     3168 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_csv2bin_tbl.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)     8743 2023-03-29 10:24:36.000000 pyspex-1.3.9/scripts/spx1_dem2l1a.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     6312 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_l1a_select.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)     4958 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_quicklook_lite.py
+-rwxrwxr-x   0 richardh  (1000) richardh  (1000)    10216 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_tif2l1a.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      434 2023-03-29 15:22:14.695713 pyspex-1.3.9/setup.cfg
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.679713 pyspex-1.3.9/src/
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      444 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/__init__.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     8700 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/binning_tables.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    20549 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ccsds_io.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     8942 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ckd_io.py
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex/data/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     3321 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/data/tai-utc.dat
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    15467 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/dem_io.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    12901 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/egse_db.py
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex/gen_l1a/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)        0 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/gen_l1a/__init__.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     2356 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/gen_l1a/cli.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     7325 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/hkt_io.py
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.695713 pyspex-1.3.9/src/pyspex/lib/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      201 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/__init__.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     3507 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/attrs_def.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     8413 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/l1a_def.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    11384 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/l1b_def.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    15027 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/l1c_def.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1617 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/leap_sec.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    26986 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/tmtc_def.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    24127 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv0_io.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    10098 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv1_args.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    10514 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv1_gse.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    35163 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv1_io.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    13316 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_db.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     2318 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_dolp.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     5868 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_grande.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)    24872 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_helios.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     2984 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_laser.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1459 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/spx_product.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     5373 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/tif_io.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     6786 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/tm_science.py
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      596 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/version.py
+drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex.egg-info/
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     2683 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/PKG-INFO
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)     1890 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/SOURCES.txt
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)        1 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/dependency_links.txt
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)       58 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/entry_points.txt
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)      162 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/requires.txt
+-rw-rw-r--   0 richardh  (1000) richardh  (1000)        7 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/top_level.txt
```

### Comparing `pyspex-1.3.8/ChangeLog.md` & `pyspex-1.3.9/ChangeLog.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/INSTALL.md` & `pyspex-1.3.9/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/LICENSE` & `pyspex-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/PKG-INFO` & `pyspex-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspex
-Version: 1.3.8
+Version: 1.3.9
 Summary: Software package to handle SPEXone Level-0 and Level-1 data
 Author-email: Richard van Hees <r.m.van.hees@sron.nl>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rmvanhees/pyspex
 Project-URL: documentation, https://pyspex.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/rmvanhees/pyspex/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyspex-1.3.8/README.md` & `pyspex-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/ToDo.md` & `pyspex-1.3.9/ToDo.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/Makefile` & `pyspex-1.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/build.rst` & `pyspex-1.3.9/docs/build.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/conf.py` & `pyspex-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/index.rst` & `pyspex-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/make.bat` & `pyspex-1.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/pyspex.lib.rst` & `pyspex-1.3.9/docs/pyspex.lib.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/pyspex.rst` & `pyspex-1.3.9/docs/pyspex.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/docs/tools.rst` & `pyspex-1.3.9/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl` & `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl` & `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl` & `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl` & `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/examples/l1agen_spex/README.rst` & `pyspex-1.3.9/examples/l1agen_spex/README.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/examples/l1agen_spex/run_393-398+hkt.yaml` & `pyspex-1.3.9/examples/l1agen_spex/run_393-398+hkt.yaml`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/pyproject.toml` & `pyspex-1.3.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -26,24 +26,22 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Atmospheric Science",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
   "importlib-resources>5.8; python_version=='3.8'",
-  "h5py~=2.10.0; python_version=='3.9'",
-  "h5py>=3.5; python_version!='3.9'",
+  "h5py>=3.7",
   "julian",
-  "moniplot>=0.5",
+  "moniplot>=0.5.9",
   "netCDF4>=1.5",
-  "numpy>=1.19",
+  "numpy>=1.23",
   "openpyxl>=3",
   "pyYAML>=6.0",
-  "xarray~=0.19.0; python_version=='3.9'",
-  "xarray>=2022.3; python_version!='3.9'",
+  "xarray>=2022.3",
 ]
 
 [project.scripts]
 spx1_level01a = "pyspex.gen_l1a.cli:main"
 
 [project.urls]
 homepage = "https://github.com/rmvanhees/pyspex"
```

### Comparing `pyspex-1.3.8/scripts/l1agen_spex.py` & `pyspex-1.3.9/scripts/l1agen_spex.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_add_egse2l1a.py` & `pyspex-1.3.9/scripts/spx1_add_egse2l1a.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_add_ogse2l1a.py` & `pyspex-1.3.9/scripts/spx1_add_ogse2l1a.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_ccsds2l1a.py` & `pyspex-1.3.9/scripts/spx1_ccsds2l1a.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_ckd_report.py` & `pyspex-1.3.9/scripts/spx1_ckd_report.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_csv2bin_tbl.py` & `pyspex-1.3.9/scripts/spx1_csv2bin_tbl.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_dem2l1a.py` & `pyspex-1.3.9/scripts/spx1_dem2l1a.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_l1a_select.py` & `pyspex-1.3.9/scripts/spx1_l1a_select.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_quicklook_lite.py` & `pyspex-1.3.9/scripts/spx1_quicklook_lite.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/scripts/spx1_tif2l1a.py` & `pyspex-1.3.9/scripts/spx1_tif2l1a.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/binning_tables.py` & `pyspex-1.3.9/src/pyspex/binning_tables.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ccsds_io.py` & `pyspex-1.3.9/src/pyspex/ccsds_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ckd_io.py` & `pyspex-1.3.9/src/pyspex/ckd_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/data/tai-utc.dat` & `pyspex-1.3.9/src/pyspex/data/tai-utc.dat`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/dem_io.py` & `pyspex-1.3.9/src/pyspex/dem_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/egse_db.py` & `pyspex-1.3.9/src/pyspex/egse_db.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/gen_l1a/cli.py` & `pyspex-1.3.9/src/pyspex/gen_l1a/cli.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/hkt_io.py` & `pyspex-1.3.9/src/pyspex/hkt_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lib/attrs_def.py` & `pyspex-1.3.9/src/pyspex/lib/attrs_def.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lib/l1a_def.py` & `pyspex-1.3.9/src/pyspex/lib/l1a_def.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lib/l1b_def.py` & `pyspex-1.3.9/src/pyspex/lib/l1b_def.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lib/l1c_def.py` & `pyspex-1.3.9/src/pyspex/lib/l1c_def.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lib/leap_sec.py` & `pyspex-1.3.9/src/pyspex/lib/leap_sec.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lib/tmtc_def.py` & `pyspex-1.3.9/src/pyspex/lib/tmtc_def.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lv0_io.py` & `pyspex-1.3.9/src/pyspex/lv0_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lv1_args.py` & `pyspex-1.3.9/src/pyspex/lv1_args.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lv1_gse.py` & `pyspex-1.3.9/src/pyspex/lv1_gse.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/lv1_io.py` & `pyspex-1.3.9/src/pyspex/lv1_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ogse_db.py` & `pyspex-1.3.9/src/pyspex/ogse_db.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ogse_dolp.py` & `pyspex-1.3.9/src/pyspex/ogse_dolp.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ogse_grande.py` & `pyspex-1.3.9/src/pyspex/ogse_grande.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ogse_helios.py` & `pyspex-1.3.9/src/pyspex/ogse_helios.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/ogse_laser.py` & `pyspex-1.3.9/src/pyspex/ogse_laser.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/spx_product.py` & `pyspex-1.3.9/src/pyspex/spx_product.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/tif_io.py` & `pyspex-1.3.9/src/pyspex/tif_io.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/tm_science.py` & `pyspex-1.3.9/src/pyspex/tm_science.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex/version.py` & `pyspex-1.3.9/src/pyspex/version.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.8/src/pyspex.egg-info/PKG-INFO` & `pyspex-1.3.9/src/pyspex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspex
-Version: 1.3.8
+Version: 1.3.9
 Summary: Software package to handle SPEXone Level-0 and Level-1 data
 Author-email: Richard van Hees <r.m.van.hees@sron.nl>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rmvanhees/pyspex
 Project-URL: documentation, https://pyspex.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/rmvanhees/pyspex/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyspex-1.3.8/src/pyspex.egg-info/SOURCES.txt` & `pyspex-1.3.9/src/pyspex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

